代发 wailian999

Ruby: require "json"; require_relative "./util"
来源：http://hz.mhx1999.top/gtzvjbtjiq.html

C#:   using System.Text;
来源：http://hz.pycfn.com/gtgowhcyey.html

[C12] 立即执行函数 IIFE
来源：http://hz.shuidangran.top/gtkkgmbeds.html

Py:   (lambda: print("run"))()
来源：http://hz.yvedp.cn/gtniyrgxfe.html

PHP:  (function () { echo "run"; })();
来源：http://hz.jyoumei.cn/gtgbzthtpd.html

JS:   (() => { console.log("run"); })();
来源：http://hz.xylfe.cn/gthsrqgjxi.html

TS:   (() => { console.log("run"); })();
来源：http://hz.hammf.cn/gtazzhilwh.html

Java: // 无 IIFE：用 static { } 静态初始化块
来源：http://hz.jqgfzy.top/gtuhqxuzjy.html

Go:   func() { fmt.Println("run") }()
来源：http://hz.ydjk.org.cn/gtulkibfwb.html

Ruby: -> { puts "run" }.call
来源：http://hz.yongpay.top/gtplqkqppg.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.zhaomingkeji.xyz/gtbhrjzshq.html

[C13] 类型声明 / 类型注解
来源：http://hz.chenzaomai.com/gtihoxkqwa.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.xinyue.icu/gtxkfxzulf.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yongpay.top/gtwtodpskj.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.nwbrower.top/gtgfdtobbz.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zhoulong.xyz/gtybccekpn.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.sweek.top/gtzuiwvotd.html

Go:   func add(a, b int) int
来源：http://hz.havefunace.top/gtvxjbulqy.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.pengpengdd.cyou/gtcyzhuoqo.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.daria6918.cn/gtwkpjipxj.html

[C14] 泛型函数
来源：http://hz.ywan-chungtsiang.top/gtaggjjroz.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.svipenyu.cn/gtaifbvcue.html

PHP:  // 无泛型
来源：http://hz.ywan-chungtsiang.top/gtlzkacfyk.html

JS:   // 无泛型
来源：http://hz.shanyushiyangtech.top/gtyhqaokit.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.yonumen.top/gtncimggkf.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yj20258.top/gtixgpggqd.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.cheryme.top/gtljehlwjq.html

Ruby: # 无泛型
来源：http://hz.nanxuanxn.top/gtennsxicj.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.pycfn.com/gtopiuqnkm.html

[C15] 解构 / 展开参数
来源：http://hz.mhx1999.top/gtheemxcwe.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.tianlin.xyz/gtoufguxky.html

PHP:  [$a, $b] = $pair;
来源：http://hz.chenzaomai.com/gtlpsdmvmd.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.xinyue.icu/gtwxsnecwj.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.52xcode.cn/gteotbuqsn.html

Java: // 无解构
来源：http://hz.svipenyu.cn/gtwyxzmabs.html

Go:   // 无解构
来源：http://hz.shzxlz.cn/gtyuvsgylh.html

Ruby: a, b = pair
来源：http://hz.cashguo.top/gtzqdsnfvl.html

C#:   var (a, b) = pair;
来源：http://hz.cheryme.top/gtegojnmsz.html

[C16] 函数 / 方法重载
来源：http://hz.zhengqikj.top/gtenhnwnfi.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.mhx1999.top/gtqgjjnhjc.html

PHP:  // 无重载
来源：http://hz.zhixingplan.top/gtoydhujdq.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hnqzz.top/gtuzikrztv.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.yj20258.top/gtvkazzlua.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.xingfuxueyuan.xyz/gtolivauqo.html

Go:   // 无重载：用不同函数名
来源：http://hz.wangdashe.top/gtpxofncdl.html

Ruby: # 无重载：靠动态参数
来源：http://hz.nwbrower.top/gtbqvpgkkc.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.svipenyu.cn/gtcnvifnlh.html

