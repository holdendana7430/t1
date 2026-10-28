代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.sxryk.cn/gttwxhmaur.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.c1oappe.top/gtrzhlhvyp.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.wangdashe.top/gtmphobwvm.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.zhongyouzk.top/gtbkjgrzxu.html

[C10] 变量作用域
来源：http://hz.xziqi.cn/gtnucrufdd.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.xinyue.icu/gtejqqycpt.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.hywenlv.cn/gtvohyftdo.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.zhijiandao.cn/gtqkpeuraq.html

TS:   同 JS
来源：http://hz.feifeiyinyue.top/gtjpwqvyxb.html

Java: 方法内为块级作用域
来源：http://hz.shanyushiyangtech.top/gtxawxsqbt.html

Go:   花括号块级作用域
来源：http://hz.tanke756.top/gtrvufadix.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.yuanzhike.top/gtrursrdzi.html

C#:   块级作用域
来源：http://hz.sysykeji.top/gtagjduoxo.html

[C11] 模块导入与导出
来源：http://hz.hfpthk.cn/gttrhzuhpx.html

Py:   from module import func
来源：http://hz.yonumen.top/gteotwguqg.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.xylfe.cn/gtymsesayj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.cqqwz.cn/gtmlrrtsjd.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.xuetiantiany.cn/gtwvwgfatw.html

Java: import java.util.List;
来源：http://hz.yongpay.top/gtijiqrsfe.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.birdmap.top/gtxinyeqcs.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.daria6918.cn/gtkjukcyka.html

C#:   using System.Text;
来源：http://hz.chenjidiqi.icu/gtguyebiam.html

[C12] 立即执行函数 IIFE
来源：http://hz.c1oappe.top/gtoznlkfoe.html

Py:   (lambda: print("run"))()
来源：http://hz.yuxming.cn/gtpuauouot.html

PHP:  (function () { echo "run"; })();
来源：http://hz.aibaodan.cn/gtrwfjglpv.html

JS:   (() => { console.log("run"); })();
来源：http://hz.zhaomingkeji.xyz/gtqqhuqbur.html

TS:   (() => { console.log("run"); })();
来源：http://hz.hnxiangtu.top/gttlcdwjke.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.shzxlz.cn/gtpdomyzob.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.hywenlv.cn/gtlcptktfi.html

Ruby: -> { puts "run" }.call
来源：http://hz.zhengqikj.top/gtqhxfacls.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.hammf.cn/gtrcxmllxl.html

[C13] 类型声明 / 类型注解
来源：http://hz.yuxming.cn/gtronegjbj.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.hongshengwenyu.top/gtgcrjnxud.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.chenlongwang.top/gtzlcxlodn.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.nanxinkj.top/gtfewwziaz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hnxiangtu.top/gtirrsiwgw.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.guannengcc.top/gtyjofvfhr.html

Go:   func add(a, b int) int
来源：http://hz.jinyuanbaomall.cn/gtchqaligu.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jyoumei.cn/gttpihqblg.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.gotoacloud.top/gtackbszfv.html

[C14] 泛型函数
来源：http://hz.cheryme.top/gtlicqqlre.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.dianchejie.cn/gthbmbdvry.html

PHP:  // 无泛型
来源：http://hz.pengpengdd.cyou/gtytcgokkq.html

JS:   // 无泛型
来源：http://hz.daria6918.cn/gtfxmmaafa.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.cdnleiting.top/gtzftdcupo.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yonumen.top/gtqepzueuy.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.quarkkingdee.top/gtpoxrbrfx.html

Ruby: # 无泛型
来源：http://hz.yongpay.top/gtqroxoplb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.guowangkeji.top/gtehkbzrma.html

[C15] 解构 / 展开参数
来源：http://hz.vqdsnc.cn/gtsnrqtvxk.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.zhongyouzk.top/gtungobtzm.html

PHP:  [$a, $b] = $pair;
来源：http://hz.daria6918.cn/gtdzelkcwj.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.jinqigufen.top/gtigjqison.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.daxiang520.top/gtvufmueqc.html

Java: // 无解构
来源：http://hz.wangdashe.top/gtpoctltct.html

Go:   // 无解构
来源：http://hz.chenlongwang.top/gttkuhcrqw.html

Ruby: a, b = pair
来源：http://hz.hnqzz.top/gtghduzeyp.html

C#:   var (a, b) = pair;
来源：http://hz.havefunace.top/gtuaosgfie.html

[C16] 函数 / 方法重载
来源：http://hz.hywenlv.cn/gtmbfiijim.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.iojbl.cn/gtdwymiutc.html

