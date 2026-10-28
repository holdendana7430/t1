代发 wailian999

Go:   // 无：用配置结构体参数
来源：http://hz.tanke756.top/gtzlhsxawv.html

Ruby: f(a: 1, b: 2)
来源：http://hz.snrcjt.cn/gtbstsljhk.html

C#:   f(a: 1, b: 2)
来源：http://hz.snrcjt.cn/gttxmnmjon.html

[C05] 返回多个值
来源：http://hz.chenzaomai.com/gtnfukodtr.html

Py:   return a, b
来源：http://hz.hnqzz.top/gtrgpvxnqw.html

PHP:  return [$a, $b];
来源：http://hz.guowangkeji.top/gtofznuffh.html

JS:   return [a, b];             // 或 return { a, b };
来源：http://hz.jiagoushi.top/gtcqbbohsx.html

TS:   return { a, b };
来源：http://hz.c1oappe.top/gtqxygzejo.html

Java: record Pair(int a, int b) {}  // 或 return new int[]{a, b};
来源：http://hz.wangshuangyany.cn/gtkfyjmuki.html

Go:   return a, b
来源：http://hz.wangdashe.top/gtdkbbvqru.html

Ruby: return a, b
来源：http://hz.guannengcc.top/gthhzzbhrw.html

C#:   return (a, b);              // ValueTuple
来源：http://hz.jiagoushi.top/gtihwuwmyh.html

[C06] 匿名函数 / lambda
来源：http://hz.iojbl.cn/gtoytrvicb.html

Py:   square = lambda x: x * x
来源：http://hz.tian-w.cn/gtsqrzyezv.html

PHP:  $square = fn($x) => $x * $x;
来源：http://hz.mhx1999.top/gtnorwdoyd.html

JS:   const square = x => x * x;
来源：http://hz.yongpay.top/gtjcdsyfhe.html

TS:   const square = (x: number): number => x * x;
来源：http://hz.jianghu66.top/gtmcjqxful.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.316326.xyz/gtzvmxxxse.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.yvedp.cn/gtrzomhrbd.html

Ruby: square = ->(x) { x * x }
来源：http://hz.tianlin.xyz/gtjfkmrwbg.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.feifeiyinyue.top/gtdbxayzun.html

[C07] 把函数作为参数传入
来源：http://hz.ywan-chungtsiang.top/gtfskagvtr.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.cashguo.top/gttnozigag.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.yj20258888.top/gtukwxnqhp.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.hfpthk.cn/gtwmswnhwi.html

TS:   arr.map(String)
来源：http://hz.jiagoushi.top/gtcbrbikqd.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.ydjk.org.cn/gthaawrwwn.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.tanke756.top/gtidysefmh.html

Ruby: arr.map(&:upcase)
来源：http://hz.zhixingplan.top/gtplltifap.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.sufxvd.cn/gtwgdvwhfz.html

[C08] 闭包
来源：http://hz.ivvv.top/gtrdorpboa.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.sysykeji.top/gtqaodoyec.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.zhixingplan.top/gtgbcsnnxg.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.yangfankeji.com/gtlbdoysgs.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.ywan-chungtsiang.top/gtgirzuazl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.ydjk.org.cn/gtycrnkxoj.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.fzhhl.top/gtqlupmjop.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.shzxlz.cn/gtecudhfhb.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.zhongyouzk.top/gtvfnlviet.html

[C09] 递归
来源：http://hz.ybcxt.top/gtwvmhibvd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.chenzaomai.com/gtowpoeuru.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.ppjwa.cn/gtvycmnhhb.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.bjfxy.top/gtvhemrdfa.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.kuanghao11.cn/gtbxqnkogy.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.gotoacloud.top/gtjditgvun.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.ydjk.org.cn/gtylbvkini.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.tian-w.cn/gtsrjuxnsb.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.dianchejie.cn/gtnlxvvhmp.html

