代发 wailian999

[C10] 变量作用域
来源：http://hz.cucudq.cn/gtftegewzb.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.jlsjyb.cn/gtzgkiunjm.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.wangshuangyany.cn/gtyrcihpog.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.zhaomingkeji.xyz/gttegpycfj.html

TS:   同 JS
来源：http://hz.ppjwa.cn/gtisrdvjuo.html

Java: 方法内为块级作用域
来源：http://hz.cqqwz.cn/gtjxjmrbvx.html

Go:   花括号块级作用域
来源：http://hz.zhongyouzk.top/gtmgarhcoz.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.jqgfzy.top/gtkrtpxhiu.html

C#:   块级作用域
来源：http://hz.kuanghao11.cn/gtnyzoholh.html

[C11] 模块导入与导出
来源：http://hz.yangfankeji.com/gtohpeqgfp.html

Py:   from module import func
来源：http://hz.wangdashe.top/gtzeygamoz.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.zhongyouzk.top/gtfswrfxbj.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.smart0.xyz/gtkckonsff.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.yanxiufei.cn/gtpveeueaw.html

Java: import java.util.List;
来源：http://hz.xinyue.icu/gtotisjzdl.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.yangfankeji.com/gtthavdgaa.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.yj20258.top/gtdyedpcjh.html

C#:   using System.Text;
来源：http://hz.wangdashe.top/gttmenpeyg.html

[C12] 立即执行函数 IIFE
来源：http://hz.sufxvd.cn/gtxyuzkkgy.html

Py:   (lambda: print("run"))()
来源：http://hz.iojbl.cn/gtpemmhecb.html

PHP:  (function () { echo "run"; })();
来源：http://hz.ivvv.top/gtgqrfmcfj.html

JS:   (() => { console.log("run"); })();
来源：http://hz.bjfxy.top/gteovxuziw.html

TS:   (() => { console.log("run"); })();
来源：http://hz.ydzc1.top/gtxbcpzqmq.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yanxiufei.cn/gtvbfgscvl.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.ehwqpu.com/gtomkpqbfn.html

Ruby: -> { puts "run" }.call
来源：http://hz.xingfuxueyuan.xyz/gtdffvrevh.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.sxryk.cn/gtaguqplnl.html

[C13] 类型声明 / 类型注解
来源：http://hz.ydjk.org.cn/gtyxalnnpv.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.xziqi.cn/gtcgkusnca.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.meibo888.top/gtwqkxmecs.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.jqgufenzy.top/gtelsxsszn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.xuanzx.com/gttmccitng.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.andypj.xyz/gtwldrdcux.html

Go:   func add(a, b int) int
来源：http://hz.52xcode.cn/gtbacdjzih.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.jlsjyb.cn/gtaakxbgpg.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.aizwys.cn/gtzpmisyaq.html

[C14] 泛型函数
来源：http://hz.shanyushiyangkeji.top/gttwesmarb.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.316326.xyz/gtfyromscs.html

PHP:  // 无泛型
来源：http://hz.zhongyouzk.top/gtokxszpkk.html

JS:   // 无泛型
来源：http://hz.yj20258.top/gtyvzzbyal.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.316326.xyz/gtmufffbjm.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.jyoumei.cn/gtuuolmiew.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.guowangkeji.top/gtfpmemydw.html

Ruby: # 无泛型
来源：http://hz.chenlongwang.top/gtkklelqhp.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.jianghu66.top/gtxfxkdgqr.html

[C15] 解构 / 展开参数
来源：http://hz.xuetiantiany.cn/gtlnhedgae.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.shanyushiyangkeji.top/gtalnsqkum.html

PHP:  [$a, $b] = $pair;
来源：http://hz.andypj.xyz/gteuadhaqp.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.nanxinkj.top/gtjudlazfb.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.redwolf501.top/gtwvwwrywj.html

