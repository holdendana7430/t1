代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.hysaishi.cn/gtmmldhmys.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.zhixingplan.top/gtebqtbces.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.zhiwuduotai.top/gtarvforqz.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.hfpthk.cn/gthmimsfwu.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.shuidangran.top/gtmovidnzb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.aizwys.cn/gtibqmzhzo.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jinqigfzy.top/gtqfhztyoz.html

[D06] 数组长度
来源：http://hz.quarkkingdee.top/gtxdojjzwb.html

Py:   len(arr)
来源：http://hz.nanxuanxn.top/gtqdxjqhvr.html

PHP:  count($arr);
来源：http://hz.yuxming.cn/gtlqdmjmsh.html

JS:   arr.length
来源：http://hz.iojbl.cn/gtwerungsr.html

TS:   arr.length
来源：http://hz.fzhhl.top/gtwxtmghtd.html

Java: list.size();
来源：http://hz.hnxiangtu.top/gthzmafibt.html

Go:   len(arr)
来源：http://hz.chenzaomai.com/gtsdybcyli.html

Ruby: arr.length; arr.size
来源：http://hz.cheryme.top/gtyemjfqzq.html

C#:   list.Count;
来源：http://hz.aizwys.cn/gtemraaxpd.html

[D07] 切片 / 取子数组
来源：http://hz.hammf.cn/gtlekzutgj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.52xcode.cn/gtwoglofjh.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.c1oappe.top/gtvbgoflhp.html

JS:   arr.slice(1, 4);
来源：http://hz.cucudq.cn/gtnfngxzix.html

TS:   arr.slice(1, 4);
来源：http://hz.dianchejie.cn/gtwbqkadoe.html

Java: list.subList(1, 4);
来源：http://hz.tian-w.cn/gtsvcqofmj.html

Go:   arr[1:4]
来源：http://hz.gotoacloud.top/gtcywcawfb.html

Ruby: arr[1, 3]
来源：http://hz.aibaodan.cn/gtjlhsuwfo.html

C#:   list.GetRange(1, 3);
来源：http://hz.yongpay.top/gtamzjarsf.html

[D08] 合并两个数组
来源：http://hz.nanxinkj.top/gturararxl.html

Py:   a + b;  a.extend(b)
来源：http://hz.shzxlz.cn/gtmabbiriz.html

PHP:  array_merge($a, $b);
来源：http://hz.nwbrower.top/gtxfkxrxjg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.fengsongda.top/gtthxtulma.html

TS:   [...a, ...b];
来源：http://hz.ydjk.org.cn/gtezdfqcow.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yangfankeji.com/gtsoyoyxkp.html

Go:   append(a, b...)
来源：http://hz.aizwys.cn/gtwelvtlre.html

Ruby: a + b;  a.concat(b)
来源：http://hz.chenzaomai.com/gtalekycfx.html

C#:   a.Concat(b).ToList()
来源：http://hz.316326.xyz/gtnmsyypzp.html

[D09] 排序（升序）
来源：http://hz.nanxuanxn.top/gtpxdoffoz.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gogol.net.cn/gtuojajsxh.html

PHP:  sort($arr);
来源：http://hz.yj202588.top/gteqjxfpcm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.pycfn.com/gtxazeiusw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.mhx1999.top/gtfhlcclba.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.shangyingyoupin.top/gtiivyymxp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yj20258.top/gtlkfibxjx.html

Ruby: arr.sort
来源：http://hz.daria6918.cn/gtzyrtqrzz.html

C#:   list.Sort();
来源：http://hz.jiagoushi.top/gtkuzbsqln.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.sxryk.cn/gtwpzjbhub.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.ppjwa.cn/gtakhqjpst.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.tanke756.top/gtlgixwhlh.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.pycfn.com/gtxdygyuaq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ppjwa.cn/gtfmwgvcne.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yj202588.top/gtvqdfxowc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.zdqjudy.top/gtgouhmyso.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.kuanghao11.cn/gtmcfhhrzs.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.daxiang520.top/gtazcuzhkt.html

[D11] 反转数组
来源：http://hz.jlsjyb.cn/gtsxxnbwpi.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.sysykeji.top/gtsookbtoh.html

PHP:  array_reverse($arr);
来源：http://hz.cucudq.cn/gtsocmsjth.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.daria6918.cn/gtlhijigwj.html

TS:   [...arr].reverse();
来源：http://hz.shanyushiyangkeji.top/gtmguscvrz.html

Java: Collections.reverse(list);
来源：http://hz.jinqigfzy.top/gtqdijvsxt.html

Go:   slices.Reverse(arr)
来源：http://hz.nwbrower.top/gtvxwhboca.html