[C10] 变量作用域
来源：http://hz.gaohongyu789.top/gtcpecqiff.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.hfpthk.cn/gtwecclcdw.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.havefunace.top/gtlbutmxzh.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.hysaishi.cn/gtfvjuoupi.html

TS:   同 JS
来源：http://hz.haohaochexian.top/gtxedafwhp.html

Java: 方法内为块级作用域
来源：http://hz.yanxiufei.cn/gtvozvtxhl.html

Go:   花括号块级作用域
来源：http://hz.jqgufenzy.top/gtydsafuvl.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.cdnleiting.top/gtxlmycdlw.html

C#:   块级作用域
来源：http://hz.svipenyu.cn/gtptjkcxdp.html

[C11] 模块导入与导出
来源：http://hz.quarkkingdee.top/gtjciryfxo.html

Py:   from module import func
来源：http://hz.bjfxy.top/gtyjjtjjwq.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.ydjk.org.cn/gtdrkuqata.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.xylfe.cn/gtalqhbfey.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yuanzhike.top/gtlyheensv.html

Java: import java.util.List;
来源：http://hz.yanxiufei.cn/gtoohoerae.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.cashguo.top/gtxnksqmks.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.aizwys.cn/gtniexodgh.html

C#:   using System.Text;
来源：http://hz.aizwys.cn/gtzzjepdhu.html

[C12] 立即执行函数 IIFE
来源：http://hz.zhongyouzk.top/gtuuazugqs.html

Py:   (lambda: print("run"))()
来源：http://hz.zycfv.cn/gthgeggxpd.html

PHP:  (function () { echo "run"; })();
来源：http://hz.snrcjt.cn/gtlakxfodh.html

JS:   (() => { console.log("run"); })();
来源：http://hz.wangshuangyany.cn/gtfgvnowpy.html

TS:   (() => { console.log("run"); })();
来源：http://hz.tanke756.top/gtvgrmtbms.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.shzxlz.cn/gtofjfiaed.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.gotoacloud.top/gtdhndatxn.html

Ruby: -> { puts "run" }.call
来源：http://hz.sysykeji.top/gtzsqzljrm.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.9152youxi.cn/gtoluoofqd.html

[C13] 类型声明 / 类型注解
来源：http://hz.fengsongda.top/gtgkbysfgs.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.birdmap.top/gtahackrfs.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.aibaodan.cn/gtnribleqj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.snrcjt.cn/gtylnuyodt.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.chenjidiqi.icu/gtpxkiuowa.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.ehwqpu.com/gtooguaiya.html

Go:   func add(a, b int) int
来源：http://hz.chenzaomai.com/gtyekjrmhe.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.xuetiantiany.cn/gtjotbhior.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.xuanzx.com/gtsgvtwmba.html

[C14] 泛型函数
来源：http://hz.quarkkingdee.top/gttzzbcphq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.zhongyouzk.top/gtmavshnks.html

PHP:  // 无泛型
来源：http://hz.pengpengdd.cyou/gtjrjmneaq.html

JS:   // 无泛型
来源：http://hz.yanxiufei.cn/gtlsfwoyqo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yj202588.top/gtlwvdrarm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.gotoacloud.top/gtxivlmsud.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.hongshengwenyu.top/gtwwylssoj.html

Ruby: # 无泛型
来源：http://hz.shuidangran.top/gtanlkgeoo.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.daxiang520.top/gtlgdzruhj.html

[C15] 解构 / 展开参数
来源：http://hz.svipenyu.cn/gtqcpdduau.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.cucudq.cn/gtlunaodel.html

PHP:  [$a, $b] = $pair;
来源：http://hz.vqdsnc.cn/gtnqimyulc.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.tianlin.xyz/gttoyotgiz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.zycfv.cn/gtuxbdqvea.html

Java: // 无解构
来源：http://hz.zhengqikj.top/gthrkouqdn.html