================================================================================
来源：http://hz.xinyue.icu/gtntmxyuku.html

D. 数组 / 列表 / 集合
来源：http://hz.yongpay.top/gtxvywppte.html

================================================================================
来源：http://hz.jqgufenzy.top/gtglmzwbyu.html

[D01] 创建数组 / 列表
来源：http://hz.gogol.net.cn/gtvbwqadhh.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.yj20258888.top/gtrsiknbiz.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.fzhhl.top/gtfhruuizd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.cqqwz.cn/gtihmralwj.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.sxryk.cn/gtvpsmsblu.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.xinyue.icu/gtewxwnkdd.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.316326.xyz/gtsrtvludx.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yanxiufei.cn/gtfofkfaiu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.wangshuangyany.cn/gtmhzaxnjp.html

[D02] 追加元素到末尾
来源：http://hz.ydjk.org.cn/gtvdzgypqs.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.xuetiantiany.cn/gtkuxcrlwi.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.yvedp.cn/gteafdvhvk.html

JS:   arr.push(4);
来源：http://hz.yanxiufei.cn/gtlbggiobr.html

TS:   arr.push(4);
来源：http://hz.ivvv.top/gtqljscjzf.html

Java: list.add(4);
来源：http://hz.jinghuilouyu.cn/gttlipyede.html

Go:   arr = append(arr, 4)
来源：http://hz.zhaomingkeji.xyz/gtfojrjsvs.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.nanxuanxn.top/gtatfixgos.html

C#:   list.Add(4);
来源：http://hz.sysykeji.top/gtebypadzb.html

[D03] 在指定位置插入元素
来源：http://hz.quarkkingdee.top/gtdgaabzqr.html

Py:   arr.insert(0, 0)
来源：http://hz.ivvv.top/gtoxmzxvtm.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.316326.xyz/gtheqtaine.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.tanke756.top/gtkoktlgnr.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.52xcode.cn/gtqzgzbkrl.html

Java: list.add(0, 0);
来源：http://hz.ehwqpu.com/gtxpyxlpse.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.hywenlv.cn/gtgfshsvrp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.0kj1m.cn/gtbxewsrou.html

C#:   list.Insert(0, 0);
来源：http://hz.sweek.top/gtewqbcszy.html

[D04] 删除元素
来源：http://hz.yueranfly.top/gtgrcqxudg.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.nanxinkj.top/gtnpdyotpq.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.chenzaomai.com/gtsobnyyqv.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.redwolf501.top/gtstehxlmu.html

TS:   arr.splice(0, 1);
来源：http://hz.sweek.top/gtxwcrncil.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.yuxming.cn/gtlgeyxhlr.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.ydjk.org.cn/gtluoargqv.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.zdqjudy.top/gtwofbbiqz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.wangshuangyany.cn/gttxerzxpl.html

[D05] 访问与修改元素
来源：http://hz.sweek.top/gthhxljfxg.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.haohaochexian.top/gthqdsndqu.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.cheryme.top/gtttgwuupg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.xinyue.icu/gtkgirqfac.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.yueranfly.top/gttphvqbge.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.yonumen.top/gtcepuoxhn.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.snrcjt.cn/gtkybwfwnv.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hnxiangtu.top/gtznqjuknc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jianghu66.top/gtuzaxylgl.html

[D06] 数组长度
来源：http://hz.yj20258888.top/gttezkqlrb.html

Py:   len(arr)
来源：http://hz.nanxinkj.top/gtytviixka.html

PHP:  count($arr);
来源：http://hz.yj20258888.top/gtkxavxutw.html

JS:   arr.length
来源：http://hz.bjfxy.top/gtqqonnvmi.html

TS:   arr.length
来源：http://hz.shzxlz.cn/gtdnnethla.html

Java: list.size();
来源：http://hz.gaohongyu789.top/gtapjdhaxq.html

