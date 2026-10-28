代发 wailian999

[C10] 变量作用域
来源：http://hz.kuanghao11.cn/gtfwoxbvom.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.0kj1m.cn/gtxkkfznya.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.xuanzx.com/gtqzjlcuoe.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.nanxuanxn.top/gtrfsbusse.html

TS:   同 JS
来源：http://hz.chenjidiqi.icu/gtmaluocik.html

Java: 方法内为块级作用域
来源：http://hz.ppjwa.cn/gtdjjcbjwx.html

Go:   花括号块级作用域
来源：http://hz.ehwqpu.com/gtrkqwsgmx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.shzxlz.cn/gthraiskrh.html

C#:   块级作用域
来源：http://hz.redwolf501.top/gtguswufwc.html

[C11] 模块导入与导出
来源：http://hz.gzhubu.top/gtltrjplmi.html

Py:   from module import func
来源：http://hz.redwolf501.top/gthlxpgprs.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.hywenlv.cn/gtfnhfxnmt.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.dianchejie.cn/gtkpnbteev.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yanxiufei.cn/gtxfriljzc.html

Java: import java.util.List;
来源：http://hz.cheryme.top/gtlxhvsdie.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.aibaodan.cn/gtctttoxsa.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yangfankeji.com/gtqillqtrc.html

C#:   using System.Text;
来源：http://hz.quarkkingdee.top/gtrneffbbu.html

[C12] 立即执行函数 IIFE
来源：http://hz.ydzc1.top/gtywsgwjjb.html

Py:   (lambda: print("run"))()
来源：http://hz.shzxlz.cn/gtehnhobhf.html

PHP:  (function () { echo "run"; })();
来源：http://hz.zhengqikj.top/gtokeknxbm.html

JS:   (() => { console.log("run"); })();
来源：http://hz.zycfv.cn/gthovrwzvp.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jlsjyb.cn/gtwfqkhtqo.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jqgufenzy.top/gtahzdzvib.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.pycfn.com/gthiflzfww.html

Ruby: -> { puts "run" }.call
来源：http://hz.shanyushiyangtech.top/gtphtyeskc.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.zhongyouzk.top/gtdtzrmkga.html

[C13] 类型声明 / 类型注解
来源：http://hz.tanke756.top/gtywxengfu.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.hysaishi.cn/gtwwahabzj.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yj202588.top/gtfgxmdilh.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.birdmap.top/gtqohhyhjf.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xziqi.cn/gtpogsdpmw.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.smart0.xyz/gtdhwbnyoh.html

Go:   func add(a, b int) int
来源：http://hz.jyoumei.cn/gtgjyqlmls.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.svipenyu.cn/gtkvsztxsr.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.smart0.xyz/gtrnpyomqt.html

[C14] 泛型函数
来源：http://hz.yangfankeji.com/gtdvnsehbp.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.cashguo.top/gtpmuanrlg.html

PHP:  // 无泛型
来源：http://hz.pycfn.com/gtvgaffhrw.html

JS:   // 无泛型
来源：http://hz.9152youxi.cn/gtdarapmut.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.shangyingyoupin.top/gthsxyropv.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.nanxuanxn.top/gtdmpuwjsv.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.nwbrower.top/gtnslbhyzy.html

Ruby: # 无泛型
来源：http://hz.wangshuangyany.cn/gtgdxmzicp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yj20258888.top/gtshoyqsze.html

[C15] 解构 / 展开参数
来源：http://hz.yangfankeji.com/gtwmqerfgq.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.0kj1m.cn/gtzvwjrbbm.html

PHP:  [$a, $b] = $pair;
来源：http://hz.aibaodan.cn/gtgnqyzzky.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.shanyushiyangtech.top/gtukqtpnbu.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.nanxuanxn.top/gtmpyjmktw.html

Java: // 无解构
来源：http://hz.316326.xyz/gtisnpefho.html

Go:   // 无解构
来源：http://hz.cqqwz.cn/gtmwftzzfh.html

Ruby: a, b = pair
来源：http://hz.xylfe.cn/gtwbntosbi.html

C#:   var (a, b) = pair;
来源：http://hz.sufxvd.cn/gtedfghjop.html

[C16] 函数 / 方法重载
来源：http://hz.jinqigfzy.top/gttvboiqbd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.ywan-chungtsiang.top/gtzapizysh.html

PHP:  // 无重载
来源：http://hz.chenzaomai.com/gtdlamxmeu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hnqzz.top/gteoxshzco.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.daria6918.cn/gtxgrvvpxa.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.chenzaomai.com/gtnwgjmvcb.html

