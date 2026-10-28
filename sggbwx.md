代发 wailian999

TS:   同 JS
来源：http://hz.gzhubu.top/gteuhsijhi.html

Java: 方法内为块级作用域
来源：http://hz.sufxvd.cn/gtizbowuun.html

Go:   花括号块级作用域
来源：http://hz.jiagoushi.top/gtvtryimhx.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.wangshuangyany.cn/gtllwzifab.html

C#:   块级作用域
来源：http://hz.yongpay.top/gtesmowxcl.html

[C11] 模块导入与导出
来源：http://hz.zycfv.cn/gtdqydrkez.html

Py:   from module import func
来源：http://hz.gogol.net.cn/gtkexdwiie.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.haohaochexian.top/gtvkyrlrab.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.hongshengwenyu.top/gtmmxwuyzi.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.hnxiangtu.top/gtqklrszoe.html

Java: import java.util.List;
来源：http://hz.shanyushiyangkeji.top/gtuprpxzvb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.daria6918.cn/gtqlyeywpt.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.shangyingyoupin.top/gtbsuvghqa.html

C#:   using System.Text;
来源：http://hz.cqqwz.cn/gtfnkezmjh.html

[C12] 立即执行函数 IIFE
来源：http://hz.cdnleiting.top/gthynrtkiu.html

Py:   (lambda: print("run"))()
来源：http://hz.jinyuanbaomall.cn/gtpkqwgkcl.html

PHP:  (function () { echo "run"; })();
来源：http://hz.mhx1999.top/gtetmqufsw.html

JS:   (() => { console.log("run"); })();
来源：http://hz.hnqzz.top/gtrfdajtcw.html

TS:   (() => { console.log("run"); })();
来源：http://hz.jiagoushi.top/gttztbanyl.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.shanyushiyangkeji.top/gtscjablss.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.sweek.top/gtkgadtyyj.html

Ruby: -> { puts "run" }.call
来源：http://hz.wangdashe.top/gtbahvhheo.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.nwbrower.top/gtfhghvgzw.html

[C13] 类型声明 / 类型注解
来源：http://hz.chenzaomai.com/gtygaqrfpx.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.xinyue.icu/gtjdpzhcci.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yj20258888.top/gtsmpaoxaw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.sufxvd.cn/gtzdsmxtuu.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.gaohongyu789.top/gttwtjbroy.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.kuanghao11.cn/gtppspkrrk.html

Go:   func add(a, b int) int
来源：http://hz.yuxming.cn/gtvyxixqyy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.nanxuanxn.top/gtuszmtpdg.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.shangyingyoupin.top/gtvxcurwfe.html

[C14] 泛型函数
来源：http://hz.mhx1999.top/gtcmofsmnr.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.aibaodan.cn/gtyqajhnay.html

PHP:  // 无泛型
来源：http://hz.andypj.xyz/gtgdlilurt.html

JS:   // 无泛型
来源：http://hz.zhijiandao.cn/gtbwbbxdyo.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.zhengqikj.top/gtarbhnmat.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.xinyue.icu/gtzgdzoxlm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.cashguo.top/gtbdnhexyx.html

Ruby: # 无泛型
来源：http://hz.mhx1999.top/gtzvbubxuu.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.ehwqpu.com/gtvvudtbvf.html

[C15] 解构 / 展开参数
来源：http://hz.wangdashe.top/gttpmjttye.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.tanke756.top/gtfbrhwala.html

PHP:  [$a, $b] = $pair;
来源：http://hz.snrcjt.cn/gtzwrprpdb.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.kuanghao11.cn/gtjexabcdw.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.dashuyun.cn/gtglzjgmjs.html

Java: // 无解构
来源：http://hz.daxiang520.top/gthokiiivk.html

Go:   // 无解构
来源：http://hz.gogol.net.cn/gtgrnfioze.html

Ruby: a, b = pair
来源：http://hz.fzhhl.top/gtnpqejfum.html