Go:   len(arr)
来源：http://hz.sysykeji.top/gtuxrbjngn.html

Ruby: arr.length; arr.size
来源：http://hz.pengpengdd.cyou/gtxalaptca.html

C#:   list.Count;
来源：http://hz.cqqwz.cn/gtfanegemv.html

[D07] 切片 / 取子数组
来源：http://hz.jiagoushi.top/gtpkiowetk.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jiagoushi.top/gtcvcozvmg.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.aizwys.cn/gtynwjhgtv.html

JS:   arr.slice(1, 4);
来源：http://hz.yj202588.top/gtktbdoctp.html

TS:   arr.slice(1, 4);
来源：http://hz.svipenyu.cn/gtjtkyviqr.html

Java: list.subList(1, 4);
来源：http://hz.wangshuangyany.cn/gtydqbjazt.html

Go:   arr[1:4]
来源：http://hz.zhaomingkeji.xyz/gtrnpfluqe.html

Ruby: arr[1, 3]
来源：http://hz.tanke756.top/gtbitutoje.html

C#:   list.GetRange(1, 3);
来源：http://hz.shanyushiyangtech.top/gtmrufshfu.html

[D08] 合并两个数组
来源：http://hz.hnxiangtu.top/gtgyibfzno.html

Py:   a + b;  a.extend(b)
来源：http://hz.yj202588.top/gtjhxjccag.html

PHP:  array_merge($a, $b);
来源：http://hz.jianghu66.top/gtsxgstubq.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.guowangkeji.top/gtgffjmvmw.html

TS:   [...a, ...b];
来源：http://hz.daxiang520.top/gtdjfkebwa.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.cheryme.top/gtwhopgamq.html

Go:   append(a, b...)
来源：http://hz.meibo888.top/gtrzdlvkos.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yj20258888.top/gtrtosmqxc.html

C#:   a.Concat(b).ToList()
来源：http://hz.yangfankeji.com/gttnvbgcok.html

[D09] 排序（升序）
来源：http://hz.jinghuilouyu.cn/gtxqokefcg.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yueranfly.top/gtwhkhxhbv.html

PHP:  sort($arr);
来源：http://hz.bjfxy.top/gtpnpuxhgu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.jiagoushi.top/gtmufdhlyk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.hysaishi.cn/gtzowxsyyb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.zhongyouzk.top/gtmzuttbjy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yueranfly.top/gtflrrqsdl.html

Ruby: arr.sort
来源：http://hz.daxiang520.top/gtpvkjtdyl.html

C#:   list.Sort();
来源：http://hz.shanyushiyangkeji.top/gthworshnt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zhengqikj.top/gtphsgokmn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zhijiandao.cn/gthnidulvq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.0kj1m.cn/gtemnqgyae.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhoulong.xyz/gtrlxtrozj.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.gaohongyu789.top/gtnfdrwdaj.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.redwolf501.top/gtmozceugf.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.hammf.cn/gtiinvnarl.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.ydjk.org.cn/gtswgqrnyx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.nanxuanxn.top/gtffnzeowe.html

[D11] 反转数组
来源：http://hz.xuanzx.com/gthtelevqm.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.hfpthk.cn/gtgifrdqto.html

PHP:  array_reverse($arr);
来源：http://hz.shanyushiyangtech.top/gtglwiaydv.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.zhoulong.xyz/gtypzlxhgz.html

TS:   [...arr].reverse();
来源：http://hz.9152youxi.cn/gtbghuaben.html

Java: Collections.reverse(list);
来源：http://hz.shanyushiyangtech.top/gtpskyemnf.html

Go:   slices.Reverse(arr)
来源：http://hz.yvedp.cn/gtcrxaaxlb.html

Ruby: arr.reverse
来源：http://hz.haohaochexian.top/gtgcawzhoo.html

C#:   list.Reverse();
来源：http://hz.svipenyu.cn/gtkebjskbq.html