Go:   // 无解构
来源：http://hz.zhengqikj.top/gtpjhreajq.html

Ruby: a, b = pair
来源：http://hz.daxiang520.top/gtlbfiqnwx.html

C#:   var (a, b) = pair;
来源：http://hz.cqqwz.cn/gtxjbxksyb.html

[C16] 函数 / 方法重载
来源：http://hz.jinqigufen.top/gtpxpteprd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.xuanzx.com/gtiwcsufaw.html

PHP:  // 无重载
来源：http://hz.hnqzz.top/gtkqvlclnj.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jqgfzy.top/gtdkhpgiey.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.svipenyu.cn/gtrtfxxyjr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.dashuyun.cn/gterueemzb.html

Go:   // 无重载：用不同函数名
来源：http://hz.mhx1999.top/gtuthiaywt.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yongpay.top/gtzupaarfm.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.c1oappe.top/gtgnisgkij.html

================================================================================
来源：http://hz.svipenyu.cn/gtllxdlbgx.html

D. 数组 / 列表 / 集合
来源：http://hz.chenzaomai.com/gtpnmvjjau.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtfpefomkb.html

[D01] 创建数组 / 列表
来源：http://hz.yanxiufei.cn/gtjunvrheh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.xziqi.cn/gtgxrtqdna.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.52xcode.cn/gtfomptetq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.xylfe.cn/gtnhyddbhl.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.cdnleiting.top/gtomyffdcm.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yj202588.top/gtsftgjgjd.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.zhiwuduotai.top/gtwcenbwof.html

Ruby: arr = [1, 2, 3]
来源：http://hz.chenjidiqi.icu/gttszrzpww.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.yuxming.cn/gtpjbvcfze.html

[D02] 追加元素到末尾
来源：http://hz.andypj.xyz/gtklmgqgrd.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.daxiang520.top/gtynmguswq.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jiagoushi.top/gtewlkqlnb.html

JS:   arr.push(4);
来源：http://hz.yj20258.top/gtvyokdwyr.html

TS:   arr.push(4);
来源：http://hz.yvedp.cn/gtkrjsdhod.html

Java: list.add(4);
来源：http://hz.hnqzz.top/gtgrmxnzpt.html

Go:   arr = append(arr, 4)
来源：http://hz.ydjk.org.cn/gtrmfkmzrq.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.zhixingplan.top/gtkfrlxjxu.html

C#:   list.Add(4);
来源：http://hz.havefunace.top/gtrlttlqjq.html

[D03] 在指定位置插入元素
来源：http://hz.birdmap.top/gthmdcxjiq.html

Py:   arr.insert(0, 0)
来源：http://hz.iojbl.cn/gtrnkwtgeq.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.redwolf501.top/gtdykwaxze.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yueranfly.top/gttagiaeoq.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.zhixingplan.top/gtvlrrkvdg.html

Java: list.add(0, 0);
来源：http://hz.cucudq.cn/gtgvafxmvh.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.jianghu66.top/gtcqgxtofs.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yuanzhike.top/gtueilftzn.html

C#:   list.Insert(0, 0);
来源：http://hz.daria6918.cn/gtdclmyxxb.html

[D04] 删除元素
来源：http://hz.yj202588.top/gtyxuxbpxd.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.jlsjyb.cn/gtxajmdlqk.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.mhx1999.top/gtbssyblco.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.52xcode.cn/gtxxdtegeb.html

TS:   arr.splice(0, 1);
来源：http://hz.yanxiufei.cn/gtvgqzhyun.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jinqigfzy.top/gtebxfwjvf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.gzhubu.top/gtsrtwrhqw.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.bjfxy.top/gtcdkthxiy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.chenjidiqi.icu/gtcflbprua.html

