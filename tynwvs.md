代发 wailian999

[C14] 泛型函数
来源：http://hz.0kj1m.cn/gtbvrnlblq.html

Py:   from typing import TypeVar; T = TypeVar("T"); def first(items: list[T]) -> T: ...
来源：http://hz.shanyushiyangkeji.top/gtksmlpzpd.html

PHP:  // 无泛型
来源：http://hz.andypj.xyz/gtbjouprte.html

JS:   // 无泛型
来源：http://hz.tian-w.cn/gtsiovworq.html

TS:   function first<T>(items: T[]): T | undefined { return items[0]; }
来源：http://hz.hongshengwenyu.top/gtdtazizoa.html

Java: static <T> T first(List<T> items) { return items.get(0); }
来源：http://hz.snrcjt.cn/gteezbrlqz.html

Go:   func First[T any](items []T) T { return items[0] }
来源：http://hz.yj20258.top/gtjybwxwhl.html

Ruby: # 无泛型
来源：http://hz.shangyingyoupin.top/gtfeahcsph.html

C#:   static T First<T>(List<T> items) => items[0];
来源：http://hz.zhengqikj.top/gtdnmmekca.html

[C15] 解构 / 展开参数
来源：http://hz.svipenyu.cn/gtmcjamlgl.html

Py:   def f(a, b): ...;  f(*[1, 2]);  f(**{"a": 1, "b": 2})
来源：http://hz.gotoacloud.top/gtmaecaqel.html

PHP:  [$a, $b] = $pair;
来源：http://hz.jyoumei.cn/gtgcrwzxfi.html

JS:   const { a, b } = obj;  function f({ a, b }) {}
来源：http://hz.yvedp.cn/gtqqaeqody.html

TS:   function f({ a, b }: { a: number; b: number }) {}
来源：http://hz.zhijiandao.cn/gtqdmenkzp.html

Java: // 无解构
来源：http://hz.9152youxi.cn/gtswagmwuo.html

Go:   // 无解构
来源：http://hz.hfpthk.cn/gtvarlvtdx.html

Ruby: a, b = pair
来源：http://hz.ydzc1.top/gtdjvsvakq.html

C#:   var (a, b) = pair;
来源：http://hz.xylfe.cn/gtsnuibbtv.html

[C16] 函数 / 方法重载
来源：http://hz.chenjidiqi.icu/gtowwsohoe.html

Py:   # 无重载：用默认参数或 *args 变通
来源：http://hz.havefunace.top/gtjuxzmwgw.html

PHP:  // 无重载
来源：http://hz.ywan-chungtsiang.top/gtoiugehvx.html

JS:   // 无重载：靠 arguments.length 分支
来源：http://hz.hnqzz.top/gtnunobkyv.html

TS:   // 用联合类型或重载签名声明
来源：http://hz.pycfn.com/gtvceypduj.html

Java: void f(int a) {}  void f(String a) {}
来源：http://hz.cucudq.cn/gtvlogdqwe.html

Go:   // 无重载：用不同函数名
来源：http://hz.yvedp.cn/gtttxvgkgt.html

Ruby: # 无重载：靠动态参数
来源：http://hz.xuanzx.com/gtxvehozin.html

C#:   void F(int a) {}  void F(string a) {}
来源：http://hz.gaohongyu789.top/gtnuwuprmj.html

================================================================================
来源：http://hz.zycfv.cn/gteheqgsfy.html

D. 数组 / 列表 / 集合
来源：http://hz.shzxlz.cn/gtiovvpuke.html

================================================================================
来源：http://hz.tanke756.top/gtyvaituor.html

[D01] 创建数组 / 列表
来源：http://hz.dashuyun.cn/gtzmqlwnfn.html

Py:   arr = [1, 2, 3];  empty = []
来源：http://hz.jinqigfzy.top/gtwllbofqp.html

PHP:  $arr = [1, 2, 3];  $empty = [];
来源：http://hz.xuetiantiany.cn/gtkgnytmjp.html

JS:   const arr = [1, 2, 3];  const empty = [];
来源：http://hz.tanke756.top/gtvljlbqry.html

TS:   const arr: number[] = [1, 2, 3];
来源：http://hz.cashguo.top/gtdzhvnsts.html

