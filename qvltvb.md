代发 wailian999

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.nanxinkj.top/gtghqemxqe.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.fengsongda.top/gtaheumthz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yj202588.top/gtswyqkirc.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.xuanzx.com/gtzfsydbgm.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.xylfe.cn/gtfkwgvkpo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.tian-w.cn/gtgfttidzq.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.mhx1999.top/gtolqvrpud.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.xuanzx.com/gtgqdiedaw.html

[C10] 变量作用域
来源：http://hz.xuanzx.com/gtbowywtuk.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.birdmap.top/gticyrfhis.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.nanxinkj.top/gtgejiirpq.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.sxryk.cn/gtlgrznvwq.html

TS:   同 JS
来源：http://hz.gotoacloud.top/gtpvlzdniq.html

Java: 方法内为块级作用域
来源：http://hz.andypj.xyz/gtgwbeeqwd.html

Go:   花括号块级作用域
来源：http://hz.pycfn.com/gttgjxixvd.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yvedp.cn/gtwspwenmv.html

C#:   块级作用域
来源：http://hz.yuxming.cn/gtnuvfbqio.html

[C11] 模块导入与导出
来源：http://hz.gogol.net.cn/gtpudtlhpm.html

Py:   from module import func
来源：http://hz.ydzc1.top/gtwxizjlhc.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.shzxlz.cn/gttnhoeavv.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.xylfe.cn/gtrcofinsi.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.svipenyu.cn/gtcxhiifky.html

Java: import java.util.List;
来源：http://hz.zhixingplan.top/gtpqfyxike.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.cqqwz.cn/gtolaxuqpo.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.dashuyun.cn/gtwcypzjjx.html

C#:   using System.Text;
来源：http://hz.316326.xyz/gtcgtpgmfw.html

[C12] 立即执行函数 IIFE
来源：http://hz.hnxiangtu.top/gtvaslhbfl.html

Py:   (lambda: print("run"))()
来源：http://hz.ehwqpu.com/gthiesgumr.html

PHP:  (function () { echo "run"; })();
来源：http://hz.zhixingplan.top/gtwfblbgrs.html

JS:   (() => { console.log("run"); })();
来源：http://hz.ydzc1.top/gtbawtrbwy.html

TS:   (() => { console.log("run"); })();
来源：http://hz.cashguo.top/gtwxetcjqt.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.feifeiyinyue.top/gtqwafnezj.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.redwolf501.top/gthvjpvxit.html

Ruby: -> { puts "run" }.call
来源：http://hz.dashuyun.cn/gtyudgfaap.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.cashguo.top/gtddtlgnjm.html

[C13] 类型声明 / 类型注解
来源：http://hz.andypj.xyz/gtvwheebsa.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.hfpthk.cn/gtlmjyuwxo.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yj20258.top/gtpadaveye.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.bjfxy.top/gtjrblmija.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yangfankeji.com/gtzbwsueat.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.hfpthk.cn/gtvdtrcewv.html

Go:   func add(a, b int) int
来源：http://hz.dianchejie.cn/gtqtqopzyp.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.xingfuxueyuan.xyz/gtllqwdqbp.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.kuanghao11.cn/gtxqpcxgab.html

[C14] 泛型函数
来源：http://hz.yanxiufei.cn/gtymodahzd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.cqqwz.cn/gtsiocgnah.html

PHP:  // 无泛型
来源：http://hz.chenlongwang.top/gtwyqcipdn.html

JS:   // 无泛型
来源：http://hz.yj202588.top/gtwleghwkz.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.ydzc1.top/gtxnlgigjx.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.pycfn.com/gtqaxiwacs.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.c1oappe.top/gtsstxvwie.html

Ruby: # 无泛型
来源：http://hz.hongshengwenyu.top/gtelumvfrt.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.chenlongwang.top/gtgsiyyzkv.html

[C15] 解构 / 展开参数
来源：http://hz.bjfxy.top/gtxdoskdlv.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.xingfuxueyuan.xyz/gtfcpitjgz.html

PHP:  [$a, $b] = $pair;
来源：http://hz.jqgufenzy.top/gtgzztnpmg.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.snrcjt.cn/gtaxjllavi.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.zhijiandao.cn/gtbtogvivz.html

Java: // 无解构
来源：http://hz.dianchejie.cn/gtecwyvief.html

Go:   // 无解构
来源：http://hz.9152youxi.cn/gtytydiltl.html

Ruby: a, b = pair
来源：http://hz.shangyingyoupin.top/gtvgemgjyz.html

