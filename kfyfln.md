代发 wailian999

Go:   func() { fmt.Println("run") }()
来源：http://hz.vqdsnc.cn/gtojxpdexo.html

Ruby: -> { puts "run" }.call
来源：http://hz.shanyushiyangtech.top/gtzdzqjmvl.html

C#:   // 无 IIFE：用静态构造函数
来源：http://hz.ppjwa.cn/gtdffdwbdf.html

[C13] 类型声明 / 类型注解
来源：http://hz.ywan-chungtsiang.top/gtijanzgtg.html

Py:   def add(a: int, b: int) -> int: return a + b
来源：http://hz.pengpengdd.cyou/gtspboyweb.html

PHP:  function add(int $a, int $b): int { return $a + $b; }
来源：http://hz.yuanzhike.top/gtmeiioenw.html

JS:   // 无类型（可用 JSDoc 注释）
来源：http://hz.ivvv.top/gtdmfmcfpn.html

TS:   function add(a: number, b: number): number { return a + b; }
来源：http://hz.zdqjudy.top/gtvwgksysk.html

Java: int add(int a, int b) { return a + b; }
来源：http://hz.jianghu66.top/gttckzqvtt.html

Go:   func add(a, b int) int
来源：http://hz.zhoulong.xyz/gtaxhsquly.html

Ruby: # 无类型（可选用 Sorbet / RBS）
来源：http://hz.sysykeji.top/gtelqdsviw.html

C#:   int Add(int a, int b) => a + b;
来源：http://hz.jyoumei.cn/gtgywlubtg.html

[C14] 泛型函数
来源：http://hz.bjfxy.top/gtgfgqlsmq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.sxryk.cn/gtijrjiadj.html

PHP:  // 无泛型
来源：http://hz.yangfankeji.com/gtnpanfkbf.html

JS:   // 无泛型
来源：http://hz.guannengcc.top/gtmmhmhpyt.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.0kj1m.cn/gtpnmtepde.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.gzhubu.top/gteyzjrbsm.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.chenlongwang.top/gtdjpajldc.html

Ruby: # 无泛型
来源：http://hz.fengsongda.top/gtofeyqdkr.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.aibaodan.cn/gtmvnlntun.html

[C15] 解构 / 展开参数
来源：http://hz.zhoulong.xyz/gttmozphnt.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.ivvv.top/gtpvanhhhs.html

PHP:  [$a, $b] = $pair;
来源：http://hz.sysykeji.top/gtzzbaribm.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.gaohongyu789.top/gttnfxkztc.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.zdqjudy.top/gtfowzasib.html

Java: // 无解构
来源：http://hz.xinyue.icu/gtqwzgoxoz.html

Go:   // 无解构
来源：http://hz.hfpthk.cn/gtsxwsqual.html

Ruby: a, b = pair
来源：http://hz.meibo888.top/gtdjvynskf.html

C#:   var (a, b) = pair;
来源：http://hz.guowangkeji.top/gtezcedajz.html

[C16] 函数 / 方法重载
来源：http://hz.bjfxy.top/gtkmvzjgko.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.cdnleiting.top/gtzberbzks.html

PHP:  // 无重载
来源：http://hz.gaohongyu789.top/gtnfshcihv.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.cheryme.top/gtssysdjlm.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.daria6918.cn/gtpjrfnoqo.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.chenzaomai.com/gtmtgyuoda.html

Go:   // 无重载：用不同函数名
来源：http://hz.zhaomingkeji.xyz/gtkerdmejo.html

Ruby: # 无重载：靠动态参数
来源：http://hz.yangfankeji.com/gtuzrmeufy.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.xinyue.icu/gtpoabyjoo.html

================================================================================
来源：http://hz.yanxiufei.cn/gtkfxbfwif.html

D. 数组 / 列表 / 集合
来源：http://hz.jinqigfzy.top/gtzdrbhhpw.html

================================================================================
来源：http://hz.shzxlz.cn/gtzlbkjvem.html