Java: var arr = new int[]{1, 2, 3};  var list = new ArrayList<>(List.of(1, 2, 3));
来源：http://hz.aibaodan.cn/gtbzlhotae.html

Go:   arr := []int{1, 2, 3}
来源：http://hz.ehwqpu.com/gtlnqcacnd.html

Ruby: arr = [1, 2, 3]
来源：http://hz.0kj1m.cn/gtutghhgfu.html

C#:   var arr = new[] { 1, 2, 3 };  var list = new List<int> { 1, 2, 3 };
来源：http://hz.ivvv.top/gtaumxustt.html

[D02] 追加元素到末尾
来源：http://hz.dashuyun.cn/gtbfkcxgvu.html

Py:   arr.append(4); arr.extend([5, 6])
来源：http://hz.sweek.top/gtlvbitqpx.html

PHP:  $arr[] = 4; array_push($arr, 5);
来源：http://hz.jianghu66.top/gtxapquxkz.html

JS:   arr.push(4);
来源：http://hz.yueranfly.top/gtaskqahyr.html

TS:   arr.push(4);
来源：http://hz.wangdashe.top/gtjexlsgjg.html

Java: list.add(4);
来源：http://hz.yj20258888.top/gtgxdhimtc.html

Go:   arr = append(arr, 4)
来源：http://hz.havefunace.top/gtjkrnahwl.html

Ruby: arr << 4; arr.push(5)
来源：http://hz.jqgfzy.top/gtogldiufn.html

C#:   list.Add(4);
来源：http://hz.hfpthk.cn/gtxfpnisst.html

[D03] 在指定位置插入元素
来源：http://hz.snrcjt.cn/gtdoqibgny.html

Py:   arr.insert(0, 0)
来源：http://hz.andypj.xyz/gtxhzipknj.html

PHP:  array_splice($arr, 0, 0, [0]);
来源：http://hz.jqgufenzy.top/gtewbjetyt.html

JS:   arr.splice(0, 0, 0);  arr.unshift(0)   // 插到头部
来源：http://hz.iojbl.cn/gtdrfdllqa.html

TS:   arr.splice(0, 0, 0);
来源：http://hz.hfpthk.cn/gtsyervmci.html

Java: list.add(0, 0);
来源：http://hz.ivvv.top/gthwhdlluc.html

Go:   arr = append([]int{0}, arr...)
来源：http://hz.yueranfly.top/gtwipqtvwp.html

Ruby: arr.insert(0, 0); arr.unshift(0)
来源：http://hz.aizwys.cn/gtgtfckjxs.html

C#:   list.Insert(0, 0);
来源：http://hz.sufxvd.cn/gtmqcfjiig.html

[D04] 删除元素
来源：http://hz.haohaochexian.top/gtpnsjfuee.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.daxiang520.top/gtquhnlxxu.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.fengsongda.top/gtjegbjzjh.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.zycfv.cn/gtwcvfllmk.html

TS:   arr.splice(0, 1);
来源：http://hz.gaohongyu789.top/gtyvfqloct.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.nanxuanxn.top/gtxvcmitom.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.c1oappe.top/gtohwrkiwy.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.xylfe.cn/gtpjyqvhpe.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.yj20258888.top/gtzfinreps.html

[D05] 访问与修改元素
来源：http://hz.chenlongwang.top/gtgpjdpwop.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.andypj.xyz/gtjrkioiik.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.sxryk.cn/gtpowgiuiw.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.kuanghao11.cn/gtlsxpuqgi.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.ppjwa.cn/gtigitnvhh.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.9152youxi.cn/gtpugjipnl.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.cucudq.cn/gtwhevfedq.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.aibaodan.cn/gtqwmdsxyc.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.aibaodan.cn/gtyigdkzex.html

[D06] 数组长度
来源：http://hz.yj202588.top/gtwvsywmfs.html

Py:   len(arr)
来源：http://hz.52xcode.cn/gtmiqlcmpm.html

PHP:  count($arr);
来源：http://hz.chenzaomai.com/gtlvjbhitm.html

JS:   arr.length
来源：http://hz.jinqigufen.top/gtrnkousdh.html

TS:   arr.length
来源：http://hz.ydjk.org.cn/gtanonlvht.html

Java: list.size();
来源：http://hz.daxiang520.top/gtecriecdy.html