C#:   var (a, b) = pair;
来源：http://hz.zhaomingkeji.xyz/gtxrgyquvc.html

[C16] 函数 / 方法重载
来源：http://hz.jinqigufen.top/gtqcuxtglo.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.sxryk.cn/gtegcgigcf.html

PHP:  // 无重载
来源：http://hz.meibo888.top/gtmdhabpyr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.redwolf501.top/gtwtklfjpg.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.jinqigufen.top/gtgjfwfglu.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.nanxuanxn.top/gtodwaldpz.html

Go:   // 无重载：用不同函数名
来源：http://hz.yuxming.cn/gtweonxrvj.html

Ruby: # 无重载：靠动态参数
来源：http://hz.daria6918.cn/gtqyckxdby.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jianghu66.top/gttiaperda.html

================================================================================
来源：http://hz.xuanzx.com/gtdtmiqxxf.html

D. 数组 / 列表 / 集合
来源：http://hz.daxiang520.top/gtdadrwepj.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtvhysnosz.html

[D01] 创建数组 / 列表
来源：http://hz.pengpengdd.cyou/gtykdyaplw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.shangyingyoupin.top/gtkzglwlbc.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jinqigufen.top/gtizwewabe.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.zhijiandao.cn/gtswquchmh.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.hysaishi.cn/gtzyzlstvi.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xinyue.icu/gtqqcbbkrq.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yvedp.cn/gttzalwdjr.html

Ruby: arr = [1, 2, 3]
来源：http://hz.wangshuangyany.cn/gtaphkvqtk.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.sysykeji.top/gtxvhxtmvt.html

[D02] 追加元素到末尾
来源：http://hz.cdnleiting.top/gtyuetmxuh.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.gzhubu.top/gtsyqqdpwu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.xuetiantiany.cn/gtzptiqjpk.html

JS:   arr.push(4);
来源：http://hz.yanxiufei.cn/gtfdbqyfkl.html

TS:   arr.push(4);
来源：http://hz.cdnleiting.top/gtsvcocqek.html

Java: list.add(4);
来源：http://hz.sxryk.cn/gtfpnhidys.html

Go:   arr = append(arr, 4)
来源：http://hz.daria6918.cn/gtgrwmhqua.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.ywan-chungtsiang.top/gtrvtkqgqr.html

C#:   list.Add(4);
来源：http://hz.aizwys.cn/gtbrifbvch.html

[D03] 在指定位置插入元素
来源：http://hz.cashguo.top/gtineggwwa.html

Py:   arr.insert(0, 0)
来源：http://hz.hywenlv.cn/gtydcheoly.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jianghu66.top/gtlyxpihqz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jqgfzy.top/gtmgjzlveo.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.pengpengdd.cyou/gteimahepw.html

Java: list.add(0, 0);
来源：http://hz.iojbl.cn/gtbgnauhij.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yangfankeji.com/gtnlxhgkjj.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.zhongyouzk.top/gtlyrcauud.html

C#:   list.Insert(0, 0);
来源：http://hz.gaohongyu789.top/gtnwmgqdii.html

[D04] 删除元素
来源：http://hz.fengsongda.top/gtmfkkkyax.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.jqgfzy.top/gtuobmaoai.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.guowangkeji.top/gtujxcvfjq.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.cashguo.top/gtgelxlkzp.html

TS:   arr.splice(0, 1);
来源：http://hz.mhx1999.top/gtqapovbym.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.ydjk.org.cn/gtrzzovfgl.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.guannengcc.top/gtuzxweufv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.vqdsnc.cn/gthbwqbymp.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.ivvv.top/gtipcckemr.html

[D05] 访问与修改元素
来源：http://hz.pengpengdd.cyou/gtrvslklgl.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.cashguo.top/gtmznltuid.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.chenzaomai.com/gtfgogrspd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.zdqjudy.top/gtpravcerf.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zhiwuduotai.top/gtoazmjtac.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.nwbrower.top/gtotfmjbvu.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jinqigfzy.top/gthylokiga.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhoulong.xyz/gtyuntefad.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.c1oappe.top/gtzelizodg.html

[D06] 数组长度
来源：http://hz.haohaochexian.top/gtxnswgvwz.html

Py:   len(arr)
来源：http://hz.shanyushiyangkeji.top/gtxuwouymt.html

PHP:  count($arr);
来源：http://hz.zycfv.cn/gtmagyltki.html

JS:   arr.length
来源：http://hz.redwolf501.top/gtqdcrkepa.html