Ruby: arr.reverse
来源：http://hz.ydzc1.top/gtoetnjplm.html

C#:   list.Reverse();
来源：http://hz.zycfv.cn/gteujezszt.html

[D12] 查找元素下标
来源：http://hz.gaohongyu789.top/gtbpqgevky.html

Py:   arr.index(x);  x in arr
来源：http://hz.yanxiufei.cn/gtrjxcezhc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.zhixingplan.top/gtaqozvxha.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shzxlz.cn/gtzagtymwl.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yj20258888.top/gtsxetlmvl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.9152youxi.cn/gtivlanodp.html

Go:   slices.Index(arr, x)
来源：http://hz.svipenyu.cn/gtnzwlmvzk.html

Ruby: arr.index(x)
来源：http://hz.9152youxi.cn/gtljkjnice.html

C#:   list.IndexOf(x);
来源：http://hz.shanyushiyangkeji.top/gttwlarukk.html

[D13] 过滤（保留满足条件的）
来源：http://hz.sysykeji.top/gtagwwajdh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.cdnleiting.top/gtbkfzgnio.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.zhongyouzk.top/gtvshekrzd.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hywenlv.cn/gtfbnhhuvd.html

TS:   arr.filter(x => x > 3)
来源：http://hz.guannengcc.top/gtsavipmbb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.sufxvd.cn/gtxkuwkpzk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.cqqwz.cn/gtvfabydxa.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.9152youxi.cn/gturfufxsr.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.snrcjt.cn/gtqcglpbhr.html

[D14] 映射转换（每个元素变形）
来源：http://hz.hysaishi.cn/gttblcgidu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ydzc1.top/gtdohmlrqa.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.chenjidiqi.icu/gtvficxhtx.html

JS:   arr.map(x => x * 2)
来源：http://hz.hysaishi.cn/gtzbmmsbdj.html

TS:   arr.map(x => x * 2)
来源：http://hz.52xcode.cn/gtkwkqplkx.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.shanyushiyangtech.top/gtoqkaqlmh.html

Go:   // 手写循环
来源：http://hz.chenjidiqi.icu/gtvoeaonek.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.shzxlz.cn/gtunsaymnm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.ivvv.top/gtsnkksscu.html

[D15] 去重
来源：http://hz.gaohongyu789.top/gtlrpibolb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yuxming.cn/gtrfmonaif.html

PHP:  array_unique($arr);
来源：http://hz.feifeiyinyue.top/gtbmfywlwh.html

JS:   [...new Set(arr)]
来源：http://hz.yueranfly.top/gtwdjzifgt.html

TS:   [...new Set(arr)]
来源：http://hz.hnqzz.top/gtvddlcwyx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.chenjidiqi.icu/gtdjqsbhed.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.hnqzz.top/gtlrjwztdr.html

Ruby: arr.uniq
来源：http://hz.jiagoushi.top/gtrmdeavbt.html

C#:   list.Distinct().ToList()
来源：http://hz.cashguo.top/gtbkfddymb.html

[D16] 求和与平均值
来源：http://hz.hammf.cn/gtdagubqeo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.xinyue.icu/gtjwebsadr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.hywenlv.cn/gtvqqrznsy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.snrcjt.cn/gtflrpmofc.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.52xcode.cn/gtzqktfyoa.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.zhiwuduotai.top/gtewpqryxm.html

Go:   // 手写循环累加
来源：http://hz.gaohongyu789.top/gtwvzqagus.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.nanxuanxn.top/gtqznhwegm.html

C#:   list.Sum();  list.Average()
来源：http://hz.shangyingyoupin.top/gtfxcuhsel.html

[D17] 最大值与最小值
来源：http://hz.jiagoushi.top/gtdfqdfkww.html

Py:   max(arr);  min(arr)
来源：http://hz.guowangkeji.top/gtcjqcfzdr.html

PHP:  max($arr);  min($arr);
来源：http://hz.haohaochexian.top/gtfkvdhkkr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.ivvv.top/gtdectontt.html

TS:   Math.max(...arr);
来源：http://hz.birdmap.top/gtirpdrxvo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.316326.xyz/gtvnpfrupy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.cdnleiting.top/gtuzoptgqh.html

Ruby: arr.max;  arr.min
来源：http://hz.316326.xyz/gthrrackpg.html

C#:   list.Max();  list.Min()
来源：http://hz.gotoacloud.top/gtnwfmpoms.html

[D18] 扁平化嵌套数组
来源：http://hz.kuanghao11.cn/gtmuqlljkc.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.xinyue.icu/gtctxjobxu.html

