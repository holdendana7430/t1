代发 wailian999

Java: static int fact(int n) { return n <= 1 ? 1 : n * fact(n - 1); }
来源：http://hz.xylfe.cn/gtdvsvetdo.html

Go:   func fact(n int) int { if n <= 1 { return 1 }; return n * fact(n-1) }
来源：http://hz.chenzaomai.com/gttnewkddt.html

Ruby: def fact(n) = n <= 1 ? 1 : n * fact(n - 1)
来源：http://hz.dashuyun.cn/gtrnwjbbxk.html

C#:   static int Fact(int n) => n <= 1 ? 1 : n * Fact(n - 1);
来源：http://hz.chenlongwang.top/gtjvzsbqqs.html

[C10] 变量作用域
来源：http://hz.zhaomingkeji.xyz/gtllpotfyl.html

Py:   函数内赋值即局部；改外层需 global / nonlocal
来源：http://hz.shangyingyoupin.top/gtyzslpuig.html

PHP:  函数内默认看不到外部变量，需 global 或 use
来源：http://hz.zhengqikj.top/gtoxjievfn.html

JS:   let/const 块级作用域，var 函数级作用域
来源：http://hz.ivvv.top/gtxagysmtw.html

TS:   同 JS
来源：http://hz.gogol.net.cn/gtgbnkhiew.html

Java: 方法内为块级作用域
来源：http://hz.jianghu66.top/gtmioeiopb.html

Go:   花括号块级作用域
来源：http://hz.ppjwa.cn/gtzcjjmwmv.html

Ruby: 局部变量 / @实例 / @@类 / $全局
来源：http://hz.ehwqpu.com/gtbtnflmmp.html

C#:   块级作用域
来源：http://hz.zhongyouzk.top/gtwcveoecd.html

[C11] 模块导入与导出
来源：http://hz.shanyushiyangkeji.top/gtjclzyodw.html

Py:   from module import func
来源：http://hz.52xcode.cn/gtjnnlybmh.html

PHP:  require "file.php";  或 use App\Service;
来源：http://hz.snrcjt.cn/gtetotjkdm.html

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.yueranfly.top/gttebmvmgj.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.hnqzz.top/gtayztpwhc.html

Java: import java.util.List;
来源：http://hz.sweek.top/gtetbdytjd.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.havefunace.top/gtivqgckko.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.52xcode.cn/gtvqxjdxvz.html

C#:   using System.Text;
来源：http://hz.zhixingplan.top/gtcyhhorod.html

[C12] 立即执行函数 IIFE
来源：http://hz.cucudq.cn/gtphsffcfh.html

Py:   (lambda: print("run"))()
来源：http://hz.hammf.cn/gtmrrahwbj.html

PHP:  (function () { echo "run"; })();
来源：http://hz.ppjwa.cn/gtgahyzghk.html

JS:   (() => { console.log("run"); })();
来源：http://hz.gzhubu.top/gtetfwerhe.html

TS:   (() => { console.log("run"); })();
来源：http://hz.svipenyu.cn/gtfrgqpymx.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yanxiufei.cn/gtxyxepcjj.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.shanyushiyangkeji.top/gtgdmkjmxs.html

Ruby: -> { puts "run" }.call
来源：http://hz.jinyuanbaomall.cn/gtvstwfzhl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.ydjk.org.cn/gtdjbquwvq.html

[C13] 类型声明 / 类型注解
来源：http://hz.dianchejie.cn/gtyzqckefr.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.gaohongyu789.top/gtcgschhoy.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.sweek.top/gtsdwivpum.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.ivvv.top/gteaclwpqs.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.hammf.cn/gtbnfpwsgn.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.dashuyun.cn/gtmaqqrrew.html

Go:   func add(a, b int) int
来源：http://hz.xuanzx.com/gtuxyedwjy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.gogol.net.cn/gtcherwmou.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.chenzaomai.com/gtktdigfbp.html