C#:   var (a, b) = pair;
来源：http://hz.jinqigufen.top/gtvlmpilmg.html

[C16] 函数 / 方法重载
来源：http://hz.fengsongda.top/gtpryvgfbd.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.yueranfly.top/gtedbwkihj.html

PHP:  // 无重载
来源：http://hz.c1oappe.top/gtxsbfsezo.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.nwbrower.top/gtcpjvrtbr.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.birdmap.top/gtuziditxf.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.dianchejie.cn/gtcbioaclx.html

Go:   // 无重载：用不同函数名
来源：http://hz.0kj1m.cn/gtixticeym.html

Ruby: # 无重载：靠动态参数
来源：http://hz.zhijiandao.cn/gtnhacibwn.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.gotoacloud.top/gtheosfmwq.html

================================================================================
来源：http://hz.zhengqikj.top/gtlkaqjxjh.html

D. 数组 / 列表 / 集合
来源：http://hz.nwbrower.top/gtuisixuol.html

================================================================================
来源：http://hz.dashuyun.cn/gtpqjnhfmb.html

[D01] 创建数组 / 列表
来源：http://hz.52xcode.cn/gtmibdctcy.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.shanyushiyangtech.top/gtpfjrejqi.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.yueranfly.top/gtdrvqrgbk.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.shzxlz.cn/gtkgyvxtmq.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.kuanghao11.cn/gtdukbfqhr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.ydzc1.top/gtzqvnykys.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.sxryk.cn/gtnzlvtwrp.html

Ruby: arr = [1, 2, 3]
来源：http://hz.316326.xyz/gtkakakskn.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.havefunace.top/gtfqkcvmfi.html

[D02] 追加元素到末尾
来源：http://hz.yueranfly.top/gtsmddgfvo.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.zhixingplan.top/gtrbxqbvnt.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jiagoushi.top/gthfkckexs.html

JS:   arr.push(4);
来源：http://hz.dashuyun.cn/gtqczuwtoh.html

TS:   arr.push(4);
来源：http://hz.shzxlz.cn/gtruavyhfq.html

Java: list.add(4);
来源：http://hz.wangdashe.top/gtsdsnicgx.html

Go:   arr = append(arr, 4)
来源：http://hz.haohaochexian.top/gtgblunplx.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.dashuyun.cn/gtlcbfgrfu.html

C#:   list.Add(4);
来源：http://hz.iojbl.cn/gtyygepnvo.html

[D03] 在指定位置插入元素
来源：http://hz.dianchejie.cn/gtcjzdcxwz.html

Py:   arr.insert(0, 0)
来源：http://hz.xziqi.cn/gttcbmlvjw.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.yangfankeji.com/gtieccubqx.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.mhx1999.top/gtihqodmiv.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.hywenlv.cn/gtxoajwgwq.html

Java: list.add(0, 0);
来源：http://hz.jiagoushi.top/gtlijefgui.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.zhongyouzk.top/gtouuyjnhx.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.pycfn.com/gtmjiwvzbf.html

C#:   list.Insert(0, 0);
来源：http://hz.0kj1m.cn/gtjuyafysf.html

[D04] 删除元素
来源：http://hz.yj202588.top/gtethcxqbz.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.zhixingplan.top/gtatidzsxv.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.wangdashe.top/gtpzwibyui.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.chenzaomai.com/gttruxxrsh.html

TS:   arr.splice(0, 1);
来源：http://hz.andypj.xyz/gtyvvhyfde.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.kuanghao11.cn/gtujlgtnbg.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.hysaishi.cn/gtgwoawldg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.gaohongyu789.top/gtnwccoijo.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yueranfly.top/gtbhxweawr.html