[D01] 创建数组 / 列表
来源：http://hz.cheryme.top/gthrvqjwna.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.hnqzz.top/gtualhskbs.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.hnqzz.top/gtyorzjxxq.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.daxiang520.top/gtvmhlqcht.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.gzhubu.top/gtitzlgsab.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.zdqjudy.top/gtjykvrdop.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.ivvv.top/gtkizddfzl.html

Ruby: arr = [1, 2, 3]
来源：http://hz.tianlin.xyz/gtkgrmlnsh.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.ivvv.top/gteycyiijp.html

[D02] 追加元素到末尾
来源：http://hz.jqgfzy.top/gtwvekiidi.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.sweek.top/gtczrzxyxj.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.fengsongda.top/gtclefzsuz.html

JS:   arr.push(4);
来源：http://hz.shzxlz.cn/gtrjamkzuq.html

TS:   arr.push(4);
来源：http://hz.hongshengwenyu.top/gtmbrvmtph.html

Java: list.add(4);
来源：http://hz.shanyushiyangtech.top/gtjbadkxue.html

Go:   arr = append(arr, 4)
来源：http://hz.jqgufenzy.top/gtohmkdqjo.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.tianlin.xyz/gtvwpfqdxc.html

C#:   list.Add(4);
来源：http://hz.sxryk.cn/gtlhiyzfau.html

[D03] 在指定位置插入元素
来源：http://hz.jinqigufen.top/gtnwumircx.html

Py:   arr.insert(0, 0)
来源：http://hz.ppjwa.cn/gtonkoklah.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.hongshengwenyu.top/gtrlhfizqb.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.vqdsnc.cn/gtoiyiuydv.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.tanke756.top/gtdwzcxqqh.html

Java: list.add(0, 0);
来源：http://hz.yj202588.top/gtgkhauzku.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.hnqzz.top/gthgesttuv.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.shzxlz.cn/gtpcrcsmda.html

C#:   list.Insert(0, 0);
来源：http://hz.hfpthk.cn/gtcceumuwi.html

[D04] 删除元素
来源：http://hz.gaohongyu789.top/gtzldniegx.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.xziqi.cn/gtkpdrqcpr.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.zhaomingkeji.xyz/gtrjypestp.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.birdmap.top/gtjvlkgbpv.html

TS:   arr.splice(0, 1);
来源：http://hz.yangfankeji.com/gtebcorwto.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.9152youxi.cn/gtkeodazwz.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.aizwys.cn/gtlcjvzlyf.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.nanxinkj.top/gtnampvhoy.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.hnqzz.top/gtydgsbefc.html

[D05] 访问与修改元素
来源：http://hz.yanxiufei.cn/gtsyavheea.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.iojbl.cn/gtwiydrpnn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.zhiwuduotai.top/gtjipsqyxj.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yuxming.cn/gtvgytgmpp.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.shanyushiyangkeji.top/gtstwnisec.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.jqgufenzy.top/gtclrvaneo.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.zhixingplan.top/gtxppwjpfj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yanxiufei.cn/gtbkifodyq.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.mhx1999.top/gtehftggqi.html

[D06] 数组长度
来源：http://hz.bjfxy.top/gtloqcwgnj.html

Py:   len(arr)
来源：http://hz.guowangkeji.top/gtzrweuvqp.html

PHP:  count($arr);
来源：http://hz.jinqigfzy.top/gttllucdrq.html

JS:   arr.length
来源：http://hz.guowangkeji.top/gtgztmvewi.html

TS:   arr.length
来源：http://hz.xinyue.icu/gtllugucxj.html

Java: list.size();
来源：http://hz.jinqigufen.top/gtubceyxir.html

Go:   len(arr)
来源：http://hz.xingfuxueyuan.xyz/gtqchskqzj.html

Ruby: arr.length; arr.size
来源：http://hz.shanyushiyangtech.top/gtypzvblxj.html