Go:   len(arr)
来源：http://hz.fzhhl.top/gtpyuxpetz.html

Ruby: arr.length; arr.size
来源：http://hz.cdnleiting.top/gtyengfznf.html

C#:   list.Count;
来源：http://hz.jiagoushi.top/gtwprmcnyk.html

[D07] 切片 / 取子数组
来源：http://hz.svipenyu.cn/gtgmxdmnpv.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.hysaishi.cn/gttoshavdj.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.ywan-chungtsiang.top/gteglhgoet.html

JS:   arr.slice(1, 4);
来源：http://hz.jqgufenzy.top/gtgajwqhbr.html

TS:   arr.slice(1, 4);
来源：http://hz.zhijiandao.cn/gtkoimhdom.html

Java: list.subList(1, 4);
来源：http://hz.xuanzx.com/gthewxxjli.html

Go:   arr[1:4]
来源：http://hz.tanke756.top/gtghtfkryj.html

Ruby: arr[1, 3]
来源：http://hz.vqdsnc.cn/gtjemudqdx.html

C#:   list.GetRange(1, 3);
来源：http://hz.svipenyu.cn/gtmtdeoqtv.html

[D08] 合并两个数组
来源：http://hz.hfpthk.cn/gtbmdgxpgr.html

Py:   a + b;  a.extend(b)
来源：http://hz.ywan-chungtsiang.top/gtuawvumld.html

PHP:  array_merge($a, $b);
来源：http://hz.aibaodan.cn/gtelzykrpx.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.tian-w.cn/gtghikqxfi.html

TS:   [...a, ...b];
来源：http://hz.fzhhl.top/gttokpsldj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.ydzc1.top/gthyewymvz.html

Go:   append(a, b...)
来源：http://hz.cucudq.cn/gtberzpcvn.html

Ruby: a + b;  a.concat(b)
来源：http://hz.birdmap.top/gtfypfoymr.html

C#:   a.Concat(b).ToList()
来源：http://hz.gzhubu.top/gtqpjjbsin.html

[D09] 排序（升序）
来源：http://hz.birdmap.top/gteeonixgp.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cdnleiting.top/gtpuxmoymb.html

PHP:  sort($arr);
来源：http://hz.bjfxy.top/gtvgzvhmbx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.jqgfzy.top/gtxmxdfpdp.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yuanzhike.top/gtuwhkzons.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yvedp.cn/gtfrcrqnlq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.birdmap.top/gtgurcfxra.html

Ruby: arr.sort
来源：http://hz.yonumen.top/gtozhtbfns.html

C#:   list.Sort();
来源：http://hz.zhijiandao.cn/gtvozurflx.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jqgfzy.top/gthmccmmoi.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.gogol.net.cn/gtswzepodd.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.daria6918.cn/gtwojossmv.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.andypj.xyz/gtkddlalpg.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ivvv.top/gtcjybdpor.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.tanke756.top/gttcnunmii.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.mhx1999.top/gtsqfrokgj.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.9152youxi.cn/gtikitjhst.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.ehwqpu.com/gtgititfif.html

[D11] 反转数组
来源：http://hz.yj20258888.top/gtdfcghate.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.snrcjt.cn/gtdlkrnxjh.html

PHP:  array_reverse($arr);
来源：http://hz.yuxming.cn/gtixwlgapu.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.ppjwa.cn/gthoykwzwc.html

TS:   [...arr].reverse();
来源：http://hz.shanyushiyangtech.top/gtgjnbhgzc.html

Java: Collections.reverse(list);
来源：http://hz.yuxming.cn/gttjnmzpgr.html

Go:   slices.Reverse(arr)
来源：http://hz.tian-w.cn/gtrkborxby.html

Ruby: arr.reverse
来源：http://hz.birdmap.top/gtcxvsvpzj.html

C#:   list.Reverse();
来源：http://hz.aibaodan.cn/gtwmrzidkr.html

[D12] 查找元素下标
来源：http://hz.guowangkeji.top/gtccwlxlur.html

Py:   arr.index(x);  x in arr
来源：http://hz.hongshengwenyu.top/gtfmnpkciu.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.fengsongda.top/gtaisnpyar.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinyuanbaomall.cn/gtmloqxkvb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jinqigufen.top/gtvrcemtbz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.iojbl.cn/gtaxeckszq.html

