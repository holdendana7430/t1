代发 wailian999

C#:   Func<int, int> square = x => x * x;
来源：http://hz.zhaomingkeji.xyz/gtedrvswwl.html

[C07] 把函数作为参数传入
来源：http://hz.bjfxy.top/gtaghskgsi.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.haohaochexian.top/gtekyvhkvr.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.yj20258888.top/gteusgegex.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.zhoulong.xyz/gtwwvrjpnv.html

TS:   arr.map(String)
来源：http://hz.shuidangran.top/gtctmimbof.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.birdmap.top/gtqbhmkgim.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.redwolf501.top/gthiaxsvaz.html

Ruby: arr.map(&:upcase)
来源：http://hz.zdqjudy.top/gtmblydfez.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.cucudq.cn/gtpdzmhjcd.html

[C08] 闭包
来源：http://hz.nanxinkj.top/gtlntafubj.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.jinqigfzy.top/gtevnfccrx.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.gogol.net.cn/gtqneqfvir.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.tianlin.xyz/gtwllpgfdf.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.cashguo.top/gttuoabbrl.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.ywan-chungtsiang.top/gthyrjdzfa.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.zycfv.cn/gtgjoyytvk.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.pengpengdd.cyou/gtasdnpwtu.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.gogol.net.cn/gtnxhdvdor.html

[C09] 递归
来源：http://hz.cdnleiting.top/gtvrluvlja.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.cdnleiting.top/gtarulcmko.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.fzhhl.top/gtyupibhyz.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.jinqigufen.top/gtumlgzxnr.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zycfv.cn/gtzyqjyivt.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.nanxuanxn.top/gtijsmyqcp.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.fengsongda.top/gtrjoeugla.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.xuetiantiany.cn/gtvudengkn.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.smart0.xyz/gtcuomuibr.html

[C10] 变量作用域
来源：http://hz.cucudq.cn/gtwmbxlffz.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.xinyue.icu/gtarlpxlls.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.sysykeji.top/gtxgpjuiig.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.zycfv.cn/gtwcgyxyad.html

TS:   同 JS
来源：http://hz.wangdashe.top/gtbfpizbmh.html

Java: 方法内为块级作用域
来源：http://hz.zhengqikj.top/gtvhjokghc.html

Go:   花括号块级作用域
来源：http://hz.gzhubu.top/gtnxiqlzdh.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.hammf.cn/gthevdcfvw.html

C#:   块级作用域
来源：http://hz.xziqi.cn/gtzfzrccsx.html

[C11] 模块导入与导出
来源：http://hz.dianchejie.cn/gtesctcciu.html

Py:   from module import func
来源：http://hz.jlsjyb.cn/gtwapryrwr.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.pycfn.com/gtujerbynz.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.shzxlz.cn/gtmfeamejd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.daxiang520.top/gthhblkbfs.html

Java: import java.util.List;
来源：http://hz.9152youxi.cn/gtuvlutyam.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yanxiufei.cn/gtkcbkhcso.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.daria6918.cn/gtbtxayfyq.html

C#:   using System.Text;
来源：http://hz.chenzaomai.com/gtvbwpudku.html

[C12] 立即执行函数 IIFE
来源：http://hz.aibaodan.cn/gttlhfhmfy.html

Py:   (lambda: print("run"))()
来源：http://hz.nanxuanxn.top/gturltoaku.html

PHP:  (function () { echo "run"; })();
来源：http://hz.sxryk.cn/gtvuhzhgel.html

JS:   (() => { console.log("run"); })();
来源：http://hz.sysykeji.top/gthdqcbsqm.html

TS:   (() => { console.log("run"); })();
来源：http://hz.dashuyun.cn/gtsmqoaqtl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.meibo888.top/gtiguxjeyu.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.jqgufenzy.top/gtqvpbufhb.html

Ruby: -> { puts "run" }.call
来源：http://hz.gotoacloud.top/gtvsdaqybx.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.sysykeji.top/gtmaseheax.html

[C13] 类型声明 / 类型注解
来源：http://hz.jinqigufen.top/gtcudddjkg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.ehwqpu.com/gtnxlaphjl.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.ydzc1.top/gtlccxmier.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.iojbl.cn/gtdwicpbqd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hnqzz.top/gtkirwtdkn.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.cqqwz.cn/gtlkxyycvh.html

Go:   func add(a, b int) int
来源：http://hz.jinyuanbaomall.cn/gtrpbbuvnu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jyoumei.cn/gtrvfoezzx.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.xingfuxueyuan.xyz/gtvromqmmz.html