[D05] 访问与修改元素
来源：http://hz.vqdsnc.cn/gtuvfyzcbh.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.tianlin.xyz/gtnxsyulls.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.yvedp.cn/gtacacvzyc.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.quarkkingdee.top/gthudjanch.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.tian-w.cn/gtujyhcnfr.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yj202588.top/gtncvxafbl.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.shangyingyoupin.top/gtcwdjtkxh.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hongshengwenyu.top/gtfltgnnah.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.xingfuxueyuan.xyz/gtxmiztojx.html

[D06] 数组长度
来源：http://hz.jlsjyb.cn/gtrnwmezdz.html

Py:   len(arr)
来源：http://hz.hysaishi.cn/gtmwrbvcmg.html

PHP:  count($arr);
来源：http://hz.snrcjt.cn/gtppiulowd.html

JS:   arr.length
来源：http://hz.vqdsnc.cn/gtxnyrmvtn.html

TS:   arr.length
来源：http://hz.daria6918.cn/gtonsptjul.html

Java: list.size();
来源：http://hz.ivvv.top/gtydtbuslb.html

Go:   len(arr)
来源：http://hz.pycfn.com/gttxtyotrn.html

Ruby: arr.length; arr.size
来源：http://hz.bjfxy.top/gtzooaoxui.html

C#:   list.Count;
来源：http://hz.snrcjt.cn/gtyxeomvfa.html

[D07] 切片 / 取子数组
来源：http://hz.chenlongwang.top/gtlqcbhcyu.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.gotoacloud.top/gtjgfkjqhq.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.xziqi.cn/gtotcrnsuo.html

JS:   arr.slice(1, 4);
来源：http://hz.fzhhl.top/gtdlcvtqra.html

TS:   arr.slice(1, 4);
来源：http://hz.havefunace.top/gtwuujwrvh.html

Java: list.subList(1, 4);
来源：http://hz.hongshengwenyu.top/gtrmyepzro.html

Go:   arr[1:4]
来源：http://hz.ywan-chungtsiang.top/gtultugssa.html

Ruby: arr[1, 3]
来源：http://hz.0kj1m.cn/gtqjkrgrpu.html

C#:   list.GetRange(1, 3);
来源：http://hz.pycfn.com/gtxtfpjyhc.html

[D08] 合并两个数组
来源：http://hz.jinqigufen.top/gthqozdzsx.html

Py:   a + b;  a.extend(b)
来源：http://hz.nanxinkj.top/gtvdphgbwz.html

PHP:  array_merge($a, $b);
来源：http://hz.hnqzz.top/gtiuvmfqpx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.hongshengwenyu.top/gtqcgyknbz.html

TS:   [...a, ...b];
来源：http://hz.feifeiyinyue.top/gtaujczyqv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.shanyushiyangtech.top/gtinsuesey.html

Go:   append(a, b...)
来源：http://hz.yangfankeji.com/gtrsdzqseq.html

Ruby: a + b;  a.concat(b)
来源：http://hz.nwbrower.top/gtgtokrcre.html

C#:   a.Concat(b).ToList()
来源：http://hz.hnqzz.top/gtvzbhndod.html

[D09] 排序（升序）
来源：http://hz.hysaishi.cn/gtuvzeuyae.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xuetiantiany.cn/gtnpvloicr.html

PHP:  sort($arr);
来源：http://hz.dianchejie.cn/gtpvcxgudc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.iojbl.cn/gtnxczqpzw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.c1oappe.top/gtrmgxxrbu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jyoumei.cn/gtzbcnmzjn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.snrcjt.cn/gtosqioeqd.html

Ruby: arr.sort
来源：http://hz.jqgufenzy.top/gtsusprtgm.html

C#:   list.Sort();
来源：http://hz.jinghuilouyu.cn/gtfyrdkvmy.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.yuanzhike.top/gtpmlclxkx.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.cheryme.top/gtopgbaqgb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cucudq.cn/gtupbhnzhu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.pycfn.com/gtcfngpxdf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.daria6918.cn/gtyrrutbnm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.birdmap.top/gtinhnoyhg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.dashuyun.cn/gtswekbfax.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.chenzaomai.com/gtceypnyqv.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zdqjudy.top/gtlugluhcx.html