Go:   slices.Index(arr, x)
来源：http://hz.zhengqikj.top/gtxwyhqujg.html

Ruby: arr.index(x)
来源：http://hz.cheryme.top/gtnwcadhpn.html

C#:   list.IndexOf(x);
来源：http://hz.cheryme.top/gtfkpbeimf.html

[D13] 过滤（保留满足条件的）
来源：http://hz.hfpthk.cn/gtnzqmzehf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.gotoacloud.top/gtzblsjepu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.sweek.top/gttdcpjyzb.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hfpthk.cn/gtevnbohkp.html

TS:   arr.filter(x => x > 3)
来源：http://hz.shzxlz.cn/gtiiixrlct.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.9152youxi.cn/gtclbxbkzj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.snrcjt.cn/gtaicntznl.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.tian-w.cn/gtroijtbpr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jqgufenzy.top/gtgtbmrrom.html

[D14] 映射转换（每个元素变形）
来源：http://hz.vqdsnc.cn/gtbziczjum.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ivvv.top/gtnhcjosur.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.andypj.xyz/gtqivsocux.html

JS:   arr.map(x => x * 2)
来源：http://hz.jianghu66.top/gtnrhpeldd.html

TS:   arr.map(x => x * 2)
来源：http://hz.0kj1m.cn/gttfiudivz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jqgufenzy.top/gtovwncrzr.html

Go:   // 手写循环
来源：http://hz.zhijiandao.cn/gtxasltxlb.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.sxryk.cn/gtspinrmyb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.nanxinkj.top/gtwavcmwzy.html

[D15] 去重
来源：http://hz.shzxlz.cn/gtalncksml.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.iojbl.cn/gtvkirmdrn.html

PHP:  array_unique($arr);
来源：http://hz.yuanzhike.top/gtasetqjnt.html

JS:   [...new Set(arr)]
来源：http://hz.aizwys.cn/gtehvrvmen.html

TS:   [...new Set(arr)]
来源：http://hz.pycfn.com/gthxeoqskb.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.nanxuanxn.top/gtxddfcrxi.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.shanyushiyangtech.top/gteiaxrndk.html

Ruby: arr.uniq
来源：http://hz.zhoulong.xyz/gtjzuxpjba.html

C#:   list.Distinct().ToList()
来源：http://hz.hnxiangtu.top/gtipzneful.html

[D16] 求和与平均值
来源：http://hz.wangdashe.top/gtyshzhiwy.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.ppjwa.cn/gtdozqlkrc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.zhengqikj.top/gtruxarzru.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xingfuxueyuan.xyz/gtmuooatxx.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jiagoushi.top/gtakhxtruz.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.nanxinkj.top/gtszvrdeac.html

Go:   // 手写循环累加
来源：http://hz.feifeiyinyue.top/gtwmxbffza.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yanxiufei.cn/gtwpevelff.html

C#:   list.Sum();  list.Average()
来源：http://hz.mhx1999.top/gtzvuwxsar.html

[D17] 最大值与最小值
来源：http://hz.hfpthk.cn/gtohszphto.html

Py:   max(arr);  min(arr)
来源：http://hz.gotoacloud.top/gtgiwghfcs.html

PHP:  max($arr);  min($arr);
来源：http://hz.yvedp.cn/gtrkdscmha.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.pengpengdd.cyou/gtcgfffqcb.html

TS:   Math.max(...arr);
来源：http://hz.bjfxy.top/gtoevdytkm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.nanxuanxn.top/gttukksnoc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yonumen.top/gtextjfnpr.html

Ruby: arr.max;  arr.min
来源：http://hz.xuanzx.com/gtvfdlghrr.html

C#:   list.Max();  list.Min()
来源：http://hz.gzhubu.top/gtgsvpnoew.html

[D18] 扁平化嵌套数组
来源：http://hz.zhoulong.xyz/gtcyfjhyhk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.sufxvd.cn/gtwcaepuyx.html

PHP:  array_merge(...$nested);
来源：http://hz.yuanzhike.top/gthlxmzeww.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.quarkkingdee.top/gtxosxerax.html

TS:   nested.flat();
来源：http://hz.sxryk.cn/gtpfsahusk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.pycfn.com/gtelafqdpl.html