[C14] 泛型函数
来源：http://hz.chenlongwang.top/gtzsfhjlfd.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.dashuyun.cn/gtqhmyyshu.html

PHP:  // 无泛型
来源：http://hz.xuetiantiany.cn/gtpzxisjgc.html

JS:   // 无泛型
来源：http://hz.jinyuanbaomall.cn/gtjmklginf.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.snrcjt.cn/gttltjxwgc.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.andypj.xyz/gtkxxtbhjj.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.hywenlv.cn/gtkosucyqz.html

Ruby: # 无泛型
来源：http://hz.nanxinkj.top/gtdoplarzb.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.hnqzz.top/gtazxpywlv.html

[C15] 解构 / 展开参数
来源：http://hz.cucudq.cn/gtrutjvcav.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.yangfankeji.com/gtcjeocqes.html

PHP:  [$a, $b] = $pair;
来源：http://hz.shzxlz.cn/gtsqnikstx.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.guannengcc.top/gtfacqvmyt.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.redwolf501.top/gtpcqeajqd.html

Java: // 无解构
来源：http://hz.xinyue.icu/gtxwrdvzxe.html

Go:   // 无解构
来源：http://hz.quarkkingdee.top/gtdtttgwbb.html

Ruby: a, b = pair
来源：http://hz.redwolf501.top/gtfrfzrrdp.html

C#:   var (a, b) = pair;
来源：http://hz.nwbrower.top/gtujmvfbbc.html

[C16] 函数 / 方法重载
来源：http://hz.dianchejie.cn/gtsdixpmkg.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.cheryme.top/gtppzyaxrm.html

PHP:  // 无重载
来源：http://hz.haohaochexian.top/gtxdzljubr.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.iojbl.cn/gtfnijjymq.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.pycfn.com/gtoorwelnm.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.jinyuanbaomall.cn/gtzehclnld.html

Go:   // 无重载：用不同函数名
来源：http://hz.chenzaomai.com/gtrqtlnlje.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yanxiufei.cn/gtnutqbjxf.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.chenzaomai.com/gtgxigcplm.html

================================================================================
来源：http://hz.smart0.xyz/gtzkppmnml.html

D. 数组 / 列表 / 集合
来源：http://hz.yongpay.top/gtlpsircll.html

================================================================================
来源：http://hz.0kj1m.cn/gtpvjwxydt.html

[D01] 创建数组 / 列表
来源：http://hz.cheryme.top/gtafcbrppx.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.chenlongwang.top/gtxdntnpze.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.jyoumei.cn/gtwctrszzs.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.smart0.xyz/gtubhqfjsi.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.gzhubu.top/gtvchkvqvr.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.smart0.xyz/gtsqpkqcan.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.smart0.xyz/gtwhohwlfi.html

Ruby: arr = [1, 2, 3]
来源：http://hz.sysykeji.top/gtvmwzdcqe.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.jinyuanbaomall.cn/gtadkjpfll.html

[D02] 追加元素到末尾
来源：http://hz.zhoulong.xyz/gtybtzoqsw.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.ehwqpu.com/gtkxajdoai.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.kuanghao11.cn/gtuceyobou.html

JS:   arr.push(4);
来源：http://hz.daria6918.cn/gtjepbblgd.html

TS:   arr.push(4);
来源：http://hz.zycfv.cn/gtrdrtruof.html

Java: list.add(4);
来源：http://hz.gzhubu.top/gtgcnpjdet.html

Go:   arr = append(arr, 4)
来源：http://hz.hammf.cn/gtvcktrxgn.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.daria6918.cn/gtsrcxfbme.html

C#:   list.Add(4);
来源：http://hz.havefunace.top/gttiseuyiz.html

[D03] 在指定位置插入元素
来源：http://hz.pengpengdd.cyou/gtnjdugyct.html

Py:   arr.insert(0, 0)
来源：http://hz.shzxlz.cn/gtmusdjabo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.smart0.xyz/gtcpczkoxt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.zhijiandao.cn/gtpnhcofqm.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.zycfv.cn/gttpivdprg.html

