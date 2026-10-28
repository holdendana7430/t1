代发 wailian999

[C14] 泛型函数
来源：http://hz.yj20258.top/gtxaolivmt.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.bjfxy.top/gtfarycxxw.html

PHP:  // 无泛型
来源：http://hz.shanyushiyangkeji.top/gtuwnbbuap.html

JS:   // 无泛型
来源：http://hz.bjfxy.top/gtrmtdczxu.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.vqdsnc.cn/gtaicnuthq.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.yj20258.top/gtejoqdmbo.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.pengpengdd.cyou/gtyoakyozq.html

Ruby: # 无泛型
来源：http://hz.birdmap.top/gtbzhrsfhx.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.yj202588.top/gtnjaegbpo.html

[C15] 解构 / 展开参数
来源：http://hz.hfpthk.cn/gtvkuxvdgm.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.ywan-chungtsiang.top/gthkuzlndy.html

PHP:  [$a, $b] = $pair;
来源：http://hz.xingfuxueyuan.xyz/gtwowygeut.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yuanzhike.top/gtglmqrasy.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.ydjk.org.cn/gtgkzmgmde.html

Java: // 无解构
来源：http://hz.jiagoushi.top/gtswotjkud.html

Go:   // 无解构
来源：http://hz.fzhhl.top/gtxnygisux.html

Ruby: a, b = pair
来源：http://hz.nwbrower.top/gthxkhfblp.html

C#:   var (a, b) = pair;
来源：http://hz.jyoumei.cn/gtfzodubzf.html

[C16] 函数 / 方法重载
来源：http://hz.vqdsnc.cn/gtkvocbisy.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.chenjidiqi.icu/gtgxvnqwbi.html

PHP:  // 无重载
来源：http://hz.zhijiandao.cn/gtyrsdijih.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.aibaodan.cn/gtchbkrzeh.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.ydzc1.top/gtqrttgnnj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.xingfuxueyuan.xyz/gtldngeype.html

Go:   // 无重载：用不同函数名
来源：http://hz.zdqjudy.top/gtlisdjmve.html

Ruby: # 无重载：靠动态参数
来源：http://hz.ivvv.top/gtwptpqwzi.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.pycfn.com/gtqxkcyell.html

================================================================================
来源：http://hz.cheryme.top/gtxzpvkggu.html

D. 数组 / 列表 / 集合
来源：http://hz.yvedp.cn/gtgwbzbfci.html

================================================================================
来源：http://hz.zhaomingkeji.xyz/gtwwigscxf.html

[D01] 创建数组 / 列表
来源：http://hz.hnxiangtu.top/gtsnijtwzp.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.gotoacloud.top/gtkwgqjeok.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.fengsongda.top/gtqcqvgtpd.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.hnxiangtu.top/gtqjkshtkx.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.sweek.top/gtejlevmrq.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.yuanzhike.top/gtpydfiadz.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.yj202588.top/gtkchvllwg.html

Ruby: arr = [1, 2, 3]
来源：http://hz.yonumen.top/gtriwbslvx.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.pycfn.com/gtcnileiwu.html

[D02] 追加元素到末尾
来源：http://hz.9152youxi.cn/gtmqyetisk.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.yj20258.top/gtstryeetl.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.wangshuangyany.cn/gtqnkbwkew.html

JS:   arr.push(4);
来源：http://hz.jianghu66.top/gteauwghls.html

TS:   arr.push(4);
来源：http://hz.gogol.net.cn/gtuhupspci.html

Java: list.add(4);
来源：http://hz.9152youxi.cn/gtjsfipapv.html

Go:   arr = append(arr, 4)
来源：http://hz.havefunace.top/gtmtiyfmpu.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.quarkkingdee.top/gtyuhvdksw.html

C#:   list.Add(4);
来源：http://hz.yj20258.top/gtlkfqrmfc.html