Java: // 无解构
来源：http://hz.fengsongda.top/gtdkjnzdxu.html

Go:   // 无解构
来源：http://hz.daria6918.cn/gtlgtsgnaa.html

Ruby: a, b = pair
来源：http://hz.kuanghao11.cn/gtbpcukfqt.html

C#:   var (a, b) = pair;
来源：http://hz.yj20258888.top/gtwhppjsnx.html

[C16] 函数 / 方法重载
来源：http://hz.gogol.net.cn/gtjrszzpeq.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yvedp.cn/gtdviijcyi.html

PHP:  // 无重载
来源：http://hz.ybcxt.top/gtpucqqrop.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.shanyushiyangkeji.top/gtobxwjjui.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.nanxinkj.top/gteuuzrjit.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.jinyuanbaomall.cn/gtxjshlcon.html

Go:   // 无重载：用不同函数名
来源：http://hz.zhoulong.xyz/gtestsfgnt.html

Ruby: # 无重载：靠动态参数
来源：http://hz.hywenlv.cn/gttrntxjrp.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.yueranfly.top/gtyiaftwnn.html

================================================================================
来源：http://hz.aizwys.cn/gtjwzsyyed.html

D. 数组 / 列表 / 集合
来源：http://hz.xingfuxueyuan.xyz/gttgcickdf.html

================================================================================
来源：http://hz.yangfankeji.com/gthctmdfcu.html

[D01] 创建数组 / 列表
来源：http://hz.daria6918.cn/gtzbuudpys.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.feifeiyinyue.top/gtmorqqqni.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.aizwys.cn/gtnbwniwhg.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.dashuyun.cn/gtkjgdsuty.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.yonumen.top/gtulipfnop.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.jinghuilouyu.cn/gtmvyfztrm.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.zhiwuduotai.top/gtbyplcjwx.html

Ruby: arr = [1, 2, 3]
来源：http://hz.jinqigufen.top/gtbycjmjbe.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.meibo888.top/gttobgecpq.html

[D02] 追加元素到末尾
来源：http://hz.gaohongyu789.top/gtyoatrymg.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.pengpengdd.cyou/gtssplyjdu.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.hnxiangtu.top/gtcimsxuyw.html

JS:   arr.push(4);
来源：http://hz.andypj.xyz/gttgrnyejz.html

TS:   arr.push(4);
来源：http://hz.jqgufenzy.top/gtkeputbjn.html

Java: list.add(4);
来源：http://hz.cqqwz.cn/gtwzpsosxl.html

Go:   arr = append(arr, 4)
来源：http://hz.9152youxi.cn/gtamuiezse.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.zhongyouzk.top/gtnpogxvnn.html

C#:   list.Add(4);
来源：http://hz.fengsongda.top/gtqwezxiwa.html

[D03] 在指定位置插入元素
来源：http://hz.jianghu66.top/gtvdgqmima.html

Py:   arr.insert(0, 0)
来源：http://hz.snrcjt.cn/gtasvqamce.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.ydzc1.top/gtmwvcndgd.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.shuidangran.top/gtdnbzwpni.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.xinyue.icu/gtohypropc.html

Java: list.add(0, 0);
来源：http://hz.shzxlz.cn/gtlqjmnnfo.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.jqgufenzy.top/gtejdmhmga.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.wangdashe.top/gtmdanhipe.html

C#:   list.Insert(0, 0);
来源：http://hz.hammf.cn/gtprggzvgs.html

[D04] 删除元素
来源：http://hz.zhijiandao.cn/gtzjiqcktw.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhengqikj.top/gtsigaiweb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zhengqikj.top/gtacwjyhcn.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.jlsjyb.cn/gtnokbitwl.html

TS:   arr.splice(0, 1);
来源：http://hz.birdmap.top/gtwgdhnlbj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.ywan-chungtsiang.top/gtxoogxnys.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.hywenlv.cn/gtycibgzqp.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.zhengqikj.top/gtffyycaee.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.ydjk.org.cn/gtmngawzip.html