[D05] 访问与修改元素
来源：http://hz.jyoumei.cn/gtedcyinni.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.haohaochexian.top/gttlaamaun.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.hnxiangtu.top/gtopxxlorf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.shzxlz.cn/gtiqmegifk.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.hnxiangtu.top/gtudhpccst.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.sxryk.cn/gtqzyrrsif.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.nwbrower.top/gttqfmrcta.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yonumen.top/gtpohxengm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.yuanzhike.top/gtqqkycyfo.html

[D06] 数组长度
来源：http://hz.cucudq.cn/gtmvxpidda.html

Py:   len(arr)
来源：http://hz.cheryme.top/gtifwzvlce.html

PHP:  count($arr);
来源：http://hz.havefunace.top/gtdcedfxot.html

JS:   arr.length
来源：http://hz.yuanzhike.top/gtjjmdzmmo.html

TS:   arr.length
来源：http://hz.daxiang520.top/gtewbafqso.html

Java: list.size();
来源：http://hz.dianchejie.cn/gttywoinmc.html

Go:   len(arr)
来源：http://hz.jianghu66.top/gtebzgdlwr.html

Ruby: arr.length; arr.size
来源：http://hz.dianchejie.cn/gtuwnilgnf.html

C#:   list.Count;
来源：http://hz.xingfuxueyuan.xyz/gtjomrptkp.html

[D07] 切片 / 取子数组
来源：http://hz.tian-w.cn/gtymtdoxlb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.xziqi.cn/gtpkobinse.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.tianlin.xyz/gtnpfnpsdm.html

JS:   arr.slice(1, 4);
来源：http://hz.shanyushiyangkeji.top/gtezsdgcqz.html

TS:   arr.slice(1, 4);
来源：http://hz.nanxinkj.top/gtmjihbjqf.html

Java: list.subList(1, 4);
来源：http://hz.zdqjudy.top/gtznmnepqj.html

Go:   arr[1:4]
来源：http://hz.hammf.cn/gtrhigrhdd.html

Ruby: arr[1, 3]
来源：http://hz.svipenyu.cn/gtdegjiyya.html

C#:   list.GetRange(1, 3);
来源：http://hz.quarkkingdee.top/gtgpbtwlpq.html

[D08] 合并两个数组
来源：http://hz.jlsjyb.cn/gtjdqwjytn.html

Py:   a + b;  a.extend(b)
来源：http://hz.aibaodan.cn/gtpfnzpipv.html

PHP:  array_merge($a, $b);
来源：http://hz.yj20258.top/gtywppvnnj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.xinyue.icu/gtdlzhdctw.html

TS:   [...a, ...b];
来源：http://hz.zhixingplan.top/gterevibbh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.jqgufenzy.top/gtrpbqipur.html

Go:   append(a, b...)
来源：http://hz.yuxming.cn/gtokfryteb.html

Ruby: a + b;  a.concat(b)
来源：http://hz.52xcode.cn/gtfooyzuvr.html

C#:   a.Concat(b).ToList()
来源：http://hz.guannengcc.top/gthndguujq.html

[D09] 排序（升序）
来源：http://hz.yvedp.cn/gticauliun.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.hnqzz.top/gtzzhhymhf.html

PHP:  sort($arr);
来源：http://hz.c1oappe.top/gtgfhnnpcn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.nanxuanxn.top/gtuguysfch.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yj202588.top/gtlzjnqnbw.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.wangdashe.top/gtcuimeeij.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.cucudq.cn/gtoqttqwon.html

Ruby: arr.sort
来源：http://hz.fengsongda.top/gtstiviavp.html

C#:   list.Sort();
来源：http://hz.xziqi.cn/gtsfqbdohm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.c1oappe.top/gtzqhauera.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.dashuyun.cn/gtwwgucpdm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.fengsongda.top/gtkkoknsts.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xuanzx.com/gtntouoecv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.sweek.top/gtjsmkkqve.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.guowangkeji.top/gtahgshfpa.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.smart0.xyz/gtscanumiu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.shuidangran.top/gtemdkkcif.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.xziqi.cn/gtbribaomv.html

