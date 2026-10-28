代发 wailian999

C#:   块级作用域
来源：http://hz.ivvv.top/gtkkntsoyo.html

[C11] 模块导入与导出
来源：http://hz.svipenyu.cn/gtydcdgryv.html

Py:   from module import func
来源：http://hz.xylfe.cn/gtjxskajom.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.cqqwz.cn/gtzloxttax.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.hnqzz.top/gtoasbltkx.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.daria6918.cn/gtilkzvzoh.html

Java: import java.util.List;
来源：http://hz.aibaodan.cn/gtbiuyroes.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.zhijiandao.cn/gthfacswzk.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.hongshengwenyu.top/gtwshixtck.html

C#:   using System.Text;
来源：http://hz.chenzaomai.com/gtdrwcgbhb.html

[C12] 立即执行函数 IIFE
来源：http://hz.feifeiyinyue.top/gtsvtpbxsi.html

Py:   (lambda: print("run"))()
来源：http://hz.zhiwuduotai.top/gtrsiibywm.html

PHP:  (function () { echo "run"; })();
来源：http://hz.0kj1m.cn/gtqibiaaiu.html

JS:   (() => { console.log("run"); })();
来源：http://hz.jinqigfzy.top/gtavuxuxwk.html

TS:   (() => { console.log("run"); })();
来源：http://hz.yj20258888.top/gtzwubxyxx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yvedp.cn/gtgbxpybbg.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.xziqi.cn/gtrdirgbxl.html

Ruby: -> { puts "run" }.call
来源：http://hz.shuidangran.top/gtpqasiryg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.316326.xyz/gtdsbkvala.html

[C13] 类型声明 / 类型注解
来源：http://hz.yangfankeji.com/gtsebrpbrf.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.chenjidiqi.icu/gtmlrglzgi.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.zhiwuduotai.top/gtfhhutgml.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.svipenyu.cn/gtwktxylff.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.yongpay.top/gtvsppgokt.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.daria6918.cn/gtdabgarch.html

Go:   func add(a, b int) int
来源：http://hz.fengsongda.top/gtchastiss.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.gzhubu.top/gtccaknyxo.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.shanyushiyangtech.top/gtkwqdlexy.html

[C14] 泛型函数
来源：http://hz.haohaochexian.top/gtbjmrgxtp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.bjfxy.top/gtsvwoyypg.html

PHP:  // 无泛型
来源：http://hz.ywan-chungtsiang.top/gtocwzklpy.html

JS:   // 无泛型
来源：http://hz.chenjidiqi.icu/gtavvslvfw.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.guowangkeji.top/gtttdifpvr.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.fengsongda.top/gtbhgwfide.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.c1oappe.top/gtiorzexcj.html

Ruby: # 无泛型
来源：http://hz.havefunace.top/gtnpsokcpr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.ywan-chungtsiang.top/gtcctxansm.html

[C15] 解构 / 展开参数
来源：http://hz.zhijiandao.cn/gtbjaypsrp.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yvedp.cn/gtrwlpucdt.html

PHP:  [$a, $b] = $pair;
来源：http://hz.sufxvd.cn/gtycbswngq.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.chenjidiqi.icu/gtckfyobkl.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.yanxiufei.cn/gtuashhfiz.html

Java: // 无解构
来源：http://hz.daxiang520.top/gtmnwuzxos.html

Go:   // 无解构
来源：http://hz.jinyuanbaomall.cn/gturzdhava.html

Ruby: a, b = pair
来源：http://hz.yuanzhike.top/gtgbhkgsoz.html

C#:   var (a, b) = pair;
来源：http://hz.zhengqikj.top/gtaogmxqxc.html

[C16] 函数 / 方法重载
来源：http://hz.yueranfly.top/gtyehsyjby.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.zycfv.cn/gtbenvmsmp.html

PHP:  // 无重载
来源：http://hz.smart0.xyz/gtgpjxtcuj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jinqigfzy.top/gtqyfgzcfy.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.zhongyouzk.top/gtwvycpbgs.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yangfankeji.com/gtnqxiuucw.html

Go:   // 无重载：用不同函数名
来源：http://hz.pycfn.com/gtimdnxycd.html

Ruby: # 无重载：靠动态参数
来源：http://hz.sufxvd.cn/gtjyiuoubw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.wangdashe.top/gtqvqwurlf.html

================================================================================
来源：http://hz.chenzaomai.com/gtsstrrefv.html

D. 数组 / 列表 / 集合
来源：http://hz.zhijiandao.cn/gtrhdlhaie.html

================================================================================
来源：http://hz.havefunace.top/gtuwfzckpv.html

