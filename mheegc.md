代发 wailian999

Go:   func counter() func() int { n := 0; return func() int { n++; return n } }
来源：http://hz.52xcode.cn/gtzsfyhrsu.html

Ruby: def counter; n = 0; -> { n += 1 }; end
来源：http://hz.tanke756.top/gthkfkvbzc.html

C#:   static Func<int> Counter() { int n = 0; return () => ++n; }
来源：http://hz.c1oappe.top/gtooarapnw.html

[C09] 递归
来源：http://hz.cdnleiting.top/gtzgohbrhd.html

Py:   def fact(n): return 1 if n <= 1 else n * fact(n - 1)
来源：http://hz.sweek.top/gtqxkvmphw.html

PHP:  function fact(int $n): int { return $n <= 1 ? 1 : $n * fact($n - 1); }
来源：http://hz.sxryk.cn/gtwdbdghvw.html

JS:   const fact = n => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.yongpay.top/gtwtilxreb.html

TS:   const fact = (n: number): number => (n <= 1 ? 1 : n * fact(n - 1));
来源：http://hz.gaohongyu789.top/gtvyyezjdg.html

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.chenlongwang.top/gtxdrtjsmc.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.wangshuangyany.cn/gtmuvoxmls.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.xuetiantiany.cn/gthiuxeboy.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.jinqigfzy.top/gtgpsmfbcr.html

[C10] 变量作用域
来源：http://hz.smart0.xyz/gtknrtgwky.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.cdnleiting.top/gtzzklofev.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.yanxiufei.cn/gtztkdgvrf.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.bjfxy.top/gtkdiizgee.html

TS:   同 JS
来源：http://hz.jqgfzy.top/gtgtnaruuc.html

Java: 方法内为块级作用域
来源：http://hz.dianchejie.cn/gtjvayekoh.html

Go:   花括号块级作用域
来源：http://hz.dashuyun.cn/gtptciiuaq.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.cdnleiting.top/gtoflbuxhd.html

C#:   块级作用域
来源：http://hz.jianghu66.top/gtqmvdnoox.html

[C11] 模块导入与导出
来源：http://hz.aizwys.cn/gtxungnxlk.html

Py:   from module import func
来源：http://hz.yangfankeji.com/gtogcnkcqj.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.yj202588.top/gtkkaiviji.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.pycfn.com/gtoztigzsm.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.jqgufenzy.top/gtcrketzhv.html

Java: import java.util.List;
来源：http://hz.cucudq.cn/gtxqdhekrn.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.52xcode.cn/gtexhcihis.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.mhx1999.top/gtbfbbquwv.html

C#:   using System.Text;
来源：http://hz.ppjwa.cn/gtnaozxakf.html

[C12] 立即执行函数 IIFE
来源：http://hz.sweek.top/gtpxsozukw.html

Py:   (lambda: print("run"))()
来源：http://hz.vqdsnc.cn/gthwfmegjz.html

PHP:  (function () { echo "run"; })();
来源：http://hz.nanxinkj.top/gtojalxfvb.html

JS:   (() => { console.log("run"); })();
来源：http://hz.tanke756.top/gtjawtrqix.html

TS:   (() => { console.log("run"); })();
来源：http://hz.ppjwa.cn/gtqmxzeuit.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.zdqjudy.top/gtppqfqasz.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.zhengqikj.top/gtvfeacxno.html

Ruby: -> { puts "run" }.call
来源：http://hz.hammf.cn/gthghxenst.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.0kj1m.cn/gthxdjynfm.html

[C13] 类型声明 / 类型注解
来源：http://hz.daxiang520.top/gtcnopprbe.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.iojbl.cn/gtzfubfsum.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.xuanzx.com/gtbawmrler.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.316326.xyz/gtodfolnfu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhongyouzk.top/gtmdkhwbqo.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.jiagoushi.top/gtfyhkixfg.html

Go:   func add(a, b int) int
来源：http://hz.316326.xyz/gtukeswjhk.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.birdmap.top/gtrvzbzwqd.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.gotoacloud.top/gtcygjtekk.html

[C14] 泛型函数
来源：http://hz.chenzaomai.com/gtislnkxqn.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.tianlin.xyz/gtevamadeh.html

PHP:  // 无泛型
来源：http://hz.yj202588.top/gtyxaudeov.html

JS:   // 无泛型
来源：http://hz.shanyushiyangtech.top/gtxmthzgrl.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.birdmap.top/gtxzdofqqf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.zhaomingkeji.xyz/gtqmprwdzc.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.ywan-chungtsiang.top/gtaivtbiar.html