Java: list.add(0, 0);
来源：http://hz.9152youxi.cn/gtmubrffgv.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.nwbrower.top/gtdtccutvw.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.zhixingplan.top/gtuavvrarc.html

C#:   list.Insert(0, 0);
来源：http://hz.316326.xyz/gtoctvoiwy.html

[D04] 删除元素
来源：http://hz.zhongyouzk.top/gtpqnpkjxg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.xylfe.cn/gtrmhojsgl.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.vqdsnc.cn/gtkyzdzadk.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.nwbrower.top/gtmbaedqxs.html

TS:   arr.splice(0, 1);
来源：http://hz.chenjidiqi.icu/gthwxrlkvv.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.zhixingplan.top/gthplibhvm.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.pycfn.com/gtsnntgrpt.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.c1oappe.top/gtsszzgmor.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.hnqzz.top/gtywwpoozi.html

[D05] 访问与修改元素
来源：http://hz.shanyushiyangkeji.top/gtzvbcvfeq.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yueranfly.top/gtxagmrgfb.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.shuidangran.top/gtaimreasa.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.hysaishi.cn/gtakwgaisn.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.daxiang520.top/gtzzsqlzsr.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.9152youxi.cn/gtkabpzufi.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.dianchejie.cn/gtmuuqjuma.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jyoumei.cn/gtdbnpljwp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.xingfuxueyuan.xyz/gtxwpwwiaj.html

[D06] 数组长度
来源：http://hz.smart0.xyz/gtqxitfxul.html

Py:   len(arr)
来源：http://hz.ydzc1.top/gthjlczalf.html

PHP:  count($arr);
来源：http://hz.xuetiantiany.cn/gtyzlfgkxi.html

JS:   arr.length
来源：http://hz.aizwys.cn/gtrogiqejk.html

TS:   arr.length
来源：http://hz.iojbl.cn/gtcyxdhssn.html

Java: list.size();
来源：http://hz.ybcxt.top/gtyknjlocv.html

Go:   len(arr)
来源：http://hz.52xcode.cn/gtpyeainqw.html

Ruby: arr.length; arr.size
来源：http://hz.c1oappe.top/gtetzeeouf.html

C#:   list.Count;
来源：http://hz.cucudq.cn/gtrbwoojre.html

[D07] 切片 / 取子数组
来源：http://hz.nanxuanxn.top/gtllyjpksm.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jqgufenzy.top/gtowgnhqhf.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yj202588.top/gtoljgmfrt.html

JS:   arr.slice(1, 4);
来源：http://hz.ywan-chungtsiang.top/gtzczjouuk.html

TS:   arr.slice(1, 4);
来源：http://hz.zhiwuduotai.top/gtsrklwfml.html

Java: list.subList(1, 4);
来源：http://hz.tanke756.top/gtnkwveekv.html

Go:   arr[1:4]
来源：http://hz.ehwqpu.com/gtkdamkzep.html

Ruby: arr[1, 3]
来源：http://hz.iojbl.cn/gtcusqkqof.html

C#:   list.GetRange(1, 3);
来源：http://hz.meibo888.top/gtiimzvwir.html

[D08] 合并两个数组
来源：http://hz.sxryk.cn/gtmqxizacm.html

Py:   a + b;  a.extend(b)
来源：http://hz.zhaomingkeji.xyz/gtcywdshjz.html

PHP:  array_merge($a, $b);
来源：http://hz.daxiang520.top/gtyunbwsea.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.aizwys.cn/gtmjughufx.html

TS:   [...a, ...b];
来源：http://hz.jinyuanbaomall.cn/gtcfaylrpv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.chenlongwang.top/gtgfdmdcqc.html

Go:   append(a, b...)
来源：http://hz.zhoulong.xyz/gtitohizbg.html

Ruby: a + b;  a.concat(b)
来源：http://hz.quarkkingdee.top/gtbcfctndr.html