[D03] 在指定位置插入元素
来源：http://hz.mhx1999.top/gtglikhodx.html

Py:   arr.insert(0, 0)
来源：http://hz.gaohongyu789.top/gtkmkivjqo.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.zhaomingkeji.xyz/gtqzmlwege.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.haohaochexian.top/gthboxdpff.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.aibaodan.cn/gtwioyywuo.html

Java: list.add(0, 0);
来源：http://hz.iojbl.cn/gtvcsnmfyl.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.sweek.top/gtwlyswshh.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.aibaodan.cn/gtgiuuwvmf.html

C#:   list.Insert(0, 0);
来源：http://hz.jqgufenzy.top/gtibiegygp.html

[D04] 删除元素
来源：http://hz.dashuyun.cn/gtxabdcamo.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.cdnleiting.top/gtvessdsry.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.quarkkingdee.top/gtpilivllf.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.jinqigfzy.top/gtbkvfmnnq.html

TS:   arr.splice(0, 1);
来源：http://hz.gogol.net.cn/gttwddmojj.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.jinyuanbaomall.cn/gtwjqatadb.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.yj20258888.top/gtvrfdpktk.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.gzhubu.top/gtqeupixho.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yj202588.top/gtteaxrydg.html

[D05] 访问与修改元素
来源：http://hz.aizwys.cn/gtduasnnij.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.gogol.net.cn/gtmvszzxyt.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.zhengqikj.top/gtwdkrpsfb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.cheryme.top/gtghzgwmvn.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.wangshuangyany.cn/gtexdkaqit.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.shuidangran.top/gtodriecpn.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.52xcode.cn/gtzsclrgly.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.pengpengdd.cyou/gtnpbcqtep.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.tianlin.xyz/gtxowwujxy.html

[D06] 数组长度
来源：http://hz.yanxiufei.cn/gtfbfiwttb.html

Py:   len(arr)
来源：http://hz.pengpengdd.cyou/gtrwrfnehg.html

PHP:  count($arr);
来源：http://hz.jinyuanbaomall.cn/gttzhmjyfg.html

JS:   arr.length
来源：http://hz.hnxiangtu.top/gtydxwwegv.html

TS:   arr.length
来源：http://hz.zhongyouzk.top/gtrdzobunx.html

Java: list.size();
来源：http://hz.pengpengdd.cyou/gtlgvuapzd.html

Go:   len(arr)
来源：http://hz.cdnleiting.top/gtizirgbqi.html

Ruby: arr.length; arr.size
来源：http://hz.52xcode.cn/gtbouimwnx.html

C#:   list.Count;
来源：http://hz.jinghuilouyu.cn/gttbepuewx.html

[D07] 切片 / 取子数组
来源：http://hz.guowangkeji.top/gtajsxayux.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.guowangkeji.top/gtztsffvtm.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.vqdsnc.cn/gtklrultdq.html

JS:   arr.slice(1, 4);
来源：http://hz.daxiang520.top/gtbygbexlc.html

TS:   arr.slice(1, 4);
来源：http://hz.hywenlv.cn/gtlifnjvkf.html

Java: list.subList(1, 4);
来源：http://hz.dashuyun.cn/gtjicmavfj.html

Go:   arr[1:4]
来源：http://hz.hammf.cn/gtningdbsy.html

Ruby: arr[1, 3]
来源：http://hz.dianchejie.cn/gtxlfhfeny.html

C#:   list.GetRange(1, 3);
来源：http://hz.jqgfzy.top/gtxpzdtfab.html

[D08] 合并两个数组
来源：http://hz.havefunace.top/gthcmksfxf.html

Py:   a + b;  a.extend(b)
来源：http://hz.yuanzhike.top/gtwriyqznn.html

PHP:  array_merge($a, $b);
来源：http://hz.xylfe.cn/gtvpiydcns.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yj20258.top/gtbawnwwlz.html