PHP:  array_merge(...$nested);
来源：http://hz.zhijiandao.cn/gtabihsbui.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.sweek.top/gtcrbxamvy.html

TS:   nested.flat();
来源：http://hz.shangyingyoupin.top/gtlcpgiyfd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.shangyingyoupin.top/gticijfisk.html

Go:   // 手写双层循环
来源：http://hz.tian-w.cn/gtgzctcamr.html

Ruby: nested.flatten
来源：http://hz.xinyue.icu/gtavzsxcrk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.gotoacloud.top/gtpfbqyslm.html

[D19] 按字段分组
来源：http://hz.cqqwz.cn/gtqwwhmtcv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.fzhhl.top/gtlygbkdfn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.dashuyun.cn/gtghnapidj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.xziqi.cn/gtubebancd.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.yanxiufei.cn/gtzczqstgf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jlsjyb.cn/gtakfroame.html

Go:   // 手写 map[string][]T
来源：http://hz.yvedp.cn/gtlwywuffi.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.jinyuanbaomall.cn/gtwjgnreef.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.sufxvd.cn/gtbxcqicxl.html

[D20] 统计每个元素出现次数
来源：http://hz.jinqigfzy.top/gtpsccaldx.html

Py:   Counter(arr)
来源：http://hz.yuanzhike.top/gtuncyirap.html

PHP:  array_count_values($arr);
来源：http://hz.ybcxt.top/gtqvwzkguv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hnqzz.top/gtpaduiklg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xinyue.icu/gtrfbjqhze.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.cdnleiting.top/gtmbtvmizz.html

Go:   // 手写 map[T]int
来源：http://hz.chenzaomai.com/gtcjthoixp.html

Ruby: arr.tally
来源：http://hz.316326.xyz/gtiaeazvvs.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.gotoacloud.top/gtondtjgqi.html

[D21] 判断是否包含某元素
来源：http://hz.pycfn.com/gthtfuqphi.html

Py:   x in arr
来源：http://hz.jinyuanbaomall.cn/gtttwwggbl.html

PHP:  in_array($x, $arr, true);
来源：http://hz.wangdashe.top/gtkluvssym.html

JS:   arr.includes(x)
来源：http://hz.yuxming.cn/gtebghlame.html

TS:   arr.includes(x)
来源：http://hz.daria6918.cn/gttfxkfdmg.html

Java: list.contains(x)
来源：http://hz.cucudq.cn/gtvfdujpjw.html

Go:   slices.Contains(arr, x)
来源：http://hz.jqgufenzy.top/gtfnfsuzrd.html

Ruby: arr.include?(x)
来源：http://hz.shanyushiyangtech.top/gtxufqoxod.html

C#:   list.Contains(x)
来源：http://hz.haohaochexian.top/gtuerrqcdu.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yvedp.cn/gtxnvvssbi.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yj20258.top/gtdjwwopwk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.wangshuangyany.cn/gtjruwlfow.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yueranfly.top/gtdsnxtrmt.html

TS:   [...arr];
来源：http://hz.jinqigfzy.top/gtmwtgawba.html

Java: new ArrayList<>(list);
来源：http://hz.hysaishi.cn/gtomwmszfd.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yuxming.cn/gtoeqxhxtt.html

Ruby: arr.dup;  arr.clone
来源：http://hz.feifeiyinyue.top/gtyyizqbdy.html

C#:   new List<int>(list);
来源：http://hz.kuanghao11.cn/gtpzomigjx.html

[D23] reduce 累积计算
来源：http://hz.kuanghao11.cn/gtafqlgjqf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.c1oappe.top/gtjmxwaqhu.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yj20258888.top/gtfueegbkx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.iojbl.cn/gtsffceyiv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zdqjudy.top/gthccngzeq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.dashuyun.cn/gtfqvxaryk.html

Go:   // 手写循环
来源：http://hz.tianlin.xyz/gtfwgumohd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.hysaishi.cn/gtgfougoxw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.svipenyu.cn/gttanalqnf.html

[D24] 字典 / Map 基本操作
来源：http://hz.pengpengdd.cyou/gtakqdxqna.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.aibaodan.cn/gtiqlprxgw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.havefunace.top/gtbidawfok.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.9152youxi.cn/gtuxnqfoij.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.9152youxi.cn/gtnfcthnsm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.chenzaomai.com/gtceuoqdxe.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yvedp.cn/gtwhuolrlg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.sweek.top/gtxpysdtdt.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.meibo888.top/gtnuwhkcph.html