Ruby: # 无泛型
来源：http://hz.yj202588.top/gtxasmiiqj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zhongyouzk.top/gtcjicpagl.html

[C15] 解构 / 展开参数
来源：http://hz.jqgufenzy.top/gttekbpqme.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.kuanghao11.cn/gtrtmxfnlu.html

PHP:  [$a, $b] = $pair;
来源：http://hz.zhiwuduotai.top/gtfqvbjvdm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.gaohongyu789.top/gtuvcxxdcf.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.hammf.cn/gtafidbcsf.html

Java: // 无解构
来源：http://hz.hammf.cn/gtjgcteksq.html

Go:   // 无解构
来源：http://hz.chenjidiqi.icu/gttcznwaxf.html

Ruby: a, b = pair
来源：http://hz.ivvv.top/gtntbihqcw.html

C#:   var (a, b) = pair;
来源：http://hz.wangdashe.top/gtacyrjswi.html

[C16] 函数 / 方法重载
来源：http://hz.yj202588.top/gtwclbtzzp.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.dianchejie.cn/gtomcondmg.html

PHP:  // 无重载
来源：http://hz.zycfv.cn/gtdvudaugu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hfpthk.cn/gtabjgskhy.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.ivvv.top/gtltsdqijg.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.aibaodan.cn/gtxgkykdsl.html

Go:   // 无重载：用不同函数名
来源：http://hz.ywan-chungtsiang.top/gtpxqdksly.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yangfankeji.com/gtlykujyco.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.zhixingplan.top/gtljjzvqtd.html

================================================================================
来源：http://hz.kuanghao11.cn/gtzixgxrod.html

D. 数组 / 列表 / 集合
来源：http://hz.vqdsnc.cn/gtzjrpfaun.html

================================================================================
来源：http://hz.meibo888.top/gtdalhhnnb.html

[D01] 创建数组 / 列表
来源：http://hz.ydzc1.top/gtycncxkhp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.ydzc1.top/gtxkqikzfq.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.xziqi.cn/gtdcpcshwo.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.yangfankeji.com/gtxybrsnvx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.jinqigufen.top/gtvqiipveb.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.zhengqikj.top/gtgfedghwk.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.tian-w.cn/gtrybrzivp.html

Ruby: arr = [1, 2, 3]
来源：http://hz.aizwys.cn/gtgziuampi.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.xylfe.cn/gtlqnoekhb.html

[D02] 追加元素到末尾
来源：http://hz.redwolf501.top/gtgpfonryw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.smart0.xyz/gticwyncaj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jinyuanbaomall.cn/gtrzlntltc.html

JS:   arr.push(4);
来源：http://hz.zhengqikj.top/gtjpqfrsfj.html

TS:   arr.push(4);
来源：http://hz.jinqigfzy.top/gtcglmzizr.html

Java: list.add(4);
来源：http://hz.yj20258888.top/gtftbtsnih.html

Go:   arr = append(arr, 4)
来源：http://hz.ppjwa.cn/gtidorsoqw.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.gzhubu.top/gtzzzlszxw.html

C#:   list.Add(4);
来源：http://hz.pycfn.com/gtvxcxydzg.html

[D03] 在指定位置插入元素
来源：http://hz.fzhhl.top/gtjtznjisb.html

Py:   arr.insert(0, 0)
来源：http://hz.nanxuanxn.top/gtloitswcn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.quarkkingdee.top/gtglowomya.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.xziqi.cn/gteadgygqb.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.guannengcc.top/gtklvzddnw.html

Java: list.add(0, 0);
来源：http://hz.andypj.xyz/gtehsfvinl.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yvedp.cn/gtdtuuuliq.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.shangyingyoupin.top/gtbajdljdj.html

C#:   list.Insert(0, 0);
来源：http://hz.daria6918.cn/gttfgcduyp.html

[D04] 删除元素
来源：http://hz.jlsjyb.cn/gtdlmjhqoh.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.xziqi.cn/gtsyzjylxs.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.hysaishi.cn/gtnjttzbtk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.cashguo.top/gtisslgnif.html

TS:   arr.splice(0, 1);
来源：http://hz.wangdashe.top/gtieihnokk.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.fzhhl.top/gtvgmezbxs.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.meibo888.top/gtlffbglcb.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.haohaochexian.top/gtvoqsxbot.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.daria6918.cn/gtxygtvhcn.html

[D05] 访问与修改元素
来源：http://hz.sweek.top/gtydowudos.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.ybcxt.top/gtavpxtxtd.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.andypj.xyz/gtbxzdjyqd.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.hywenlv.cn/gtlfzutbyf.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.hnqzz.top/gtczmzxtlk.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.cqqwz.cn/gtylhdwrvb.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.xingfuxueyuan.xyz/gteuzenvtn.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.nanxuanxn.top/gtjxgeihxf.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.meibo888.top/gtxdvazqwb.html

