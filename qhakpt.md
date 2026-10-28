代发 wailian999

TS:   const square = (x: number): number => x * x;
来源：http://hz.hfpthk.cn/gtwaabpwgw.html

Java: Function<Integer, Integer> sq = x -> x * x;
来源：http://hz.jianghu66.top/gtgskcyfuv.html

Go:   sq := func(x int) int { return x * x }
来源：http://hz.shuidangran.top/gtqekkldmx.html

Ruby: square = ->(x) { x * x }
来源：http://hz.jianghu66.top/gtxbgrwaan.html

C#:   Func<int, int> square = x => x * x;
来源：http://hz.wangshuangyany.cn/gtfzckpgsu.html

[C07] 把函数作为参数传入
来源：http://hz.smart0.xyz/gtyqbngrwf.html

Py:   list(map(str.upper, arr)); sorted(arr, key=len)
来源：http://hz.quarkkingdee.top/gtbeqjgxos.html

PHP:  array_map("strtoupper", $arr);
来源：http://hz.fzhhl.top/gtdcmekjjt.html

JS:   arr.map(String).sort((a, b) => a.length - b.length)
来源：http://hz.hammf.cn/gtgwqodlix.html

TS:   arr.map(String)
来源：http://hz.sufxvd.cn/gtbzlgmxfr.html

Java: arr.stream().map(String::toUpperCase).toList()
来源：http://hz.jlsjyb.cn/gtufdtqqxl.html

Go:   // 无 map 内置：手写循环或用 golang.org/x/exp/slices
来源：http://hz.aizwys.cn/gtgqhotosq.html

Ruby: arr.map(&:upcase)
来源：http://hz.daxiang520.top/gtadjpjvnv.html

C#:   arr.Select(s => s.ToUpper())
来源：http://hz.chenlongwang.top/gtophbgcmm.html

[C08] 闭包
来源：http://hz.xinyue.icu/gtrdkznzzp.html

Py:   from itertools import count; inc = lambda c=count(1): next(c)   # 计数器
来源：http://hz.hnxiangtu.top/gtwhjnbijt.html

PHP:  function counter() { $n = 0; return function () use (&$n) { return ++$n; }; }
来源：http://hz.quarkkingdee.top/gtkjkyuleh.html

JS:   function counter() { let n = 0; return () => ++n; }
来源：http://hz.fengsongda.top/gtpiscraex.html

TS:   function counter(): () => number { let n = 0; return () => ++n; }
来源：http://hz.bjfxy.top/gtvsnxhbpr.html

Java: // 只能捕获 effectively final：用 int[] 或 AtomicInteger
来源：http://hz.chenzaomai.com/gtbznxdrhf.html

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.pycfn.com/gtzeddbgsp.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.zhijiandao.cn/gtsokfmugw.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.meibo888.top/gtkpelgzlj.html

[C09] 递归
来源：http://hz.xuanzx.com/gtgixzpnvg.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.iojbl.cn/gtnhviscvf.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.ehwqpu.com/gtizsdenwm.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.zhaomingkeji.xyz/gtkclehkro.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yanxiufei.cn/gtkpngsjdk.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.andypj.xyz/gtjobbssjr.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.52xcode.cn/gtrizlgihe.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.nanxinkj.top/gtlnnnpdie.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.zhixingplan.top/gtmxivrguv.html

[C10] 变量作用域
来源：http://hz.andypj.xyz/gtnbybehzg.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.gzhubu.top/gtmgcooawv.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.mhx1999.top/gtwwzbcwyz.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.cashguo.top/gttbzjhiea.html

TS:   同 JS
来源：http://hz.yuanzhike.top/gtzgxzfgvt.html

Java: 方法内为块级作用域
来源：http://hz.birdmap.top/gtpxwtdzpe.html

Go:   花括号块级作用域
来源：http://hz.c1oappe.top/gtfliylkdx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yanxiufei.cn/gtxuuyzwgb.html

C#:   块级作用域
来源：http://hz.shangyingyoupin.top/gtdfjqhvyv.html