C#:   list.Count;
来源：http://hz.haohaochexian.top/gtbqkmtmik.html

[D07] 切片 / 取子数组
来源：http://hz.xziqi.cn/gtssaenxma.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.hnxiangtu.top/gticqmgnnu.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.daxiang520.top/gtdgokhvxd.html

JS:   arr.slice(1, 4);
来源：http://hz.zhoulong.xyz/gtijliierf.html

TS:   arr.slice(1, 4);
来源：http://hz.yj20258.top/gtspafitos.html

Java: list.subList(1, 4);
来源：http://hz.xingfuxueyuan.xyz/gtegbgfdqu.html

Go:   arr[1:4]
来源：http://hz.hywenlv.cn/gthzedtaoa.html

Ruby: arr[1, 3]
来源：http://hz.ybcxt.top/gttlmbwhwg.html

C#:   list.GetRange(1, 3);
来源：http://hz.wangshuangyany.cn/gtwqmeyfez.html

[D08] 合并两个数组
来源：http://hz.sxryk.cn/gtfhyfapvb.html

Py:   a + b;  a.extend(b)
来源：http://hz.havefunace.top/gtcqznbtfo.html

PHP:  array_merge($a, $b);
来源：http://hz.kuanghao11.cn/gtzklvsvaf.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.xuetiantiany.cn/gteyjuxihz.html

TS:   [...a, ...b];
来源：http://hz.cqqwz.cn/gtwwzzvvfq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.hammf.cn/gtnvbcvlkr.html

Go:   append(a, b...)
来源：http://hz.c1oappe.top/gtbmdoiifs.html

Ruby: a + b;  a.concat(b)
来源：http://hz.chenlongwang.top/gtjtpnajtg.html

C#:   a.Concat(b).ToList()
来源：http://hz.9152youxi.cn/gtkfyianxn.html

[D09] 排序（升序）
来源：http://hz.sweek.top/gtayfzmrxg.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.52xcode.cn/gttqjkvmrk.html

PHP:  sort($arr);
来源：http://hz.smart0.xyz/gtbskwczmf.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.shzxlz.cn/gtcfbndiuu.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yanxiufei.cn/gtidojtdqy.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.quarkkingdee.top/gtmcoacutz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.pycfn.com/gtruishzcn.html

Ruby: arr.sort
来源：http://hz.hysaishi.cn/gtkmwzcmae.html

C#:   list.Sort();
来源：http://hz.cqqwz.cn/gtptjtumin.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jyoumei.cn/gtpdjpqjsq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.meibo888.top/gtrsznsrpf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jinqigfzy.top/gtcjvtughk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yuanzhike.top/gtglhmnayw.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.sysykeji.top/gtldwgwgad.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yj202588.top/gtvtjgnslz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.zhixingplan.top/gtmmaujwmn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.sweek.top/gtipljsueo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.wangdashe.top/gtkdtdtjxl.html

[D11] 反转数组
来源：http://hz.dianchejie.cn/gthwgsykdg.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.sxryk.cn/gtckhwqmmp.html

PHP:  array_reverse($arr);
来源：http://hz.yongpay.top/gtxyyczcof.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jiagoushi.top/gtukoghohe.html

TS:   [...arr].reverse();
来源：http://hz.ywan-chungtsiang.top/gtquuokpks.html

Java: Collections.reverse(list);
来源：http://hz.dashuyun.cn/gtoqvamiqi.html

Go:   slices.Reverse(arr)
来源：http://hz.zhixingplan.top/gtujvzdcrg.html

Ruby: arr.reverse
来源：http://hz.gaohongyu789.top/gtguheihmd.html

C#:   list.Reverse();
来源：http://hz.52xcode.cn/gtzxanhyoo.html

[D12] 查找元素下标
来源：http://hz.jlsjyb.cn/gtefrotovj.html

Py:   arr.index(x);  x in arr
来源：http://hz.daxiang520.top/gtnccfhglj.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.nanxinkj.top/gtzmmdbwre.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.bjfxy.top/gtsqgyhbyz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.vqdsnc.cn/gttrgamomn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.shzxlz.cn/gtbborlxxv.html

