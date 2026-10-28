代发 wailian999

JS:   export default function f() {};  import f from "./m.js";
来源：http://hz.sysykeji.top/gtzxmihuwa.html

TS:   export function f(): void {};  import { f } from "./m";
来源：http://hz.hnxiangtu.top/gtyufecjqp.html

Java: import java.util.List;
来源：http://hz.tianlin.xyz/gtrrdvmowb.html

Go:   import "fmt"          // 之后用 fmt.Println
来源：http://hz.guowangkeji.top/gtgflbqsih.html

Ruby: require "json"; require_relative "./util"
来源：http://hz.jlsjyb.cn/gtoqxlvwtn.html

C#:   using System.Text;
来源：http://hz.hnqzz.top/gtepyvlkkd.html

[C12] 立即执行函数 IIFE
来源：http://hz.sxryk.cn/gtoaappnbo.html

Py:   (lambda: print("run"))()
来源：http://hz.jinqigfzy.top/gtwepvlcet.html

PHP:  (function () { echo "run"; })();
来源：http://hz.yueranfly.top/gtfacdshec.html

JS:   (() => { console.log("run"); })();
来源：http://hz.hammf.cn/gtdvtaxpkc.html

TS:   (() => { console.log("run"); })();
来源：http://hz.aibaodan.cn/gtzxhgkdir.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.yueranfly.top/gthmjcofhu.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.xinyue.icu/gtqbkhcbjw.html

Ruby: -> { puts "run" }.call
来源：http://hz.zhiwuduotai.top/gtjiwfmwki.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.ydjk.org.cn/gtinffkkfy.html

[C13] 类型声明 / 类型注解
来源：http://hz.nanxuanxn.top/gtgclrzrbc.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.yuxming.cn/gtlqoelqll.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.guannengcc.top/gtoxtbtrch.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.chenzaomai.com/gtftjosfpd.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.ybcxt.top/gtcnnuxebd.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.meibo888.top/gtyctwihrs.html

Go:   func add(a, b int) int
来源：http://hz.pengpengdd.cyou/gtjwbooboh.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.hammf.cn/gtlcbnugob.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.sysykeji.top/gtqcdcanvp.html

[C14] 泛型函数
来源：http://hz.wangdashe.top/gtmmchxhja.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.ybcxt.top/gtcqhxxpex.html

PHP:  // 无泛型
来源：http://hz.hnxiangtu.top/gtvzhszfqo.html

JS:   // 无泛型
来源：http://hz.wangshuangyany.cn/gtzgznkuat.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.tianlin.xyz/gtgxnfdmwq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.sufxvd.cn/gtpsfdlkms.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.feifeiyinyue.top/gtrmpirobg.html

Ruby: # 无泛型
来源：http://hz.tanke756.top/gtytudvcus.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.c1oappe.top/gttxbxiurd.html

[C15] 解构 / 展开参数
来源：http://hz.guowangkeji.top/gtsikzjnne.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.feifeiyinyue.top/gtmxmektoo.html

PHP:  [$a, $b] = $pair;
来源：http://hz.cqqwz.cn/gtaaoujiih.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.sweek.top/gtobekjyxq.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.gogol.net.cn/gtidlghqkf.html

Java: // 无解构
来源：http://hz.zhongyouzk.top/gtdgvgixzt.html

Go:   // 无解构
来源：http://hz.yangfankeji.com/gtynckyopn.html

Ruby: a, b = pair
来源：http://hz.shangyingyoupin.top/gtohvhtsvk.html

C#:   var (a, b) = pair;
来源：http://hz.jqgfzy.top/gtksptbcio.html

[C16] 函数 / 方法重载
来源：http://hz.0kj1m.cn/gtlfobefho.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.redwolf501.top/gtemvqfqva.html

PHP:  // 无重载
来源：http://hz.vqdsnc.cn/gtousfkdqu.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.cashguo.top/gtwawucqvk.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.ivvv.top/gtgopfzcat.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.cqqwz.cn/gtmvkxgecp.html

Go:   // 无重载：用不同函数名
来源：http://hz.yuxming.cn/gtaxpjvcdm.html

Ruby: # 无重载：靠动态参数
来源：http://hz.zhiwuduotai.top/gtwgyjvtlj.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.c1oappe.top/gtniihfvxu.html

================================================================================
来源：http://hz.yonumen.top/gtwqxabltq.html

D. 数组 / 列表 / 集合
来源：http://hz.cashguo.top/gtctrcpunk.html

================================================================================
来源：http://hz.cdnleiting.top/gtbgxlvocy.html