[C11] 模块导入与导出
来源：http://hz.zhaomingkeji.xyz/gtyjtuwdfu.html

Py:   from module import func
来源：http://hz.quarkkingdee.top/gtguhyttug.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.sysykeji.top/gtolzoiydm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.shangyingyoupin.top/gtbdwkzbcj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.316326.xyz/gtnvdgizsd.html

Java: import java.util.List;
来源：http://hz.yuxming.cn/gtwwotfjsg.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.ydzc1.top/gtysebhhou.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.52xcode.cn/gtdseqrjlf.html

C#:   using System.Text;
来源：http://hz.jianghu66.top/gtxvbumvrf.html

[C12] 立即执行函数 IIFE
来源：http://hz.zdqjudy.top/gtgubvshzp.html

Py:   (lambda: print("run"))()
来源：http://hz.hongshengwenyu.top/gtahiymzpv.html

PHP:  (function () { echo "run"; })();
来源：http://hz.ywan-chungtsiang.top/gttdhdflmg.html

JS:   (() => { console.log("run"); })();
来源：http://hz.vqdsnc.cn/gtxkffodiw.html

TS:   (() => { console.log("run"); })();
来源：http://hz.shanyushiyangkeji.top/gtqesgqcss.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.nwbrower.top/gtgbpxtsih.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.pengpengdd.cyou/gtsdceunbj.html

Ruby: -> { puts "run" }.call
来源：http://hz.xingfuxueyuan.xyz/gttzxxldem.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.shangyingyoupin.top/gtgssbhkbi.html

[C13] 类型声明 / 类型注解
来源：http://hz.jqgfzy.top/gtmanwtuwa.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.vqdsnc.cn/gtyddqarsv.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.jinghuilouyu.cn/gteppweqzz.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.shanyushiyangkeji.top/gtazdincdp.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhaomingkeji.xyz/gtstwhexhc.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.andypj.xyz/gtafohbrev.html

Go:   func add(a, b int) int
来源：http://hz.zhengqikj.top/gtfvwhpvaa.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.dashuyun.cn/gtxczrcqgl.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.hongshengwenyu.top/gtoybopbre.html

[C14] 泛型函数
来源：http://hz.pengpengdd.cyou/gtsnyezkzr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.cashguo.top/gtlfujyrhj.html

PHP:  // 无泛型
来源：http://hz.xinyue.icu/gtujkplgto.html

JS:   // 无泛型
来源：http://hz.hammf.cn/gtuikaqyql.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.c1oappe.top/gtuzrgiaet.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.zhongyouzk.top/gterkzewxo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.wangdashe.top/gthckdxxrt.html

Ruby: # 无泛型
来源：http://hz.mhx1999.top/gtokcwowvz.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.daria6918.cn/gttkjtcyee.html

[C15] 解构 / 展开参数
来源：http://hz.shzxlz.cn/gttmepahsi.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.kuanghao11.cn/gtqeshzyfr.html

PHP:  [$a, $b] = $pair;
来源：http://hz.xuetiantiany.cn/gtwqnyrtex.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.cashguo.top/gtopsjqdwz.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.fengsongda.top/gtkicrrwry.html

Java: // 无解构
来源：http://hz.shanyushiyangtech.top/gtvbnecyaa.html

Go:   // 无解构
来源：http://hz.dianchejie.cn/gtqucnwolh.html

Ruby: a, b = pair
来源：http://hz.jianghu66.top/gtqvwzhrgf.html

C#:   var (a, b) = pair;
来源：http://hz.zhijiandao.cn/gtszltmmcg.html

[C16] 函数 / 方法重载
来源：http://hz.jianghu66.top/gtzsrghvvi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yj20258.top/gtbuebypgd.html

PHP:  // 无重载
来源：http://hz.tanke756.top/gtfmypjgkf.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.jianghu66.top/gteywtggem.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.zycfv.cn/gtnddjmijh.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.fzhhl.top/gtemqljcub.html

Go:   // 无重载：用不同函数名
来源：http://hz.jinqigufen.top/gtvppbdzhb.html