TS:   arr.length
来源：http://hz.zhoulong.xyz/gttvmjzfhc.html

Java: list.size();
来源：http://hz.52xcode.cn/gtxnhawoxu.html

Go:   len(arr)
来源：http://hz.guannengcc.top/gterjtbxae.html

Ruby: arr.length; arr.size
来源：http://hz.9152youxi.cn/gtpkuihtya.html

C#:   list.Count;
来源：http://hz.shanyushiyangkeji.top/gtpyulqzot.html

[D07] 切片 / 取子数组
来源：http://hz.yongpay.top/gthhyjvioa.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.guannengcc.top/gtbpgknpmh.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.gaohongyu789.top/gtzizjgmic.html

JS:   arr.slice(1, 4);
来源：http://hz.jlsjyb.cn/gttpytxuyp.html

TS:   arr.slice(1, 4);
来源：http://hz.sysykeji.top/gtoonvnsjz.html

Java: list.subList(1, 4);
来源：http://hz.hnxiangtu.top/gtzaugdcgj.html

Go:   arr[1:4]
来源：http://hz.xinyue.icu/gtgtumehxe.html

Ruby: arr[1, 3]
来源：http://hz.shzxlz.cn/gtzmeuvggr.html

C#:   list.GetRange(1, 3);
来源：http://hz.chenzaomai.com/gteygpllrl.html

[D08] 合并两个数组
来源：http://hz.aibaodan.cn/gtnsmqbmdz.html

Py:   a + b;  a.extend(b)
来源：http://hz.aizwys.cn/gtyfvegjni.html

PHP:  array_merge($a, $b);
来源：http://hz.jinqigufen.top/gttujlvivf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.snrcjt.cn/gtxojvzwjz.html

TS:   [...a, ...b];
来源：http://hz.tian-w.cn/gtfoyeodul.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.ydzc1.top/gtruybibma.html

Go:   append(a, b...)
来源：http://hz.hammf.cn/gtndjtciwh.html

Ruby: a + b;  a.concat(b)
来源：http://hz.guowangkeji.top/gtnujpwntg.html

C#:   a.Concat(b).ToList()
来源：http://hz.ivvv.top/gtdgancuix.html

[D09] 排序（升序）
来源：http://hz.yuanzhike.top/gtrebmjozi.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.pengpengdd.cyou/gtmzcvvdoe.html

PHP:  sort($arr);
来源：http://hz.hysaishi.cn/gtushxniwi.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.xuanzx.com/gtdvhphjjb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.xuanzx.com/gtnhbllwai.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.cdnleiting.top/gtitkazffk.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.gzhubu.top/gtzkzwngup.html

Ruby: arr.sort
来源：http://hz.wangshuangyany.cn/gtdwxnxgwk.html

C#:   list.Sort();
来源：http://hz.havefunace.top/gtdiidfcpr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.wangdashe.top/gttvclblpw.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yonumen.top/gtcsbewxwk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.svipenyu.cn/gtwpacdjws.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinyuanbaomall.cn/gtinxvjjii.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cashguo.top/gtuduwabyv.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.c1oappe.top/gtgvflaaid.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.gaohongyu789.top/gtwvhvqfmv.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.chenlongwang.top/gtxafvxblf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yueranfly.top/gtrwodpady.html

[D11] 反转数组
来源：http://hz.yanxiufei.cn/gthcsxtxcs.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.gotoacloud.top/gtdbglysfu.html

PHP:  array_reverse($arr);
来源：http://hz.hnxiangtu.top/gtifcenhjd.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.fzhhl.top/gtbwrspekm.html

TS:   [...arr].reverse();
来源：http://hz.mhx1999.top/gtjzzvnkda.html

Java: Collections.reverse(list);
来源：http://hz.ywan-chungtsiang.top/gtpbmkbfgj.html

Go:   slices.Reverse(arr)
来源：http://hz.0kj1m.cn/gtfxifgjli.html

Ruby: arr.reverse
来源：http://hz.yangfankeji.com/gtrhimryvu.html

C#:   list.Reverse();
来源：http://hz.vqdsnc.cn/gttxyvnbvq.html

[D12] 查找元素下标
来源：http://hz.iojbl.cn/gtmsbxjidl.html

Py:   arr.index(x);  x in arr
来源：http://hz.jlsjyb.cn/gtnpjmgmxf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.zhengqikj.top/gtuvnzgbll.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinqigfzy.top/gtauheamrs.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhengqikj.top/gtggufneol.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.c1oappe.top/gtcqaacyyl.html