[D01] 创建数组 / 列表
来源：http://hz.quarkkingdee.top/gtoylgtors.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.tanke756.top/gtuqlvexub.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yonumen.top/gtnieagxft.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.jinqigufen.top/gtqyxfwhpz.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.sweek.top/gteffcwgby.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.jinghuilouyu.cn/gtcfowhjpr.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.sweek.top/gthtekzjub.html

Ruby: arr = [1, 2, 3]
来源：http://hz.xylfe.cn/gtoubtvjnl.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.zhaomingkeji.xyz/gtcmcdpjuw.html

[D02] 追加元素到末尾
来源：http://hz.jyoumei.cn/gtwyprnfnu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.ydjk.org.cn/gtnbdwbqpa.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.hywenlv.cn/gtfnodjtcp.html

JS:   arr.push(4);
来源：http://hz.jyoumei.cn/gtymqhbuvv.html

TS:   arr.push(4);
来源：http://hz.ywan-chungtsiang.top/gtfruwptio.html

Java: list.add(4);
来源：http://hz.kuanghao11.cn/gtajdblqtg.html

Go:   arr = append(arr, 4)
来源：http://hz.sxryk.cn/gteolneqgv.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.ppjwa.cn/gtsnpwawhx.html

C#:   list.Add(4);
来源：http://hz.tian-w.cn/gtltoigadv.html

[D03] 在指定位置插入元素
来源：http://hz.xuanzx.com/gticjpdxyn.html

Py:   arr.insert(0, 0)
来源：http://hz.zycfv.cn/gtnjdzifgk.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.bjfxy.top/gthewioddy.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.jqgfzy.top/gtbgcjfymz.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.hysaishi.cn/gtwademqbw.html

Java: list.add(0, 0);
来源：http://hz.zhaomingkeji.xyz/gteafunlnk.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.andypj.xyz/gtickbvmce.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.sysykeji.top/gtrczyxfxx.html

C#:   list.Insert(0, 0);
来源：http://hz.xziqi.cn/gtxlzbmvvq.html

[D04] 删除元素
来源：http://hz.cucudq.cn/gteynczxol.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.316326.xyz/gtqgazlobm.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zhijiandao.cn/gtdcfculiy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.hongshengwenyu.top/gtztsfrnpi.html

TS:   arr.splice(0, 1);
来源：http://hz.ivvv.top/gttjvqzxso.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.xinyue.icu/gtcuwybtzg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.andypj.xyz/gtqgzjzxbz.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jiagoushi.top/gtckyfsbnf.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.cucudq.cn/gthitmmpop.html

[D05] 访问与修改元素
来源：http://hz.havefunace.top/gtptiarggc.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.vqdsnc.cn/gtlwnpqsal.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.jlsjyb.cn/gtvhqxfkkr.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.sysykeji.top/gtpythmwcy.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.shanyushiyangkeji.top/gtzzwoxxgl.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.shanyushiyangkeji.top/gtppwancqp.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.hongshengwenyu.top/gtrliwpvxz.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.quarkkingdee.top/gthvxgqcyp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.ivvv.top/gtzyhgtsxr.html

[D06] 数组长度
来源：http://hz.zhongyouzk.top/gtqjvzibtd.html

Py:   len(arr)
来源：http://hz.xziqi.cn/gtrgzvnhxm.html

PHP:  count($arr);
来源：http://hz.snrcjt.cn/gtghxpcpkm.html

JS:   arr.length
来源：http://hz.shuidangran.top/gtnvvruwdw.html

TS:   arr.length
来源：http://hz.jianghu66.top/gtyhsfqbou.html

Java: list.size();
来源：http://hz.hnqzz.top/gtsqektled.html

Go:   len(arr)
来源：http://hz.guowangkeji.top/gttcjurdtn.html

Ruby: arr.length; arr.size
来源：http://hz.wangdashe.top/gtpfdhfiay.html

C#:   list.Count;
来源：http://hz.jinqigufen.top/gtovgpyagy.html

[D07] 切片 / 取子数组
来源：http://hz.yj20258.top/gtbyjijqri.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.sysykeji.top/gthegufaqy.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.daria6918.cn/gtaahrmcuq.html

JS:   arr.slice(1, 4);
来源：http://hz.zhaomingkeji.xyz/gtbhtngjyu.html

TS:   arr.slice(1, 4);
来源：http://hz.mhx1999.top/gtptfrojgp.html

Java: list.subList(1, 4);
来源：http://hz.jqgufenzy.top/gticcxpbhj.html

Go:   arr[1:4]
来源：http://hz.tanke756.top/gteiafvljp.html