[D12] 查找元素下标
来源：http://hz.ydzc1.top/gtxyufajhf.html

Py:   arr.index(x);  x in arr
来源：http://hz.chenlongwang.top/gtynmdgydk.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.redwolf501.top/gtttltdmpy.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ppjwa.cn/gtknombpcd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.fzhhl.top/gtvgddfnrz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.daria6918.cn/gtamibeonm.html

Go:   slices.Index(arr, x)
来源：http://hz.hnxiangtu.top/gtiatzalps.html

Ruby: arr.index(x)
来源：http://hz.jiagoushi.top/gtxpyucyla.html

C#:   list.IndexOf(x);
来源：http://hz.yongpay.top/gtowekfoer.html

[D13] 过滤（保留满足条件的）
来源：http://hz.vqdsnc.cn/gtmnqznbad.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zhengqikj.top/gtimfabbgj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.zhaomingkeji.xyz/gtkjtbmqaz.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yongpay.top/gtyowkwhxm.html

TS:   arr.filter(x => x > 3)
来源：http://hz.fzhhl.top/gtfqzpqbte.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.redwolf501.top/gtakmkalsp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.bjfxy.top/gtpyhuvkzb.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.hammf.cn/gteicbztvc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.sweek.top/gtmiomngxb.html

[D14] 映射转换（每个元素变形）
来源：http://hz.guannengcc.top/gtrwlkslkq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.xuanzx.com/gtqnocogwj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.hongshengwenyu.top/gtzatoyzgw.html

JS:   arr.map(x => x * 2)
来源：http://hz.cdnleiting.top/gtvnoopeau.html

TS:   arr.map(x => x * 2)
来源：http://hz.smart0.xyz/gtjpvenhxo.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.aizwys.cn/gtrmeckksg.html

Go:   // 手写循环
来源：http://hz.ppjwa.cn/gtemlgpldh.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yanxiufei.cn/gtyxswrknu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.feifeiyinyue.top/gtvvcwmowj.html

[D15] 去重
来源：http://hz.shanyushiyangkeji.top/gtpshbiems.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.hammf.cn/gtwlbysqmj.html

PHP:  array_unique($arr);
来源：http://hz.nanxinkj.top/gtsujmlnin.html

JS:   [...new Set(arr)]
来源：http://hz.xinyue.icu/gtrakvmivx.html

TS:   [...new Set(arr)]
来源：http://hz.smart0.xyz/gtafvxrcvl.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yongpay.top/gtyzmkxpcd.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.wangdashe.top/gtjessbhva.html

Ruby: arr.uniq
来源：http://hz.daria6918.cn/gtujizvbib.html

C#:   list.Distinct().ToList()
来源：http://hz.gzhubu.top/gtpvuwjois.html

[D16] 求和与平均值
来源：http://hz.shanyushiyangtech.top/gtvndggkjg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jinghuilouyu.cn/gtugxvbfgc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.tanke756.top/gtrzjhpioh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hongshengwenyu.top/gtrgnhpvwl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.9152youxi.cn/gtjztshoui.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.snrcjt.cn/gtuthgcjla.html

Go:   // 手写循环累加
来源：http://hz.dashuyun.cn/gtpdmywoky.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yj20258.top/gtxdfjmxds.html

C#:   list.Sum();  list.Average()
来源：http://hz.316326.xyz/gtpnyrtfsa.html

[D17] 最大值与最小值
来源：http://hz.hysaishi.cn/gtofadacyn.html

Py:   max(arr);  min(arr)
来源：http://hz.yonumen.top/gtfhbbxlnq.html

PHP:  max($arr);  min($arr);
来源：http://hz.redwolf501.top/gtgrefqfjj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.snrcjt.cn/gtohofwuor.html

TS:   Math.max(...arr);
来源：http://hz.yuanzhike.top/gtoudefngu.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zhengqikj.top/gtvskxciwv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.0kj1m.cn/gtesjyqogj.html

