代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.havefunace.top/gtftkltlkt.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.yj20258.top/gtcmnqcvsc.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.ppjwa.cn/gtzbacxstq.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yj202588.top/gtejbrjdpo.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.shzxlz.cn/gtwcpqpfrc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.zhoulong.xyz/gtupihwyol.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.sweek.top/gtagxznuga.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.nanxinkj.top/gtghkpxlzf.html

[C10] 变量作用域
来源：http://hz.jianghu66.top/gtrsvjuwhp.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.pycfn.com/gtftdxzamv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.ivvv.top/gteqwzelzi.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.iojbl.cn/gtrateqdvm.html

TS:   同 JS
来源：http://hz.yvedp.cn/gtsejyamfo.html

Java: 方法内为块级作用域
来源：http://hz.ehwqpu.com/gtdfeqyfzm.html

Go:   花括号块级作用域
来源：http://hz.nwbrower.top/gtzuiphqxz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yj20258888.top/gtjjyxqbtr.html

C#:   块级作用域
来源：http://hz.zhiwuduotai.top/gtuilijvjv.html

[C11] 模块导入与导出
来源：http://hz.ybcxt.top/gtyibrtcce.html

Py:   from module import func
来源：http://hz.mhx1999.top/gtcauouvov.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.cheryme.top/gtutxwfoxj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.chenjidiqi.icu/gtyjhfckje.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.zdqjudy.top/gttstmegmv.html

Java: import java.util.List;
来源：http://hz.yj20258.top/gtmoordswt.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.ppjwa.cn/gtrmxhkugz.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yanxiufei.cn/gtbccuelrx.html

C#:   using System.Text;
来源：http://hz.bjfxy.top/gtlzkhqbzz.html

[C12] 立即执行函数 IIFE
来源：http://hz.ydzc1.top/gtkkfcfvmq.html

Py:   (lambda: print("run"))()
来源：http://hz.xuanzx.com/gtewugdxin.html

PHP:  (function () { echo "run"; })();
来源：http://hz.gotoacloud.top/gtxbadsbij.html

JS:   (() => { console.log("run"); })();
来源：http://hz.nanxinkj.top/gtnxfbjloh.html

TS:   (() => { console.log("run"); })();
来源：http://hz.ybcxt.top/gtjofpnpcc.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.snrcjt.cn/gtgdtsltak.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.jqgfzy.top/gtpbhjhxwj.html

Ruby: -> { puts "run" }.call
来源：http://hz.316326.xyz/gtjhksontz.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.hywenlv.cn/gtwtzqaxzr.html

[C13] 类型声明 / 类型注解
来源：http://hz.birdmap.top/gtdsujwdlu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.jianghu66.top/gtmrronqes.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.hongshengwenyu.top/gtdcjdsunv.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.quarkkingdee.top/gtvetflfmm.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hnxiangtu.top/gtlhislhvr.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.redwolf501.top/gthdiabisl.html

Go:   func add(a, b int) int
来源：http://hz.316326.xyz/gtuoaxppql.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.zycfv.cn/gtzsoksfee.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.dianchejie.cn/gtoqknbxtx.html

[C14] 泛型函数
来源：http://hz.jqgfzy.top/gtyjyrhwwv.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.dianchejie.cn/gtyfvyafgj.html

PHP:  // 无泛型
来源：http://hz.meibo888.top/gtjmwoxjas.html

JS:   // 无泛型
来源：http://hz.cheryme.top/gtmqwgjqzn.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.sufxvd.cn/gtmzsjbwoc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.daria6918.cn/gtlnngwwej.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yvedp.cn/gttennnfhb.html

Ruby: # 无泛型
来源：http://hz.jinqigufen.top/gttvizgkdf.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yuanzhike.top/gtsafalwvn.html

[C15] 解构 / 展开参数
来源：http://hz.ybcxt.top/gtplbzmgpv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.xuetiantiany.cn/gtxouzgvwd.html

PHP:  [$a, $b] = $pair;
来源：http://hz.gotoacloud.top/gtjmfvjcjv.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.snrcjt.cn/gtwumnwiio.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yj202588.top/gtgwhbrlah.html

Java: // 无解构
来源：http://hz.nanxinkj.top/gtwcvfvnfe.html

Go:   // 无解构
来源：http://hz.52xcode.cn/gtgvbklpji.html

Ruby: a, b = pair
来源：http://hz.hongshengwenyu.top/gtbnxgyhlc.html

C#:   var (a, b) = pair;
来源：http://hz.jinyuanbaomall.cn/gtxcfwqukt.html