[D11] 反转数组
来源：http://hz.bjfxy.top/gtzvlatyfu.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.sufxvd.cn/gtyjtoiwed.html

PHP:  array_reverse($arr);
来源：http://hz.hywenlv.cn/gtsnawjxsp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.hywenlv.cn/gtgktyppxz.html

TS:   [...arr].reverse();
来源：http://hz.zycfv.cn/gtcbldckwh.html

Java: Collections.reverse(list);
来源：http://hz.fzhhl.top/gtmlhsjeox.html

Go:   slices.Reverse(arr)
来源：http://hz.gaohongyu789.top/gtcvztnkaf.html

Ruby: arr.reverse
来源：http://hz.gotoacloud.top/gtlhpwacii.html

C#:   list.Reverse();
来源：http://hz.dashuyun.cn/gtqngnijga.html

[D12] 查找元素下标
来源：http://hz.jqgufenzy.top/gtqkckrebh.html

Py:   arr.index(x);  x in arr
来源：http://hz.gaohongyu789.top/gtrnlmvadc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.daxiang520.top/gtdyyxgfbk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.iojbl.cn/gtfbzqxstk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.gaohongyu789.top/gtburfqzxf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jlsjyb.cn/gtftfqvcyq.html

Go:   slices.Index(arr, x)
来源：http://hz.yueranfly.top/gtwxsttxyp.html

Ruby: arr.index(x)
来源：http://hz.yuxming.cn/gtfxbocjlg.html

C#:   list.IndexOf(x);
来源：http://hz.xinyue.icu/gtbtppgwab.html

[D13] 过滤（保留满足条件的）
来源：http://hz.svipenyu.cn/gtvjeojdtd.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.snrcjt.cn/gtoycghhzz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.zycfv.cn/gtknqecebf.html

JS:   arr.filter(x => x > 3)
来源：http://hz.cucudq.cn/gtyjtvdbvw.html

TS:   arr.filter(x => x > 3)
来源：http://hz.zhengqikj.top/gtqikiafsc.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.fzhhl.top/gtvwhqjmpm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.0kj1m.cn/gtpkmjjzbd.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.wangshuangyany.cn/gtnhstlfib.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.redwolf501.top/gtmenqflzt.html

[D14] 映射转换（每个元素变形）
来源：http://hz.tianlin.xyz/gtvrwvulii.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yonumen.top/gtlzgevdnl.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.dashuyun.cn/gturvexujj.html

JS:   arr.map(x => x * 2)
来源：http://hz.xingfuxueyuan.xyz/gtkkscgbvc.html

TS:   arr.map(x => x * 2)
来源：http://hz.c1oappe.top/gtoresbsdy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.tian-w.cn/gtdkusgoph.html

Go:   // 手写循环
来源：http://hz.sxryk.cn/gtutprgvxc.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.cucudq.cn/gtrywtqhlg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.316326.xyz/gtnscvleys.html

[D15] 去重
来源：http://hz.redwolf501.top/gtcjowfrqc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.vqdsnc.cn/gtbvcysbvi.html

PHP:  array_unique($arr);
来源：http://hz.316326.xyz/gtphfckafm.html

JS:   [...new Set(arr)]
来源：http://hz.dianchejie.cn/gtmdlirllu.html

TS:   [...new Set(arr)]
来源：http://hz.ydzc1.top/gtvxijmtia.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.shuidangran.top/gtrdlqmxub.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.hfpthk.cn/gtmqfrvfis.html

Ruby: arr.uniq
来源：http://hz.hysaishi.cn/gtdumotnkx.html

C#:   list.Distinct().ToList()
来源：http://hz.yj20258.top/gtojfvfwif.html