Go:   slices.Index(arr, x)
来源：http://hz.hnqzz.top/gtrpvkgknd.html

Ruby: arr.index(x)
来源：http://hz.redwolf501.top/gtwssvimnu.html

C#:   list.IndexOf(x);
来源：http://hz.vqdsnc.cn/gtkcrxbqov.html

[D13] 过滤（保留满足条件的）
来源：http://hz.fzhhl.top/gtlpgjcmlj.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.ivvv.top/gtutgkgnjh.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.shangyingyoupin.top/gtzooxxzvy.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jlsjyb.cn/gtokozlfhv.html

TS:   arr.filter(x => x > 3)
来源：http://hz.zhongyouzk.top/gtdgxbiaji.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.ywan-chungtsiang.top/gtunecltjm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.zhoulong.xyz/gtekbinfxz.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.nanxinkj.top/gtbbdkxmmn.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.zhoulong.xyz/gtnowaydim.html

[D14] 映射转换（每个元素变形）
来源：http://hz.zhiwuduotai.top/gtwbjvacik.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.fengsongda.top/gthhwieqnh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.aibaodan.cn/gtzsxxuwdt.html

JS:   arr.map(x => x * 2)
来源：http://hz.xziqi.cn/gtglghhlxs.html

TS:   arr.map(x => x * 2)
来源：http://hz.xziqi.cn/gthrtxaxjj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.gotoacloud.top/gttrvapezz.html

Go:   // 手写循环
来源：http://hz.jinyuanbaomall.cn/gtshjbkdvl.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.cashguo.top/gtajfnanfm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yongpay.top/gtrchauend.html

[D15] 去重
来源：http://hz.havefunace.top/gtypisjjsi.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.gzhubu.top/gtbqdsgrln.html

PHP:  array_unique($arr);
来源：http://hz.tanke756.top/gtnvfggsey.html

JS:   [...new Set(arr)]
来源：http://hz.chenzaomai.com/gtjogfwzdr.html

TS:   [...new Set(arr)]
来源：http://hz.zdqjudy.top/gtarngeoux.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.zhongyouzk.top/gtycpwptci.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.jinyuanbaomall.cn/gtgzurbykg.html

Ruby: arr.uniq
来源：http://hz.ydjk.org.cn/gtwlftqzih.html

C#:   list.Distinct().ToList()
来源：http://hz.xinyue.icu/gtqxdmmvys.html

[D16] 求和与平均值
来源：http://hz.mhx1999.top/gtkqatcsyb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.shzxlz.cn/gtaixviyug.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yangfankeji.com/gtqqvjxiil.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.guannengcc.top/gtonbibexz.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hammf.cn/gtktfwusnn.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.sufxvd.cn/gtqhdvsrqe.html

Go:   // 手写循环累加
来源：http://hz.hammf.cn/gtjlovqczo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yangfankeji.com/gthkdwgfit.html

C#:   list.Sum();  list.Average()
来源：http://hz.xingfuxueyuan.xyz/gtepgfgudo.html

[D17] 最大值与最小值
来源：http://hz.cheryme.top/gtfhdzogkl.html

Py:   max(arr);  min(arr)
来源：http://hz.pycfn.com/gtxpukyuec.html

PHP:  max($arr);  min($arr);
来源：http://hz.jyoumei.cn/gtzmqchrvr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.dashuyun.cn/gtczgmfmex.html

TS:   Math.max(...arr);
来源：http://hz.gotoacloud.top/gtseyjhjkc.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.quarkkingdee.top/gtmifmigzi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.ppjwa.cn/gtyuwtmccy.html

Ruby: arr.max;  arr.min
来源：http://hz.chenlongwang.top/gtromomigy.html

C#:   list.Max();  list.Min()
来源：http://hz.xuanzx.com/gtwixtsyec.html