[D05] 访问与修改元素
来源：http://hz.sufxvd.cn/gtngpmmett.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.guowangkeji.top/gtzmztaqar.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.sweek.top/gtjwhrimkf.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.chenjidiqi.icu/gterfpizcd.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jinyuanbaomall.cn/gtdhlukqey.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.nwbrower.top/gtorsfwewb.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.vqdsnc.cn/gtzyeneqvi.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zhixingplan.top/gtplaimgal.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jyoumei.cn/gtclglvdfv.html

[D06] 数组长度
来源：http://hz.andypj.xyz/gtudazadll.html

Py:   len(arr)
来源：http://hz.shanyushiyangtech.top/gtwhszjlmp.html

PHP:  count($arr);
来源：http://hz.nanxuanxn.top/gtcaoyulyw.html

JS:   arr.length
来源：http://hz.jiagoushi.top/gtvjcvxizb.html

TS:   arr.length
来源：http://hz.jlsjyb.cn/gtlcjqxoxo.html

Java: list.size();
来源：http://hz.xylfe.cn/gtrwtjngyw.html

Go:   len(arr)
来源：http://hz.zhixingplan.top/gtrkrivbqe.html

Ruby: arr.length; arr.size
来源：http://hz.daria6918.cn/gtwhrxunvk.html

C#:   list.Count;
来源：http://hz.bjfxy.top/gtjzvvxvmn.html

[D07] 切片 / 取子数组
来源：http://hz.fengsongda.top/gtsdrrvnjy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.xuanzx.com/gtfkavqhkq.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.zycfv.cn/gttkrldaku.html

JS:   arr.slice(1, 4);
来源：http://hz.iojbl.cn/gtmpjxjdhz.html

TS:   arr.slice(1, 4);
来源：http://hz.xuetiantiany.cn/gtuxgbxmqm.html

Java: list.subList(1, 4);
来源：http://hz.cdnleiting.top/gtfhkgxuvz.html

Go:   arr[1:4]
来源：http://hz.ywan-chungtsiang.top/gtotjmcycj.html

Ruby: arr[1, 3]
来源：http://hz.sufxvd.cn/gtnyxuomgn.html

C#:   list.GetRange(1, 3);
来源：http://hz.jyoumei.cn/gtxwnvxmuh.html

[D08] 合并两个数组
来源：http://hz.yj20258.top/gttqrxvyro.html

Py:   a + b;  a.extend(b)
来源：http://hz.hnqzz.top/gtliofllpo.html

PHP:  array_merge($a, $b);
来源：http://hz.xziqi.cn/gtnfrbwdta.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.smart0.xyz/gterwurcmd.html

TS:   [...a, ...b];
来源：http://hz.yueranfly.top/gtggxvnbjg.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.andypj.xyz/gtgrzkivqc.html

Go:   append(a, b...)
来源：http://hz.hammf.cn/gtxpagipsp.html

Ruby: a + b;  a.concat(b)
来源：http://hz.gotoacloud.top/gtlgabnecf.html

C#:   a.Concat(b).ToList()
来源：http://hz.aibaodan.cn/gthsldvjgv.html

[D09] 排序（升序）
来源：http://hz.jqgufenzy.top/gthanupmqw.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xuetiantiany.cn/gtgwxztshl.html

PHP:  sort($arr);
来源：http://hz.guowangkeji.top/gtcxuiurhm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.ydjk.org.cn/gtjjlvlxwj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.chenjidiqi.icu/gtmmzoaqcf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jiagoushi.top/gtlkivnybh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.ybcxt.top/gtccqutmdi.html

Ruby: arr.sort
来源：http://hz.nwbrower.top/gtrewhtapg.html