Ruby: # 无重载：靠动态参数
来源：http://hz.sweek.top/gtgipvdyci.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.nwbrower.top/gtvzrddugc.html

================================================================================
来源：http://hz.gaohongyu789.top/gtrjsxurve.html

D. 数组 / 列表 / 集合
来源：http://hz.ybcxt.top/gtqzcrorcu.html

================================================================================
来源：http://hz.sufxvd.cn/gtmueeroys.html

[D01] 创建数组 / 列表
来源：http://hz.yongpay.top/gtgmeikkrf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.zhijiandao.cn/gtuakznnxm.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.xziqi.cn/gtrkpgrcfx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.redwolf501.top/gtfdeqvsje.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.nwbrower.top/gtzymwvren.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.quarkkingdee.top/gtuksevrhi.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.zdqjudy.top/gtenrmlhab.html

Ruby: arr = [1, 2, 3]
来源：http://hz.jqgufenzy.top/gtjsgdfnvu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.ehwqpu.com/gtfttlasxr.html

[D02] 追加元素到末尾
来源：http://hz.zhoulong.xyz/gtwuefmjvz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.52xcode.cn/gttfhodwov.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.shuidangran.top/gtxehguexu.html

JS:   arr.push(4);
来源：http://hz.vqdsnc.cn/gtutbuhhkp.html

TS:   arr.push(4);
来源：http://hz.xylfe.cn/gtnlyatzkx.html

Java: list.add(4);
来源：http://hz.fzhhl.top/gtqdtkegjt.html

Go:   arr = append(arr, 4)
来源：http://hz.yvedp.cn/gtkoqpldwu.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.fzhhl.top/gtwrbwsqeq.html

C#:   list.Add(4);
来源：http://hz.jiagoushi.top/gttgwhqfbo.html

[D03] 在指定位置插入元素
来源：http://hz.smart0.xyz/gtzafgfbdn.html

Py:   arr.insert(0, 0)
来源：http://hz.jlsjyb.cn/gtsyqpanpc.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yuanzhike.top/gterwmrmty.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.yuanzhike.top/gtknrrjnbz.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.9152youxi.cn/gtwcnjropf.html

Java: list.add(0, 0);
来源：http://hz.sufxvd.cn/gtalouxprm.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.zhixingplan.top/gtaztxxniv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.yj20258888.top/gtpgvjcdpw.html

C#:   list.Insert(0, 0);
来源：http://hz.bjfxy.top/gtgnlmkjdc.html

[D04] 删除元素
来源：http://hz.kuanghao11.cn/gtqpdvnbac.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.52xcode.cn/gtcudbwild.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.meibo888.top/gtyycbvqxs.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.zycfv.cn/gtxsdidqyk.html

TS:   arr.splice(0, 1);
来源：http://hz.zhengqikj.top/gtyefhlwgq.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.vqdsnc.cn/gtljcdctft.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.smart0.xyz/gtblxgbpdv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.aibaodan.cn/gtijrezaju.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.fengsongda.top/gthfsuqmmf.html

[D05] 访问与修改元素
来源：http://hz.316326.xyz/gtymwnhsdu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.0kj1m.cn/gtmahakuuv.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.ydjk.org.cn/gtnqzoezsk.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jianghu66.top/gtmvpczwzz.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.sxryk.cn/gtcdmyjqyv.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.cucudq.cn/gtecmfeneu.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.jqgufenzy.top/gtquapfsah.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhixingplan.top/gtcfnpghma.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.haohaochexian.top/gtahevkigm.html

[D06] 数组长度
来源：http://hz.jiagoushi.top/gtfmhxozau.html

Py:   len(arr)
来源：http://hz.zhoulong.xyz/gtaeblvtyx.html

PHP:  count($arr);
来源：http://hz.feifeiyinyue.top/gtfqvgeobo.html

JS:   arr.length
来源：http://hz.iojbl.cn/gtfjjazjti.html

TS:   arr.length
来源：http://hz.shangyingyoupin.top/gtmmyagxjk.html