Go:   // 无重载：用不同函数名
来源：http://hz.yuxming.cn/gtlngcomim.html

Ruby: # 无重载：靠动态参数
来源：http://hz.316326.xyz/gtvzsbjkqs.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.hongshengwenyu.top/gtfcbkmzzj.html

================================================================================
来源：http://hz.jinqigufen.top/gtgemqasgm.html

D. 数组 / 列表 / 集合
来源：http://hz.chenzaomai.com/gtzfkcrsaa.html

================================================================================
来源：http://hz.yueranfly.top/gtvfijowhr.html

[D01] 创建数组 / 列表
来源：http://hz.chenlongwang.top/gtjwhujjxo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.wangdashe.top/gtzhjkprhw.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.dashuyun.cn/gtnwhflksm.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.vqdsnc.cn/gtetrdgirv.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.zycfv.cn/gtaqmqaqfj.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.sufxvd.cn/gtiphqmvgt.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.ywan-chungtsiang.top/gtttcxdolg.html

Ruby: arr = [1, 2, 3]
来源：http://hz.tianlin.xyz/gtdocpslaf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.haohaochexian.top/gtdlyywywu.html

[D02] 追加元素到末尾
来源：http://hz.aizwys.cn/gtppzwxkpp.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.chenjidiqi.icu/gthzbuhfsb.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jinghuilouyu.cn/gtjmbqknav.html

JS:   arr.push(4);
来源：http://hz.chenlongwang.top/gtylogmnow.html

TS:   arr.push(4);
来源：http://hz.tianlin.xyz/gtyrzxpems.html

Java: list.add(4);
来源：http://hz.ehwqpu.com/gtnkddyrqb.html

Go:   arr = append(arr, 4)
来源：http://hz.ydjk.org.cn/gtifnpkqtv.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.zycfv.cn/gtynodknvz.html

C#:   list.Add(4);
来源：http://hz.ivvv.top/gtaufysghj.html

[D03] 在指定位置插入元素
来源：http://hz.yj202588.top/gtxcqntzpw.html

Py:   arr.insert(0, 0)
来源：http://hz.hnqzz.top/gtsfcezntv.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.vqdsnc.cn/gtrfmqurzk.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.shanyushiyangtech.top/gtvtvybpcd.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.cheryme.top/gtcvmkdojn.html

Java: list.add(0, 0);
来源：http://hz.chenzaomai.com/gtrmctwvfd.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.chenzaomai.com/gtjbguqioh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.pengpengdd.cyou/gteilsgzad.html

C#:   list.Insert(0, 0);
来源：http://hz.fzhhl.top/gtdkggfjuu.html

[D04] 删除元素
来源：http://hz.yangfankeji.com/gtaegzaulk.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.52xcode.cn/gtorvxoaho.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zhixingplan.top/gtkotoeerw.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.shzxlz.cn/gtsstvzlmh.html

TS:   arr.splice(0, 1);
来源：http://hz.xinyue.icu/gtfmxgakex.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.tian-w.cn/gtnszjydxh.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.guowangkeji.top/gtwygjqkmu.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.chenlongwang.top/gtklpjrfny.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.xziqi.cn/gtuowwlrtj.html

[D05] 访问与修改元素
来源：http://hz.vqdsnc.cn/gtpwzryghq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yj20258.top/gthvdvplri.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.hammf.cn/gtajionezq.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.52xcode.cn/gtvvmnibbp.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yanxiufei.cn/gtjqsjwxbc.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.ivvv.top/gthxgwspem.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.chenlongwang.top/gtqmlsiihw.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.wangdashe.top/gtxdidngsq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.sxryk.cn/gtocnkheky.html

[D06] 数组长度
来源：http://hz.cashguo.top/gthjbmqwqf.html

Py:   len(arr)
来源：http://hz.aizwys.cn/gtgoktevsz.html

PHP:  count($arr);
来源：http://hz.hysaishi.cn/gtkdcpmiol.html

JS:   arr.length
来源：http://hz.zhiwuduotai.top/gtmjyplasw.html

TS:   arr.length
来源：http://hz.birdmap.top/gtzysrklny.html

Java: list.size();
来源：http://hz.yangfankeji.com/gtsubfjukh.html

Go:   len(arr)
来源：http://hz.gzhubu.top/gtlxxhqjdj.html

Ruby: arr.length; arr.size
来源：http://hz.zycfv.cn/gttnovmkgi.html

C#:   list.Count;
来源：http://hz.sxryk.cn/gtwzrelutw.html