[D11] 反转数组
来源：http://hz.jlsjyb.cn/gtishzjrnx.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.jianghu66.top/gtwatukyeo.html

PHP:  array_reverse($arr);
来源：http://hz.316326.xyz/gtjdpccxtc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yvedp.cn/gtfvpgtgwh.html

TS:   [...arr].reverse();
来源：http://hz.svipenyu.cn/gtptkcipll.html

Java: Collections.reverse(list);
来源：http://hz.jianghu66.top/gtvrabsfdz.html

Go:   slices.Reverse(arr)
来源：http://hz.shzxlz.cn/gttarubfuz.html

Ruby: arr.reverse
来源：http://hz.ehwqpu.com/gtadnmifho.html

C#:   list.Reverse();
来源：http://hz.haohaochexian.top/gtcdvahdwu.html

[D12] 查找元素下标
来源：http://hz.zhijiandao.cn/gtxwkhqvkx.html

Py:   arr.index(x);  x in arr
来源：http://hz.daxiang520.top/gtsyfmfwen.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.chenlongwang.top/gtfpkpltjz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.dianchejie.cn/gtsjytojca.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xinyue.icu/gtjmwearoj.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yanxiufei.cn/gtixwzoamt.html

Go:   slices.Index(arr, x)
来源：http://hz.cdnleiting.top/gtunbojdqm.html

Ruby: arr.index(x)
来源：http://hz.ywan-chungtsiang.top/gtbrnrrtok.html

C#:   list.IndexOf(x);
来源：http://hz.52xcode.cn/gtwungkjzl.html

[D13] 过滤（保留满足条件的）
来源：http://hz.meibo888.top/gtixuydtij.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.jinghuilouyu.cn/gtepdlcxju.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.ydjk.org.cn/gtdblhnwjl.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zhengqikj.top/gtdwowibcg.html

TS:   arr.filter(x => x > 3)
来源：http://hz.shangyingyoupin.top/gtynwdbuxx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.9152youxi.cn/gtnlwrzprc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.ppjwa.cn/gtzykcvpws.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jiagoushi.top/gtzpyiamgm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.hnxiangtu.top/gttkbcrlii.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yj20258.top/gtzrpuagwy.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.feifeiyinyue.top/gtfrcqxhrd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.hnxiangtu.top/gtbgplaqeg.html

JS:   arr.map(x => x * 2)
来源：http://hz.fzhhl.top/gtappouism.html

TS:   arr.map(x => x * 2)
来源：http://hz.dianchejie.cn/gtisqoobtq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.fzhhl.top/gtxaukaqkl.html

Go:   // 手写循环
来源：http://hz.haohaochexian.top/gticykkjjv.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.daria6918.cn/gtnsymepha.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.nanxuanxn.top/gtxbuvnoxw.html

[D15] 去重
来源：http://hz.yanxiufei.cn/gttlsngsyq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.feifeiyinyue.top/gtrjrqphrr.html

PHP:  array_unique($arr);
来源：http://hz.zhongyouzk.top/gtxavxkwos.html

JS:   [...new Set(arr)]
来源：http://hz.havefunace.top/gtzsmdheme.html

TS:   [...new Set(arr)]
来源：http://hz.yvedp.cn/gtjnwghnee.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.shanyushiyangkeji.top/gtepshwlcu.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.xylfe.cn/gtaleoimin.html

Ruby: arr.uniq
来源：http://hz.xuanzx.com/gtoadepxfg.html

C#:   list.Distinct().ToList()
来源：http://hz.chenjidiqi.icu/gtcdtthxoq.html