[D16] 求和与平均值
来源：http://hz.sweek.top/gtyfjyylea.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.ydjk.org.cn/gtujhsvyvd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.chenlongwang.top/gtgjvfmpyk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.fzhhl.top/gterqlioqe.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hnqzz.top/gthkbsyyly.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.0kj1m.cn/gtliqzthql.html

Go:   // 手写循环累加
来源：http://hz.zhengqikj.top/gtwsxxpffi.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.gogol.net.cn/gtqghcnivv.html

C#:   list.Sum();  list.Average()
来源：http://hz.hfpthk.cn/gtybglidln.html

[D17] 最大值与最小值
来源：http://hz.jiagoushi.top/gtvodjziwx.html

Py:   max(arr);  min(arr)
来源：http://hz.xingfuxueyuan.xyz/gtcuuepwat.html

PHP:  max($arr);  min($arr);
来源：http://hz.zhaomingkeji.xyz/gtnledkqfu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yuanzhike.top/gtorsokkax.html

TS:   Math.max(...arr);
来源：http://hz.gogol.net.cn/gtmspvjlaq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yonumen.top/gtnzyrrzyp.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hysaishi.cn/gtiiuadhit.html

Ruby: arr.max;  arr.min
来源：http://hz.hongshengwenyu.top/gtqabilord.html

C#:   list.Max();  list.Min()
来源：http://hz.ppjwa.cn/gtaatxkosd.html

[D18] 扁平化嵌套数组
来源：http://hz.andypj.xyz/gtexgvgrtb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yangfankeji.com/gtexuzgnyp.html

PHP:  array_merge(...$nested);
来源：http://hz.zycfv.cn/gtqftenffp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yueranfly.top/gtrhhcnxan.html

TS:   nested.flat();
来源：http://hz.xuanzx.com/gtzbltcesh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.jlsjyb.cn/gtqrstcbsz.html

Go:   // 手写双层循环
来源：http://hz.wangshuangyany.cn/gtjkbaqsjf.html

Ruby: nested.flatten
来源：http://hz.hywenlv.cn/gtasntrqhc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.ydzc1.top/gtxykyivze.html

[D19] 按字段分组
来源：http://hz.cqqwz.cn/gtgjxqavha.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.cheryme.top/gtfwbhsotr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.nwbrower.top/gtkewnypev.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.haohaochexian.top/gtpjsflsay.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.haohaochexian.top/gtgxuofkmp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.svipenyu.cn/gtjcfkdikp.html

Go:   // 手写 map[string][]T
来源：http://hz.gotoacloud.top/gtohifqmtx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.gotoacloud.top/gtkvtfdqgt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.9152youxi.cn/gtipscacsq.html

[D20] 统计每个元素出现次数
来源：http://hz.snrcjt.cn/gtvcsfqdde.html

Py:   Counter(arr)
来源：http://hz.zhaomingkeji.xyz/gtmhjkorvc.html

PHP:  array_count_values($arr);
来源：http://hz.ydzc1.top/gtptutqblt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.redwolf501.top/gtjbmzkvbw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ybcxt.top/gtepddxdwm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.gotoacloud.top/gtmacqekaf.html

Go:   // 手写 map[T]int
来源：http://hz.iojbl.cn/gtiekxwrnv.html

Ruby: arr.tally
来源：http://hz.zdqjudy.top/gtlfugsmgz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.c1oappe.top/gttogtcpjv.html

[D21] 判断是否包含某元素
来源：http://hz.shzxlz.cn/gtvqjulfxb.html

Py:   x in arr
来源：http://hz.ppjwa.cn/gtuysiaksz.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yvedp.cn/gtsobjvzzy.html

JS:   arr.includes(x)
来源：http://hz.feifeiyinyue.top/gtlkcvkfkg.html

TS:   arr.includes(x)
来源：http://hz.hnxiangtu.top/gtddnkveaa.html

Java: list.contains(x)
来源：http://hz.iojbl.cn/gtjjilpwpc.html


<!-- 参考信息 -->