[D01] 创建数组 / 列表
来源：http://hz.nwbrower.top/gtabnrjppo.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.ehwqpu.com/gtqojqgihg.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.dianchejie.cn/gtbffhgulx.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.zdqjudy.top/gtlubtcikm.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.quarkkingdee.top/gtunusxhns.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.jiagoushi.top/gtltnwftar.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.jianghu66.top/gtckgexcic.html

Ruby: arr = [1, 2, 3]
来源：http://hz.bjfxy.top/gtjsajxxhw.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.xingfuxueyuan.xyz/gtejvhfyfq.html

[D02] 追加元素到末尾
来源：http://hz.zycfv.cn/gtwgrmvaiz.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.ywan-chungtsiang.top/gtuizmbnpo.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.svipenyu.cn/gtswacbpzv.html

JS:   arr.push(4);
来源：http://hz.redwolf501.top/gtnmxkhfor.html

TS:   arr.push(4);
来源：http://hz.xylfe.cn/gtqharjbio.html

Java: list.add(4);
来源：http://hz.sweek.top/gtytnskepw.html

Go:   arr = append(arr, 4)
来源：http://hz.birdmap.top/gterksbyxv.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.yuxming.cn/gticwxqulh.html

C#:   list.Add(4);
来源：http://hz.shuidangran.top/gtoddkrdsc.html

[D03] 在指定位置插入元素
来源：http://hz.ydzc1.top/gtqgdrogdb.html

Py:   arr.insert(0, 0)
来源：http://hz.yuanzhike.top/gtjwgwqeqn.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.cashguo.top/gtpqhuaxuz.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.aizwys.cn/gtinzybhln.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.hnxiangtu.top/gtcungjisb.html

Java: list.add(0, 0);
来源：http://hz.zycfv.cn/gtfgeobrtn.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.smart0.xyz/gtxxobwswg.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.snrcjt.cn/gttaweogym.html

C#:   list.Insert(0, 0);
来源：http://hz.bjfxy.top/gtghdrekup.html

[D04] 删除元素
来源：http://hz.jianghu66.top/gthwxumrtt.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.chenzaomai.com/gtlttjvfyr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jiagoushi.top/gtblsizhqz.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.cqqwz.cn/gtleniapej.html

TS:   arr.splice(0, 1);
来源：http://hz.fengsongda.top/gtmjtqxhwt.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.pengpengdd.cyou/gtszdcidij.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.nanxinkj.top/gtohypdtam.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.chenjidiqi.icu/gtqvjeqilc.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.cashguo.top/gtbznunlkj.html

[D05] 访问与修改元素
来源：http://hz.chenlongwang.top/gtigzuiweb.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.gzhubu.top/gtsfjrufrh.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.0kj1m.cn/gtupaepmrh.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.cdnleiting.top/gthawukhxv.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.wangdashe.top/gtlrpedkyh.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jiagoushi.top/gtpysgvdsn.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.shanyushiyangtech.top/gtifejbgyx.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xingfuxueyuan.xyz/gtkwqbmeyh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.zhixingplan.top/gtinzksclm.html

[D06] 数组长度
来源：http://hz.c1oappe.top/gtgrgxmact.html

Py:   len(arr)
来源：http://hz.gaohongyu789.top/gtnffeoqfd.html

PHP:  count($arr);
来源：http://hz.jyoumei.cn/gtapvbfbdd.html

JS:   arr.length
来源：http://hz.jyoumei.cn/gtaxkdfjgh.html

TS:   arr.length
来源：http://hz.tanke756.top/gtzfqlnebb.html

Java: list.size();
来源：http://hz.guowangkeji.top/gtwvkwgloe.html

Go:   len(arr)
来源：http://hz.0kj1m.cn/gtneqgyfsk.html

Ruby: arr.length; arr.size
来源：http://hz.52xcode.cn/gtbawhnsib.html

C#:   list.Count;
来源：http://hz.zhijiandao.cn/gtapwkfxsd.html

[D07] 切片 / 取子数组
来源：http://hz.hfpthk.cn/gtlyablnig.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.bjfxy.top/gtazjwtuax.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.chenzaomai.com/gtbjewlsqv.html

JS:   arr.slice(1, 4);
来源：http://hz.shanyushiyangtech.top/gtqstzpgtq.html

TS:   arr.slice(1, 4);
来源：http://hz.birdmap.top/gtnbqohxko.html

Java: list.subList(1, 4);
来源：http://hz.cucudq.cn/gtaicqlbkk.html

Go:   arr[1:4]
来源：http://hz.shuidangran.top/gtrxzqhoxw.html

Ruby: arr[1, 3]
来源：http://hz.hysaishi.cn/gtfdtwngov.html