C#:   a.Concat(b).ToList()
来源：http://hz.316326.xyz/gtniliohgc.html

[D09] 排序（升序）
来源：http://hz.sufxvd.cn/gtohbrcomu.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.daria6918.cn/gtsamfrpvq.html

PHP:  sort($arr);
来源：http://hz.hammf.cn/gtwnegogkn.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.jqgufenzy.top/gtvqvewcgx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.ydjk.org.cn/gtkuvfyomh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.svipenyu.cn/gtzbngirem.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.jqgufenzy.top/gtgohhgjpm.html

Ruby: arr.sort
来源：http://hz.aizwys.cn/gtoowgnxqd.html

C#:   list.Sort();
来源：http://hz.ydjk.org.cn/gtdnjyfxbr.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.havefunace.top/gtvfqkahsu.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.chenjidiqi.icu/gtqpnekgok.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.pycfn.com/gtblqhavqu.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yuanzhike.top/gtdjxxiars.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.aibaodan.cn/gtgylogafb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.haohaochexian.top/gtzswztwvl.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yj20258888.top/gtkogubfhm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.nwbrower.top/gtpvzmgzng.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.hywenlv.cn/gtayfvpcte.html

[D11] 反转数组
来源：http://hz.chenlongwang.top/gtzkmhsopr.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.snrcjt.cn/gtlnblitrj.html

PHP:  array_reverse($arr);
来源：http://hz.quarkkingdee.top/gtykmqnujm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.gzhubu.top/gtjzuiolxq.html

TS:   [...arr].reverse();
来源：http://hz.yj202588.top/gthovlcbzb.html

Java: Collections.reverse(list);
来源：http://hz.dianchejie.cn/gtfzaulnvp.html

Go:   slices.Reverse(arr)
来源：http://hz.ehwqpu.com/gtmnobvnqc.html

Ruby: arr.reverse
来源：http://hz.fengsongda.top/gtmwcnxnqd.html

C#:   list.Reverse();
来源：http://hz.tian-w.cn/gtoqnziyin.html

[D12] 查找元素下标
来源：http://hz.jqgfzy.top/gtulljxuxt.html

Py:   arr.index(x);  x in arr
来源：http://hz.zhiwuduotai.top/gtscthcezu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.cqqwz.cn/gtxbwkocnh.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.tian-w.cn/gtxuqdsbpn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.dashuyun.cn/gtzhcnqfmb.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.ppjwa.cn/gtuacpnutp.html

Go:   slices.Index(arr, x)
来源：http://hz.shzxlz.cn/gtnyneijty.html

Ruby: arr.index(x)
来源：http://hz.redwolf501.top/gtjlmmqiuk.html

C#:   list.IndexOf(x);
来源：http://hz.daria6918.cn/gtbfebdrnu.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zdqjudy.top/gtjulvfeql.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zhiwuduotai.top/gtirtvvyvr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.gaohongyu789.top/gtisjoeeqm.html

JS:   arr.filter(x => x > 3)
来源：http://hz.sxryk.cn/gtrcghvvrd.html

TS:   arr.filter(x => x > 3)
来源：http://hz.ywan-chungtsiang.top/gthobdgicy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.shuidangran.top/gtufazzlaq.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yvedp.cn/gtyqynaxmm.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.sufxvd.cn/gtaenerkru.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.gzhubu.top/gtdemrajcx.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yj202588.top/gtqhhbkrfl.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jinyuanbaomall.cn/gtqwuorwwi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jlsjyb.cn/gtcamyhafk.html

JS:   arr.map(x => x * 2)
来源：http://hz.guannengcc.top/gtwkvvfftu.html

TS:   arr.map(x => x * 2)
来源：http://hz.jiagoushi.top/gtqntpcxcf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.c1oappe.top/gtkpxtlpxp.html

Go:   // 手写循环
来源：http://hz.sweek.top/gtznamfcqi.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yj20258888.top/gtnnovbbdn.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.iojbl.cn/gtvwnnkcdl.html