C#:   list.Sort();
来源：http://hz.ydjk.org.cn/gtlgtcvwqi.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zhengqikj.top/gtwlhaukea.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.nanxinkj.top/gttdahdmyx.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jiagoushi.top/gtmicowtwg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhengqikj.top/gtimpnvdoj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ywan-chungtsiang.top/gtlbkvoosj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.cqqwz.cn/gtemlicbja.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.c1oappe.top/gtidhepzhl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.0kj1m.cn/gthrqdbecj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jinqigfzy.top/gtkybmtwkx.html

[D11] 反转数组
来源：http://hz.nwbrower.top/gtwynlahiw.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.redwolf501.top/gtkiotliwt.html

PHP:  array_reverse($arr);
来源：http://hz.yj20258888.top/gtrxbmrjkk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.ehwqpu.com/gtewjmxmet.html

TS:   [...arr].reverse();
来源：http://hz.hysaishi.cn/gtbgtxnnor.html

Java: Collections.reverse(list);
来源：http://hz.yueranfly.top/gtkjuuwdte.html

Go:   slices.Reverse(arr)
来源：http://hz.tianlin.xyz/gtoqnvjgbu.html

Ruby: arr.reverse
来源：http://hz.wangshuangyany.cn/gtrdauvkuf.html

C#:   list.Reverse();
来源：http://hz.ivvv.top/gtqrtslwwf.html

[D12] 查找元素下标
来源：http://hz.shanyushiyangkeji.top/gtopvhukiu.html

Py:   arr.index(x);  x in arr
来源：http://hz.daria6918.cn/gtlzxmkkbf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.meibo888.top/gtwibqbjxe.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.pycfn.com/gtalgkfvoi.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.aizwys.cn/gtjlgmcggy.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yj202588.top/gtrsqgebmx.html

Go:   slices.Index(arr, x)
来源：http://hz.ydjk.org.cn/gtlttfffqs.html

Ruby: arr.index(x)
来源：http://hz.yj20258.top/gthyuvnpha.html

C#:   list.IndexOf(x);
来源：http://hz.chenzaomai.com/gtrvflrzaq.html

[D13] 过滤（保留满足条件的）
来源：http://hz.aibaodan.cn/gtakdauyzh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.cqqwz.cn/gttpstcmjo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jinghuilouyu.cn/gthmymurgn.html

JS:   arr.filter(x => x > 3)
来源：http://hz.aizwys.cn/gtrrfnwjrz.html

TS:   arr.filter(x => x > 3)
来源：http://hz.svipenyu.cn/gtrvprvffq.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.sweek.top/gtxhjnmtty.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jianghu66.top/gtyrnnxhwa.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.yj202588.top/gtwvvspjiy.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yongpay.top/gtvlncnmor.html

[D14] 映射转换（每个元素变形）
来源：http://hz.gotoacloud.top/gtdymzyccc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.redwolf501.top/gtpbtdzwek.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.kuanghao11.cn/gtlpfbddah.html

JS:   arr.map(x => x * 2)
来源：http://hz.pycfn.com/gtixmilewf.html

TS:   arr.map(x => x * 2)
来源：http://hz.xingfuxueyuan.xyz/gtgblowiwy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jinqigufen.top/gtzzwrdszh.html

Go:   // 手写循环
来源：http://hz.tian-w.cn/gtntndvhvq.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.ivvv.top/gtkrkikecv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jianghu66.top/gtbwswfcsw.html

[D15] 去重
来源：http://hz.tanke756.top/gtdocbbqnu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yuxming.cn/gtnqegnsuw.html

PHP:  array_unique($arr);
来源：http://hz.yongpay.top/gtcadjjrpx.html

JS:   [...new Set(arr)]
来源：http://hz.svipenyu.cn/gtkvgwtvhj.html

TS:   [...new Set(arr)]
来源：http://hz.sweek.top/gtbeawfgkl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yongpay.top/gtckpfmlts.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.xuetiantiany.cn/gterizcsqe.html