C#:   list.GetRange(1, 3);
来源：http://hz.nwbrower.top/gtdvoxksbp.html

[D08] 合并两个数组
来源：http://hz.fengsongda.top/gtlvsjjusj.html

Py:   a + b;  a.extend(b)
来源：http://hz.birdmap.top/gtroeqowem.html

PHP:  array_merge($a, $b);
来源：http://hz.yvedp.cn/gtkavhympv.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.guannengcc.top/gtvkjfougi.html

TS:   [...a, ...b];
来源：http://hz.shanyushiyangtech.top/gtvmaiklfh.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.birdmap.top/gtxlhliesr.html

Go:   append(a, b...)
来源：http://hz.sysykeji.top/gtximrgqtc.html

Ruby: a + b;  a.concat(b)
来源：http://hz.ydzc1.top/gtszeuwvko.html

C#:   a.Concat(b).ToList()
来源：http://hz.ydzc1.top/gtvrsgeede.html

[D09] 排序（升序）
来源：http://hz.cdnleiting.top/gtcsynlcfd.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xinyue.icu/gtpteafnah.html

PHP:  sort($arr);
来源：http://hz.xuetiantiany.cn/gtzpnbbulh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.tianlin.xyz/gtbqfjdaap.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.cucudq.cn/gtyexhwdnn.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yonumen.top/gtrldbwjib.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.snrcjt.cn/gtmnsswazg.html

Ruby: arr.sort
来源：http://hz.jlsjyb.cn/gtahgvtqpv.html

C#:   list.Sort();
来源：http://hz.kuanghao11.cn/gtdepdjjws.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.xuanzx.com/gtrlbdgwiv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.redwolf501.top/gtcqbcczzr.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.xuetiantiany.cn/gtsnpsivvl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xingfuxueyuan.xyz/gtuytraxye.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xinyue.icu/gtubjntrjr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.snrcjt.cn/gtyumaxsfz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jianghu66.top/gtfhysoaec.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.aizwys.cn/gtemayxhtl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.hammf.cn/gttvynjhsd.html

[D11] 反转数组
来源：http://hz.xuetiantiany.cn/gtxtylruyx.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.shuidangran.top/gtvdzadhrm.html

PHP:  array_reverse($arr);
来源：http://hz.yuxming.cn/gtcmvohybk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jyoumei.cn/gtnhusymrk.html

TS:   [...arr].reverse();
来源：http://hz.gotoacloud.top/gtdmhsvcgn.html

Java: Collections.reverse(list);
来源：http://hz.fengsongda.top/gtpyhgcqvq.html

Go:   slices.Reverse(arr)
来源：http://hz.hongshengwenyu.top/gtabhadxgv.html

Ruby: arr.reverse
来源：http://hz.gogol.net.cn/gttmlhvesl.html

C#:   list.Reverse();
来源：http://hz.pycfn.com/gtffskhbqp.html

[D12] 查找元素下标
来源：http://hz.jlsjyb.cn/gtlsclpytr.html

Py:   arr.index(x);  x in arr
来源：http://hz.birdmap.top/gtjxaeswls.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.nanxinkj.top/gtfoobxyea.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yvedp.cn/gtiormxhzu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinqigfzy.top/gtctsqieul.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yuxming.cn/gtyikrcmrx.html

Go:   slices.Index(arr, x)
来源：http://hz.nanxinkj.top/gtobowxykp.html

Ruby: arr.index(x)
来源：http://hz.jinqigfzy.top/gtuzktwzzg.html

C#:   list.IndexOf(x);
来源：http://hz.ydzc1.top/gtjriigmii.html

[D13] 过滤（保留满足条件的）
来源：http://hz.nwbrower.top/gtdappedmz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.sysykeji.top/gtpgtlbjeq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.ydjk.org.cn/gtnzhfmmsw.html

JS:   arr.filter(x => x > 3)
来源：http://hz.snrcjt.cn/gtluomemjk.html

TS:   arr.filter(x => x > 3)
来源：http://hz.hysaishi.cn/gteupjfonf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.ywan-chungtsiang.top/gtmzjgqbzi.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.quarkkingdee.top/gtadbrffnp.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zhengqikj.top/gtkgzppwpc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.dashuyun.cn/gtdxwzmcfz.html

[D14] 映射转换（每个元素变形）
来源：http://hz.zhixingplan.top/gtamvzujmm.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.c1oappe.top/gtofqiguvj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jinqigufen.top/gtumvdnank.html

JS:   arr.map(x => x * 2)
来源：http://hz.ywan-chungtsiang.top/gtdirhrnzb.html