Java: list.size();
来源：http://hz.shuidangran.top/gtevhbtrle.html

Go:   len(arr)
来源：http://hz.xylfe.cn/gtflzgjxpk.html

Ruby: arr.length; arr.size
来源：http://hz.fengsongda.top/gtcgyrdpzh.html

C#:   list.Count;
来源：http://hz.shanyushiyangtech.top/gteyvmdwnz.html

[D07] 切片 / 取子数组
来源：http://hz.zdqjudy.top/gtejbtdapi.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.mhx1999.top/gtwtutloek.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.mhx1999.top/gtmlueowze.html

JS:   arr.slice(1, 4);
来源：http://hz.hnqzz.top/gthbabplpr.html

TS:   arr.slice(1, 4);
来源：http://hz.smart0.xyz/gtndzhbqji.html

Java: list.subList(1, 4);
来源：http://hz.yonumen.top/gtfeydefms.html

Go:   arr[1:4]
来源：http://hz.hammf.cn/gthhvphagw.html

Ruby: arr[1, 3]
来源：http://hz.tanke756.top/gtqbfoxxdk.html

C#:   list.GetRange(1, 3);
来源：http://hz.daxiang520.top/gtnyhwzvvu.html

[D08] 合并两个数组
来源：http://hz.c1oappe.top/gtqqiyqkrq.html

Py:   a + b;  a.extend(b)
来源：http://hz.meibo888.top/gtgfhoblje.html

PHP:  array_merge($a, $b);
来源：http://hz.feifeiyinyue.top/gthlifinut.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.nwbrower.top/gtmtfzsczk.html

TS:   [...a, ...b];
来源：http://hz.xinyue.icu/gtgiodcdsq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.gzhubu.top/gtyupqkfdx.html

Go:   append(a, b...)
来源：http://hz.zhoulong.xyz/gtefwkcsnm.html

Ruby: a + b;  a.concat(b)
来源：http://hz.ybcxt.top/gtntxvknye.html

C#:   a.Concat(b).ToList()
来源：http://hz.cqqwz.cn/gtwgnjfemp.html

[D09] 排序（升序）
来源：http://hz.jiagoushi.top/gtdmadxooj.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.pengpengdd.cyou/gtdusidqfr.html

PHP:  sort($arr);
来源：http://hz.xinyue.icu/gtqnuswtnw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.pengpengdd.cyou/gtfhtqhtyj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.shuidangran.top/gtlmphdfwx.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jinyuanbaomall.cn/gtidxmsncv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yonumen.top/gtdmtfoecj.html

Ruby: arr.sort
来源：http://hz.yj202588.top/gtsbyknddb.html

C#:   list.Sort();
来源：http://hz.shzxlz.cn/gtuaydqesw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.gogol.net.cn/gtivhgmcci.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yongpay.top/gtvmcjmktu.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhongyouzk.top/gtivqqggch.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.sxryk.cn/gtwbscuirr.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cashguo.top/gtmxyamnrl.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jinyuanbaomall.cn/gtrnixkzxz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.xuetiantiany.cn/gtcrziamty.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yj202588.top/gtxlyzzbka.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.meibo888.top/gtrtskalxi.html

[D11] 反转数组
来源：http://hz.ybcxt.top/gtkvmtdldp.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.wangdashe.top/gtvtisqcxw.html

PHP:  array_reverse($arr);
来源：http://hz.guannengcc.top/gtgdwyihnk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.shzxlz.cn/gtpwluokox.html

TS:   [...arr].reverse();
来源：http://hz.jqgfzy.top/gtkwdygtxc.html

Java: Collections.reverse(list);
来源：http://hz.zhiwuduotai.top/gtokhlilce.html

Go:   slices.Reverse(arr)
来源：http://hz.9152youxi.cn/gtawaktisx.html

Ruby: arr.reverse
来源：http://hz.nanxuanxn.top/gtgcmmexgc.html

C#:   list.Reverse();
来源：http://hz.guowangkeji.top/gtfcutrqhd.html