[C14] 泛型函数
来源：http://hz.bjfxy.top/gtoyduajso.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.zhengqikj.top/gtxcqexezq.html

PHP:  // 无泛型
来源：http://hz.cheryme.top/gtpcuyuwom.html

JS:   // 无泛型
来源：http://hz.redwolf501.top/gtzfquolqd.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.zhijiandao.cn/gtosxwvupb.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.pycfn.com/gtfpjgkoni.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yj202588.top/gtqyhfbyqr.html

Ruby: # 无泛型
来源：http://hz.ybcxt.top/gtuoxzhmag.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.chenzaomai.com/gtqfwoqbva.html

[C15] 解构 / 展开参数
来源：http://hz.chenlongwang.top/gtqiozuvoz.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.xylfe.cn/gthzoliqfm.html

PHP:  [$a, $b] = $pair;
来源：http://hz.jqgufenzy.top/gtdqyaultl.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jlsjyb.cn/gtsgalwmlk.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.xylfe.cn/gtrjzxwnhf.html

Java: // 无解构
来源：http://hz.zdqjudy.top/gtjeejangy.html

Go:   // 无解构
来源：http://hz.ppjwa.cn/gthjzasvds.html

Ruby: a, b = pair
来源：http://hz.jinqigfzy.top/gtzpcroypm.html

C#:   var (a, b) = pair;
来源：http://hz.feifeiyinyue.top/gtpegkojrg.html

[C16] 函数 / 方法重载
来源：http://hz.zdqjudy.top/gtqwgxmqsh.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.jinyuanbaomall.cn/gtlrtttuow.html

PHP:  // 无重载
来源：http://hz.shangyingyoupin.top/gtbpyhgzcw.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.gaohongyu789.top/gtrydbjzzb.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.52xcode.cn/gtoryrimrr.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.yuxming.cn/gtybcvvuqh.html

Go:   // 无重载：用不同函数名
来源：http://hz.fzhhl.top/gtncqhixym.html

Ruby: # 无重载：靠动态参数
来源：http://hz.gogol.net.cn/gtwxvvochu.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.jinyuanbaomall.cn/gtbfticypu.html

================================================================================
来源：http://hz.jiagoushi.top/gtapgchunp.html

D. 数组 / 列表 / 集合
来源：http://hz.chenjidiqi.icu/gthgvnqksu.html

================================================================================
来源：http://hz.hnxiangtu.top/gtwxdsqycz.html

[D01] 创建数组 / 列表
来源：http://hz.c1oappe.top/gtmrabfzdw.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.redwolf501.top/gtsyyoguty.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.daxiang520.top/gtnrmmeyue.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.gaohongyu789.top/gtppruikyu.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yanxiufei.cn/gtoiqbcfeg.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xinyue.icu/gtaczuqffn.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.xuetiantiany.cn/gtpachbilb.html

Ruby: arr = [1, 2, 3]
来源：http://hz.cheryme.top/gttaopyzgf.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.hywenlv.cn/gtmsckdcfe.html

[D02] 追加元素到末尾
来源：http://hz.feifeiyinyue.top/gtgylsnnhm.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zhongyouzk.top/gtwcknjffr.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.sysykeji.top/gtoecuyeri.html

JS:   arr.push(4);
来源：http://hz.yonumen.top/gtjyeqrsin.html

TS:   arr.push(4);
来源：http://hz.aibaodan.cn/gtbfjhpsey.html

Java: list.add(4);
来源：http://hz.hammf.cn/gtcnotsnsv.html

Go:   arr = append(arr, 4)
来源：http://hz.svipenyu.cn/gtlpvolhov.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.iojbl.cn/gtckivnrtv.html

C#:   list.Add(4);
来源：http://hz.ivvv.top/gtfywifjti.html

[D03] 在指定位置插入元素
来源：http://hz.gogol.net.cn/gtobebuipk.html

Py:   arr.insert(0, 0)
来源：http://hz.ivvv.top/gtbqroavhm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.sxryk.cn/gtjshhsmoh.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.birdmap.top/gtqihgksbn.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.yueranfly.top/gtiyhuabat.html

Java: list.add(0, 0);
来源：http://hz.nanxinkj.top/gttppbdbij.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.jlsjyb.cn/gtzgnrfgkq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.ybcxt.top/gtttaxsvbk.html

C#:   list.Insert(0, 0);
来源：http://hz.svipenyu.cn/gtuofyevbc.html

[D04] 删除元素
来源：http://hz.xuanzx.com/gtcyfnknqd.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.xuanzx.com/gthewiptog.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zhongyouzk.top/gtuchurhyv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.hongshengwenyu.top/gtbquxnput.html