[D15] 去重
来源：http://hz.havefunace.top/gtotrjlcvl.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.cashguo.top/gthyaubzvw.html

PHP:  array_unique($arr);
来源：http://hz.316326.xyz/gtzfprbbur.html

JS:   [...new Set(arr)]
来源：http://hz.jiagoushi.top/gtbnddnsol.html

TS:   [...new Set(arr)]
来源：http://hz.kuanghao11.cn/gtwzsxxeed.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.kuanghao11.cn/gtgwwrxhwn.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.iojbl.cn/gtrpefeqop.html

Ruby: arr.uniq
来源：http://hz.jiagoushi.top/gtzjzlfnuj.html

C#:   list.Distinct().ToList()
来源：http://hz.shzxlz.cn/gtkrnnyhhj.html

[D16] 求和与平均值
来源：http://hz.shangyingyoupin.top/gteklldewc.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.chenlongwang.top/gtrrqarwkl.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jinghuilouyu.cn/gtsogtzhuj.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yanxiufei.cn/gttroqoczx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hammf.cn/gtnbfblxuo.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.feifeiyinyue.top/gtrvlfxgrc.html

Go:   // 手写循环累加
来源：http://hz.ybcxt.top/gtkxysrauk.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yueranfly.top/gtmhepgpls.html

C#:   list.Sum();  list.Average()
来源：http://hz.jinqigufen.top/gtblisagsz.html

[D17] 最大值与最小值
来源：http://hz.chenjidiqi.icu/gtsswyadfu.html

Py:   max(arr);  min(arr)
来源：http://hz.pycfn.com/gtvzilkkrc.html

PHP:  max($arr);  min($arr);
来源：http://hz.daria6918.cn/gtqjnpqedv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.hywenlv.cn/gtjaiowtrt.html

TS:   Math.max(...arr);
来源：http://hz.bjfxy.top/gtahqxjozz.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zhongyouzk.top/gtgkhrfafl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.feifeiyinyue.top/gtviimlzht.html

Ruby: arr.max;  arr.min
来源：http://hz.jinqigufen.top/gtdwakjyvs.html

C#:   list.Max();  list.Min()
来源：http://hz.shangyingyoupin.top/gtbkfsxdhm.html

[D18] 扁平化嵌套数组
来源：http://hz.smart0.xyz/gtmmvdeuzp.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yangfankeji.com/gtevueaaok.html

PHP:  array_merge(...$nested);
来源：http://hz.ppjwa.cn/gtknouyyxu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.smart0.xyz/gthojhdofb.html

TS:   nested.flat();
来源：http://hz.ydzc1.top/gtjogsmyqm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.sufxvd.cn/gteubmpspt.html

Go:   // 手写双层循环
来源：http://hz.shanyushiyangkeji.top/gtnoxnxvod.html

Ruby: nested.flatten
来源：http://hz.kuanghao11.cn/gtsyiwojaw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yanxiufei.cn/gtlwpkyjwb.html

[D19] 按字段分组
来源：http://hz.sysykeji.top/gtkwprbizg.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.ydjk.org.cn/gtlxkgynux.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yj20258.top/gtuvmgihkb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jinqigufen.top/gtxwtvgycz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.ivvv.top/gtimbsipvc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.hnxiangtu.top/gtclmmppfk.html

Go:   // 手写 map[string][]T
来源：http://hz.zhijiandao.cn/gtdoimnvrf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.iojbl.cn/gttlpqogsj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jinqigfzy.top/gtrwpseaal.html

[D20] 统计每个元素出现次数
来源：http://hz.jqgfzy.top/gteqkfsywh.html

Py:   Counter(arr)
来源：http://hz.mhx1999.top/gtdckrbpuv.html

PHP:  array_count_values($arr);
来源：http://hz.gzhubu.top/gtsqduwhoo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.pycfn.com/gtdrwzruxn.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.feifeiyinyue.top/gtzwfoymxs.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yuanzhike.top/gtahytfxxy.html