PHP:  // 无重载
来源：http://hz.cashguo.top/gtgcgskkgr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.zycfv.cn/gtkmkfsqmz.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yuxming.cn/gtsufgxrrc.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.pycfn.com/gthuuwhjpd.html

Go:   // 无重载：用不同函数名
来源：http://hz.tian-w.cn/gtbraqdunb.html

Ruby: # 无重载：靠动态参数
来源：http://hz.birdmap.top/gtrlyvkvqw.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.gzhubu.top/gtgmfwiwrw.html

================================================================================
来源：http://hz.gogol.net.cn/gtcnpchqao.html

D. 数组 / 列表 / 集合
来源：http://hz.aibaodan.cn/gtxlnehoke.html

================================================================================
来源：http://hz.mhx1999.top/gthsdimjnc.html

[D01] 创建数组 / 列表
来源：http://hz.hnqzz.top/gtyznjceyf.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.zhiwuduotai.top/gtypdiqfqu.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.hammf.cn/gteneatrex.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.zdqjudy.top/gtrmfxxnsj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.jinqigfzy.top/gtwoxhbhsr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.zhongyouzk.top/gtfxvcqwso.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.daxiang520.top/gtyxwbcetd.html

Ruby: arr = [1, 2, 3]
来源：http://hz.shanyushiyangkeji.top/gtsczgmxnh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.gaohongyu789.top/gtewspxeiy.html

[D02] 追加元素到末尾
来源：http://hz.cashguo.top/gtmzcymdhk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.gogol.net.cn/gtgyhmekgo.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jinqigfzy.top/gthqagldrt.html

JS:   arr.push(4);
来源：http://hz.shanyushiyangkeji.top/gtpooxnpzi.html

TS:   arr.push(4);
来源：http://hz.yvedp.cn/gtsjxllklq.html

Java: list.add(4);
来源：http://hz.hfpthk.cn/gtlvnjpdde.html

Go:   arr = append(arr, 4)
来源：http://hz.nanxinkj.top/gtkxqbykks.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yongpay.top/gtidelxlfm.html

C#:   list.Add(4);
来源：http://hz.zhengqikj.top/gtmqdzfumj.html

[D03] 在指定位置插入元素
来源：http://hz.jqgfzy.top/gtqnjvivtb.html

Py:   arr.insert(0, 0)
来源：http://hz.zhaomingkeji.xyz/gtfmopvaik.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.wangshuangyany.cn/gtuuhoxejd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.feifeiyinyue.top/gtcebtljnb.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.zdqjudy.top/gtblqejdmx.html

Java: list.add(0, 0);
来源：http://hz.hammf.cn/gtkxnhzvga.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.gzhubu.top/gtaqhdwyax.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.c1oappe.top/gtaydvfeqa.html

C#:   list.Insert(0, 0);
来源：http://hz.yj202588.top/gtzrjjnfnl.html

[D04] 删除元素
来源：http://hz.ybcxt.top/gtttenllou.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.cdnleiting.top/gtueuelkac.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.quarkkingdee.top/gtobtcwrvy.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.hnqzz.top/gthxuxcndw.html

TS:   arr.splice(0, 1);
来源：http://hz.chenlongwang.top/gthwnzottm.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.zycfv.cn/gtikrxtwwv.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yangfankeji.com/gtcrgrjvap.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.jianghu66.top/gttrusnmls.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.quarkkingdee.top/gtvutrpvqk.html

[D05] 访问与修改元素
来源：http://hz.xingfuxueyuan.xyz/gtvqdthrir.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhijiandao.cn/gttuyyyjgh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.hammf.cn/gthzzwwljz.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.zhiwuduotai.top/gtjapxnway.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.gogol.net.cn/gtpqdcensg.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.zhixingplan.top/gtlpludvyy.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.ywan-chungtsiang.top/gtkwalcucu.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhijiandao.cn/gtnmhpurti.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.bjfxy.top/gtgslwafts.html

[D06] 数组长度
来源：http://hz.shuidangran.top/gtgztpcdmh.html

Py:   len(arr)
来源：http://hz.gotoacloud.top/gtspyccupm.html

PHP:  count($arr);
来源：http://hz.xuanzx.com/gtxahxivpd.html

JS:   arr.length
来源：http://hz.andypj.xyz/gturnncpbu.html

TS:   arr.length
来源：http://hz.smart0.xyz/gtdjbdzvon.html

Java: list.size();
来源：http://hz.andypj.xyz/gtcivdpvez.html

Go:   len(arr)
来源：http://hz.zycfv.cn/gtqijbwkdo.html