Go:   slices.Index(arr, x)
来源：http://hz.gogol.net.cn/gtygaoegrb.html

Ruby: arr.index(x)
来源：http://hz.daria6918.cn/gtynhgusda.html

C#:   list.IndexOf(x);
来源：http://hz.havefunace.top/gtkbcctsaw.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zycfv.cn/gttmauzths.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.andypj.xyz/gtwethvtil.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.shangyingyoupin.top/gtjcjrkstn.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zhengqikj.top/gtwgoemhhj.html

TS:   arr.filter(x => x > 3)
来源：http://hz.andypj.xyz/gtimlesseo.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.shangyingyoupin.top/gtoylbzffs.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.gogol.net.cn/gtbxqwnrns.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jianghu66.top/gtrexwjwhf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.chenjidiqi.icu/gtveotfxzo.html

[D14] 映射转换（每个元素变形）
来源：http://hz.316326.xyz/gtcyftjjfy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yanxiufei.cn/gthwkqoxsk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.wangshuangyany.cn/gtpapfklkc.html

JS:   arr.map(x => x * 2)
来源：http://hz.quarkkingdee.top/gtosmulxcf.html

TS:   arr.map(x => x * 2)
来源：http://hz.0kj1m.cn/gthbburzdo.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.redwolf501.top/gtptkwefjt.html

Go:   // 手写循环
来源：http://hz.zhongyouzk.top/gtcnnzbmqw.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.shanyushiyangtech.top/gtwmidnjfu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.nwbrower.top/gteefgecln.html

[D15] 去重
来源：http://hz.pycfn.com/gtlvpfeqer.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.guannengcc.top/gtklavxrbn.html

PHP:  array_unique($arr);
来源：http://hz.jyoumei.cn/gthllkdzvt.html

JS:   [...new Set(arr)]
来源：http://hz.ppjwa.cn/gtxlkzpobz.html

TS:   [...new Set(arr)]
来源：http://hz.gaohongyu789.top/gtvlhvfffg.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.xuanzx.com/gtneufqnie.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.0kj1m.cn/gtkhmkzevq.html

Ruby: arr.uniq
来源：http://hz.fzhhl.top/gtrtcxuusm.html

C#:   list.Distinct().ToList()
来源：http://hz.jinqigfzy.top/gtgchwrcty.html

[D16] 求和与平均值
来源：http://hz.nanxuanxn.top/gthrsqtcdw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yonumen.top/gtzkspkskq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.meibo888.top/gtmqelakil.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.bjfxy.top/gtgntgxdac.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.aibaodan.cn/gtunmqztlx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.aibaodan.cn/gtxraltmbf.html

Go:   // 手写循环累加
来源：http://hz.pengpengdd.cyou/gtyyabazgh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.xuanzx.com/gtcjczavwe.html

C#:   list.Sum();  list.Average()
来源：http://hz.zhijiandao.cn/gtwaxnhmdo.html

[D17] 最大值与最小值
来源：http://hz.zhiwuduotai.top/gtgcyupinr.html

Py:   max(arr);  min(arr)
来源：http://hz.chenjidiqi.icu/gttmvsacwh.html

PHP:  max($arr);  min($arr);
来源：http://hz.sysykeji.top/gtaqmshjou.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.316326.xyz/gtkmjroxpn.html

TS:   Math.max(...arr);
来源：http://hz.jinqigfzy.top/gtwswnivjc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.vqdsnc.cn/gtrrtonuam.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.guannengcc.top/gtnrwtbuit.html

Ruby: arr.max;  arr.min
来源：http://hz.shzxlz.cn/gtvnvzmatj.html

C#:   list.Max();  list.Min()
来源：http://hz.nanxuanxn.top/gtgamyxnid.html

[D18] 扁平化嵌套数组
来源：http://hz.bjfxy.top/gtxkpsxlyd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.birdmap.top/gtwqaxvrpz.html

PHP:  array_merge(...$nested);
来源：http://hz.andypj.xyz/gtfdtxxgiw.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.cheryme.top/gtvtbvxffs.html

TS:   nested.flat();
来源：http://hz.shangyingyoupin.top/gtzfmdwxjy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.zycfv.cn/gtkuioxqvp.html

Go:   // 手写双层循环
来源：http://hz.ppjwa.cn/gtguyjzbnx.html

Ruby: nested.flatten
来源：http://hz.pycfn.com/gtnkalkxrm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zhongyouzk.top/gtnkcgqujk.html