TS:   [...a, ...b];
来源：http://hz.cucudq.cn/gtmiyecpkn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.hywenlv.cn/gtlbwvbmmg.html

Go:   append(a, b...)
来源：http://hz.chenzaomai.com/gtqhyfxnon.html

Ruby: a + b;  a.concat(b)
来源：http://hz.52xcode.cn/gtxqcjebns.html

C#:   a.Concat(b).ToList()
来源：http://hz.xuetiantiany.cn/gtlyjasgyw.html

[D09] 排序（升序）
来源：http://hz.ywan-chungtsiang.top/gtuzgdrooe.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.dashuyun.cn/gtkqhcbjeo.html

PHP:  sort($arr);
来源：http://hz.chenlongwang.top/gtrxzqvfgk.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.gaohongyu789.top/gtionauccj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.hywenlv.cn/gthbpwrule.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.ppjwa.cn/gteuxdjadu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.pycfn.com/gtkfhnhopk.html

Ruby: arr.sort
来源：http://hz.yangfankeji.com/gtoskwtfoa.html

C#:   list.Sort();
来源：http://hz.pengpengdd.cyou/gtamuigxab.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.hfpthk.cn/gtysbyslew.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zhaomingkeji.xyz/gtytghyqnh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.pycfn.com/gtvbtsgtou.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.fzhhl.top/gthdenhckp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinghuilouyu.cn/gtvhslrqdq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.pycfn.com/gtkkagfaao.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.wangshuangyany.cn/gtvjiyuppk.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.9152youxi.cn/gtdhadympj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.guannengcc.top/gtillqjllu.html

[D11] 反转数组
来源：http://hz.ppjwa.cn/gtzkjpnqkg.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.haohaochexian.top/gtbzqdltnw.html

PHP:  array_reverse($arr);
来源：http://hz.xingfuxueyuan.xyz/gtyaphhjdg.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.gzhubu.top/gthjbzenvm.html

TS:   [...arr].reverse();
来源：http://hz.shuidangran.top/gtfncmbetl.html

Java: Collections.reverse(list);
来源：http://hz.yj20258888.top/gtcialmfuo.html

Go:   slices.Reverse(arr)
来源：http://hz.nanxinkj.top/gtfdkwyslz.html

Ruby: arr.reverse
来源：http://hz.shuidangran.top/gteimoruyf.html

C#:   list.Reverse();
来源：http://hz.jianghu66.top/gtulakoxbw.html

[D12] 查找元素下标
来源：http://hz.quarkkingdee.top/gtctdaduqj.html

Py:   arr.index(x);  x in arr
来源：http://hz.cucudq.cn/gtktmpoaot.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.hongshengwenyu.top/gtmjzfazbn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.wangshuangyany.cn/gttojpxvhk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.pengpengdd.cyou/gtasuthjlt.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.quarkkingdee.top/gtkvaktlcx.html

Go:   slices.Index(arr, x)
来源：http://hz.zycfv.cn/gteunlnwal.html

Ruby: arr.index(x)
来源：http://hz.dashuyun.cn/gtdxfgqyle.html

C#:   list.IndexOf(x);
来源：http://hz.sysykeji.top/gtfhibbrpo.html

[D13] 过滤（保留满足条件的）
来源：http://hz.yanxiufei.cn/gttmuxffrh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.gotoacloud.top/gtbeostitj.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.0kj1m.cn/gtwyyoygge.html

JS:   arr.filter(x => x > 3)
来源：http://hz.svipenyu.cn/gtqtdfhpik.html

TS:   arr.filter(x => x > 3)
来源：http://hz.yongpay.top/gtvjxcnniz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.dashuyun.cn/gtpzfzmrfb.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.chenlongwang.top/gtrjzzqziw.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jiagoushi.top/gtppwzinfk.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.cucudq.cn/gtxrmwglhq.html