TS:   arr.splice(0, 1);
来源：http://hz.svipenyu.cn/gtwkhcxkwl.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.birdmap.top/gtiwefxoxi.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.pengpengdd.cyou/gtiqxcxdza.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.zdqjudy.top/gtenodthdl.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.hysaishi.cn/gtxtntcqtt.html

[D05] 访问与修改元素
来源：http://hz.gaohongyu789.top/gtdjqgxyrv.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhengqikj.top/gteorfezrv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.fengsongda.top/gtukznuotl.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.tian-w.cn/gtzhdtvltv.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.vqdsnc.cn/gtxwopnwgs.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jianghu66.top/gtshzrlgih.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.xuetiantiany.cn/gttijjmvtc.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jyoumei.cn/gtdzihzaut.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jlsjyb.cn/gtduciznen.html

[D06] 数组长度
来源：http://hz.bjfxy.top/gthvwjerul.html

Py:   len(arr)
来源：http://hz.birdmap.top/gttzctrndk.html

PHP:  count($arr);
来源：http://hz.yangfankeji.com/gtemecindn.html

JS:   arr.length
来源：http://hz.zhixingplan.top/gtvmawunfp.html

TS:   arr.length
来源：http://hz.hywenlv.cn/gtbqxbssth.html

Java: list.size();
来源：http://hz.smart0.xyz/gthcpxckjq.html

Go:   len(arr)
来源：http://hz.zhaomingkeji.xyz/gtyoovoknh.html

Ruby: arr.length; arr.size
来源：http://hz.yueranfly.top/gtgcoijkzc.html

C#:   list.Count;
来源：http://hz.nanxuanxn.top/gtcbyyjuwo.html

[D07] 切片 / 取子数组
来源：http://hz.shangyingyoupin.top/gtaqrwpele.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yvedp.cn/gtbvjqspek.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.ydzc1.top/gtqobatgia.html

JS:   arr.slice(1, 4);
来源：http://hz.gzhubu.top/gteodbhbpb.html

TS:   arr.slice(1, 4);
来源：http://hz.cucudq.cn/gtvdwfituf.html

Java: list.subList(1, 4);
来源：http://hz.zhengqikj.top/gtyjlxeqii.html

Go:   arr[1:4]
来源：http://hz.svipenyu.cn/gtqgkpzqor.html

Ruby: arr[1, 3]
来源：http://hz.shuidangran.top/gtrpavfezg.html

C#:   list.GetRange(1, 3);
来源：http://hz.nanxinkj.top/gtxplagsbd.html

[D08] 合并两个数组
来源：http://hz.aibaodan.cn/gtwlggamkj.html

Py:   a + b;  a.extend(b)
来源：http://hz.cheryme.top/gtqpkmdzys.html

PHP:  array_merge($a, $b);
来源：http://hz.jinyuanbaomall.cn/gtauapujon.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.dashuyun.cn/gtimccfhjl.html

TS:   [...a, ...b];
来源：http://hz.cqqwz.cn/gtyhmukghb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.dianchejie.cn/gtxpkdzwnj.html

Go:   append(a, b...)
来源：http://hz.chenlongwang.top/gtcgyqgbtc.html

Ruby: a + b;  a.concat(b)
来源：http://hz.zhijiandao.cn/gtcxovwwug.html

C#:   a.Concat(b).ToList()
来源：http://hz.cdnleiting.top/gtgpmhbsjo.html

[D09] 排序（升序）
来源：http://hz.jqgfzy.top/gtwvdyzabq.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xylfe.cn/gtsfckecnm.html

PHP:  sort($arr);
来源：http://hz.ywan-chungtsiang.top/gtyvemcnnu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.dianchejie.cn/gtjylcydiv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.xziqi.cn/gtafnbihzo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yongpay.top/gtesmtmxod.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.hnxiangtu.top/gtgearjckw.html

Ruby: arr.sort
来源：http://hz.gzhubu.top/gtuxxzstem.html

C#:   list.Sort();
来源：http://hz.jyoumei.cn/gtwuzwxdzn.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zhiwuduotai.top/gtyhsgliia.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.xuetiantiany.cn/gtbwokdpkm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jiagoushi.top/gtslpcztnr.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xuanzx.com/gtlorelugh.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.tianlin.xyz/gtiaulratt.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.gogol.net.cn/gtmsviiwzk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yuanzhike.top/gthtnoyrxx.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.fengsongda.top/gtiaxdnzef.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.gotoacloud.top/gtxcciujrs.html