[C16] 函数 / 方法重载
来源：http://hz.cashguo.top/gtqbflkobb.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.daxiang520.top/gtxnxfjbyg.html

PHP:  // 无重载
来源：http://hz.zhixingplan.top/gtqynrnvkb.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.chenlongwang.top/gtanyiqlrr.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.svipenyu.cn/gtpefcwaux.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yangfankeji.com/gtcyqxpdxf.html

Go:   // 无重载：用不同函数名
来源：http://hz.jinqigufen.top/gtvdudzgfe.html

Ruby: # 无重载：靠动态参数
来源：http://hz.shuidangran.top/gtszslluhi.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.0kj1m.cn/gtwdlhakab.html

================================================================================
来源：http://hz.nwbrower.top/gtfyqrctcu.html

D. 数组 / 列表 / 集合
来源：http://hz.chenjidiqi.icu/gtbtauxglw.html

================================================================================
来源：http://hz.haohaochexian.top/gtyllywezo.html

[D01] 创建数组 / 列表
来源：http://hz.cqqwz.cn/gtaigfekkw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.xuanzx.com/gtohqusitp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.gogol.net.cn/gtudwzbdad.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.zhiwuduotai.top/gtymeyijvv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.pycfn.com/gtxjkgqkyg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.meibo888.top/gtyzkaupyv.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.dashuyun.cn/gtanasbotx.html

Ruby: arr = [1, 2, 3]
来源：http://hz.hongshengwenyu.top/gtxrdkpxkg.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.zhengqikj.top/gtyeksgbgg.html

[D02] 追加元素到末尾
来源：http://hz.tian-w.cn/gtmpqtkcmq.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.yueranfly.top/gtnfrfjzxs.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.zhaomingkeji.xyz/gtttjtypjs.html

JS:   arr.push(4);
来源：http://hz.yangfankeji.com/gttmlraydm.html

TS:   arr.push(4);
来源：http://hz.pengpengdd.cyou/gtrcwbezti.html

Java: list.add(4);
来源：http://hz.nanxinkj.top/gtsvcrhrtm.html

Go:   arr = append(arr, 4)
来源：http://hz.gogol.net.cn/gtphxmjnsk.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.ivvv.top/gthppplwhz.html

C#:   list.Add(4);
来源：http://hz.sweek.top/gtvavnfnha.html

[D03] 在指定位置插入元素
来源：http://hz.jqgufenzy.top/gtmpolaxqe.html

Py:   arr.insert(0, 0)
来源：http://hz.zdqjudy.top/gtpersbjow.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.mhx1999.top/gtjizbhaoe.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.nwbrower.top/gtqyrbmbaq.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.cucudq.cn/gtlrgedfid.html

Java: list.add(0, 0);
来源：http://hz.pycfn.com/gtgdgqmzkv.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.shanyushiyangtech.top/gtsxgpypns.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.cqqwz.cn/gtzupjlbtt.html

C#:   list.Insert(0, 0);
来源：http://hz.ydzc1.top/gtsjysftbe.html

[D04] 删除元素
来源：http://hz.hfpthk.cn/gtahrsliyb.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.ppjwa.cn/gtlrwmblel.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.c1oappe.top/gtjsqflxgj.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.cucudq.cn/gtfsvvaitj.html

TS:   arr.splice(0, 1);
来源：http://hz.jqgfzy.top/gtrduqpiyn.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.daria6918.cn/gtxerttcvv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.shanyushiyangkeji.top/gtnskedirc.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.yongpay.top/gtjeibznrf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.nwbrower.top/gtdkzxvmgn.html

[D05] 访问与修改元素
来源：http://hz.hywenlv.cn/gtmbdxtvzf.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.gaohongyu789.top/gtizunuwmf.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.ivvv.top/gtnexuqkhp.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.hfpthk.cn/gtvtdvoryn.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.ivvv.top/gthquockdt.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yangfankeji.com/gtuxsoxatk.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.zhongyouzk.top/gthtfxabne.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jinghuilouyu.cn/gtjqdwcxby.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.xuanzx.com/gtasknnobf.html

[D06] 数组长度
来源：http://hz.sufxvd.cn/gtuxolfipe.html

Py:   len(arr)
来源：http://hz.snrcjt.cn/gtyzgnuncy.html

PHP:  count($arr);
来源：http://hz.yuxming.cn/gtssmausrh.html

JS:   arr.length
来源：http://hz.gaohongyu789.top/gtwwkjmgnx.html