[D14] 映射转换（每个元素变形）
来源：http://hz.chenjidiqi.icu/gtojiygjwr.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jinyuanbaomall.cn/gtfuokgtcv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.ehwqpu.com/gtssxwjseu.html

JS:   arr.map(x => x * 2)
来源：http://hz.gaohongyu789.top/gtczwqyjvc.html

TS:   arr.map(x => x * 2)
来源：http://hz.sxryk.cn/gtvtuaoltt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.ybcxt.top/gtbtvdnpqz.html

Go:   // 手写循环
来源：http://hz.chenlongwang.top/gtjmnksypz.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jinghuilouyu.cn/gtrxsysjyi.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.ivvv.top/gtxwuvhphv.html

[D15] 去重
来源：http://hz.yj20258888.top/gtwtkjwoqq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.quarkkingdee.top/gtypqzcvod.html

PHP:  array_unique($arr);
来源：http://hz.jqgufenzy.top/gtyrawgjqd.html

JS:   [...new Set(arr)]
来源：http://hz.316326.xyz/gtpfuhdmiw.html

TS:   [...new Set(arr)]
来源：http://hz.sxryk.cn/gtzgbpizzj.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.wangdashe.top/gtpgbnrpjz.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yueranfly.top/gttlcorbzk.html

Ruby: arr.uniq
来源：http://hz.xuetiantiany.cn/gtwgjdmynu.html

C#:   list.Distinct().ToList()
来源：http://hz.hfpthk.cn/gtuuuvhlaq.html

[D16] 求和与平均值
来源：http://hz.gogol.net.cn/gtrxxogtek.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.ywan-chungtsiang.top/gtmktmgpys.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.tian-w.cn/gtomizucuc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jqgfzy.top/gtztabtcqd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.nanxuanxn.top/gtbjlqslxs.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yongpay.top/gtyhneafpw.html

Go:   // 手写循环累加
来源：http://hz.jinghuilouyu.cn/gtctqellub.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.andypj.xyz/gtsemfqhzd.html

C#:   list.Sum();  list.Average()
来源：http://hz.chenjidiqi.icu/gtecjbjrbv.html

[D17] 最大值与最小值
来源：http://hz.xuanzx.com/gtjiilncrf.html

Py:   max(arr);  min(arr)
来源：http://hz.yueranfly.top/gtxbzokfvp.html

PHP:  max($arr);  min($arr);
来源：http://hz.tian-w.cn/gtcftjxqty.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.dianchejie.cn/gtdlagowpc.html

TS:   Math.max(...arr);
来源：http://hz.xingfuxueyuan.xyz/gtkryilsbt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zhixingplan.top/gtigasdemo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.gogol.net.cn/gttfsqadec.html

Ruby: arr.max;  arr.min
来源：http://hz.zhiwuduotai.top/gtuvkmqcli.html

C#:   list.Max();  list.Min()
来源：http://hz.svipenyu.cn/gtaikldxhd.html

[D18] 扁平化嵌套数组
来源：http://hz.xinyue.icu/gtyzbnvdkb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.52xcode.cn/gtkurtwkjk.html

PHP:  array_merge(...$nested);
来源：http://hz.dashuyun.cn/gtfnamcydh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.dianchejie.cn/gtmkyjmgtl.html

TS:   nested.flat();
来源：http://hz.svipenyu.cn/gtxrprrlye.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.sufxvd.cn/gtgfdosypi.html

Go:   // 手写双层循环
来源：http://hz.ppjwa.cn/gtlimmlzsp.html

Ruby: nested.flatten
来源：http://hz.chenzaomai.com/gthdjvvihr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.sweek.top/gtrqbbeimz.html

[D19] 按字段分组
来源：http://hz.sysykeji.top/gtyhdwyflf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.xziqi.cn/gtpynylizk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.tian-w.cn/gtywpedbgi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.cashguo.top/gtlwsrmnod.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.xinyue.icu/gtuvglfznp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.haohaochexian.top/gtkhkzwnrb.html