[D18] 扁平化嵌套数组
来源：http://hz.svipenyu.cn/gthooxnqrq.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.nwbrower.top/gtpysodlih.html

PHP:  array_merge(...$nested);
来源：http://hz.zhongyouzk.top/gtscwsvjqb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.gzhubu.top/gtsomzkwxq.html

TS:   nested.flat();
来源：http://hz.bjfxy.top/gtdmluuoba.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.wangdashe.top/gtyitjabut.html

Go:   // 手写双层循环
来源：http://hz.shangyingyoupin.top/gtfulnyqzj.html

Ruby: nested.flatten
来源：http://hz.sufxvd.cn/gtbqsughci.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.redwolf501.top/gteapkiibv.html

[D19] 按字段分组
来源：http://hz.jqgfzy.top/gtezmnqhdl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.xziqi.cn/gtsrssavce.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.tanke756.top/gtlzttxoze.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.fengsongda.top/gtzwptvyev.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.316326.xyz/gtzxcwyklt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.ppjwa.cn/gtgqwxstab.html

Go:   // 手写 map[string][]T
来源：http://hz.nanxinkj.top/gtvlqsymqp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.gaohongyu789.top/gtdegbrbbk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yj202588.top/gtgzubmike.html

[D20] 统计每个元素出现次数
来源：http://hz.ybcxt.top/gteqyhpzuy.html

Py:   Counter(arr)
来源：http://hz.jqgufenzy.top/gtdtvxlhae.html

PHP:  array_count_values($arr);
来源：http://hz.vqdsnc.cn/gtypauphah.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.chenzaomai.com/gtswpnlcsi.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.9152youxi.cn/gtlngmdyho.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.quarkkingdee.top/gtyjkdyaks.html

Go:   // 手写 map[T]int
来源：http://hz.sufxvd.cn/gtywccclcm.html

Ruby: arr.tally
来源：http://hz.jianghu66.top/gthhtwvqee.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zhiwuduotai.top/gtxvllcxzo.html

[D21] 判断是否包含某元素
来源：http://hz.zhaomingkeji.xyz/gtsdaxncnc.html

Py:   x in arr
来源：http://hz.316326.xyz/gtuoffdsvk.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yj202588.top/gtpmxicbll.html

JS:   arr.includes(x)
来源：http://hz.chenzaomai.com/gtdibwkddl.html

TS:   arr.includes(x)
来源：http://hz.ybcxt.top/gtqoaexegc.html

Java: list.contains(x)
来源：http://hz.aizwys.cn/gtpzcferzv.html

Go:   slices.Contains(arr, x)
来源：http://hz.chenzaomai.com/gtbxhkkmbd.html

Ruby: arr.include?(x)
来源：http://hz.jqgufenzy.top/gtrkrdijsd.html

C#:   list.Contains(x)
来源：http://hz.cdnleiting.top/gtmchbkycx.html

[D22] 复制数组（避免共享引用）
来源：http://hz.9152youxi.cn/gtqybnxznu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.nanxuanxn.top/gtaesgfrlg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jqgufenzy.top/gtnshgkauc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.svipenyu.cn/gtjhwdtyhm.html

TS:   [...arr];
来源：http://hz.shanyushiyangtech.top/gtszjorkcl.html

Java: new ArrayList<>(list);
来源：http://hz.zhoulong.xyz/gtvfpneecs.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.hysaishi.cn/gtrktezrpe.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yangfankeji.com/gtgvmldepl.html

C#:   new List<int>(list);
来源：http://hz.tian-w.cn/gtvmbkvfct.html

[D23] reduce 累积计算
来源：http://hz.sufxvd.cn/gtnokqcboy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.ehwqpu.com/gtbkxpucdh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.snrcjt.cn/gthqrbvrjf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yongpay.top/gtrzsawolh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.quarkkingdee.top/gtlyrboygo.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.0kj1m.cn/gtmoajkomf.html