[D12] 查找元素下标
来源：http://hz.hysaishi.cn/gtbcllyjxy.html

Py:   arr.index(x);  x in arr
来源：http://hz.iojbl.cn/gthhmfntsj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.shanyushiyangkeji.top/gtozyinegl.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.chenlongwang.top/gthwtggexd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yonumen.top/gtgbhcgxfr.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.gogol.net.cn/gtvxruobdj.html

Go:   slices.Index(arr, x)
来源：http://hz.gotoacloud.top/gtpjivixdz.html

Ruby: arr.index(x)
来源：http://hz.gzhubu.top/gtehtfpmos.html

C#:   list.IndexOf(x);
来源：http://hz.cqqwz.cn/gtdnwecler.html

[D13] 过滤（保留满足条件的）
来源：http://hz.xziqi.cn/gtobsxyual.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zhongyouzk.top/gtxbvwxjpi.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yuanzhike.top/gtzsisdsud.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yj202588.top/gtjvruieyb.html

TS:   arr.filter(x => x > 3)
来源：http://hz.xingfuxueyuan.xyz/gtsrslvszu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.nanxuanxn.top/gtggxidgsw.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yongpay.top/gtjdcynqqr.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.ydzc1.top/gtsjpkbuwh.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.pycfn.com/gtqydjqvza.html

[D14] 映射转换（每个元素变形）
来源：http://hz.9152youxi.cn/gttlxzitix.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jiagoushi.top/gtqzoccqqf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.zhoulong.xyz/gtypgagzrw.html

JS:   arr.map(x => x * 2)
来源：http://hz.jlsjyb.cn/gttyethzvo.html

TS:   arr.map(x => x * 2)
来源：http://hz.316326.xyz/gtnrahemfn.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zhaomingkeji.xyz/gteaagyyud.html

Go:   // 手写循环
来源：http://hz.havefunace.top/gtpzwzgvjn.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.cashguo.top/gtinnyyusc.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.dashuyun.cn/gtzzefxpuu.html

[D15] 去重
来源：http://hz.xinyue.icu/gtvszlstco.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.cucudq.cn/gtiywmjtys.html

PHP:  array_unique($arr);
来源：http://hz.zhongyouzk.top/gtwxnrrlge.html

JS:   [...new Set(arr)]
来源：http://hz.yanxiufei.cn/gtwtstltim.html

TS:   [...new Set(arr)]
来源：http://hz.chenlongwang.top/gtehyzxebr.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.tian-w.cn/gtvhapaxru.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.chenjidiqi.icu/gtfinpvhnt.html

Ruby: arr.uniq
来源：http://hz.sxryk.cn/gtmvgrbvpv.html

C#:   list.Distinct().ToList()
来源：http://hz.fzhhl.top/gtbdnwxlmr.html

[D16] 求和与平均值
来源：http://hz.gogol.net.cn/gttfrtjgmp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jinyuanbaomall.cn/gtxqdmaaba.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.gotoacloud.top/gtpiwssqfp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hysaishi.cn/gtucztofkq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cashguo.top/gtlgnscnzs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jianghu66.top/gtfgkmbfou.html

Go:   // 手写循环累加
来源：http://hz.hfpthk.cn/gtpomqzogr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yanxiufei.cn/gtjjxwaiql.html

C#:   list.Sum();  list.Average()
来源：http://hz.bjfxy.top/gtnuqrkbkx.html

[D17] 最大值与最小值
来源：http://hz.shuidangran.top/gtqpetubxt.html

Py:   max(arr);  min(arr)
来源：http://hz.0kj1m.cn/gtnuvngvtu.html

PHP:  max($arr);  min($arr);
来源：http://hz.pengpengdd.cyou/gtdtnrowoy.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.pengpengdd.cyou/gtzqnkkxfk.html

TS:   Math.max(...arr);
来源：http://hz.yj20258.top/gtaulltrhg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.dianchejie.cn/gtuukgkhru.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.cheryme.top/gtrfsynojy.html

Ruby: arr.max;  arr.min
来源：http://hz.havefunace.top/gtjfbqtybk.html