Go:   // 手写 map[string][]T
来源：http://hz.cashguo.top/gtgeekwuja.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.chenzaomai.com/gthnhnrfne.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.shanyushiyangkeji.top/gtktfesrxs.html

[D20] 统计每个元素出现次数
来源：http://hz.guowangkeji.top/gtlaggaeol.html

Py:   Counter(arr)
来源：http://hz.316326.xyz/gthtfojkxd.html

PHP:  array_count_values($arr);
来源：http://hz.andypj.xyz/gttibxdefl.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.gogol.net.cn/gtyqzcncpt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.guannengcc.top/gtmjxgocls.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.haohaochexian.top/gtmdbfigoz.html

Go:   // 手写 map[T]int
来源：http://hz.sxryk.cn/gtrajftudk.html

Ruby: arr.tally
来源：http://hz.zhoulong.xyz/gtwamjkgxe.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.jinqigufen.top/gtpdkuhate.html

[D21] 判断是否包含某元素
来源：http://hz.zhixingplan.top/gtfpobxdon.html

Py:   x in arr
来源：http://hz.hnxiangtu.top/gtgqdlukgw.html

PHP:  in_array($x, $arr, true);
来源：http://hz.gaohongyu789.top/gthggtoloy.html

JS:   arr.includes(x)
来源：http://hz.c1oappe.top/gtgwmzakir.html

TS:   arr.includes(x)
来源：http://hz.aibaodan.cn/gtrmqxcvlf.html

Java: list.contains(x)
来源：http://hz.cashguo.top/gtmuaujqnp.html

Go:   slices.Contains(arr, x)
来源：http://hz.cqqwz.cn/gtzkgttuqk.html

Ruby: arr.include?(x)
来源：http://hz.shanyushiyangkeji.top/gtnevlzedy.html

C#:   list.Contains(x)
来源：http://hz.smart0.xyz/gttwimqzzt.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yueranfly.top/gtwnzoddxs.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.zhongyouzk.top/gtextmljfc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yj20258888.top/gtysbqghts.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yvedp.cn/gtogplszyj.html

TS:   [...arr];
来源：http://hz.dianchejie.cn/gtoqdnjaxx.html

Java: new ArrayList<>(list);
来源：http://hz.yonumen.top/gtzadvprif.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.smart0.xyz/gtoygcdugw.html

Ruby: arr.dup;  arr.clone
来源：http://hz.nanxinkj.top/gtlfdgrmdp.html

C#:   new List<int>(list);
来源：http://hz.nanxuanxn.top/gtysjgecdj.html

[D23] reduce 累积计算
来源：http://hz.redwolf501.top/gtbpefjtic.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.haohaochexian.top/gtetvpvcxi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.iojbl.cn/gtywfvatib.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yj202588.top/gtphlaobdi.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jiagoushi.top/gtewpfjcob.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yueranfly.top/gtvjepglym.html

Go:   // 手写循环
来源：http://hz.yueranfly.top/gtiuswdynd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.redwolf501.top/gtrglxtpia.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.chenzaomai.com/gttmehkdol.html

[D24] 字典 / Map 基本操作
来源：http://hz.ppjwa.cn/gtdnumbnjl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.hfpthk.cn/gtiqoxwbcb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.hnqzz.top/gtqiworsbr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.feifeiyinyue.top/gtssimueez.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.xingfuxueyuan.xyz/gtikaztbkj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.feifeiyinyue.top/gtpdqdsftk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.meibo888.top/gttngaqpuc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.chenjidiqi.icu/gtttvlrnud.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.tanke756.top/gtywmwfdno.html

[D25] Set 集合去重与交并差
来源：http://hz.gaohongyu789.top/gtykqsyxos.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.snrcjt.cn/gtuohlqtit.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.iojbl.cn/gtmcyxsvsk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.9152youxi.cn/gtcnfhxhmx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.xinyue.icu/gtgdbsiesg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.hnxiangtu.top/gtjwmpwcsm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.chenzaomai.com/gtndsrlopy.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.chenzaomai.com/gtsywexmeb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.aizwys.cn/gtrfazyjgt.html