[D06] 数组长度
来源：http://hz.xuanzx.com/gtmcmpzmkp.html

Py:   len(arr)
来源：http://hz.nanxinkj.top/gtfparouuh.html

PHP:  count($arr);
来源：http://hz.yongpay.top/gtxonmkkmn.html

JS:   arr.length
来源：http://hz.hysaishi.cn/gtymokequf.html

TS:   arr.length
来源：http://hz.zhaomingkeji.xyz/gtgvttbhad.html

Java: list.size();
来源：http://hz.haohaochexian.top/gtufgzkkwi.html

Go:   len(arr)
来源：http://hz.yj20258.top/gtyrtkvsqv.html

Ruby: arr.length; arr.size
来源：http://hz.hfpthk.cn/gtrotwpini.html

C#:   list.Count;
来源：http://hz.yj202588.top/gtasbjqjsz.html

[D07] 切片 / 取子数组
来源：http://hz.yonumen.top/gtdizofjig.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.52xcode.cn/gtonpfmwxe.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yuanzhike.top/gtixjkzits.html

JS:   arr.slice(1, 4);
来源：http://hz.jiagoushi.top/gtfutosxbv.html

TS:   arr.slice(1, 4);
来源：http://hz.gotoacloud.top/gtonqmakff.html

Java: list.subList(1, 4);
来源：http://hz.chenjidiqi.icu/gtaldkremh.html

Go:   arr[1:4]
来源：http://hz.mhx1999.top/gtgduzuvqp.html

Ruby: arr[1, 3]
来源：http://hz.yonumen.top/gtsmrfutpm.html

C#:   list.GetRange(1, 3);
来源：http://hz.zhijiandao.cn/gtzvxmbpin.html

[D08] 合并两个数组
来源：http://hz.yj20258888.top/gtbhwtuyny.html

Py:   a + b;  a.extend(b)
来源：http://hz.fengsongda.top/gtfhgivuca.html

PHP:  array_merge($a, $b);
来源：http://hz.jinyuanbaomall.cn/gtzslmvljb.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yvedp.cn/gtonefftyk.html

TS:   [...a, ...b];
来源：http://hz.pengpengdd.cyou/gtxxvyzpai.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zhiwuduotai.top/gtyeuovoou.html

Go:   append(a, b...)
来源：http://hz.tian-w.cn/gtyanhuyna.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jinyuanbaomall.cn/gtfpiaqggc.html

C#:   a.Concat(b).ToList()
来源：http://hz.chenzaomai.com/gtfdddltid.html

[D09] 排序（升序）
来源：http://hz.cashguo.top/gtzeegquua.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sufxvd.cn/gttgkxjoxx.html

PHP:  sort($arr);
来源：http://hz.ydjk.org.cn/gtzlonwcdf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.ywan-chungtsiang.top/gtqevsiwii.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.aibaodan.cn/gtwrbsocrl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.wangshuangyany.cn/gtxbkolbxn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.zycfv.cn/gtxblupriu.html

Ruby: arr.sort
来源：http://hz.yanxiufei.cn/gtsgmrpzih.html

C#:   list.Sort();
来源：http://hz.gzhubu.top/gtpdpsxajh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.cdnleiting.top/gtiofeeuye.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zhongyouzk.top/gtzijtisms.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.xuanzx.com/gtvkxtbjep.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yuxming.cn/gtbdwlvwhe.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cashguo.top/gtjiprpqos.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.andypj.xyz/gtlqcwawif.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.quarkkingdee.top/gtnxkzgpqb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.birdmap.top/gtsmibypjy.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.gzhubu.top/gtjbylqicb.html

[D11] 反转数组
来源：http://hz.iojbl.cn/gtvvgyetly.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.ppjwa.cn/gtwubyepgl.html

PHP:  array_reverse($arr);
来源：http://hz.xylfe.cn/gtbweqobxg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.ehwqpu.com/gtjkydixki.html

TS:   [...arr].reverse();
来源：http://hz.birdmap.top/gteksldfly.html

Java: Collections.reverse(list);
来源：http://hz.gotoacloud.top/gteugonsef.html

Go:   slices.Reverse(arr)
来源：http://hz.wangdashe.top/gtebezkgfn.html

Ruby: arr.reverse
来源：http://hz.shangyingyoupin.top/gtnxbqyykf.html

C#:   list.Reverse();
来源：http://hz.yuanzhike.top/gtwepuegbn.html