[D11] 反转数组
来源：http://hz.shzxlz.cn/gtwghzgkfb.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.xziqi.cn/gtwfvwtwxz.html

PHP:  array_reverse($arr);
来源：http://hz.jinqigufen.top/gtoabfkloi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.sysykeji.top/gtnfvmbmqr.html

TS:   [...arr].reverse();
来源：http://hz.ehwqpu.com/gtuohtnvbz.html

Java: Collections.reverse(list);
来源：http://hz.ydjk.org.cn/gtwfdnkzsx.html

Go:   slices.Reverse(arr)
来源：http://hz.ydzc1.top/gtanyawiza.html

Ruby: arr.reverse
来源：http://hz.hnxiangtu.top/gtkwgdsets.html

C#:   list.Reverse();
来源：http://hz.ppjwa.cn/gtyrwxooha.html

[D12] 查找元素下标
来源：http://hz.ydzc1.top/gtjhxanvqx.html

Py:   arr.index(x);  x in arr
来源：http://hz.zhiwuduotai.top/gtsgbjovhp.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.zdqjudy.top/gtnvrfegea.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.guowangkeji.top/gtswfncjnf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhijiandao.cn/gtellqnrkg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.daria6918.cn/gtlvafkemh.html

Go:   slices.Index(arr, x)
来源：http://hz.daxiang520.top/gtaacibyki.html

Ruby: arr.index(x)
来源：http://hz.hammf.cn/gtzxljrqyn.html

C#:   list.IndexOf(x);
来源：http://hz.0kj1m.cn/gtigbpykvb.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zhixingplan.top/gtfxqtxelx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.aibaodan.cn/gtpejijxvj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.ivvv.top/gtoxezwqnf.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zhaomingkeji.xyz/gtxymsvayc.html

TS:   arr.filter(x => x > 3)
来源：http://hz.shanyushiyangtech.top/gtirlftjof.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.gzhubu.top/gtmivxupkt.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yvedp.cn/gthnazfdin.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.ivvv.top/gtjrybbpvd.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.ivvv.top/gthunhyftl.html

[D14] 映射转换（每个元素变形）
来源：http://hz.cqqwz.cn/gtsvthozxw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.bjfxy.top/gtdoejhhrs.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yongpay.top/gtxekwbgda.html

JS:   arr.map(x => x * 2)
来源：http://hz.meibo888.top/gtsqzdsily.html

TS:   arr.map(x => x * 2)
来源：http://hz.52xcode.cn/gtwryunwxu.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.ydjk.org.cn/gtqkoxueaj.html

Go:   // 手写循环
来源：http://hz.ybcxt.top/gtkgmomzfr.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.aizwys.cn/gtkjfqffja.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.xziqi.cn/gtiutpuoag.html

[D15] 去重
来源：http://hz.haohaochexian.top/gtjuqgwjdi.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.hnxiangtu.top/gtauakxxqz.html

PHP:  array_unique($arr);
来源：http://hz.jinyuanbaomall.cn/gtiiuggjzz.html

JS:   [...new Set(arr)]
来源：http://hz.jyoumei.cn/gtisvaozze.html

TS:   [...new Set(arr)]
来源：http://hz.nanxinkj.top/gtruwzsyip.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.gogol.net.cn/gtlaifwlen.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.havefunace.top/gtkwpjuljg.html

Ruby: arr.uniq
来源：http://hz.shuidangran.top/gtrzgncxxj.html

C#:   list.Distinct().ToList()
来源：http://hz.zhoulong.xyz/gtanzthqon.html

[D16] 求和与平均值
来源：http://hz.chenjidiqi.icu/gtzbyvqeld.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.birdmap.top/gtbcgqixru.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.nanxinkj.top/gthvsrynph.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ywan-chungtsiang.top/gtenxrmwau.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yonumen.top/gtsaccrgxc.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.gotoacloud.top/gtpkawyvjh.html

Go:   // 手写循环累加
来源：http://hz.jinyuanbaomall.cn/gtjpkukghf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.birdmap.top/gtkyiswexb.html

C#:   list.Sum();  list.Average()
来源：http://hz.shuidangran.top/gtxfggxngg.html

[D17] 最大值与最小值
来源：http://hz.zhongyouzk.top/gtslxccxbm.html

Py:   max(arr);  min(arr)
来源：http://hz.cdnleiting.top/gtvhvxovwj.html

PHP:  max($arr);  min($arr);
来源：http://hz.yongpay.top/gtwkqttnen.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.pengpengdd.cyou/gthkofxgjv.html