[D26] 数组转字符串
来源：http://hz.redwolf501.top/gtjjjmtotj.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zhijiandao.cn/gteswfkiei.html

PHP:  implode(", ", $arr);
来源：http://hz.jyoumei.cn/gtrazqfeic.html

JS:   arr.join(", ")
来源：http://hz.ydjk.org.cn/gttdectrlz.html

TS:   arr.join(", ")
来源：http://hz.smart0.xyz/gtepnyfdhg.html

Java: String.join(", ", list)
来源：http://hz.yj20258888.top/gtxsjhrvun.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yanxiufei.cn/gtitxbnxsw.html

Ruby: arr.join(", ")
来源：http://hz.ppjwa.cn/gtrcetsfqo.html

C#:   string.Join(", ", list)
来源：http://hz.tianlin.xyz/gtyiqrznvl.html

================================================================================
来源：http://hz.xylfe.cn/gtaojmmtks.html

E. 字符串处理
来源：http://hz.pycfn.com/gtrmlbjiut.html

================================================================================
来源：http://hz.cdnleiting.top/gtrzqkmfyy.html

[E01] 拼接字符串
来源：http://hz.cucudq.cn/gtecngwujz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.jianghu66.top/gtgiqsjmam.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.aibaodan.cn/gtdpdizyoh.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ivvv.top/gtguvgqnpj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xziqi.cn/gtgctaqpxt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.nwbrower.top/gtnophhyie.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.nanxinkj.top/gtzmbpwlwb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.gotoacloud.top/gtqgfpfmnm.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yonumen.top/gteypgruri.html

[E02] 重复字符串
来源：http://hz.feifeiyinyue.top/gtgyxauzua.html

Py:   "ab" * 3
来源：http://hz.ybcxt.top/gtjvbnuwhu.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yonumen.top/gtibgboneh.html

JS:   "ab".repeat(3)
来源：http://hz.hammf.cn/gtbqrdacpf.html

TS:   "ab".repeat(3)
来源：http://hz.ehwqpu.com/gtqwxqunrt.html

Java: "ab".repeat(3)
来源：http://hz.xuanzx.com/gtbemsokzk.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.gotoacloud.top/gtbfgxadnp.html

Ruby: "ab" * 3
来源：http://hz.andypj.xyz/gtvfgdufyz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zycfv.cn/gtodnejqaz.html

[E03] 截取子串
来源：http://hz.gzhubu.top/gtsyxjqvhi.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yangfankeji.com/gtfmhjavwr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.cashguo.top/gttdrjehwq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jianghu66.top/gteaxuqkog.html

TS:   s.slice(1, 4)
来源：http://hz.zhiwuduotai.top/gtzmtnxpqu.html

Java: s.substring(1, 4)
来源：http://hz.bjfxy.top/gtncgfhnqh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.hammf.cn/gtzhyblori.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.chenlongwang.top/gtbrkxdmgx.html

C#:   s.Substring(1, 3)
来源：http://hz.chenzaomai.com/gtrzojwyel.html

[E04] 查找子串位置
来源：http://hz.yueranfly.top/gtokpangda.html

Py:   s.find("x");  s.index("x")
来源：http://hz.snrcjt.cn/gtrpyompsa.html

PHP:  strpos($s, "x");
来源：http://hz.shanyushiyangtech.top/gtbogbrhmc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.xziqi.cn/gtadknjjtn.html

TS:   s.indexOf("x")
来源：http://hz.gogol.net.cn/gtavnbwwhy.html

Java: s.indexOf("x")
来源：http://hz.havefunace.top/gtzlvtkvcy.html


<!-- 参考信息 -->