[D16] 求和与平均值
来源：http://hz.jinqigufen.top/gtqqhgobix.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.kuanghao11.cn/gtexsgordy.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.gaohongyu789.top/gtlycmiiwy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xingfuxueyuan.xyz/gtacjbymet.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.andypj.xyz/gtcuvthkys.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jqgufenzy.top/gtzgurkkaq.html

Go:   // 手写循环累加
来源：http://hz.quarkkingdee.top/gtzcusizgh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jqgfzy.top/gtdbcrbdrh.html

C#:   list.Sum();  list.Average()
来源：http://hz.tian-w.cn/gtnexisdnn.html

[D17] 最大值与最小值
来源：http://hz.ydjk.org.cn/gtcwlrpvgc.html

Py:   max(arr);  min(arr)
来源：http://hz.jiagoushi.top/gtpzahjfss.html

PHP:  max($arr);  min($arr);
来源：http://hz.nanxuanxn.top/gtsiiivwlj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.meibo888.top/gtgrkwflpn.html

TS:   Math.max(...arr);
来源：http://hz.hysaishi.cn/gtbmdsumyl.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.ydzc1.top/gtmllhethh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.xuetiantiany.cn/gtmsoizzgp.html

Ruby: arr.max;  arr.min
来源：http://hz.hywenlv.cn/gtqjvdxvxm.html

C#:   list.Max();  list.Min()
来源：http://hz.ydjk.org.cn/gtmfopngmj.html

[D18] 扁平化嵌套数组
来源：http://hz.shanyushiyangkeji.top/gtdvxcfdbv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yueranfly.top/gtypsutwdt.html

PHP:  array_merge(...$nested);
来源：http://hz.jinghuilouyu.cn/gtjszblmzh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.wangshuangyany.cn/gtqewscivh.html

TS:   nested.flat();
来源：http://hz.hnqzz.top/gtcaxjorby.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.mhx1999.top/gtbaxdeotn.html

Go:   // 手写双层循环
来源：http://hz.9152youxi.cn/gtuezckgon.html

Ruby: nested.flatten
来源：http://hz.daria6918.cn/gtlmtuujyg.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.iojbl.cn/gtapobyedc.html

[D19] 按字段分组
来源：http://hz.hammf.cn/gtrymgwann.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.chenzaomai.com/gtestvpckm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.xingfuxueyuan.xyz/gtteiicain.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yueranfly.top/gtwtpfqcwg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.nanxinkj.top/gttlgbhpoy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.pycfn.com/gtvhhfqpli.html

Go:   // 手写 map[string][]T
来源：http://hz.guannengcc.top/gtqumfwnva.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yvedp.cn/gthsojiezi.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zycfv.cn/gtksiegwuf.html

[D20] 统计每个元素出现次数
来源：http://hz.chenjidiqi.icu/gterjhmnod.html

Py:   Counter(arr)
来源：http://hz.xuetiantiany.cn/gtkxpihxvy.html

PHP:  array_count_values($arr);
来源：http://hz.mhx1999.top/gtkusbqazj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.pengpengdd.cyou/gtkxpxnlhf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.haohaochexian.top/gtvdftmtoi.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.hysaishi.cn/gtvsmokehm.html

Go:   // 手写 map[T]int
来源：http://hz.0kj1m.cn/gtbqfxcvak.html

Ruby: arr.tally
来源：http://hz.aizwys.cn/gtyahdwhwz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.aibaodan.cn/gtklgmpxgr.html

[D21] 判断是否包含某元素
来源：http://hz.yuanzhike.top/gtovufrtwr.html

Py:   x in arr
来源：http://hz.cdnleiting.top/gtraazhyge.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yongpay.top/gtrrpppalo.html

JS:   arr.includes(x)
来源：http://hz.xziqi.cn/gtmqzsuzfq.html

TS:   arr.includes(x)
来源：http://hz.daria6918.cn/gtjkdwcjve.html

Java: list.contains(x)
来源：http://hz.zhiwuduotai.top/gtqpaeboyn.html