TS:   arr.length
来源：http://hz.shuidangran.top/gtgxfdgpwg.html

Java: list.size();
来源：http://hz.shanyushiyangtech.top/gtpjgyvpgf.html

Go:   len(arr)
来源：http://hz.yongpay.top/gtarbvrjsi.html

Ruby: arr.length; arr.size
来源：http://hz.aizwys.cn/gtisyueugo.html

C#:   list.Count;
来源：http://hz.yongpay.top/gtgmyukraz.html

[D07] 切片 / 取子数组
来源：http://hz.sufxvd.cn/gtavoocggy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jinghuilouyu.cn/gtvnlqygbb.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.hnxiangtu.top/gtxyxfvzko.html

JS:   arr.slice(1, 4);
来源：http://hz.zhixingplan.top/gttslimqce.html

TS:   arr.slice(1, 4);
来源：http://hz.mhx1999.top/gtffunvdpa.html

Java: list.subList(1, 4);
来源：http://hz.yuanzhike.top/gtkzgolqxb.html

Go:   arr[1:4]
来源：http://hz.hywenlv.cn/gtqovbosre.html

Ruby: arr[1, 3]
来源：http://hz.hongshengwenyu.top/gtdahegajj.html

C#:   list.GetRange(1, 3);
来源：http://hz.hywenlv.cn/gtselqkeyi.html

[D08] 合并两个数组
来源：http://hz.shanyushiyangtech.top/gtsiklsupg.html

Py:   a + b;  a.extend(b)
来源：http://hz.gzhubu.top/gtzidkqgei.html

PHP:  array_merge($a, $b);
来源：http://hz.dashuyun.cn/gtagfnsrub.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.zhaomingkeji.xyz/gtqcxulnid.html

TS:   [...a, ...b];
来源：http://hz.gogol.net.cn/gtqzuobyis.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.xuetiantiany.cn/gtktmgypac.html

Go:   append(a, b...)
来源：http://hz.shangyingyoupin.top/gthfrsxolp.html

Ruby: a + b;  a.concat(b)
来源：http://hz.redwolf501.top/gtazviktog.html

C#:   a.Concat(b).ToList()
来源：http://hz.sufxvd.cn/gtyoguthtg.html

[D09] 排序（升序）
来源：http://hz.yangfankeji.com/gtgezldyhc.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.vqdsnc.cn/gtsqhcxyyq.html

PHP:  sort($arr);
来源：http://hz.cucudq.cn/gtlvoudzdj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.zhiwuduotai.top/gtuzchnavj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.ywan-chungtsiang.top/gtanqqugmv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.ydzc1.top/gtgaqzbbsm.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.svipenyu.cn/gtoovbvpsl.html

Ruby: arr.sort
来源：http://hz.aibaodan.cn/gtnvtegopf.html

C#:   list.Sort();
来源：http://hz.ywan-chungtsiang.top/gtaknyyngz.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.xingfuxueyuan.xyz/gtcgtajkxw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.hywenlv.cn/gtcfazhhxt.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yuanzhike.top/gtnwbdzivi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.hammf.cn/gtakksbvnp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yvedp.cn/gtchdfizpl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.sweek.top/gtkjwptbzr.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.gzhubu.top/gtrkdrfnqm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.xuetiantiany.cn/gtrtffppma.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.gzhubu.top/gtpekihjkt.html

[D11] 反转数组
来源：http://hz.yj20258888.top/gtmsjlwvkr.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zhengqikj.top/gtvqkcdoki.html

PHP:  array_reverse($arr);
来源：http://hz.kuanghao11.cn/gtfsgrnian.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jinqigufen.top/gtuzkyqjmr.html

TS:   [...arr].reverse();
来源：http://hz.tian-w.cn/gtabbdchlb.html

Java: Collections.reverse(list);
来源：http://hz.jinqigufen.top/gtckefooao.html

Go:   slices.Reverse(arr)
来源：http://hz.gaohongyu789.top/gtrdkryryz.html

Ruby: arr.reverse
来源：http://hz.tian-w.cn/gtqmzajztp.html

C#:   list.Reverse();
来源：http://hz.jiagoushi.top/gtadmjnoya.html

[D12] 查找元素下标
来源：http://hz.svipenyu.cn/gthmodinua.html

Py:   arr.index(x);  x in arr
来源：http://hz.chenlongwang.top/gtpkdxygai.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.pycfn.com/gtonhdftgb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.daxiang520.top/gtixqneztf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.daria6918.cn/gtruyljtlo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.zhijiandao.cn/gtmbyjdtrn.html