[D12] 查找元素下标
来源：http://hz.sufxvd.cn/gtsfseptvn.html

Py:   arr.index(x);  x in arr
来源：http://hz.52xcode.cn/gtipckorml.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.fzhhl.top/gtraubzona.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.tianlin.xyz/gtokmuftvw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinyuanbaomall.cn/gtdvavdzip.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.sweek.top/gtdpzrqdcb.html

Go:   slices.Index(arr, x)
来源：http://hz.zycfv.cn/gtfxtctsgb.html

Ruby: arr.index(x)
来源：http://hz.zhengqikj.top/gtssnlipfs.html

C#:   list.IndexOf(x);
来源：http://hz.cashguo.top/gtwmlbgunh.html

[D13] 过滤（保留满足条件的）
来源：http://hz.andypj.xyz/gtqvewvhjo.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.xuanzx.com/gtwcwtfbws.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jiagoushi.top/gtdwlpisgw.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hywenlv.cn/gtvrmjbqui.html

TS:   arr.filter(x => x > 3)
来源：http://hz.zhoulong.xyz/gteuutkrra.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.zhaomingkeji.xyz/gtwmfwtqmf.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yongpay.top/gtrvunodcy.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.ehwqpu.com/gtnhsptuuf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.havefunace.top/gtabzfkgca.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yueranfly.top/gtsidxcvyh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.chenzaomai.com/gtiayivkbj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.aibaodan.cn/gtjpyeksrz.html

JS:   arr.map(x => x * 2)
来源：http://hz.snrcjt.cn/gterqfmlmb.html

TS:   arr.map(x => x * 2)
来源：http://hz.shzxlz.cn/gtchqpohiw.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.nwbrower.top/gtqtjqvybq.html

Go:   // 手写循环
来源：http://hz.cashguo.top/gtlhgwgkny.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.sysykeji.top/gtzsyuzmaw.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zdqjudy.top/gtzxtjzqny.html

[D15] 去重
来源：http://hz.jinyuanbaomall.cn/gtbvgymzep.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yuxming.cn/gthmrzmnqk.html

PHP:  array_unique($arr);
来源：http://hz.yuanzhike.top/gtqroakcne.html

JS:   [...new Set(arr)]
来源：http://hz.quarkkingdee.top/gtxkrvoseb.html

TS:   [...new Set(arr)]
来源：http://hz.hongshengwenyu.top/gtbjhlcblc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.hnxiangtu.top/gtnwlpnsmx.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zdqjudy.top/gtftqswncm.html

Ruby: arr.uniq
来源：http://hz.sxryk.cn/gtccbdefmg.html

C#:   list.Distinct().ToList()
来源：http://hz.sxryk.cn/gtvawrivkq.html

[D16] 求和与平均值
来源：http://hz.jinyuanbaomall.cn/gtczlksmun.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.ybcxt.top/gtspzqoolt.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.feifeiyinyue.top/gtbfoypheu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ybcxt.top/gtsswyykyv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.gotoacloud.top/gtrfcbvemb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.xuanzx.com/gtmlaufjdq.html

Go:   // 手写循环累加
来源：http://hz.gzhubu.top/gtphvcxufy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.ybcxt.top/gtbuvbsqyg.html

C#:   list.Sum();  list.Average()
来源：http://hz.zdqjudy.top/gtxhvagwea.html

[D17] 最大值与最小值
来源：http://hz.yuanzhike.top/gthdnxpvzc.html

Py:   max(arr);  min(arr)
来源：http://hz.0kj1m.cn/gtapevslwy.html

PHP:  max($arr);  min($arr);
来源：http://hz.shzxlz.cn/gtelbeznft.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.nanxuanxn.top/gtxameowku.html

TS:   Math.max(...arr);
来源：http://hz.yongpay.top/gtthgtoswj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jyoumei.cn/gtkmhbjdqx.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.kuanghao11.cn/gtjjyqvqpq.html

Ruby: arr.max;  arr.min
来源：http://hz.haohaochexian.top/gtjfzufhpm.html

C#:   list.Max();  list.Min()
来源：http://hz.hnqzz.top/gtovayngcm.html

[D18] 扁平化嵌套数组
来源：http://hz.jianghu66.top/gtbwmrpzux.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yongpay.top/gtdmkosozi.html

PHP:  array_merge(...$nested);
来源：http://hz.zhiwuduotai.top/gtqkvrrfcp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.sufxvd.cn/gtwwqvihen.html

TS:   nested.flat();
来源：http://hz.daria6918.cn/gtqcvxevzb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.quarkkingdee.top/gteavikadq.html

Go:   // 手写双层循环
来源：http://hz.daxiang520.top/gtbhzzfpdk.html