[D25] Set 集合去重与交并差
来源：http://hz.wangshuangyany.cn/gtbgxollta.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.guowangkeji.top/gtyxkbubmx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.gaohongyu789.top/gtfaeniukx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.haohaochexian.top/gtvcdbjsbf.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.zhixingplan.top/gtodyvsmdh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.ywan-chungtsiang.top/gtrtcgcwqp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.pycfn.com/gtvtgakjrn.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.sxryk.cn/gtgppaiwlr.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yj20258.top/gteveqzdqo.html

[D26] 数组转字符串
来源：http://hz.jinqigfzy.top/gtgkzwdcsc.html

Py:   ", ".join(map(str, arr))
来源：http://hz.hysaishi.cn/gtwiquahku.html

PHP:  implode(", ", $arr);
来源：http://hz.sysykeji.top/gtzvevyebt.html

JS:   arr.join(", ")
来源：http://hz.fengsongda.top/gtiijrebun.html

TS:   arr.join(", ")
来源：http://hz.iojbl.cn/gtvjgopuyr.html

Java: String.join(", ", list)
来源：http://hz.52xcode.cn/gthwqzbrcz.html

Go:   strings.Join(strs, ", ")
来源：http://hz.feifeiyinyue.top/gtlgwuvnnp.html

Ruby: arr.join(", ")
来源：http://hz.bjfxy.top/gtucmhzcyg.html

C#:   string.Join(", ", list)
来源：http://hz.jyoumei.cn/gtfdwkliue.html

================================================================================
来源：http://hz.xziqi.cn/gtlcpekqaq.html

E. 字符串处理
来源：http://hz.gaohongyu789.top/gtdvcrifrv.html

================================================================================
来源：http://hz.birdmap.top/gthtqfukto.html

[E01] 拼接字符串
来源：http://hz.hywenlv.cn/gtcxqaqoql.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.gaohongyu789.top/gttqwrmxfj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yuanzhike.top/gtxgitnpyg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.yongpay.top/gtgzgwinfq.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.bjfxy.top/gtrzvvsoqr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.pengpengdd.cyou/gtelrevkon.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.sufxvd.cn/gtezdlwgdy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jinghuilouyu.cn/gtagtmiivg.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.shzxlz.cn/gtiyawksng.html

[E02] 重复字符串
来源：http://hz.shzxlz.cn/gtlqtlpmqb.html

Py:   "ab" * 3
来源：http://hz.meibo888.top/gthmzftwwe.html

PHP:  str_repeat("ab", 3);
来源：http://hz.nwbrower.top/gtvhxpqaqq.html

JS:   "ab".repeat(3)
来源：http://hz.redwolf501.top/gthkolprid.html

TS:   "ab".repeat(3)
来源：http://hz.xingfuxueyuan.xyz/gtoiiqpmlq.html

Java: "ab".repeat(3)
来源：http://hz.jyoumei.cn/gtedpfvchi.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zhixingplan.top/gthokflcct.html

Ruby: "ab" * 3
来源：http://hz.shzxlz.cn/gtnufqssbk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.ehwqpu.com/gtfygnegny.html

[E03] 截取子串
来源：http://hz.birdmap.top/gtouhnanhs.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.aibaodan.cn/gtjdhkiewd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.dashuyun.cn/gtyvpdcuey.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.cheryme.top/gtauqlfrnb.html

TS:   s.slice(1, 4)
来源：http://hz.mhx1999.top/gtcbnaithz.html

Java: s.substring(1, 4)
来源：http://hz.wangshuangyany.cn/gtacxpzxto.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.jinyuanbaomall.cn/gtjrnfxpmk.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.snrcjt.cn/gtajxjsvbt.html

C#:   s.Substring(1, 3)
来源：http://hz.yj202588.top/gtxlmgxdsy.html

[E04] 查找子串位置
来源：http://hz.cheryme.top/gtctgnjnma.html

Py:   s.find("x");  s.index("x")
来源：http://hz.yangfankeji.com/gteotpnejq.html

PHP:  strpos($s, "x");
来源：http://hz.kuanghao11.cn/gtpzdhwfat.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.sysykeji.top/gtlfnnlyxh.html

TS:   s.indexOf("x")
来源：http://hz.yj202588.top/gtatzrlpib.html

Java: s.indexOf("x")
来源：http://hz.snrcjt.cn/gtpvacjllj.html

Go:   strings.Index(s, "x")
来源：http://hz.xziqi.cn/gtxcvmwtol.html

Ruby: s.index("x")
来源：http://hz.yongpay.top/gtnebqpgln.html