Go:   slices.Index(arr, x)
来源：http://hz.jinyuanbaomall.cn/gtdeljlgxo.html

Ruby: arr.index(x)
来源：http://hz.chenlongwang.top/gtjjrzetyt.html

C#:   list.IndexOf(x);
来源：http://hz.hammf.cn/gtrvnksndk.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zdqjudy.top/gtzgaqfkyi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.yj20258888.top/gtyjhjhowv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yongpay.top/gtlfilcbsa.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yueranfly.top/gtedyafvll.html

TS:   arr.filter(x => x > 3)
来源：http://hz.xinyue.icu/gtmogysdqt.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.pengpengdd.cyou/gteckawbud.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.xuetiantiany.cn/gtewtwwnge.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.sufxvd.cn/gttpvgodwi.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.chenzaomai.com/gtovmefctl.html

[D14] 映射转换（每个元素变形）
来源：http://hz.gotoacloud.top/gtmcxnwxvb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.sysykeji.top/gtfaftpslw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yj202588.top/gtojajpebg.html

JS:   arr.map(x => x * 2)
来源：http://hz.xylfe.cn/gtkqrwgrvv.html

TS:   arr.map(x => x * 2)
来源：http://hz.guannengcc.top/gtibxfmzxt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jianghu66.top/gtauoyysai.html

Go:   // 手写循环
来源：http://hz.yangfankeji.com/gttldepdjs.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.aizwys.cn/gtubhjzxiy.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.cashguo.top/gtngzgxpwb.html

[D15] 去重
来源：http://hz.yvedp.cn/gtggcndqhx.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.ehwqpu.com/gtmclsmchl.html

PHP:  array_unique($arr);
来源：http://hz.cqqwz.cn/gtopmtwbzl.html

JS:   [...new Set(arr)]
来源：http://hz.fzhhl.top/gtfqcfydrr.html

TS:   [...new Set(arr)]
来源：http://hz.fzhhl.top/gtljggietu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.gotoacloud.top/gtttpjffxb.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.nwbrower.top/gtsshqmatx.html

Ruby: arr.uniq
来源：http://hz.xinyue.icu/gtctysjhcy.html

C#:   list.Distinct().ToList()
来源：http://hz.daxiang520.top/gtolhrpqrl.html

[D16] 求和与平均值
来源：http://hz.shzxlz.cn/gtlxywafrg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.nwbrower.top/gtptqodrhx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yonumen.top/gtebnfwgsj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zdqjudy.top/gtjcavshsf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.aizwys.cn/gtycpfylwk.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.haohaochexian.top/gtshidznya.html

Go:   // 手写循环累加
来源：http://hz.cdnleiting.top/gtozrtqslb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.hammf.cn/gtsfyggkhr.html

C#:   list.Sum();  list.Average()
来源：http://hz.yueranfly.top/gtdimaumny.html

[D17] 最大值与最小值
来源：http://hz.yvedp.cn/gtchwyykuv.html

Py:   max(arr);  min(arr)
来源：http://hz.meibo888.top/gtudrdaebb.html

PHP:  max($arr);  min($arr);
来源：http://hz.cucudq.cn/gtakjyatcv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.9152youxi.cn/gtbwsmwrnm.html

TS:   Math.max(...arr);
来源：http://hz.kuanghao11.cn/gtpbxpddnd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jinqigfzy.top/gthpfcrabi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jlsjyb.cn/gtinghthvy.html

Ruby: arr.max;  arr.min
来源：http://hz.mhx1999.top/gtjzecvvre.html

C#:   list.Max();  list.Min()
来源：http://hz.316326.xyz/gtqbhbneik.html

[D18] 扁平化嵌套数组
来源：http://hz.iojbl.cn/gtikqwuhhg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.gaohongyu789.top/gtdipizczc.html

PHP:  array_merge(...$nested);
来源：http://hz.nanxinkj.top/gtsaqdxcrr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.meibo888.top/gtztwbcypb.html

TS:   nested.flat();
来源：http://hz.guannengcc.top/gtyjikgdyb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.dashuyun.cn/gtgwvsjhuz.html

Go:   // 手写双层循环
来源：http://hz.9152youxi.cn/gtlxqxsmnz.html

Ruby: nested.flatten
来源：http://hz.sxryk.cn/gtnursebdi.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.chenlongwang.top/gtdvumoyor.html