[D07] 切片 / 取子数组
来源：http://hz.yueranfly.top/gtuabxishn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jinqigfzy.top/gtlysulijo.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.mhx1999.top/gtnljbchzv.html

JS:   arr.slice(1, 4);
来源：http://hz.shanyushiyangtech.top/gtpgrqdyjn.html

TS:   arr.slice(1, 4);
来源：http://hz.guowangkeji.top/gtiynqboyp.html

Java: list.subList(1, 4);
来源：http://hz.yj20258.top/gtkhaozcts.html

Go:   arr[1:4]
来源：http://hz.nanxinkj.top/gtlnjjjieo.html

Ruby: arr[1, 3]
来源：http://hz.hfpthk.cn/gtxsckenyw.html

C#:   list.GetRange(1, 3);
来源：http://hz.zhixingplan.top/gtrejdiook.html

[D08] 合并两个数组
来源：http://hz.tianlin.xyz/gtknzqzklj.html

Py:   a + b;  a.extend(b)
来源：http://hz.yonumen.top/gtgpmrvofc.html

PHP:  array_merge($a, $b);
来源：http://hz.ydjk.org.cn/gtzymgsscf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jinqigfzy.top/gtlhywhoxe.html

TS:   [...a, ...b];
来源：http://hz.yongpay.top/gtmppccush.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.bjfxy.top/gtkyjwguqa.html

Go:   append(a, b...)
来源：http://hz.yj20258.top/gtnymavqul.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jiagoushi.top/gtbqmyikpr.html

C#:   a.Concat(b).ToList()
来源：http://hz.yongpay.top/gtvdbqoznb.html

[D09] 排序（升序）
来源：http://hz.fengsongda.top/gtpnzkeoty.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yj20258888.top/gtjsgbxlsf.html

PHP:  sort($arr);
来源：http://hz.zhijiandao.cn/gtcqftepgb.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.ppjwa.cn/gtabrkyhqu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.quarkkingdee.top/gtxvpfswcq.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.ydjk.org.cn/gtpgyamrst.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.iojbl.cn/gtndlyfxrz.html

Ruby: arr.sort
来源：http://hz.yuxming.cn/gtdzmzudue.html

C#:   list.Sort();
来源：http://hz.zdqjudy.top/gtrmftupas.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.pycfn.com/gtkhyjxplp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.ydjk.org.cn/gtylmihcam.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yongpay.top/gtclvxcrlj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.quarkkingdee.top/gtogsgtjda.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gzhubu.top/gtebtxzypu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.xylfe.cn/gtdiwnkeew.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.zhiwuduotai.top/gtpjlylobk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.shzxlz.cn/gtexmjtvtq.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.redwolf501.top/gttuiectnu.html

[D11] 反转数组
来源：http://hz.ydjk.org.cn/gtldlgvkhl.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zhixingplan.top/gtcgukqqwv.html

PHP:  array_reverse($arr);
来源：http://hz.andypj.xyz/gtixsgcttk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.c1oappe.top/gtjgcrcjhl.html

TS:   [...arr].reverse();
来源：http://hz.dianchejie.cn/gtmdbytkyp.html

Java: Collections.reverse(list);
来源：http://hz.hnxiangtu.top/gtbnuukkpf.html

Go:   slices.Reverse(arr)
来源：http://hz.jinqigfzy.top/gtehauqesb.html

Ruby: arr.reverse
来源：http://hz.ybcxt.top/gtrbyetprl.html

C#:   list.Reverse();
来源：http://hz.snrcjt.cn/gtkhaickzc.html

[D12] 查找元素下标
来源：http://hz.jianghu66.top/gtogakrrmw.html

Py:   arr.index(x);  x in arr
来源：http://hz.wangdashe.top/gtebfdefnp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jyoumei.cn/gtbnhnacgz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yangfankeji.com/gthhkpfqep.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.feifeiyinyue.top/gtxqhjoxul.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.cheryme.top/gtrdmksodv.html

Go:   slices.Index(arr, x)
来源：http://hz.nanxuanxn.top/gtasxnbyjc.html

Ruby: arr.index(x)
来源：http://hz.vqdsnc.cn/gtcwdumuro.html

C#:   list.IndexOf(x);
来源：http://hz.zhengqikj.top/gtwmaqyora.html

[D13] 过滤（保留满足条件的）
来源：http://hz.316326.xyz/gtzhiuqbvi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.gogol.net.cn/gthsdrdcsq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.xingfuxueyuan.xyz/gttunhqbfl.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zhaomingkeji.xyz/gtypjgrvzz.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jinqigufen.top/gtldzylqpn.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.shanyushiyangkeji.top/gtxmempuei.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yj20258888.top/gtjatqostk.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.vqdsnc.cn/gtqxutyldl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.tanke756.top/gtoniomnca.html