Ruby: arr.uniq
来源：http://hz.zycfv.cn/gttecqcead.html

C#:   list.Distinct().ToList()
来源：http://hz.daxiang520.top/gtclxnvzrr.html

[D16] 求和与平均值
来源：http://hz.gzhubu.top/gtbxxvjfzk.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.aizwys.cn/gttlnbmpar.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.sxryk.cn/gtacheqfkf.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.guowangkeji.top/gtsdtmkfmb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.redwolf501.top/gtukjeqxvx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.cheryme.top/gtmkkhmvqp.html

Go:   // 手写循环累加
来源：http://hz.shzxlz.cn/gtfabwusjd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhongyouzk.top/gtiioddtlt.html

C#:   list.Sum();  list.Average()
来源：http://hz.sweek.top/gtqvjofqhm.html

[D17] 最大值与最小值
来源：http://hz.sufxvd.cn/gtdfylpqaw.html

Py:   max(arr);  min(arr)
来源：http://hz.zhaomingkeji.xyz/gtiiporkhe.html

PHP:  max($arr);  min($arr);
来源：http://hz.hywenlv.cn/gtvomjrakq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.gaohongyu789.top/gtqbxsehbt.html

TS:   Math.max(...arr);
来源：http://hz.nanxuanxn.top/gtirajwiqq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.xuanzx.com/gteuukyzam.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jinghuilouyu.cn/gtuchynvqu.html

Ruby: arr.max;  arr.min
来源：http://hz.xylfe.cn/gtylaqcnav.html

C#:   list.Max();  list.Min()
来源：http://hz.redwolf501.top/gtwdvavivl.html

[D18] 扁平化嵌套数组
来源：http://hz.ivvv.top/gtxztaxtyf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.ybcxt.top/gtpqkuqkux.html

PHP:  array_merge(...$nested);
来源：http://hz.andypj.xyz/gtlihiupec.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.52xcode.cn/gtpsizfybb.html

TS:   nested.flat();
来源：http://hz.mhx1999.top/gtmlbpacrj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.daria6918.cn/gtrfrthubh.html

Go:   // 手写双层循环
来源：http://hz.xuetiantiany.cn/gtugpewzrv.html

Ruby: nested.flatten
来源：http://hz.daria6918.cn/gtbugftdih.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.xuetiantiany.cn/gtowxztznh.html

[D19] 按字段分组
来源：http://hz.ybcxt.top/gtjijstghe.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jiagoushi.top/gthjnxjees.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.hysaishi.cn/gtruqofdvq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.cheryme.top/gtgpgpgpsm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.nanxuanxn.top/gtjqhoduzc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.sxryk.cn/gtfvxydimu.html

Go:   // 手写 map[string][]T
来源：http://hz.jyoumei.cn/gtkoasvqog.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.haohaochexian.top/gtbojvruyd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.smart0.xyz/gthdvbquwg.html

[D20] 统计每个元素出现次数
来源：http://hz.quarkkingdee.top/gtqktfjlhv.html

Py:   Counter(arr)
来源：http://hz.hfpthk.cn/gtsqmrpxah.html

PHP:  array_count_values($arr);
来源：http://hz.pengpengdd.cyou/gtwojmtoxy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.haohaochexian.top/gtdssfboif.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.meibo888.top/gtyqjavqyb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.hfpthk.cn/gtztsehioi.html

Go:   // 手写 map[T]int
来源：http://hz.jqgufenzy.top/gtqgitwjpp.html

Ruby: arr.tally
来源：http://hz.hfpthk.cn/gthaitxakr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.hnqzz.top/gthwuzinis.html

[D21] 判断是否包含某元素
来源：http://hz.zhijiandao.cn/gtcmzrziij.html

Py:   x in arr
来源：http://hz.dashuyun.cn/gtcggqznld.html

PHP:  in_array($x, $arr, true);
来源：http://hz.meibo888.top/gtvhtalgby.html