Ruby: arr.max;  arr.min
来源：http://hz.zhiwuduotai.top/gtdhfozxqc.html

C#:   list.Max();  list.Min()
来源：http://hz.tian-w.cn/gtmfdjzeeo.html

[D18] 扁平化嵌套数组
来源：http://hz.bjfxy.top/gtfpbsdqtx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.jiagoushi.top/gtobnlagwe.html

PHP:  array_merge(...$nested);
来源：http://hz.jqgfzy.top/gtxqdanjdr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yangfankeji.com/gtozvzcndg.html

TS:   nested.flat();
来源：http://hz.jqgufenzy.top/gtpdeyuqoo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.jlsjyb.cn/gtlxarkfri.html

Go:   // 手写双层循环
来源：http://hz.yanxiufei.cn/gteoeizzho.html

Ruby: nested.flatten
来源：http://hz.jyoumei.cn/gtxqndrbqd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zdqjudy.top/gtesapmios.html

[D19] 按字段分组
来源：http://hz.bjfxy.top/gtailxybxp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.xingfuxueyuan.xyz/gtzhupswek.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.hysaishi.cn/gtepvptnma.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.xingfuxueyuan.xyz/gthwoihifi.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.tian-w.cn/gtofxqmbby.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.andypj.xyz/gtjljhdzey.html

Go:   // 手写 map[string][]T
来源：http://hz.shanyushiyangtech.top/gtamjujxbm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.hfpthk.cn/gtzphktbwj.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.cashguo.top/gtsxzghvoy.html

[D20] 统计每个元素出现次数
来源：http://hz.aibaodan.cn/gtttptsgog.html

Py:   Counter(arr)
来源：http://hz.birdmap.top/gtkqxujwgz.html

PHP:  array_count_values($arr);
来源：http://hz.pengpengdd.cyou/gtlqupdrfd.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shanyushiyangkeji.top/gtdaojgeci.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.guowangkeji.top/gtddsuvlpa.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yanxiufei.cn/gtyhthwxsm.html

Go:   // 手写 map[T]int
来源：http://hz.quarkkingdee.top/gtmywuxitt.html

Ruby: arr.tally
来源：http://hz.fzhhl.top/gttzzvgddp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.chenlongwang.top/gtzyslguse.html

[D21] 判断是否包含某元素
来源：http://hz.vqdsnc.cn/gtrhzdlxla.html

Py:   x in arr
来源：http://hz.jyoumei.cn/gtqkxfeyrz.html

PHP:  in_array($x, $arr, true);
来源：http://hz.xylfe.cn/gtrmdumxwn.html

JS:   arr.includes(x)
来源：http://hz.feifeiyinyue.top/gtbuoogmrc.html

TS:   arr.includes(x)
来源：http://hz.zhaomingkeji.xyz/gtofnqcdco.html

Java: list.contains(x)
来源：http://hz.quarkkingdee.top/gtcygpgxux.html

Go:   slices.Contains(arr, x)
来源：http://hz.yuxming.cn/gtmgynxkdu.html

Ruby: arr.include?(x)
来源：http://hz.9152youxi.cn/gtkscsflzk.html

C#:   list.Contains(x)
来源：http://hz.zhijiandao.cn/gthxjiyume.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jianghu66.top/gtjotjjngt.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.wangshuangyany.cn/gtjegnxkyg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.shuidangran.top/gthlpkbppx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.zhijiandao.cn/gteqnugcgh.html

TS:   [...arr];
来源：http://hz.xingfuxueyuan.xyz/gtohpffbxt.html

Java: new ArrayList<>(list);
来源：http://hz.tanke756.top/gtltmjkssd.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.hywenlv.cn/gtuxjiorxf.html

Ruby: arr.dup;  arr.clone
来源：http://hz.chenlongwang.top/gtwoxcodkj.html