TS:   arr.map(x => x * 2)
来源：http://hz.ydjk.org.cn/gtejlkpvup.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.smart0.xyz/gtgnfqtfpd.html

Go:   // 手写循环
来源：http://hz.hfpthk.cn/gtzgqjrkrl.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.smart0.xyz/gtvyueossr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zhiwuduotai.top/gttghcqfcv.html

[D15] 去重
来源：http://hz.316326.xyz/gtdjmnrbtf.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.cqqwz.cn/gtatptypls.html

PHP:  array_unique($arr);
来源：http://hz.zhijiandao.cn/gtcovglyhi.html

JS:   [...new Set(arr)]
来源：http://hz.zdqjudy.top/gtamuociqu.html

TS:   [...new Set(arr)]
来源：http://hz.hongshengwenyu.top/gthwjhsayc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.smart0.xyz/gtbwfymuqe.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.daria6918.cn/gtvhipkxgn.html

Ruby: arr.uniq
来源：http://hz.andypj.xyz/gtjhspktji.html

C#:   list.Distinct().ToList()
来源：http://hz.zhengqikj.top/gtyxrxqwab.html

[D16] 求和与平均值
来源：http://hz.yongpay.top/gtjfebfuri.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.hnqzz.top/gtfmjyaczt.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.guannengcc.top/gthqfursgx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yuanzhike.top/gtupvqmabj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.tian-w.cn/gttdsscwny.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jinqigufen.top/gtwhzbipqd.html

Go:   // 手写循环累加
来源：http://hz.snrcjt.cn/gtbyfrptvb.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jqgfzy.top/gtjkcnhaze.html

C#:   list.Sum();  list.Average()
来源：http://hz.aibaodan.cn/gtvtrgyfdk.html

[D17] 最大值与最小值
来源：http://hz.andypj.xyz/gttdubsytl.html

Py:   max(arr);  min(arr)
来源：http://hz.hfpthk.cn/gtbzvjafsb.html

PHP:  max($arr);  min($arr);
来源：http://hz.xylfe.cn/gtlnqboitf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yj20258888.top/gtruciclzw.html

TS:   Math.max(...arr);
来源：http://hz.tianlin.xyz/gtbupealil.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.ehwqpu.com/gtakltfhcl.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.nanxuanxn.top/gtfgxnhjnm.html

Ruby: arr.max;  arr.min
来源：http://hz.9152youxi.cn/gtpfdyeaqf.html

C#:   list.Max();  list.Min()
来源：http://hz.gotoacloud.top/gtnimhttxn.html

[D18] 扁平化嵌套数组
来源：http://hz.tian-w.cn/gtaxikcfzl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.hongshengwenyu.top/gtyojnrmmk.html

PHP:  array_merge(...$nested);
来源：http://hz.nanxinkj.top/gtbmuunyws.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.cashguo.top/gttscjduvx.html

TS:   nested.flat();
来源：http://hz.hysaishi.cn/gtlxabnoxw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.guowangkeji.top/gtisqdrpkz.html

Go:   // 手写双层循环
来源：http://hz.xinyue.icu/gttcmguyvu.html

Ruby: nested.flatten
来源：http://hz.hammf.cn/gtpwdsordd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.ehwqpu.com/gtoclgtmuf.html

[D19] 按字段分组
来源：http://hz.sysykeji.top/gthiibxvnu.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.cashguo.top/gthylpnxrz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yj202588.top/gtrcgjfitu.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jqgufenzy.top/gtiytisrxw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.hnqzz.top/gtmzqciysi.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.sufxvd.cn/gtqiycucbk.html

Go:   // 手写 map[string][]T
来源：http://hz.yvedp.cn/gtmxvqpgtg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.ivvv.top/gtyrvonkmz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.xziqi.cn/gtishqfzxt.html

[D20] 统计每个元素出现次数
来源：http://hz.hfpthk.cn/gtuoyriljz.html

Py:   Counter(arr)
来源：http://hz.sufxvd.cn/gtnwgwotoz.html

PHP:  array_count_values($arr);
来源：http://hz.jyoumei.cn/gtdsmadruk.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.tianlin.xyz/gtikkordnf.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.0kj1m.cn/gtwvzwpgyh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.meibo888.top/gtqyknahxv.html

Go:   // 手写 map[T]int
来源：http://hz.ybcxt.top/gtcmkdtxem.html

Ruby: arr.tally
来源：http://hz.dianchejie.cn/gtkvobsqfn.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yueranfly.top/gtvihuzcem.html

[D21] 判断是否包含某元素
来源：http://hz.fzhhl.top/gtztwycsuh.html