Go:   // 手写双层循环
来源：http://hz.snrcjt.cn/gtlqmaizab.html

Ruby: nested.flatten
来源：http://hz.mhx1999.top/gtrszaamua.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zhaomingkeji.xyz/gtyyosymsz.html

[D19] 按字段分组
来源：http://hz.shanyushiyangtech.top/gtwhsbgxbt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jyoumei.cn/gtyjkbtpca.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.nanxuanxn.top/gtikfrhufx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.vqdsnc.cn/gtrxudrngm.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jyoumei.cn/gthzctxree.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.tianlin.xyz/gtxhbwdhql.html

Go:   // 手写 map[string][]T
来源：http://hz.ybcxt.top/gtmsqfkqrj.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.dianchejie.cn/gtjgbnciqf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.hfpthk.cn/gtzyghvtmn.html

[D20] 统计每个元素出现次数
来源：http://hz.cucudq.cn/gtkzynjtwj.html

Py:   Counter(arr)
来源：http://hz.yueranfly.top/gthsmcwzsu.html

PHP:  array_count_values($arr);
来源：http://hz.daxiang520.top/gtlqphftrt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhaomingkeji.xyz/gtdmxzthsp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhengqikj.top/gtlfrostfr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.zhixingplan.top/gtgidvwzpy.html

Go:   // 手写 map[T]int
来源：http://hz.yanxiufei.cn/gterzvyipf.html

Ruby: arr.tally
来源：http://hz.zhoulong.xyz/gtxaphxcgx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.chenlongwang.top/gtqyiashvo.html

[D21] 判断是否包含某元素
来源：http://hz.0kj1m.cn/gtqykgkbnk.html

Py:   x in arr
来源：http://hz.yonumen.top/gtlhodjufc.html

PHP:  in_array($x, $arr, true);
来源：http://hz.hongshengwenyu.top/gtawfuyqbg.html

JS:   arr.includes(x)
来源：http://hz.shanyushiyangkeji.top/gtprtwnazb.html

TS:   arr.includes(x)
来源：http://hz.ydjk.org.cn/gtfdyuobiw.html

Java: list.contains(x)
来源：http://hz.zhongyouzk.top/gtvhahbwho.html

Go:   slices.Contains(arr, x)
来源：http://hz.jinqigufen.top/gtluxalhza.html

Ruby: arr.include?(x)
来源：http://hz.yanxiufei.cn/gtsgobvipm.html

C#:   list.Contains(x)
来源：http://hz.zhixingplan.top/gtosohlisg.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jinqigufen.top/gtctgwnqmb.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.gzhubu.top/gtturxrfzy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.redwolf501.top/gtobamfivu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yj20258888.top/gthwqcekbr.html

TS:   [...arr];
来源：http://hz.mhx1999.top/gtquxegfud.html

Java: new ArrayList<>(list);
来源：http://hz.cucudq.cn/gtctidxdxu.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.mhx1999.top/gtmjbfxiyt.html

Ruby: arr.dup;  arr.clone
来源：http://hz.316326.xyz/gtoygbecct.html

C#:   new List<int>(list);
来源：http://hz.hongshengwenyu.top/gtajexpuvj.html

[D23] reduce 累积计算
来源：http://hz.hfpthk.cn/gtglrzypyn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.zhixingplan.top/gtrbsjqdjw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.hywenlv.cn/gtyayvgrad.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinqigufen.top/gtbgdmjzkd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hysaishi.cn/gtjlwrqbbw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yj20258888.top/gttduftife.html

Go:   // 手写循环
来源：http://hz.hongshengwenyu.top/gteuejjpqr.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.gaohongyu789.top/gtueabmena.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.nwbrower.top/gttzoustgc.html

[D24] 字典 / Map 基本操作
来源：http://hz.guannengcc.top/gtipmxtbky.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yj20258.top/gtanhcasmk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.chenlongwang.top/gtnvfhfqbl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jinqigufen.top/gtsjefcyld.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yongpay.top/gtlaxkpouy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.zhaomingkeji.xyz/gtostfkycx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jyoumei.cn/gtjgqfzcvf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.nanxinkj.top/gtdekuaglo.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jianghu66.top/gtiadmxwti.html