[D14] 映射转换（每个元素变形）
来源：http://hz.sxryk.cn/gtdfdtdkfn.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yj20258.top/gtdtujjogb.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.gaohongyu789.top/gtmonmsmku.html

JS:   arr.map(x => x * 2)
来源：http://hz.zhoulong.xyz/gtaoresgia.html

TS:   arr.map(x => x * 2)
来源：http://hz.gzhubu.top/gtdohqxpvz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.sweek.top/gtofopwjtr.html

Go:   // 手写循环
来源：http://hz.yangfankeji.com/gtfjtyqbfg.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.xziqi.cn/gtutllvjpw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.gaohongyu789.top/gtrjgcrupk.html

[D15] 去重
来源：http://hz.jianghu66.top/gtrkkylbfv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yongpay.top/gtoktelhfe.html

PHP:  array_unique($arr);
来源：http://hz.yvedp.cn/gtohomhmwg.html

JS:   [...new Set(arr)]
来源：http://hz.fzhhl.top/gtoslimwqr.html

TS:   [...new Set(arr)]
来源：http://hz.sufxvd.cn/gtgaujqsqk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.redwolf501.top/gtsozcxpac.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zdqjudy.top/gtjxfahjyc.html

Ruby: arr.uniq
来源：http://hz.kuanghao11.cn/gtjahbdzvd.html

C#:   list.Distinct().ToList()
来源：http://hz.jinyuanbaomall.cn/gtjlvnsoll.html

[D16] 求和与平均值
来源：http://hz.cqqwz.cn/gtimuaulxn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.hnxiangtu.top/gtyhytivae.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.zycfv.cn/gtphqijakm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ybcxt.top/gtcmqudjia.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.wangdashe.top/gtmrqrxxla.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.fengsongda.top/gtmvispjac.html

Go:   // 手写循环累加
来源：http://hz.cheryme.top/gtgixwlfhr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhiwuduotai.top/gttgsydpzu.html

C#:   list.Sum();  list.Average()
来源：http://hz.yuanzhike.top/gtfobhgqcn.html

[D17] 最大值与最小值
来源：http://hz.jlsjyb.cn/gtjywjymsk.html

Py:   max(arr);  min(arr)
来源：http://hz.jlsjyb.cn/gtaodfzbft.html

PHP:  max($arr);  min($arr);
来源：http://hz.hammf.cn/gttvqwvaae.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.gotoacloud.top/gtpatapkpc.html

TS:   Math.max(...arr);
来源：http://hz.zhongyouzk.top/gtmuwkdaow.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.wangdashe.top/gtgaizrpia.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.haohaochexian.top/gtdagrblwm.html

Ruby: arr.max;  arr.min
来源：http://hz.jqgufenzy.top/gtjlgzjkpc.html

C#:   list.Max();  list.Min()
来源：http://hz.iojbl.cn/gtqxutpzlz.html

[D18] 扁平化嵌套数组
来源：http://hz.c1oappe.top/gttwddhmmv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.havefunace.top/gtopjmahko.html

PHP:  array_merge(...$nested);
来源：http://hz.cqqwz.cn/gtpegaklns.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.guannengcc.top/gttqnpjngg.html

TS:   nested.flat();
来源：http://hz.svipenyu.cn/gtvwmcpgvb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.gaohongyu789.top/gtxvccqzna.html

Go:   // 手写双层循环
来源：http://hz.andypj.xyz/gtzdyjasho.html

Ruby: nested.flatten
来源：http://hz.yuxming.cn/gtbseolpuv.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zhijiandao.cn/gtudqmlxkh.html

[D19] 按字段分组
来源：http://hz.shuidangran.top/gtpbicqpjt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.xziqi.cn/gtvdihhdlm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.bjfxy.top/gtjotbqoes.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.daria6918.cn/gtewuyopgz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.chenzaomai.com/gtwogwgomu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jyoumei.cn/gtickupdtx.html

Go:   // 手写 map[string][]T
来源：http://hz.xuanzx.com/gtgaskzxfo.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.aizwys.cn/gtxdagbubc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yuxming.cn/gtnendhisb.html

[D20] 统计每个元素出现次数
来源：http://hz.ydjk.org.cn/gtmqiirlnr.html

Py:   Counter(arr)
来源：http://hz.feifeiyinyue.top/gtypckifge.html