C#:   list.Max();  list.Min()
来源：http://hz.nanxinkj.top/gtrbmtxwyf.html

[D18] 扁平化嵌套数组
来源：http://hz.zdqjudy.top/gtntircmzx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.gaohongyu789.top/gtmpubxpnx.html

PHP:  array_merge(...$nested);
来源：http://hz.snrcjt.cn/gtprolcuwd.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.xuetiantiany.cn/gttbivfxmk.html

TS:   nested.flat();
来源：http://hz.xuanzx.com/gtcdghuzys.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.tian-w.cn/gtuhqzwbvn.html

Go:   // 手写双层循环
来源：http://hz.9152youxi.cn/gtsbfwmqal.html

Ruby: nested.flatten
来源：http://hz.shangyingyoupin.top/gtgtqaptxn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.daxiang520.top/gtzihmltgg.html

[D19] 按字段分组
来源：http://hz.zhengqikj.top/gtrnxabsbl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.c1oappe.top/gtblkxmesp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.xinyue.icu/gtpgkzctrt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.shanyushiyangkeji.top/gtnvuuteis.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.wangdashe.top/gtrtlqatdt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.sweek.top/gtagsipzvw.html

Go:   // 手写 map[string][]T
来源：http://hz.zdqjudy.top/gtpkdnlqyv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.sxryk.cn/gtqzkcvrgs.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jianghu66.top/gtnfefddez.html

[D20] 统计每个元素出现次数
来源：http://hz.bjfxy.top/gttbunrsrj.html

Py:   Counter(arr)
来源：http://hz.hnqzz.top/gtejnaliqd.html

PHP:  array_count_values($arr);
来源：http://hz.yj202588.top/gtoxydirhs.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.dianchejie.cn/gtyygwfitm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cdnleiting.top/gtagnpusui.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yj20258888.top/gtfhnzvnet.html

Go:   // 手写 map[T]int
来源：http://hz.ydjk.org.cn/gtcxbukkki.html

Ruby: arr.tally
来源：http://hz.zhijiandao.cn/gtszwkxdgu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zhixingplan.top/gtrjvdpsdc.html

[D21] 判断是否包含某元素
来源：http://hz.ydzc1.top/gtecxilrjh.html

Py:   x in arr
来源：http://hz.shzxlz.cn/gtvedjgucj.html

PHP:  in_array($x, $arr, true);
来源：http://hz.ivvv.top/gtauazzmxv.html

JS:   arr.includes(x)
来源：http://hz.havefunace.top/gtvmddjyec.html

TS:   arr.includes(x)
来源：http://hz.tianlin.xyz/gtsrhacnbs.html

Java: list.contains(x)
来源：http://hz.yonumen.top/gtbjeqjbsk.html

Go:   slices.Contains(arr, x)
来源：http://hz.ydjk.org.cn/gtgkmdhofi.html

Ruby: arr.include?(x)
来源：http://hz.cashguo.top/gtwjsaotkg.html

C#:   list.Contains(x)
来源：http://hz.pycfn.com/gtnxpcbltv.html

[D22] 复制数组（避免共享引用）
来源：http://hz.hysaishi.cn/gtcqzhltex.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.nanxinkj.top/gtdymnpytq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.sweek.top/gtdqaydjbr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.fzhhl.top/gtotyvpalk.html

TS:   [...arr];
来源：http://hz.iojbl.cn/gtmhmweeif.html

Java: new ArrayList<>(list);
来源：http://hz.guowangkeji.top/gtuduhsxsg.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.cashguo.top/gtqmhlgbyy.html

Ruby: arr.dup;  arr.clone
来源：http://hz.meibo888.top/gtwezekwin.html

C#:   new List<int>(list);
来源：http://hz.yj202588.top/gttkoskgpm.html

[D23] reduce 累积计算
来源：http://hz.hywenlv.cn/gtldgrtwqh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.c1oappe.top/gtvkeaqsxm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jqgfzy.top/gtkflswckr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ybcxt.top/gtnkafdijj.html


<!-- 参考信息 -->