Ruby: arr.length; arr.size
来源：http://hz.jianghu66.top/gtchtboipi.html

C#:   list.Count;
来源：http://hz.wangdashe.top/gtvfsassxl.html

[D07] 切片 / 取子数组
来源：http://hz.jinqigufen.top/gttbhhkoop.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yj20258.top/gtijihmkaz.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.9152youxi.cn/gtxvmhmjtr.html

JS:   arr.slice(1, 4);
来源：http://hz.yanxiufei.cn/gtjchjykpm.html

TS:   arr.slice(1, 4);
来源：http://hz.quarkkingdee.top/gtorrkzcnv.html

Java: list.subList(1, 4);
来源：http://hz.sufxvd.cn/gtosudsuhe.html

Go:   arr[1:4]
来源：http://hz.guannengcc.top/gtbjruhvbq.html

Ruby: arr[1, 3]
来源：http://hz.jinqigfzy.top/gthekxoldg.html

C#:   list.GetRange(1, 3);
来源：http://hz.shanyushiyangtech.top/gtrjpkzksx.html

[D08] 合并两个数组
来源：http://hz.kuanghao11.cn/gtvupbeomj.html

Py:   a + b;  a.extend(b)
来源：http://hz.jinghuilouyu.cn/gtiuacncit.html

PHP:  array_merge($a, $b);
来源：http://hz.gotoacloud.top/gtrxnyppum.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.dashuyun.cn/gtalrhagsg.html

TS:   [...a, ...b];
来源：http://hz.zhongyouzk.top/gtnhwuootp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.shanyushiyangkeji.top/gtxdsbzobf.html

Go:   append(a, b...)
来源：http://hz.hnxiangtu.top/gtfejhnuhc.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yuanzhike.top/gthjeukrzq.html

C#:   a.Concat(b).ToList()
来源：http://hz.gogol.net.cn/gtetqckong.html

[D09] 排序（升序）
来源：http://hz.hywenlv.cn/gtezcrbzvf.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.mhx1999.top/gthyeqekgv.html

PHP:  sort($arr);
来源：http://hz.jlsjyb.cn/gtarxxoasz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.iojbl.cn/gtmhgnxrrb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yuanzhike.top/gtbcbahxqe.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.shzxlz.cn/gtttsajajc.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.9152youxi.cn/gtqnqbnqks.html

Ruby: arr.sort
来源：http://hz.gzhubu.top/gtjovymfyz.html

C#:   list.Sort();
来源：http://hz.andypj.xyz/gtofkpjdii.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.iojbl.cn/gtxvfvxnno.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.meibo888.top/gttfylfhed.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cucudq.cn/gtxchulizh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gzhubu.top/gtmzvggasa.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yonumen.top/gtczxeohhg.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.shanyushiyangtech.top/gtbgtjhncv.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.iojbl.cn/gtpblthwip.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.meibo888.top/gtycsljlcr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.hywenlv.cn/gtzwrisihd.html

[D11] 反转数组
来源：http://hz.jiagoushi.top/gtoyoweods.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zhixingplan.top/gtsknrjtlq.html

PHP:  array_reverse($arr);
来源：http://hz.hfpthk.cn/gtywmoxpiu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.c1oappe.top/gtivobuncu.html

TS:   [...arr].reverse();
来源：http://hz.quarkkingdee.top/gtltxmfcvt.html

Java: Collections.reverse(list);
来源：http://hz.guannengcc.top/gtcgbpgqmq.html

Go:   slices.Reverse(arr)
来源：http://hz.chenjidiqi.icu/gtocmawwcr.html

Ruby: arr.reverse
来源：http://hz.zhoulong.xyz/gtyxssfnun.html

C#:   list.Reverse();
来源：http://hz.daxiang520.top/gtrvzizgxd.html

[D12] 查找元素下标
来源：http://hz.sufxvd.cn/gtciobzwex.html

Py:   arr.index(x);  x in arr
来源：http://hz.316326.xyz/gtrjbspgxu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.ywan-chungtsiang.top/gttragynpi.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.wangdashe.top/gtzizrwrtu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.sysykeji.top/gttuzuiaoo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.bjfxy.top/gttbnmoely.html

Go:   slices.Index(arr, x)
来源：http://hz.cashguo.top/gtknawthns.html

Ruby: arr.index(x)
来源：http://hz.dianchejie.cn/gtuuhxamwc.html

C#:   list.IndexOf(x);
来源：http://hz.andypj.xyz/gtakkfsqjw.html