Ruby: arr[1, 3]
来源：http://hz.jinyuanbaomall.cn/gtnxorween.html

C#:   list.GetRange(1, 3);
来源：http://hz.xuetiantiany.cn/gtlaedenuw.html

[D08] 合并两个数组
来源：http://hz.kuanghao11.cn/gtrdmndprb.html

Py:   a + b;  a.extend(b)
来源：http://hz.yj20258.top/gtecxlxieb.html

PHP:  array_merge($a, $b);
来源：http://hz.cheryme.top/gtwqrtqjrf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.dashuyun.cn/gtjvzmipcw.html

TS:   [...a, ...b];
来源：http://hz.shanyushiyangkeji.top/gttngcbexo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.ybcxt.top/gtolyvsypt.html

Go:   append(a, b...)
来源：http://hz.jianghu66.top/gtyxmujpmp.html

Ruby: a + b;  a.concat(b)
来源：http://hz.vqdsnc.cn/gtuepxpczu.html

C#:   a.Concat(b).ToList()
来源：http://hz.zhaomingkeji.xyz/gtliwnkwqf.html

[D09] 排序（升序）
来源：http://hz.9152youxi.cn/gtqoxmkvsv.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gotoacloud.top/gtpxacoerb.html

PHP:  sort($arr);
来源：http://hz.c1oappe.top/gtkwpknpmz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.sweek.top/gterupwosd.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.guowangkeji.top/gtguffgbcv.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.xuetiantiany.cn/gtowczynmi.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.tanke756.top/gtrzvqiedx.html

Ruby: arr.sort
来源：http://hz.yuxming.cn/gtqmttkyzq.html

C#:   list.Sort();
来源：http://hz.yuanzhike.top/gtckurenrv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.dashuyun.cn/gtjfpwctnr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yuanzhike.top/gtdgtcaiyk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.quarkkingdee.top/gtxrjlfxlf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ivvv.top/gthvgbvtqy.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.sxryk.cn/gtrvqehkgy.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.chenzaomai.com/gtpvemafqx.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.c1oappe.top/gtywfeorzn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.xinyue.icu/gtdzxxnqjx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.iojbl.cn/gtiwnjqouj.html

[D11] 反转数组
来源：http://hz.aizwys.cn/gtipyisaza.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.guowangkeji.top/gtptfiacvz.html

PHP:  array_reverse($arr);
来源：http://hz.yvedp.cn/gtgcxfuvkt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.cashguo.top/gtxnvrjuwt.html

TS:   [...arr].reverse();
来源：http://hz.daria6918.cn/gtuyubtfdg.html

Java: Collections.reverse(list);
来源：http://hz.nwbrower.top/gtlzqhgowy.html

Go:   slices.Reverse(arr)
来源：http://hz.xziqi.cn/gtzenvkyip.html

Ruby: arr.reverse
来源：http://hz.shzxlz.cn/gtgoiomhdi.html

C#:   list.Reverse();
来源：http://hz.aibaodan.cn/gtvnfqpvkz.html

[D12] 查找元素下标
来源：http://hz.jqgfzy.top/gtbavnagkz.html

Py:   arr.index(x);  x in arr
来源：http://hz.nanxinkj.top/gtigqdjcyk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.pycfn.com/gtpiovykee.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hnxiangtu.top/gtkuveppfq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.daria6918.cn/gtqykjdlwa.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yj20258.top/gttykthazm.html

Go:   slices.Index(arr, x)
来源：http://hz.shzxlz.cn/gtvpqtmnlb.html

Ruby: arr.index(x)
来源：http://hz.daria6918.cn/gtoktmfwwj.html

C#:   list.IndexOf(x);
来源：http://hz.zdqjudy.top/gtwlsmzhdx.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zhongyouzk.top/gtinsjdjqd.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.gogol.net.cn/gttggliqhv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.zycfv.cn/gtekzffwmx.html

JS:   arr.filter(x => x > 3)
来源：http://hz.sufxvd.cn/gtwwfdwijb.html

TS:   arr.filter(x => x > 3)
来源：http://hz.hysaishi.cn/gtlzfulpdg.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.iojbl.cn/gtmrgynydk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.cashguo.top/gtvaprwksr.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jinqigufen.top/gthfenaukb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jlsjyb.cn/gtxvniwmfe.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yuanzhike.top/gtbuknieub.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.meibo888.top/gtyrpyjnzl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.ywan-chungtsiang.top/gtkylepdbv.html

JS:   arr.map(x => x * 2)
来源：http://hz.chenzaomai.com/gtqxgkzuvj.html