[D19] 按字段分组
来源：http://hz.hammf.cn/gtrveuqquk.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.mhx1999.top/gtssyffumn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.aizwys.cn/gtmbltyvjc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.pycfn.com/gtiepmpuqz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.meibo888.top/gtzgexvobf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.sxryk.cn/gtujfmcfzj.html

Go:   // 手写 map[string][]T
来源：http://hz.gaohongyu789.top/gtgvqejzqp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.ydjk.org.cn/gtcefslcsa.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.mhx1999.top/gttqamkpka.html

[D20] 统计每个元素出现次数
来源：http://hz.9152youxi.cn/gtvmvleyei.html

Py:   Counter(arr)
来源：http://hz.wangdashe.top/gtelwsldct.html

PHP:  array_count_values($arr);
来源：http://hz.zycfv.cn/gtfeljiono.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.gotoacloud.top/gtitvhebij.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.mhx1999.top/gtxtfqijqn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.haohaochexian.top/gttpwppfvr.html

Go:   // 手写 map[T]int
来源：http://hz.ppjwa.cn/gtxavtbsis.html

Ruby: arr.tally
来源：http://hz.xinyue.icu/gtqijwqffe.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.wangdashe.top/gtgtrdkzmm.html

[D21] 判断是否包含某元素
来源：http://hz.chenzaomai.com/gtwcvvfoaa.html

Py:   x in arr
来源：http://hz.haohaochexian.top/gtfyasbckh.html

PHP:  in_array($x, $arr, true);
来源：http://hz.zhengqikj.top/gtrmtlchao.html

JS:   arr.includes(x)
来源：http://hz.gotoacloud.top/gtcrbsphta.html

TS:   arr.includes(x)
来源：http://hz.jyoumei.cn/gtiokyuxpm.html

Java: list.contains(x)
来源：http://hz.zhongyouzk.top/gtwltzgosp.html

Go:   slices.Contains(arr, x)
来源：http://hz.pycfn.com/gtvgsqdvoh.html

Ruby: arr.include?(x)
来源：http://hz.guowangkeji.top/gttmzzmlup.html

C#:   list.Contains(x)
来源：http://hz.redwolf501.top/gtdojwdvfo.html

[D22] 复制数组（避免共享引用）
来源：http://hz.sxryk.cn/gtnxhzumrt.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.chenlongwang.top/gtdahazipx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.sxryk.cn/gthddvscfr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yj20258.top/gtfmqssvmf.html

TS:   [...arr];
来源：http://hz.shzxlz.cn/gtiqxdbyiy.html

Java: new ArrayList<>(list);
来源：http://hz.mhx1999.top/gtuqrjziji.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.zhiwuduotai.top/gtjamzhhbw.html

Ruby: arr.dup;  arr.clone
来源：http://hz.xylfe.cn/gtgpnsfwph.html

C#:   new List<int>(list);
来源：http://hz.xylfe.cn/gtomuffctc.html

[D23] reduce 累积计算
来源：http://hz.hywenlv.cn/gtvxvyhneu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.ydzc1.top/gthhptozyh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.cheryme.top/gtkwtildbq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cdnleiting.top/gtillrfdtg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.feifeiyinyue.top/gtlqhpseyj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.zhaomingkeji.xyz/gtwngygbkq.html

Go:   // 手写循环
来源：http://hz.snrcjt.cn/gtidizvucl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.meibo888.top/gtnlgihsla.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.tianlin.xyz/gtrrcqlbgf.html

[D24] 字典 / Map 基本操作
来源：http://hz.jqgfzy.top/gtzfwoymub.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.52xcode.cn/gtmkntquko.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.wangshuangyany.cn/gtznnhjiod.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.redwolf501.top/gtffspwsjn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yj202588.top/gtyydokijc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.hongshengwenyu.top/gtzrgmfnvx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.zhaomingkeji.xyz/gtzuglloqs.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.0kj1m.cn/gtnzzvjtlf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jinqigfzy.top/gtwvensscj.html

[D25] Set 集合去重与交并差
来源：http://hz.andypj.xyz/gtvdrgdayx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.tanke756.top/gtqqrkzcrj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.chenlongwang.top/gtxezyqmdo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.gotoacloud.top/gtuziqorfh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.ehwqpu.com/gthhzfjnqi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.sufxvd.cn/gtciiinmxy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.aizwys.cn/gthidsqbfh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.nanxinkj.top/gtmudhmxue.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.gotoacloud.top/gtqiovicle.html

[D26] 数组转字符串
来源：http://hz.hysaishi.cn/gtkbdtrswu.html


<!-- 参考信息 -->