[D13] 过滤（保留满足条件的）
来源：http://hz.shuidangran.top/gtozlovuat.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.gzhubu.top/gthltohdqu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jinqigfzy.top/gtixvdwpmt.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zhijiandao.cn/gtlnqksbyz.html

TS:   arr.filter(x => x > 3)
来源：http://hz.316326.xyz/gtekkshlbh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.svipenyu.cn/gtbeusfohe.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.ppjwa.cn/gtollzfehy.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jqgfzy.top/gtapwfpkvn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.chenzaomai.com/gtrejtcmpc.html

[D14] 映射转换（每个元素变形）
来源：http://hz.andypj.xyz/gtkwnwaxzm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.quarkkingdee.top/gtssgmzrlr.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.nanxinkj.top/gtkaomchew.html

JS:   arr.map(x => x * 2)
来源：http://hz.cheryme.top/gtbjpifdkb.html

TS:   arr.map(x => x * 2)
来源：http://hz.sysykeji.top/gtydtfmhdt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.aizwys.cn/gtwxcewzwb.html

Go:   // 手写循环
来源：http://hz.birdmap.top/gtniiqtmky.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.smart0.xyz/gtqadtndpw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.aibaodan.cn/gtzwiqghpq.html

[D15] 去重
来源：http://hz.pycfn.com/gtiummmqkj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.zhiwuduotai.top/gtzornuovn.html

PHP:  array_unique($arr);
来源：http://hz.nwbrower.top/gtvxlmjagl.html

JS:   [...new Set(arr)]
来源：http://hz.zdqjudy.top/gtvsvcfrki.html

TS:   [...new Set(arr)]
来源：http://hz.smart0.xyz/gtvjayjdfo.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.xinyue.icu/gtzaedoupz.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zycfv.cn/gtywdppfhh.html

Ruby: arr.uniq
来源：http://hz.jqgufenzy.top/gtbtzkijdj.html

C#:   list.Distinct().ToList()
来源：http://hz.zhixingplan.top/gtrwpowdcq.html

[D16] 求和与平均值
来源：http://hz.birdmap.top/gtxqzbgdaq.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.nanxinkj.top/gtpmirdvzt.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.pengpengdd.cyou/gtltydqgpu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.aibaodan.cn/gtbpwigtto.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cashguo.top/gtfppfgurr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.aibaodan.cn/gtsqemvmjw.html

Go:   // 手写循环累加
来源：http://hz.316326.xyz/gtumwtipfa.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.ivvv.top/gtahmmcaio.html

C#:   list.Sum();  list.Average()
来源：http://hz.chenjidiqi.icu/gttkyzpali.html

[D17] 最大值与最小值
来源：http://hz.sufxvd.cn/gtotciaywz.html

Py:   max(arr);  min(arr)
来源：http://hz.yueranfly.top/gticdesepe.html

PHP:  max($arr);  min($arr);
来源：http://hz.yj20258888.top/gthucoogze.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.ehwqpu.com/gtxdahtalz.html

TS:   Math.max(...arr);
来源：http://hz.chenlongwang.top/gtpbwjmukp.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.havefunace.top/gtnblrqnhu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zhaomingkeji.xyz/gtcqhylvqd.html

Ruby: arr.max;  arr.min
来源：http://hz.redwolf501.top/gtpkewdyym.html

C#:   list.Max();  list.Min()
来源：http://hz.xuetiantiany.cn/gtoodhrebb.html

[D18] 扁平化嵌套数组
来源：http://hz.9152youxi.cn/gtpaagvvsj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.aibaodan.cn/gtqtdwytfc.html

PHP:  array_merge(...$nested);
来源：http://hz.feifeiyinyue.top/gtxqgyxcji.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.wangdashe.top/gtpiuuhqoe.html

TS:   nested.flat();
来源：http://hz.xuetiantiany.cn/gtdiywzuvb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.ehwqpu.com/gtikxhmgtw.html

Go:   // 手写双层循环
来源：http://hz.hnxiangtu.top/gtxjoyuade.html

Ruby: nested.flatten
来源：http://hz.wangdashe.top/gtxcklrrbw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.ywan-chungtsiang.top/gtfnkkrhaf.html

[D19] 按字段分组
来源：http://hz.yj202588.top/gtqiptwzgd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jyoumei.cn/gttsuosokm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.fengsongda.top/gththkhvnl.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jianghu66.top/gturlwgurp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.ywan-chungtsiang.top/gtgtlwcaza.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.gzhubu.top/gtiovharfn.html

Go:   // 手写 map[string][]T
来源：http://hz.hnqzz.top/gtckzancib.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.jiagoushi.top/gtncogxveu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.gogol.net.cn/gtbikatsew.html