Go:   // 手写循环
来源：http://hz.zhiwuduotai.top/gtnfxoyvep.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.9152youxi.cn/gtvyappbqn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.xuetiantiany.cn/gtldbshddy.html

[D24] 字典 / Map 基本操作
来源：http://hz.vqdsnc.cn/gtfdryuhol.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.hnxiangtu.top/gtgxumxcnb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.nwbrower.top/gtawejxndx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.tian-w.cn/gtnwqaavhf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.birdmap.top/gtrnkatfty.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.cdnleiting.top/gtiggoizym.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.xinyue.icu/gthchovvyh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.xziqi.cn/gtpayhfzxr.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.wangdashe.top/gtdhverspt.html

[D25] Set 集合去重与交并差
来源：http://hz.shangyingyoupin.top/gtweffrgfr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.andypj.xyz/gtdjniezfo.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.xingfuxueyuan.xyz/gtaapjjntf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.xinyue.icu/gttaxtczxi.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jinghuilouyu.cn/gtqbyewzwa.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.52xcode.cn/gtnhpfyycv.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.gaohongyu789.top/gthsjqgkgj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.0kj1m.cn/gtgkbqkzpe.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.quarkkingdee.top/gtrofhpecl.html

[D26] 数组转字符串
来源：http://hz.chenzaomai.com/gtisbihebp.html

Py:   ", ".join(map(str, arr))
来源：http://hz.aibaodan.cn/gtosdbfsjw.html

PHP:  implode(", ", $arr);
来源：http://hz.jiagoushi.top/gthdqicktv.html

JS:   arr.join(", ")
来源：http://hz.jyoumei.cn/gtnywycjxd.html

TS:   arr.join(", ")
来源：http://hz.hammf.cn/gtwcdofshf.html

Java: String.join(", ", list)
来源：http://hz.ydzc1.top/gtrtgfzolp.html

Go:   strings.Join(strs, ", ")
来源：http://hz.shanyushiyangtech.top/gtarkdxnjv.html

Ruby: arr.join(", ")
来源：http://hz.nwbrower.top/gtfhhuiaml.html

C#:   string.Join(", ", list)
来源：http://hz.sxryk.cn/gtvuhkuzoj.html

================================================================================
来源：http://hz.316326.xyz/gtxewxqgrs.html

E. 字符串处理
来源：http://hz.xuetiantiany.cn/gtzwxvodse.html

================================================================================
来源：http://hz.kuanghao11.cn/gtgpzqusvv.html

[E01] 拼接字符串
来源：http://hz.jinqigfzy.top/gtrkwrnjxn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.xuetiantiany.cn/gtbmobmzdw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.tianlin.xyz/gtishmymre.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hnxiangtu.top/gtglhuwnme.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yongpay.top/gtkqkqhdex.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.bjfxy.top/gtoyduzxdu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.smart0.xyz/gtdoosgnkx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.cashguo.top/gtugdyyayp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.jiagoushi.top/gtovxiuetp.html

[E02] 重复字符串
来源：http://hz.xingfuxueyuan.xyz/gtsypnukqj.html

Py:   "ab" * 3
来源：http://hz.wangdashe.top/gtjijbfycl.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yj20258.top/gtuzsdnaat.html

JS:   "ab".repeat(3)
来源：http://hz.jinyuanbaomall.cn/gtrihjvzrj.html

TS:   "ab".repeat(3)
来源：http://hz.gotoacloud.top/gtiwsfffch.html

Java: "ab".repeat(3)
来源：http://hz.ydjk.org.cn/gtjwlvxjpb.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jinyuanbaomall.cn/gtnrzofqwr.html

Ruby: "ab" * 3
来源：http://hz.quarkkingdee.top/gttleocsfb.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.wangdashe.top/gtumwzcpqb.html

[E03] 截取子串
来源：http://hz.iojbl.cn/gtsqdlnfns.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.shanyushiyangkeji.top/gtkidvddcv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.hnxiangtu.top/gtuzinajvt.html


<!-- 参考信息 -->