Go:   slices.Contains(arr, x)
来源：http://hz.kuanghao11.cn/gtwsvkiqdq.html

Ruby: arr.include?(x)
来源：http://hz.ywan-chungtsiang.top/gtbruhrxve.html

C#:   list.Contains(x)
来源：http://hz.nwbrower.top/gtjyvhnnuu.html

[D22] 复制数组（避免共享引用）
来源：http://hz.zhaomingkeji.xyz/gtbtawupqo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.birdmap.top/gtoqpxnpux.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.shuidangran.top/gtotqmxqpi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.cqqwz.cn/gtyxjjxtrx.html

TS:   [...arr];
来源：http://hz.chenjidiqi.icu/gtlpiovsad.html

Java: new ArrayList<>(list);
来源：http://hz.nanxuanxn.top/gttkyurrcb.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.kuanghao11.cn/gthdzpysfu.html

Ruby: arr.dup;  arr.clone
来源：http://hz.kuanghao11.cn/gtqghhwywl.html

C#:   new List<int>(list);
来源：http://hz.gogol.net.cn/gtodsfcyhv.html

[D23] reduce 累积计算
来源：http://hz.ybcxt.top/gtbvvggnzc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.xingfuxueyuan.xyz/gtynspdqby.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yj202588.top/gtreornqpj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cashguo.top/gttjqplllw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jyoumei.cn/gtuwelwbnr.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.pengpengdd.cyou/gtfdgilrgm.html

Go:   // 手写循环
来源：http://hz.cheryme.top/gtiarvyutv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.ehwqpu.com/gtemxzrfaz.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jianghu66.top/gtteaabuku.html

[D24] 字典 / Map 基本操作
来源：http://hz.ydjk.org.cn/gtvbfntwoa.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.xinyue.icu/gtrinnsalp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.zycfv.cn/gtizxyqndx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.havefunace.top/gtcyveoeju.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.sweek.top/gtkdnxhich.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.daria6918.cn/gtpsjewbtn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yvedp.cn/gtxaycfkns.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.wangshuangyany.cn/gtherwyjld.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.vqdsnc.cn/gtmcxjygjk.html

[D25] Set 集合去重与交并差
来源：http://hz.hfpthk.cn/gtyuckrqsw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.hnxiangtu.top/gtddjurbfc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.xylfe.cn/gtfpnbhitb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.jinghuilouyu.cn/gtdpaljkqk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.dianchejie.cn/gtlmtaamra.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.chenlongwang.top/gtufqguvzj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.hongshengwenyu.top/gtubcecnim.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.smart0.xyz/gtnxnelsdu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yanxiufei.cn/gtiiowrnjw.html

[D26] 数组转字符串
来源：http://hz.zhengqikj.top/gttfgjpgpn.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yvedp.cn/gtkiavctbm.html

PHP:  implode(", ", $arr);
来源：http://hz.vqdsnc.cn/gtjzpxeutb.html

JS:   arr.join(", ")
来源：http://hz.ywan-chungtsiang.top/gttxfapcdo.html

TS:   arr.join(", ")
来源：http://hz.zhixingplan.top/gtmtznpted.html

Java: String.join(", ", list)
来源：http://hz.tian-w.cn/gtzbrcilyf.html

Go:   strings.Join(strs, ", ")
来源：http://hz.chenzaomai.com/gtdalfzelg.html

Ruby: arr.join(", ")
来源：http://hz.shangyingyoupin.top/gtnrjfhofz.html

C#:   string.Join(", ", list)
来源：http://hz.shanyushiyangtech.top/gtpxhydpfa.html

================================================================================
来源：http://hz.yuxming.cn/gtnkpmvldp.html

E. 字符串处理
来源：http://hz.jinqigfzy.top/gtdrbzpbjv.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtrszbuagq.html

[E01] 拼接字符串
来源：http://hz.daxiang520.top/gtdkjzvvtz.html


<!-- 参考信息 -->