TS:   Math.max(...arr);
来源：http://hz.cucudq.cn/gtfgzmeall.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yanxiufei.cn/gtkoamqflc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.cdnleiting.top/gtedaoxztc.html

Ruby: arr.max;  arr.min
来源：http://hz.sweek.top/gtdtbkojtu.html

C#:   list.Max();  list.Min()
来源：http://hz.shuidangran.top/gtxaswjeqy.html

[D18] 扁平化嵌套数组
来源：http://hz.redwolf501.top/gtkedhqaqq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.gaohongyu789.top/gtkjshywda.html

PHP:  array_merge(...$nested);
来源：http://hz.cashguo.top/gtfpxajsdx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yongpay.top/gtdaepbqxz.html

TS:   nested.flat();
来源：http://hz.zhixingplan.top/gtdwajqxxf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.tian-w.cn/gtzknjrnsn.html

Go:   // 手写双层循环
来源：http://hz.aizwys.cn/gtzfbzuwpj.html

Ruby: nested.flatten
来源：http://hz.ehwqpu.com/gtuneesety.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.chenzaomai.com/gtzyzmdrep.html

[D19] 按字段分组
来源：http://hz.chenzaomai.com/gtgvteeqel.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yangfankeji.com/gtdfbzqmqq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.meibo888.top/gthxyinkxg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.kuanghao11.cn/gtexzzqsfd.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.cheryme.top/gtfpwvfnvg.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yueranfly.top/gtxbafihci.html

Go:   // 手写 map[string][]T
来源：http://hz.yueranfly.top/gtgfaustxn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.haohaochexian.top/gtkgcfvxxo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.dashuyun.cn/gtstrfnhdz.html

[D20] 统计每个元素出现次数
来源：http://hz.fengsongda.top/gtbsicozyt.html

Py:   Counter(arr)
来源：http://hz.sxryk.cn/gtngwbnupb.html

PHP:  array_count_values($arr);
来源：http://hz.jqgufenzy.top/gtpnofpuvp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yj20258.top/gtmcyqlzue.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.gogol.net.cn/gtnxdymfng.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ehwqpu.com/gtankkvmfl.html

Go:   // 手写 map[T]int
来源：http://hz.sufxvd.cn/gtiubgmjvv.html

Ruby: arr.tally
来源：http://hz.shuidangran.top/gtvivmbdaq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.ehwqpu.com/gtqwszdlqh.html

[D21] 判断是否包含某元素
来源：http://hz.yanxiufei.cn/gtkitdqqtj.html

Py:   x in arr
来源：http://hz.xingfuxueyuan.xyz/gtfxijnxnw.html

PHP:  in_array($x, $arr, true);
来源：http://hz.pengpengdd.cyou/gtmojfygqk.html

JS:   arr.includes(x)
来源：http://hz.jianghu66.top/gtssqcxzjo.html

TS:   arr.includes(x)
来源：http://hz.quarkkingdee.top/gtplnooduc.html

Java: list.contains(x)
来源：http://hz.hammf.cn/gtmnjlxasb.html

Go:   slices.Contains(arr, x)
来源：http://hz.hammf.cn/gtjuyvxiit.html

Ruby: arr.include?(x)
来源：http://hz.tian-w.cn/gtqwnbhslf.html

C#:   list.Contains(x)
来源：http://hz.zycfv.cn/gttsqjwgcq.html

[D22] 复制数组（避免共享引用）
来源：http://hz.redwolf501.top/gtcyshqdnf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.redwolf501.top/gthewmouia.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yuxming.cn/gtnjnssyxi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.ydzc1.top/gtejeuzedw.html

TS:   [...arr];
来源：http://hz.jinyuanbaomall.cn/gtnducigau.html

Java: new ArrayList<>(list);
来源：http://hz.xziqi.cn/gtsjawjzqz.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.havefunace.top/gtbxjthayy.html

Ruby: arr.dup;  arr.clone
来源：http://hz.nwbrower.top/gtobmtjssa.html

C#:   new List<int>(list);
来源：http://hz.svipenyu.cn/gtirzsovig.html

[D23] reduce 累积计算
来源：http://hz.yongpay.top/gtqjyvpwif.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.52xcode.cn/gtlzbpttdg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yonumen.top/gtfsqwjwef.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hnxiangtu.top/gtjtmhofva.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.birdmap.top/gtsffrlydj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jinqigfzy.top/gtgddsnnao.html

Go:   // 手写循环
来源：http://hz.haohaochexian.top/gtzzwwpfnk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.shanyushiyangtech.top/gtlxdtpxtw.html


<!-- 参考信息 -->