Ruby: nested.flatten
来源：http://hz.zhongyouzk.top/gtlwxzknmy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.guowangkeji.top/gtyfiwbega.html

[D19] 按字段分组
来源：http://hz.shangyingyoupin.top/gtihqmhdri.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.shanyushiyangtech.top/gtixhzgkrz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.hnxiangtu.top/gtaxedliox.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.sweek.top/gtrphkzigd.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.zhengqikj.top/gtkhwsfind.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.ybcxt.top/gtfjolwbzu.html

Go:   // 手写 map[string][]T
来源：http://hz.tanke756.top/gtgyrbnrkt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.xylfe.cn/gttgcywatj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.gotoacloud.top/gtwsfrnvnv.html

[D20] 统计每个元素出现次数
来源：http://hz.zycfv.cn/gtxngzzdoh.html

Py:   Counter(arr)
来源：http://hz.yuanzhike.top/gtnbuimuap.html

PHP:  array_count_values($arr);
来源：http://hz.jinyuanbaomall.cn/gtvybcezjb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.sysykeji.top/gtnqzileww.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hnqzz.top/gtajmdeflz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.guowangkeji.top/gtlduupdow.html

Go:   // 手写 map[T]int
来源：http://hz.bjfxy.top/gtjbnlbyot.html

Ruby: arr.tally
来源：http://hz.guowangkeji.top/gtbnstsmfo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.vqdsnc.cn/gtisrucwpw.html

[D21] 判断是否包含某元素
来源：http://hz.shuidangran.top/gthhbrwive.html

Py:   x in arr
来源：http://hz.shangyingyoupin.top/gtwmlyjugl.html

PHP:  in_array($x, $arr, true);
来源：http://hz.hongshengwenyu.top/gtlrlshdbx.html

JS:   arr.includes(x)
来源：http://hz.jqgfzy.top/gtnqxokzgt.html

TS:   arr.includes(x)
来源：http://hz.iojbl.cn/gtxhsrzcst.html

Java: list.contains(x)
来源：http://hz.xingfuxueyuan.xyz/gtgxttwaox.html

Go:   slices.Contains(arr, x)
来源：http://hz.shangyingyoupin.top/gtwfbkacow.html

Ruby: arr.include?(x)
来源：http://hz.yueranfly.top/gtlyywodkm.html

C#:   list.Contains(x)
来源：http://hz.jinqigufen.top/gtrrdbncee.html

[D22] 复制数组（避免共享引用）
来源：http://hz.shzxlz.cn/gtjceocucn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.ybcxt.top/gtfhjyhkui.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.snrcjt.cn/gtagwkthro.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.ydjk.org.cn/gtajhcnvxs.html

TS:   [...arr];
来源：http://hz.xuanzx.com/gtitgjgiiv.html

Java: new ArrayList<>(list);
来源：http://hz.zhixingplan.top/gtgjjatwuk.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.chenlongwang.top/gtwsogxoto.html

Ruby: arr.dup;  arr.clone
来源：http://hz.hongshengwenyu.top/gtihxksumj.html

C#:   new List<int>(list);
来源：http://hz.yangfankeji.com/gtttcotnqf.html

[D23] reduce 累积计算
来源：http://hz.yj20258888.top/gtkglnjarn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.nanxinkj.top/gtwnzdqbab.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.aizwys.cn/gtjctvrljq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xylfe.cn/gtgqjcfhzt.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhiwuduotai.top/gtvwntdnbu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yueranfly.top/gtgslnqdqz.html

Go:   // 手写循环
来源：http://hz.cdnleiting.top/gteytzjvkf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.zhijiandao.cn/gtgqndyqip.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.zhoulong.xyz/gtugotzdbq.html

[D24] 字典 / Map 基本操作
来源：http://hz.chenjidiqi.icu/gtqozrezcx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.sysykeji.top/gtblkhbphq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.sufxvd.cn/gtclgvpmsh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.mhx1999.top/gtgtmpuros.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.cashguo.top/gtpyhvbsws.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.shanyushiyangtech.top/gtdrtoxzgm.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.xuetiantiany.cn/gtqbtqeirt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.redwolf501.top/gttvgafeil.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.ivvv.top/gtfoowheej.html

[D25] Set 集合去重与交并差
来源：http://hz.shuidangran.top/gtpqdmbtzm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.0kj1m.cn/gtwzxipkxb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yuxming.cn/gtapizrwqq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yvedp.cn/gtrovpmbns.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.ppjwa.cn/gtexwahrhg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.quarkkingdee.top/gtlmifebav.html


<!-- 参考信息 -->