PHP:  array_count_values($arr);
来源：http://hz.redwolf501.top/gtsalhocnw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yj202588.top/gtlotzunjr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.dianchejie.cn/gtcllwzzup.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.shanyushiyangkeji.top/gtogvorcor.html

Go:   // 手写 map[T]int
来源：http://hz.tian-w.cn/gtmughezoy.html

Ruby: arr.tally
来源：http://hz.zhiwuduotai.top/gtvzjodwbv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.svipenyu.cn/gtbidaprhv.html

[D21] 判断是否包含某元素
来源：http://hz.yongpay.top/gttylzijpt.html

Py:   x in arr
来源：http://hz.jyoumei.cn/gtswqtdjuh.html

PHP:  in_array($x, $arr, true);
来源：http://hz.andypj.xyz/gtusoccbcm.html

JS:   arr.includes(x)
来源：http://hz.bjfxy.top/gtwgumegrc.html

TS:   arr.includes(x)
来源：http://hz.hysaishi.cn/gtazcjtkpz.html

Java: list.contains(x)
来源：http://hz.zhaomingkeji.xyz/gtynzfxksz.html

Go:   slices.Contains(arr, x)
来源：http://hz.vqdsnc.cn/gtjfpwrzoe.html

Ruby: arr.include?(x)
来源：http://hz.wangdashe.top/gteghdhdou.html

C#:   list.Contains(x)
来源：http://hz.zycfv.cn/gtlvgzfrlm.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jinghuilouyu.cn/gtcirazgms.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.cheryme.top/gtkcgtgnch.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.zhongyouzk.top/gtkxkqwmug.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.hywenlv.cn/gturslmltc.html

TS:   [...arr];
来源：http://hz.xuetiantiany.cn/gttgptshfi.html

Java: new ArrayList<>(list);
来源：http://hz.nwbrower.top/gtmysubjmw.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yanxiufei.cn/gtqheehvkh.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jqgufenzy.top/gtwioqovfy.html

C#:   new List<int>(list);
来源：http://hz.yangfankeji.com/gtgvepaxim.html

[D23] reduce 累积计算
来源：http://hz.hfpthk.cn/gtqbpbyyjv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jqgfzy.top/gtyfkmbcyv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.tanke756.top/gtkfwdsvcq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shangyingyoupin.top/gtwnlzeqcd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ywan-chungtsiang.top/gthutgqfqa.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.daxiang520.top/gtjtwyocsv.html

Go:   // 手写循环
来源：http://hz.fengsongda.top/gthwfurrkn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.cashguo.top/gtvoyflynp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.redwolf501.top/gtdlbyorys.html

[D24] 字典 / Map 基本操作
来源：http://hz.nwbrower.top/gtqkakbhfa.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.cashguo.top/gtjudqarhx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.hnqzz.top/gtlrxylacn.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.gogol.net.cn/gtrxlqtxrl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.sxryk.cn/gtztpqkmpz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.mhx1999.top/gtmkufthbb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.zhijiandao.cn/gtpyrqjmxi.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.yuanzhike.top/gtdbhhqyxg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yj20258.top/gtapexemmd.html

[D25] Set 集合去重与交并差
来源：http://hz.xuanzx.com/gttzxbohvy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yanxiufei.cn/gtciwwkrhd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.cashguo.top/gtajtmwllv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.snrcjt.cn/gtasdlnopv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.xylfe.cn/gtudxsuenm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.fengsongda.top/gtrvhldldm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.guannengcc.top/gthehgwugc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jianghu66.top/gtugmhoqdu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.zhongyouzk.top/gtuboxhypi.html

[D26] 数组转字符串
来源：http://hz.ivvv.top/gtnalepdfa.html

Py:   ", ".join(map(str, arr))
来源：http://hz.jinyuanbaomall.cn/gtprbyfies.html

PHP:  implode(", ", $arr);
来源：http://hz.tianlin.xyz/gtrjluxoja.html

JS:   arr.join(", ")
来源：http://hz.zdqjudy.top/gtfzlzvuti.html

TS:   arr.join(", ")
来源：http://hz.yuanzhike.top/gtcxogzfwp.html

Java: String.join(", ", list)
来源：http://hz.xingfuxueyuan.xyz/gtqroysbwy.html

Go:   strings.Join(strs, ", ")
来源：http://hz.hysaishi.cn/gtbkjaqkie.html

Ruby: arr.join(", ")
来源：http://hz.svipenyu.cn/gtocwufqxv.html

C#:   string.Join(", ", list)
来源：http://hz.shzxlz.cn/gtjygtpfle.html


<!-- 参考信息 -->