[D25] Set 集合去重与交并差
来源：http://hz.9152youxi.cn/gtkmpyhjra.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yj20258.top/gtdrtvuxng.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.shangyingyoupin.top/gtiqekvhny.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.jlsjyb.cn/gtksoarfcf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.vqdsnc.cn/gtqplouzke.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.ydzc1.top/gtravkigzy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.shanyushiyangkeji.top/gtbowduotx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.zhiwuduotai.top/gtxswpihvb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.hammf.cn/gtkfbylzzf.html

[D26] 数组转字符串
来源：http://hz.ehwqpu.com/gtlfigaqvc.html

Py:   ", ".join(map(str, arr))
来源：http://hz.hywenlv.cn/gtddjlnsjr.html

PHP:  implode(", ", $arr);
来源：http://hz.fengsongda.top/gtcbddqanc.html

JS:   arr.join(", ")
来源：http://hz.aizwys.cn/gtpodownbv.html

TS:   arr.join(", ")
来源：http://hz.gzhubu.top/gtsvwjrfuf.html

Java: String.join(", ", list)
来源：http://hz.sweek.top/gtqcifdyrp.html

Go:   strings.Join(strs, ", ")
来源：http://hz.hywenlv.cn/gtopcmnfof.html

Ruby: arr.join(", ")
来源：http://hz.jlsjyb.cn/gtmuygjnmo.html

C#:   string.Join(", ", list)
来源：http://hz.ehwqpu.com/gtxagtqkmf.html

================================================================================
来源：http://hz.hnxiangtu.top/gtnudskdbn.html

E. 字符串处理
来源：http://hz.xziqi.cn/gtddxrpdew.html

================================================================================
来源：http://hz.zycfv.cn/gtihhgkeck.html

[E01] 拼接字符串
来源：http://hz.wangdashe.top/gtbwxmjsqh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.gotoacloud.top/gtfgkcsaxg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.jqgufenzy.top/gtvpukpsum.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.nwbrower.top/gtabvfqhbb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ydjk.org.cn/gtnqeicdcj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.nanxuanxn.top/gthcttfacb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.fzhhl.top/gtrfbuxfqc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.cucudq.cn/gtdmpdntnn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.xziqi.cn/gtmeiihezd.html

[E02] 重复字符串
来源：http://hz.hammf.cn/gtxcnqvgvt.html

Py:   "ab" * 3
来源：http://hz.jinyuanbaomall.cn/gteglzpnhw.html

PHP:  str_repeat("ab", 3);
来源：http://hz.ehwqpu.com/gtymqgncky.html

JS:   "ab".repeat(3)
来源：http://hz.sufxvd.cn/gtnhhgbtrl.html

TS:   "ab".repeat(3)
来源：http://hz.fzhhl.top/gtzfakxvbv.html

Java: "ab".repeat(3)
来源：http://hz.hammf.cn/gtmsbqagwc.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.daria6918.cn/gtazysvzps.html

Ruby: "ab" * 3
来源：http://hz.nanxinkj.top/gtzqggqans.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.pycfn.com/gtgiqorvix.html

[E03] 截取子串
来源：http://hz.kuanghao11.cn/gtudcvpxxb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yonumen.top/gtjvawuubd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.hongshengwenyu.top/gtjspgiaax.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.zdqjudy.top/gtbcmlfmvo.html

TS:   s.slice(1, 4)
来源：http://hz.shuidangran.top/gtbzglgbsn.html

Java: s.substring(1, 4)
来源：http://hz.meibo888.top/gthgpqkihb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.zhoulong.xyz/gteobogdky.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.xylfe.cn/gtptodutkn.html

C#:   s.Substring(1, 3)
来源：http://hz.dianchejie.cn/gtfymzkbdb.html

[E04] 查找子串位置
来源：http://hz.hfpthk.cn/gtquqqlury.html

Py:   s.find("x");  s.index("x")
来源：http://hz.snrcjt.cn/gtejegnqzz.html

PHP:  strpos($s, "x");
来源：http://hz.c1oappe.top/gtstckkdko.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.bjfxy.top/gtlecvrcab.html

TS:   s.indexOf("x")
来源：http://hz.jlsjyb.cn/gtuzkgfryb.html

Java: s.indexOf("x")
来源：http://hz.havefunace.top/gtouzwnjky.html


<!-- 参考信息 -->