JS:   arr.includes(x)
来源：http://hz.gzhubu.top/gtzmcvvsgq.html

TS:   arr.includes(x)
来源：http://hz.ywan-chungtsiang.top/gtgvxpaski.html

Java: list.contains(x)
来源：http://hz.zhiwuduotai.top/gtgvlhddct.html

Go:   slices.Contains(arr, x)
来源：http://hz.ywan-chungtsiang.top/gtnuleijmo.html

Ruby: arr.include?(x)
来源：http://hz.birdmap.top/gtpqhyceqr.html

C#:   list.Contains(x)
来源：http://hz.jyoumei.cn/gtgdlygyby.html

[D22] 复制数组（避免共享引用）
来源：http://hz.pycfn.com/gtbmhgvnjx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.cucudq.cn/gtkpenjtqp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yuanzhike.top/gtkjvbyklw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.snrcjt.cn/gtnucuwfbb.html

TS:   [...arr];
来源：http://hz.zdqjudy.top/gtlxmceuai.html

Java: new ArrayList<>(list);
来源：http://hz.wangshuangyany.cn/gtivazyspu.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.c1oappe.top/gthxshcrro.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jinqigufen.top/gtceydnnvu.html

C#:   new List<int>(list);
来源：http://hz.xylfe.cn/gtvnqbwwft.html

[D23] reduce 累积计算
来源：http://hz.quarkkingdee.top/gtfeflxuyf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.pengpengdd.cyou/gtpocxexkl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jinqigfzy.top/gtskijsfud.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shzxlz.cn/gtmdfjdmyx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinghuilouyu.cn/gtauecezws.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.zhoulong.xyz/gtxhxqqbjo.html

Go:   // 手写循环
来源：http://hz.gotoacloud.top/gtoeajjuho.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.shangyingyoupin.top/gtrxvetmop.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.ivvv.top/gtdgqazvqx.html

[D24] 字典 / Map 基本操作
来源：http://hz.feifeiyinyue.top/gtjoceecjv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.quarkkingdee.top/gtcuekoxsh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.sysykeji.top/gtjhhmnjfh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.ydzc1.top/gtagubwcnz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.hongshengwenyu.top/gtxarwlojb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.havefunace.top/gtsubtyjhw.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.xingfuxueyuan.xyz/gtncrbmfsx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.cdnleiting.top/gtagkzpndb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.shanyushiyangtech.top/gtieryhdht.html

[D25] Set 集合去重与交并差
来源：http://hz.ehwqpu.com/gtaujqgiul.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.hfpthk.cn/gttkxgrbex.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jinqigfzy.top/gtvbslydni.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.kuanghao11.cn/gtahgstvbb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.chenjidiqi.icu/gtzrrzgwpa.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.aizwys.cn/gtwensghvv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.ehwqpu.com/gtzmbpxpdb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.tian-w.cn/gtlnnchvix.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.svipenyu.cn/gtzityfeqb.html

[D26] 数组转字符串
来源：http://hz.ivvv.top/gtwdhqkncc.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yuxming.cn/gtntmmwhjk.html

PHP:  implode(", ", $arr);
来源：http://hz.zhaomingkeji.xyz/gtoueqafue.html

JS:   arr.join(", ")
来源：http://hz.aibaodan.cn/gtrwhndokg.html

TS:   arr.join(", ")
来源：http://hz.jlsjyb.cn/gteezpmvvt.html

Java: String.join(", ", list)
来源：http://hz.zhongyouzk.top/gtfkudrrnq.html

Go:   strings.Join(strs, ", ")
来源：http://hz.mhx1999.top/gtlynpdfcp.html

Ruby: arr.join(", ")
来源：http://hz.ywan-chungtsiang.top/gtyxwktbjy.html

C#:   string.Join(", ", list)
来源：http://hz.nwbrower.top/gtvnmlerio.html


<!-- 参考信息 -->