[D20] 统计每个元素出现次数
来源：http://hz.snrcjt.cn/gtpfruaybb.html

Py:   Counter(arr)
来源：http://hz.pycfn.com/gtpqftoxle.html

PHP:  array_count_values($arr);
来源：http://hz.fzhhl.top/gtcvqutrtg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.snrcjt.cn/gtxpzbpbza.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ydjk.org.cn/gtbdlfblgv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.hammf.cn/gtnxdaprws.html

Go:   // 手写 map[T]int
来源：http://hz.jyoumei.cn/gtenlscrsr.html

Ruby: arr.tally
来源：http://hz.yongpay.top/gtvjccjljh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.andypj.xyz/gteeeovvkm.html

[D21] 判断是否包含某元素
来源：http://hz.bjfxy.top/gtffowfecp.html

Py:   x in arr
来源：http://hz.tianlin.xyz/gtmehkowsl.html

PHP:  in_array($x, $arr, true);
来源：http://hz.tian-w.cn/gtdifupxsb.html

JS:   arr.includes(x)
来源：http://hz.jyoumei.cn/gtiqrqqtpn.html

TS:   arr.includes(x)
来源：http://hz.9152youxi.cn/gtkbbuhmnr.html

Java: list.contains(x)
来源：http://hz.andypj.xyz/gtfnqywfgt.html

Go:   slices.Contains(arr, x)
来源：http://hz.chenjidiqi.icu/gtpgqdpxyr.html

Ruby: arr.include?(x)
来源：http://hz.guowangkeji.top/gtbwrnjrsu.html

C#:   list.Contains(x)
来源：http://hz.zhixingplan.top/gtlpoynrzl.html

[D22] 复制数组（避免共享引用）
来源：http://hz.wangshuangyany.cn/gtanrcgdte.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jianghu66.top/gtpxuhdemq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.hysaishi.cn/gtuqanhsbq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yongpay.top/gtpkjgiqiq.html

TS:   [...arr];
来源：http://hz.chenjidiqi.icu/gtujrhsrgt.html

Java: new ArrayList<>(list);
来源：http://hz.havefunace.top/gtvtnoeujs.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.shzxlz.cn/gtpecipyza.html

Ruby: arr.dup;  arr.clone
来源：http://hz.sxryk.cn/gtmwcnztdl.html

C#:   new List<int>(list);
来源：http://hz.cdnleiting.top/gtvmwpxxpw.html

[D23] reduce 累积计算
来源：http://hz.xziqi.cn/gtmgdgegkt.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.hysaishi.cn/gtqtplobcy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.sysykeji.top/gtqjfpkaqh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xinyue.icu/gtpliqznos.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinqigfzy.top/gtllyvhpmi.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.gaohongyu789.top/gtjehlhnxw.html

Go:   // 手写循环
来源：http://hz.andypj.xyz/gttsycbjtb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.mhx1999.top/gtuiakcrpf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yj20258888.top/gtppxtlkyn.html

[D24] 字典 / Map 基本操作
来源：http://hz.hongshengwenyu.top/gtvpjqdxgd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.andypj.xyz/gtwfyoedwa.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.c1oappe.top/gtpyoovdvw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.aibaodan.cn/gtufixgtat.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yj20258888.top/gtbntwvrab.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jqgfzy.top/gtjmfdweup.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.dianchejie.cn/gttjwlkhab.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.c1oappe.top/gtxoacurfr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.haohaochexian.top/gtrbylqsuk.html

[D25] Set 集合去重与交并差
来源：http://hz.redwolf501.top/gtpvwmcnuy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.wangshuangyany.cn/gtbphtcbtd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jinqigfzy.top/gtajohawmd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.chenlongwang.top/gtymqsoxfq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.ydzc1.top/gtrihsetsv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.vqdsnc.cn/gthinhudfm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.shuidangran.top/gtyxszctoz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yj20258888.top/gtpenxqkgg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.chenzaomai.com/gtytsuxtlf.html

[D26] 数组转字符串
来源：http://hz.wangdashe.top/gtrhdjojxi.html

Py:   ", ".join(map(str, arr))
来源：http://hz.hfpthk.cn/gtnxhvvsla.html

PHP:  implode(", ", $arr);
来源：http://hz.hfpthk.cn/gtrjhftdli.html

JS:   arr.join(", ")
来源：http://hz.sysykeji.top/gtibrasaeg.html

TS:   arr.join(", ")
来源：http://hz.cashguo.top/gtzpbnvvfk.html


<!-- 参考信息 -->