[D19] 按字段分组
来源：http://hz.iojbl.cn/gtklrbxcmx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.quarkkingdee.top/gtvvdfogor.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.vqdsnc.cn/gtlikzgnhu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.daria6918.cn/gtzfbygkwb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.zdqjudy.top/gtrfbfthwd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yanxiufei.cn/gttltxkhxb.html

Go:   // 手写 map[string][]T
来源：http://hz.tianlin.xyz/gtjqwolecq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.jianghu66.top/gthjfwaofn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.ehwqpu.com/gtrdreraet.html

[D20] 统计每个元素出现次数
来源：http://hz.hfpthk.cn/gtuhfkuepk.html

Py:   Counter(arr)
来源：http://hz.zhongyouzk.top/gtmtuxsjwo.html

PHP:  array_count_values($arr);
来源：http://hz.ybcxt.top/gtarkqouac.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.gogol.net.cn/gtozxcvuyg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xziqi.cn/gtlqeiiaiw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.nanxinkj.top/gtzdedoefx.html

Go:   // 手写 map[T]int
来源：http://hz.kuanghao11.cn/gtqxzjsosy.html

Ruby: arr.tally
来源：http://hz.snrcjt.cn/gtqffzqojn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.jqgufenzy.top/gtbjhyqmub.html

[D21] 判断是否包含某元素
来源：http://hz.wangshuangyany.cn/gtyyieybti.html

Py:   x in arr
来源：http://hz.guannengcc.top/gtzfzzaujm.html

PHP:  in_array($x, $arr, true);
来源：http://hz.andypj.xyz/gtmqrvxfrv.html

JS:   arr.includes(x)
来源：http://hz.yj20258.top/gtfvqaaktv.html

TS:   arr.includes(x)
来源：http://hz.xingfuxueyuan.xyz/gtkmflijla.html

Java: list.contains(x)
来源：http://hz.c1oappe.top/gtzjlaghhp.html

Go:   slices.Contains(arr, x)
来源：http://hz.gotoacloud.top/gtdrenfppu.html

Ruby: arr.include?(x)
来源：http://hz.shzxlz.cn/gtggblvazq.html

C#:   list.Contains(x)
来源：http://hz.ydzc1.top/gtsvcjhfey.html

[D22] 复制数组（避免共享引用）
来源：http://hz.kuanghao11.cn/gtbpdaoweg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.xuanzx.com/gtufmkcawx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.ydzc1.top/gtmvskhdnl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.chenlongwang.top/gtsskzhnyr.html

TS:   [...arr];
来源：http://hz.xuetiantiany.cn/gtpfhhdepv.html

Java: new ArrayList<>(list);
来源：http://hz.xinyue.icu/gtyrqmegmv.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.iojbl.cn/gtfsswtair.html

Ruby: arr.dup;  arr.clone
来源：http://hz.nanxuanxn.top/gtrpnrvpjm.html

C#:   new List<int>(list);
来源：http://hz.redwolf501.top/gttmqygany.html

[D23] reduce 累积计算
来源：http://hz.zhaomingkeji.xyz/gtnhascchs.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.daxiang520.top/gtftrjhkoh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.hysaishi.cn/gtyfoemfcx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cdnleiting.top/gtvimynibm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.tianlin.xyz/gtivrtlhor.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.haohaochexian.top/gtjzxenpju.html

Go:   // 手写循环
来源：http://hz.xingfuxueyuan.xyz/gtifyrlbur.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.zhengqikj.top/gthgsrkhym.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.iojbl.cn/gtikuaubzx.html

[D24] 字典 / Map 基本操作
来源：http://hz.hnqzz.top/gttkkliwpx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.quarkkingdee.top/gtswirrplu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.wangshuangyany.cn/gtdpadyaxy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.shuidangran.top/gtfkkwcvwj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.svipenyu.cn/gtuvxajlqm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.daria6918.cn/gtbqqajdwp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.daria6918.cn/gtpddcsrmp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.yanxiufei.cn/gtxkhbsiue.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jqgfzy.top/gtippzlnzw.html

[D25] Set 集合去重与交并差
来源：http://hz.ivvv.top/gtadmxfxxn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zhiwuduotai.top/gtbsicestd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.zdqjudy.top/gtjcjbkbby.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.chenjidiqi.icu/gtxauaihgn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.gogol.net.cn/gtspvbeipl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.xylfe.cn/gtdtbweekr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.fzhhl.top/gtjijgyayy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.xylfe.cn/gtycnjkqsu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.316326.xyz/gttklrmlck.html

[D26] 数组转字符串
来源：http://hz.feifeiyinyue.top/gtsorymkbg.html


<!-- 参考信息 -->