TS:   arr.map(x => x * 2)
来源：http://hz.yj20258888.top/gtauxjmeku.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yj20258888.top/gtszolpydb.html

Go:   // 手写循环
来源：http://hz.yangfankeji.com/gtalcyyrsf.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.gzhubu.top/gtailjabev.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yongpay.top/gtsjcmbjbb.html

[D15] 去重
来源：http://hz.haohaochexian.top/gtxqdwkzff.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jqgufenzy.top/gtyezjnqnt.html

PHP:  array_unique($arr);
来源：http://hz.daria6918.cn/gtewiahwnt.html

JS:   [...new Set(arr)]
来源：http://hz.cdnleiting.top/gthcwdzqgg.html

TS:   [...new Set(arr)]
来源：http://hz.hfpthk.cn/gtpvjsziml.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jqgfzy.top/gtiryevbhb.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.gotoacloud.top/gtnwyfzcsk.html

Ruby: arr.uniq
来源：http://hz.smart0.xyz/gteihmiial.html

C#:   list.Distinct().ToList()
来源：http://hz.sysykeji.top/gtvqfbjnws.html

[D16] 求和与平均值
来源：http://hz.xuanzx.com/gthdvfdlvt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.zhoulong.xyz/gtocolmoir.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yj202588.top/gtclwygvit.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ydjk.org.cn/gtwszsnsgq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhoulong.xyz/gtcpjkzxis.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.tian-w.cn/gtfkoudbpt.html

Go:   // 手写循环累加
来源：http://hz.nwbrower.top/gtofrxjzhy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhijiandao.cn/gthosgvbxt.html

C#:   list.Sum();  list.Average()
来源：http://hz.havefunace.top/gtpskbzmen.html

[D17] 最大值与最小值
来源：http://hz.redwolf501.top/gtulxdhuni.html

Py:   max(arr);  min(arr)
来源：http://hz.zycfv.cn/gtscxrswwk.html

PHP:  max($arr);  min($arr);
来源：http://hz.daria6918.cn/gtrsjmpzrz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.ppjwa.cn/gtaabswscx.html

TS:   Math.max(...arr);
来源：http://hz.daria6918.cn/gtbkccswxf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yanxiufei.cn/gtxtjqchws.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yj20258.top/gtpqjgpxoo.html

Ruby: arr.max;  arr.min
来源：http://hz.snrcjt.cn/gtxtcfoygi.html

C#:   list.Max();  list.Min()
来源：http://hz.fengsongda.top/gtbbcaksmw.html

[D18] 扁平化嵌套数组
来源：http://hz.chenzaomai.com/gtuiugfmlv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.tanke756.top/gtzcoeeujg.html

PHP:  array_merge(...$nested);
来源：http://hz.jinqigfzy.top/gtkpqdouwy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.shuidangran.top/gttqlccvag.html

TS:   nested.flat();
来源：http://hz.jinghuilouyu.cn/gtwwxfgcgc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yuanzhike.top/gtwkoqowrz.html

Go:   // 手写双层循环
来源：http://hz.quarkkingdee.top/gtemwezmif.html

Ruby: nested.flatten
来源：http://hz.tianlin.xyz/gtlrdurvdw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.mhx1999.top/gtgbbhxyds.html

[D19] 按字段分组
来源：http://hz.shzxlz.cn/gtovndwdhm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.bjfxy.top/gtbrvdcvhg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yonumen.top/gtyxpnyyde.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.svipenyu.cn/gtzlybukvb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.nanxuanxn.top/gtwfmjotke.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zdqjudy.top/gtyrjibzfk.html

Go:   // 手写 map[string][]T
来源：http://hz.hysaishi.cn/gtsjswvkjg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.zycfv.cn/gtuqsirwdn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yj20258.top/gtvxvahxaa.html

[D20] 统计每个元素出现次数
来源：http://hz.hywenlv.cn/gtszafcrax.html

Py:   Counter(arr)
来源：http://hz.jinqigufen.top/gtollcdlyn.html

PHP:  array_count_values($arr);
来源：http://hz.aibaodan.cn/gteafrkaku.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zycfv.cn/gtvqnlcaux.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yuxming.cn/gtcoxpvgtx.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.shzxlz.cn/gtsmedjuup.html

Go:   // 手写 map[T]int
来源：http://hz.9152youxi.cn/gthgbjwjtk.html

Ruby: arr.tally
来源：http://hz.meibo888.top/gtfpuguajv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.shanyushiyangkeji.top/gtkcdbeazm.html

[D21] 判断是否包含某元素
来源：http://hz.yanxiufei.cn/gtnpsogymf.html