C#:   s.IndexOf("x")
来源：http://hz.snrcjt.cn/gtquzxbmmy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.xziqi.cn/gteklbdjdy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.guowangkeji.top/gtjmuqxizn.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.gaohongyu789.top/gtoonthesa.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jinqigufen.top/gtfhlwnztz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zhiwuduotai.top/gtbmdlxbzc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hysaishi.cn/gtwrzhccbb.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.nwbrower.top/gtwabbrqjr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.zycfv.cn/gttxkyhcej.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.cqqwz.cn/gthwgeiwjz.html

[E06] 替换子串
来源：http://hz.tian-w.cn/gtvolanopk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.cqqwz.cn/gteuscihuj.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.yueranfly.top/gtahhogdlz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.guowangkeji.top/gtvzgdnllo.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jinqigfzy.top/gtmelcrjtj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yueranfly.top/gtjirlgigz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.quarkkingdee.top/gtkmcphskx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.chenjidiqi.icu/gtnlkpmzgw.html

C#:   s.Replace("a", "b")
来源：http://hz.daria6918.cn/gtcfuraubk.html

[E07] 按分隔符拆分
来源：http://hz.zhijiandao.cn/gtkfvuvoks.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.cashguo.top/gtlivjoske.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.meibo888.top/gttfgoueqf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.jinghuilouyu.cn/gtpbudqqjh.html

TS:   s.split(",")
来源：http://hz.jqgufenzy.top/gtxceqcsgt.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.gaohongyu789.top/gtyljiwusq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zycfv.cn/gtkrpkjfsd.html

Ruby: s.split(",");  s.split
来源：http://hz.yanxiufei.cn/gtfprpwxer.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.zhaomingkeji.xyz/gtdmvcxmms.html

[E08] 数组按分隔符合并
来源：http://hz.iojbl.cn/gtvuyzlvto.html

Py:   ",".join(items)
来源：http://hz.xuanzx.com/gtfhngatqr.html

PHP:  implode(",", $items);
来源：http://hz.tanke756.top/gtxlqwtgcz.html

JS:   items.join(",")
来源：http://hz.birdmap.top/gtqhllchjk.html

TS:   items.join(",")
来源：http://hz.zdqjudy.top/gtbulzicpv.html

Java: String.join(",", items)
来源：http://hz.sysykeji.top/gtdiogkzkk.html

Go:   strings.Join(items, ",")
来源：http://hz.birdmap.top/gtklezfnti.html

Ruby: items.join(",")
来源：http://hz.nanxuanxn.top/gtrzybytsx.html

C#:   string.Join(",", items)
来源：http://hz.shzxlz.cn/gtvegeackn.html

[E09] 去除所有空白字符
来源：http://hz.xylfe.cn/gtlkloyqvh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.birdmap.top/gtcmmtvmqv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.nwbrower.top/gtawjhyjow.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.chenlongwang.top/gtvdzzbgzn.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.shanyushiyangkeji.top/gtfgjhicuk.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.9152youxi.cn/gthndrwdka.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.hnxiangtu.top/gtvlfomjhn.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.wangdashe.top/gtusyfexrh.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.xuanzx.com/gtbfsomyas.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zycfv.cn/gtgklgksks.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.fengsongda.top/gtolufagoe.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.vqdsnc.cn/gtjlpizkzl.html

JS:   "7".padStart(3, "0")
来源：http://hz.shzxlz.cn/gtrrfwropv.html

TS:   "7".padStart(3, "0")
来源：http://hz.yangfankeji.com/gtujrowkyb.html

Java: String.format("%03d", 7)
来源：http://hz.yj20258888.top/gtjugnuqeg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.sufxvd.cn/gtbvmuzyjr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.pengpengdd.cyou/gtyoqipoos.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.guowangkeji.top/gtguvgwxab.html

[E11] 反转字符串
来源：http://hz.xingfuxueyuan.xyz/gttvtexkui.html

Py:   s[::-1]
来源：http://hz.shanyushiyangtech.top/gtjynknqis.html

PHP:  strrev($s);
来源：http://hz.yj20258888.top/gtydjztexs.html

JS:   [...s].reverse().join("")
来源：http://hz.jinghuilouyu.cn/gtqwrjhklz.html

TS:   [...s].reverse().join("")
来源：http://hz.ybcxt.top/gtnkdskfyi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jianghu66.top/gtbacvqqck.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.dashuyun.cn/gthbbryzbt.html

Ruby: s.reverse
来源：http://hz.guowangkeji.top/gtrafbidle.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.snrcjt.cn/gtmsjdvwxf.html

[E12] 统计某字符出现次数
来源：http://hz.zhijiandao.cn/gtuzfymagi.html

Py:   s.count("a")
来源：http://hz.snrcjt.cn/gtwnfmdufg.html


<!-- 参考信息 -->