Go:   // 手写 map[T]int
来源：http://hz.yvedp.cn/gtuvudqxat.html

Ruby: arr.tally
来源：http://hz.wangdashe.top/gtibzmcspr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.sxryk.cn/gtjguaoplg.html

[D21] 判断是否包含某元素
来源：http://hz.ybcxt.top/gtiyttvbpd.html

Py:   x in arr
来源：http://hz.c1oappe.top/gtjsaezadj.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yueranfly.top/gtbhuesjmc.html

JS:   arr.includes(x)
来源：http://hz.yj202588.top/gtaaaneewh.html

TS:   arr.includes(x)
来源：http://hz.ydjk.org.cn/gtsepxadxh.html

Java: list.contains(x)
来源：http://hz.ivvv.top/gtpkmabnjs.html

Go:   slices.Contains(arr, x)
来源：http://hz.aibaodan.cn/gtlzzamrup.html

Ruby: arr.include?(x)
来源：http://hz.zycfv.cn/gtdqxrkkxb.html

C#:   list.Contains(x)
来源：http://hz.wangshuangyany.cn/gtsonxxjcu.html

[D22] 复制数组（避免共享引用）
来源：http://hz.cashguo.top/gtbzftrxor.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.316326.xyz/gtosjzwabd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.316326.xyz/gtvirfqcvt.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.hnxiangtu.top/gtrvbvftcv.html

TS:   [...arr];
来源：http://hz.hammf.cn/gtmvznxfme.html

Java: new ArrayList<>(list);
来源：http://hz.c1oappe.top/gtcmewwoip.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.gaohongyu789.top/gtyrodizhe.html

Ruby: arr.dup;  arr.clone
来源：http://hz.chenjidiqi.icu/gtzflhejbl.html

C#:   new List<int>(list);
来源：http://hz.tanke756.top/gthyofxqtv.html

[D23] reduce 累积计算
来源：http://hz.ywan-chungtsiang.top/gtkxmjdpmq.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.nanxuanxn.top/gtrdhvjyug.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.snrcjt.cn/gtsnhmlsuu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.meibo888.top/gtitxzxxxb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yuxming.cn/gtreklaayl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jqgfzy.top/gtmppbnbdv.html

Go:   // 手写循环
来源：http://hz.pycfn.com/gtdrtrlyot.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.cheryme.top/gtzdvnpsrf.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.mhx1999.top/gtzvoxjebu.html

[D24] 字典 / Map 基本操作
来源：http://hz.gaohongyu789.top/gtlntgaqzx.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.haohaochexian.top/gtoatizbuv.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.cucudq.cn/gtywnsvyld.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.yj20258.top/gtnrwbrzcj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.havefunace.top/gtptycnpmq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.guowangkeji.top/gtdtydtilz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jiagoushi.top/gtfaibkldf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jinqigfzy.top/gtiuiymfuc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.pycfn.com/gtejtpvvao.html

[D25] Set 集合去重与交并差
来源：http://hz.chenlongwang.top/gtxobyjphh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.ydzc1.top/gtzfqytifm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.bjfxy.top/gtqxtoblbf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.aibaodan.cn/gtumdksgas.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.vqdsnc.cn/gtxnpkrajs.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.gogol.net.cn/gtblgbdoun.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.jqgfzy.top/gtghtcjyrb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.9152youxi.cn/gtpgwkwndq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.sufxvd.cn/gtcqptyyvv.html

[D26] 数组转字符串
来源：http://hz.c1oappe.top/gttzbjgmbc.html

Py:   ", ".join(map(str, arr))
来源：http://hz.hnxiangtu.top/gtxbluaghr.html

PHP:  implode(", ", $arr);
来源：http://hz.sxryk.cn/gtitgjgzgz.html

JS:   arr.join(", ")
来源：http://hz.guowangkeji.top/gtbnbpzpmz.html

TS:   arr.join(", ")
来源：http://hz.birdmap.top/gtdlgbhorm.html


<!-- 参考信息 -->