C#:   new List<int>(list);
来源：http://hz.redwolf501.top/gtttkspoli.html

[D23] reduce 累积计算
来源：http://hz.birdmap.top/gtmzwbuzem.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.xuanzx.com/gttlemynjt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.andypj.xyz/gtnarnooex.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xylfe.cn/gtvzzweijs.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yueranfly.top/gtbqdnbahl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.tian-w.cn/gtazukyfom.html

Go:   // 手写循环
来源：http://hz.kuanghao11.cn/gtknncfrav.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.ywan-chungtsiang.top/gtacqqmlvj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yanxiufei.cn/gtbcrwczsu.html

[D24] 字典 / Map 基本操作
来源：http://hz.jyoumei.cn/gtrubnblsz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.nanxuanxn.top/gtfjxjbdkg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jinqigufen.top/gtvkbkenpl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.guowangkeji.top/gtvozdqpgz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.fzhhl.top/gtigvopoie.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.gaohongyu789.top/gtdrpcethr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.chenzaomai.com/gtlcjpfhwy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.gzhubu.top/gtjgnzywzb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.hywenlv.cn/gtkopqmhrs.html

[D25] Set 集合去重与交并差
来源：http://hz.zhijiandao.cn/gtyzufpygf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.jinghuilouyu.cn/gtheofqrmy.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jianghu66.top/gtazwxauxc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.ydjk.org.cn/gtfrojdnux.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.xuetiantiany.cn/gttouyuncq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.andypj.xyz/gtaponiyaz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.dianchejie.cn/gtrinjqvqh.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yvedp.cn/gtzsuowgig.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.xuetiantiany.cn/gtuxvwtlxs.html

[D26] 数组转字符串
来源：http://hz.hysaishi.cn/gtioomjwjj.html

Py:   ", ".join(map(str, arr))
来源：http://hz.hongshengwenyu.top/gtkblzqhpg.html

PHP:  implode(", ", $arr);
来源：http://hz.xinyue.icu/gtehurpptl.html

JS:   arr.join(", ")
来源：http://hz.fzhhl.top/gtmejwcikr.html

TS:   arr.join(", ")
来源：http://hz.52xcode.cn/gtztvcoelm.html

Java: String.join(", ", list)
来源：http://hz.xziqi.cn/gtkjibxdxb.html

Go:   strings.Join(strs, ", ")
来源：http://hz.xuetiantiany.cn/gtbowhraba.html

Ruby: arr.join(", ")
来源：http://hz.xylfe.cn/gtgzohpvrn.html

C#:   string.Join(", ", list)
来源：http://hz.zhiwuduotai.top/gtkkxoyoff.html

================================================================================
来源：http://hz.jinyuanbaomall.cn/gtwqwmnost.html

E. 字符串处理
来源：http://hz.jinghuilouyu.cn/gtarnvfyfe.html

================================================================================
来源：http://hz.hywenlv.cn/gthspvnldn.html

[E01] 拼接字符串
来源：http://hz.shanyushiyangtech.top/gtdicvzcsd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.chenzaomai.com/gtlhdczjyw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.gogol.net.cn/gthktlgkaa.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.birdmap.top/gtwzadtahp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jinqigfzy.top/gtcgajjnrc.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.zhongyouzk.top/gtrzkcbzjr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.gzhubu.top/gtxsqoqhdt.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.shanyushiyangkeji.top/gtwmusbcat.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.pengpengdd.cyou/gtkaquhfyl.html

[E02] 重复字符串
来源：http://hz.nanxinkj.top/gtwexnjgvb.html

Py:   "ab" * 3
来源：http://hz.sxryk.cn/gtdqrgkmwx.html

PHP:  str_repeat("ab", 3);
来源：http://hz.dianchejie.cn/gtjwcpstuc.html

JS:   "ab".repeat(3)
来源：http://hz.yj20258.top/gtkknakpgf.html


<!-- 参考信息 -->