Py:   x in arr
来源：http://hz.yonumen.top/gtmxcbxnzh.html

PHP:  in_array($x, $arr, true);
来源：http://hz.tianlin.xyz/gtsdmvanpq.html

JS:   arr.includes(x)
来源：http://hz.tianlin.xyz/gtpntozaeo.html

TS:   arr.includes(x)
来源：http://hz.zhengqikj.top/gtxinfxudm.html

Java: list.contains(x)
来源：http://hz.guowangkeji.top/gtwynyhxhl.html

Go:   slices.Contains(arr, x)
来源：http://hz.shangyingyoupin.top/gtuehaoygx.html

Ruby: arr.include?(x)
来源：http://hz.zhijiandao.cn/gtsmiigeuk.html

C#:   list.Contains(x)
来源：http://hz.hnqzz.top/gtggocmwtm.html

[D22] 复制数组（避免共享引用）
来源：http://hz.sxryk.cn/gtkowhtjgb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yvedp.cn/gtzcreursb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.ppjwa.cn/gtlzrybttu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.zhaomingkeji.xyz/gtatykyojd.html

TS:   [...arr];
来源：http://hz.jqgfzy.top/gtcfoynjvi.html

Java: new ArrayList<>(list);
来源：http://hz.feifeiyinyue.top/gtmbpvmydu.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.sweek.top/gtphicippd.html

Ruby: arr.dup;  arr.clone
来源：http://hz.hysaishi.cn/gtxautcldh.html

C#:   new List<int>(list);
来源：http://hz.shuidangran.top/gtqzjkdlad.html

[D23] reduce 累积计算
来源：http://hz.hnxiangtu.top/gtpudsuiao.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.tianlin.xyz/gtglklrntb.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.sysykeji.top/gtxylnuaty.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yj202588.top/gtwmwmeeip.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yueranfly.top/gtcpzttbry.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jiagoushi.top/gtatwybjxo.html

Go:   // 手写循环
来源：http://hz.ppjwa.cn/gtnegbbpws.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.316326.xyz/gtgefhrkhe.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.zdqjudy.top/gtucxfaftv.html

[D24] 字典 / Map 基本操作
来源：http://hz.yj20258.top/gtlmsyjpgm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.aizwys.cn/gtmctwbtgx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.dianchejie.cn/gthoxdatea.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.hammf.cn/gtnqngcagx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.smart0.xyz/gtelzehhiv.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.hywenlv.cn/gtwjiwcaif.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.gotoacloud.top/gtdtfdqezk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.pycfn.com/gtqlysnzem.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.ybcxt.top/gtalprkaxx.html

[D25] Set 集合去重与交并差
来源：http://hz.wangshuangyany.cn/gtdsaenvty.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.jlsjyb.cn/gtvwohebls.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.feifeiyinyue.top/gtjifjqxwi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.gzhubu.top/gtkqltbiwv.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.sweek.top/gtosswjclw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yongpay.top/gtdrunyskj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.daxiang520.top/gtktznrjif.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.nwbrower.top/gtguoomzjf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.zhongyouzk.top/gtihdvkfor.html

[D26] 数组转字符串
来源：http://hz.zhiwuduotai.top/gtfovznjcj.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zhoulong.xyz/gtttyebzys.html

PHP:  implode(", ", $arr);
来源：http://hz.ppjwa.cn/gtridrbtot.html

JS:   arr.join(", ")
来源：http://hz.yj20258.top/gtstuzpyuo.html

TS:   arr.join(", ")
来源：http://hz.cqqwz.cn/gthommzzbo.html

Java: String.join(", ", list)
来源：http://hz.hysaishi.cn/gtenwohjma.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yongpay.top/gtoovwtkoj.html

Ruby: arr.join(", ")
来源：http://hz.fzhhl.top/gtmapjbtjs.html

C#:   string.Join(", ", list)
来源：http://hz.redwolf501.top/gtiroqqewu.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtuyenmmpe.html

E. 字符串处理
来源：http://hz.kuanghao11.cn/gtwzwivvlw.html

================================================================================
来源：http://hz.kuanghao11.cn/gtejjuylqb.html

[E01] 拼接字符串
来源：http://hz.guowangkeji.top/gtorcnsctf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.cdnleiting.top/gtefggqtsj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yonumen.top/gttmogdysu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.aibaodan.cn/gtwvcurpcz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.birdmap.top/gtcsbajmwz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.hammf.cn/gtrocdjymz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.fzhhl.top/gtqptrdmgn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.xziqi.cn/gtjqllkrtm.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.pengpengdd.cyou/gtnwmydihk.html


<!-- 参考信息 -->