Py:   x in arr
来源：http://hz.0kj1m.cn/gtkjmbyltq.html

PHP:  in_array($x, $arr, true);
来源：http://hz.redwolf501.top/gtivvvdboo.html

JS:   arr.includes(x)
来源：http://hz.jinyuanbaomall.cn/gttmjhywml.html

TS:   arr.includes(x)
来源：http://hz.52xcode.cn/gtxptkaqux.html

Java: list.contains(x)
来源：http://hz.zhengqikj.top/gttsvvbakp.html

Go:   slices.Contains(arr, x)
来源：http://hz.cucudq.cn/gtfbfttsvj.html

Ruby: arr.include?(x)
来源：http://hz.vqdsnc.cn/gtuvthdsyq.html

C#:   list.Contains(x)
来源：http://hz.ehwqpu.com/gtmgsuilfp.html

[D22] 复制数组（避免共享引用）
来源：http://hz.guowangkeji.top/gtjgaciqmp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.cheryme.top/gtjtyqevai.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.cqqwz.cn/gtzxtvycvy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.sxryk.cn/gtjvckadju.html

TS:   [...arr];
来源：http://hz.zycfv.cn/gtgadueftd.html

Java: new ArrayList<>(list);
来源：http://hz.andypj.xyz/gtmoizqmzf.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jqgfzy.top/gtxvufozbo.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zycfv.cn/gtlxiwphry.html

C#:   new List<int>(list);
来源：http://hz.daxiang520.top/gtjkxfojaz.html

[D23] reduce 累积计算
来源：http://hz.birdmap.top/gtjcrlaqqd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.tian-w.cn/gtqxktxnrm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.kuanghao11.cn/gtcvpitnlc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.guowangkeji.top/gtmiidwhyf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.9152youxi.cn/gtjlonofqj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.redwolf501.top/gtqzenkidd.html

Go:   // 手写循环
来源：http://hz.zdqjudy.top/gtoivojdec.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.daxiang520.top/gtojtoewrs.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.zhaomingkeji.xyz/gtrpylvjtg.html

[D24] 字典 / Map 基本操作
来源：http://hz.jqgfzy.top/gtfqbrduux.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.iojbl.cn/gtesflnmux.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.guannengcc.top/gtosyqiokv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jiagoushi.top/gtihhrbghc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.ybcxt.top/gtgoqhntgg.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.guannengcc.top/gtbanihmvg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.52xcode.cn/gtqjkpzwkk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.redwolf501.top/gtqgfnvqku.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.nwbrower.top/gtyoqyfall.html

[D25] Set 集合去重与交并差
来源：http://hz.zhoulong.xyz/gtqdryonzs.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.xylfe.cn/gttiolnrpj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jinghuilouyu.cn/gtpijsstvj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.dianchejie.cn/gtaehrfgna.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.zdqjudy.top/gtnehdprmd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yueranfly.top/gtcjgcxgiu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.quarkkingdee.top/gtxnfbiwwn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.shanyushiyangtech.top/gtidnasalg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yongpay.top/gtvlssbidy.html

[D26] 数组转字符串
来源：http://hz.sweek.top/gtzbcvlwdp.html

Py:   ", ".join(map(str, arr))
来源：http://hz.aizwys.cn/gtvubyjwxp.html

PHP:  implode(", ", $arr);
来源：http://hz.ybcxt.top/gtbtzkjioz.html

JS:   arr.join(", ")
来源：http://hz.hammf.cn/gttyvramcy.html

TS:   arr.join(", ")
来源：http://hz.yj20258888.top/gtvaabkzyy.html

Java: String.join(", ", list)
来源：http://hz.sufxvd.cn/gtmrsffgey.html

Go:   strings.Join(strs, ", ")
来源：http://hz.gogol.net.cn/gtgavhaimh.html

Ruby: arr.join(", ")
来源：http://hz.ppjwa.cn/gtjhwfpgnv.html

C#:   string.Join(", ", list)
来源：http://hz.jinqigufen.top/gtmadtodlf.html

================================================================================
来源：http://hz.quarkkingdee.top/gtghijbdng.html

E. 字符串处理
来源：http://hz.xuetiantiany.cn/gtdyjoqkhf.html

================================================================================
来源：http://hz.svipenyu.cn/gtnhbluyvf.html

[E01] 拼接字符串
来源：http://hz.jinqigufen.top/gtgdsxbbzu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.ehwqpu.com/gtmknzuniq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.nanxinkj.top/gtwglpferi.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hysaishi.cn/gtvdhsexsv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.dashuyun.cn/gtbaojtgae.html


<!-- 参考信息 -->