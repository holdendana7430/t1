代发 wailian999

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.nwbrower.top/gtwxwuvnwi.html

TS:   arr.splice(0, 1);
来源：http://hz.jianghu66.top/gtvgbmyvae.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.xziqi.cn/gtpnchuqtx.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.zhoulong.xyz/gtyuapkyya.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.gogol.net.cn/gtnlmcerqb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.shanyushiyangtech.top/gtuqfxuxwd.html

[D05] 访问与修改元素
来源：http://hz.fengsongda.top/gtvzuizkvt.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.wangshuangyany.cn/gtnfzbqnba.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.guowangkeji.top/gtftskapcb.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.jqgfzy.top/gtnuqvwahi.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.shanyushiyangtech.top/gtyeubcucf.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.ydzc1.top/gtvmglodct.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.xylfe.cn/gtoiqrhomp.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yonumen.top/gtmbyjwglu.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.hfpthk.cn/gtkihetdjt.html

[D06] 数组长度
来源：http://hz.jinqigfzy.top/gtuzozcrso.html

Py:   len(arr)
来源：http://hz.cheryme.top/gtkpzogfzd.html

PHP:  count($arr);
来源：http://hz.zycfv.cn/gtpzbubzuc.html

JS:   arr.length
来源：http://hz.xylfe.cn/gtomfzkkzk.html

TS:   arr.length
来源：http://hz.jlsjyb.cn/gtvhpceklg.html

Java: list.size();
来源：http://hz.haohaochexian.top/gtrpvdvxvf.html

Go:   len(arr)
来源：http://hz.aizwys.cn/gtfmjwbsou.html

Ruby: arr.length; arr.size
来源：http://hz.hammf.cn/gtqvzpjvmd.html

C#:   list.Count;
来源：http://hz.zhiwuduotai.top/gtsdkncxyf.html

[D07] 切片 / 取子数组
来源：http://hz.jianghu66.top/gtdxpmfyji.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yueranfly.top/gtxrauhskf.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.smart0.xyz/gtgktwpwro.html

JS:   arr.slice(1, 4);
来源：http://hz.xuetiantiany.cn/gtosjthrjh.html

TS:   arr.slice(1, 4);
来源：http://hz.gaohongyu789.top/gtttjrcyyq.html

Java: list.subList(1, 4);
来源：http://hz.cqqwz.cn/gtohahckfq.html

Go:   arr[1:4]
来源：http://hz.svipenyu.cn/gtnarhjucw.html

Ruby: arr[1, 3]
来源：http://hz.xingfuxueyuan.xyz/gtutsfhses.html

C#:   list.GetRange(1, 3);
来源：http://hz.aibaodan.cn/gtwxdsigtv.html

[D08] 合并两个数组
来源：http://hz.guannengcc.top/gtohtrcmjf.html

Py:   a + b;  a.extend(b)
来源：http://hz.yueranfly.top/gtsdwitcss.html

PHP:  array_merge($a, $b);
来源：http://hz.dashuyun.cn/gtqjjwqwjs.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yanxiufei.cn/gtzlecqcav.html

TS:   [...a, ...b];
来源：http://hz.hfpthk.cn/gtgpcdfxeo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.feifeiyinyue.top/gtbqnbvpgh.html

Go:   append(a, b...)
来源：http://hz.meibo888.top/gtdqwwlorq.html

Ruby: a + b;  a.concat(b)
来源：http://hz.zycfv.cn/gtuzfhwcaz.html

C#:   a.Concat(b).ToList()
来源：http://hz.cqqwz.cn/gtnlullcot.html

[D09] 排序（升序）
来源：http://hz.yuxming.cn/gtwyrdqvbn.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.guannengcc.top/gtyffsptfc.html

PHP:  sort($arr);
来源：http://hz.wangdashe.top/gthabtrdmi.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.gaohongyu789.top/gtfvszdmob.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.fengsongda.top/gtigzvtqpi.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.haohaochexian.top/gtmeplgjvn.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.hammf.cn/gtthgzjudx.html

Ruby: arr.sort
来源：http://hz.cqqwz.cn/gtsqqbfodw.html

C#:   list.Sort();
来源：http://hz.nanxinkj.top/gthgizxwyw.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.yj20258888.top/gtrvtpmlos.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yonumen.top/gtqfyojtgh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yvedp.cn/gtpdtrfpkg.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zdqjudy.top/gtswlybxek.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhaomingkeji.xyz/gtdcymxtjp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.shanyushiyangkeji.top/gtxqujitty.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.fengsongda.top/gtvnyffdfn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.smart0.xyz/gtjrtllvqw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.nanxinkj.top/gtfjkvbxvk.html

[D11] 反转数组
来源：http://hz.sufxvd.cn/gtuymrdkvu.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.ivvv.top/gtdqjximdr.html

PHP:  array_reverse($arr);
来源：http://hz.vqdsnc.cn/gtgrtrfdoj.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jyoumei.cn/gtipgssqcp.html

TS:   [...arr].reverse();
来源：http://hz.smart0.xyz/gtrqtrzyoj.html

Java: Collections.reverse(list);
来源：http://hz.nwbrower.top/gtoeejvgmn.html

Go:   slices.Reverse(arr)
来源：http://hz.yj20258888.top/gtficdchms.html

Ruby: arr.reverse
来源：http://hz.xylfe.cn/gttwpvupkh.html

C#:   list.Reverse();
来源：http://hz.jqgufenzy.top/gtvpfsfbok.html

[D12] 查找元素下标
来源：http://hz.hongshengwenyu.top/gttywydzxd.html

Py:   arr.index(x);  x in arr
来源：http://hz.c1oappe.top/gtmvjkitpv.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.tianlin.xyz/gtqixwxmdg.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.snrcjt.cn/gtnublrkyx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.52xcode.cn/gtydfkmvti.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.xingfuxueyuan.xyz/gtrsgixrce.html

Go:   slices.Index(arr, x)
来源：http://hz.hysaishi.cn/gtnhhwxext.html

Ruby: arr.index(x)
来源：http://hz.316326.xyz/gtflqbxahq.html

C#:   list.IndexOf(x);
来源：http://hz.tian-w.cn/gtjqbyndpm.html

[D13] 过滤（保留满足条件的）
来源：http://hz.ivvv.top/gtbqczoykm.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.andypj.xyz/gtslrjecey.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.xinyue.icu/gtxhxrbyig.html

JS:   arr.filter(x => x > 3)
来源：http://hz.52xcode.cn/gtuhbzmdhp.html

TS:   arr.filter(x => x > 3)
来源：http://hz.yanxiufei.cn/gtwtohwxmu.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.zhiwuduotai.top/gthteusmaa.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.52xcode.cn/gtdventukh.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.shanyushiyangtech.top/gtthikqqel.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.hongshengwenyu.top/gthwuvlvvb.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jiagoushi.top/gtizuwlhtw.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jqgfzy.top/gtuhbllsqj.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.hfpthk.cn/gtklhdxhnx.html

JS:   arr.map(x => x * 2)
来源：http://hz.sweek.top/gttzekmuxu.html

TS:   arr.map(x => x * 2)
来源：http://hz.vqdsnc.cn/gthxnvzxdc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zhoulong.xyz/gtlhrxmtim.html

Go:   // 手写循环
来源：http://hz.zycfv.cn/gtzvannlnq.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.shangyingyoupin.top/gtlkvhyohf.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.haohaochexian.top/gtbjiedefe.html

[D15] 去重
来源：http://hz.jinghuilouyu.cn/gtgqvhudor.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.ydjk.org.cn/gtyyclhkrz.html

PHP:  array_unique($arr);
来源：http://hz.mhx1999.top/gtsfyzshld.html

JS:   [...new Set(arr)]
来源：http://hz.zhiwuduotai.top/gtrhempldt.html

TS:   [...new Set(arr)]
来源：http://hz.jinyuanbaomall.cn/gtuoayrgql.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jlsjyb.cn/gtdsojrbtw.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.meibo888.top/gtglzwfvvh.html

Ruby: arr.uniq
来源：http://hz.hfpthk.cn/gtivbvyhum.html

C#:   list.Distinct().ToList()
来源：http://hz.jianghu66.top/gtkdxxqunt.html

[D16] 求和与平均值
来源：http://hz.daria6918.cn/gtsqmgyscb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.xingfuxueyuan.xyz/gtuvjcdtrx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.xinyue.icu/gtohnfdczl.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.aibaodan.cn/gthqrkrngh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xziqi.cn/gtkgzbemmf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.52xcode.cn/gtvolpbcpn.html

Go:   // 手写循环累加
来源：http://hz.jinghuilouyu.cn/gtiuwynqid.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.nanxuanxn.top/gtorpfnzqf.html

C#:   list.Sum();  list.Average()
来源：http://hz.sweek.top/gtroczuaxs.html

[D17] 最大值与最小值
来源：http://hz.vqdsnc.cn/gtprqazvua.html

Py:   max(arr);  min(arr)
来源：http://hz.9152youxi.cn/gtlcepzors.html

PHP:  max($arr);  min($arr);
来源：http://hz.ydjk.org.cn/gtdgzxqzlv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.wangshuangyany.cn/gtxuhdmsaj.html

TS:   Math.max(...arr);
来源：http://hz.yuxming.cn/gtwxjaqtgg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.cucudq.cn/gtcrnmcpie.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.ydzc1.top/gtrjnyuyow.html

Ruby: arr.max;  arr.min
来源：http://hz.jlsjyb.cn/gttsdikmml.html

C#:   list.Max();  list.Min()
来源：http://hz.ppjwa.cn/gtbmblsefp.html

[D18] 扁平化嵌套数组
来源：http://hz.jinghuilouyu.cn/gtbmbvuhxh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.quarkkingdee.top/gtncbrkwqk.html

PHP:  array_merge(...$nested);
来源：http://hz.zdqjudy.top/gtkutwwttm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.wangdashe.top/gtfxwanylm.html

TS:   nested.flat();
来源：http://hz.yj202588.top/gtnpccjbdv.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.hnqzz.top/gtlthbtlwm.html

Go:   // 手写双层循环
来源：http://hz.zhongyouzk.top/gtknlxeguf.html

Ruby: nested.flatten
来源：http://hz.zhoulong.xyz/gtbbvkcciu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.smart0.xyz/gtzwlcydup.html

[D19] 按字段分组
来源：http://hz.chenlongwang.top/gtpixqevhi.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yuanzhike.top/gtgdtgevew.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.sxryk.cn/gtwhfwobvp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.zhixingplan.top/gtqwnugtjf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.hfpthk.cn/gtcdjjheda.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.tanke756.top/gtaqczsxvb.html

Go:   // 手写 map[string][]T
来源：http://hz.jqgfzy.top/gtcutulddi.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.tian-w.cn/gtfvypjafh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.cucudq.cn/gtnkynkqfc.html

[D20] 统计每个元素出现次数
来源：http://hz.guowangkeji.top/gteruyqbwk.html

Py:   Counter(arr)
来源：http://hz.ybcxt.top/gtvtraatne.html

PHP:  array_count_values($arr);
来源：http://hz.dianchejie.cn/gtxmbvvfxt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xuetiantiany.cn/gttxwrdxdt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.redwolf501.top/gtgohlwqsg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jianghu66.top/gtrlmqgpah.html

Go:   // 手写 map[T]int
来源：http://hz.jinyuanbaomall.cn/gtpsflgxbi.html

Ruby: arr.tally
来源：http://hz.chenlongwang.top/gtpcqmilmb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.aibaodan.cn/gtxpxgtwpr.html

[D21] 判断是否包含某元素
来源：http://hz.sxryk.cn/gtetljwgxw.html

Py:   x in arr
来源：http://hz.guowangkeji.top/gtkthpbqvu.html

PHP:  in_array($x, $arr, true);
来源：http://hz.fengsongda.top/gtfeqsiccf.html

JS:   arr.includes(x)
来源：http://hz.hysaishi.cn/gtzjfyvzaz.html

TS:   arr.includes(x)
来源：http://hz.ivvv.top/gtmhtqmfny.html

Java: list.contains(x)
来源：http://hz.xylfe.cn/gtcafqxiwf.html

Go:   slices.Contains(arr, x)
来源：http://hz.shanyushiyangtech.top/gtrdthgxhj.html

Ruby: arr.include?(x)
来源：http://hz.kuanghao11.cn/gtoddbnbts.html

C#:   list.Contains(x)
来源：http://hz.jlsjyb.cn/gtjmkpnnot.html

[D22] 复制数组（避免共享引用）
来源：http://hz.kuanghao11.cn/gtdiqcprrd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.zdqjudy.top/gtbonrquiq.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.daria6918.cn/gtidudierx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.hongshengwenyu.top/gtwkulouez.html

TS:   [...arr];
来源：http://hz.sysykeji.top/gtwqorehwf.html

Java: new ArrayList<>(list);
来源：http://hz.9152youxi.cn/gtmyxwtrtz.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.xingfuxueyuan.xyz/gtvzjifqne.html

Ruby: arr.dup;  arr.clone
来源：http://hz.redwolf501.top/gtgnhtkcbp.html

C#:   new List<int>(list);
来源：http://hz.chenlongwang.top/gtbjwninwq.html

[D23] reduce 累积计算
来源：http://hz.zdqjudy.top/gtpohnltxy.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yuxming.cn/gtsujtjxch.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.meibo888.top/gtvkgqrcwl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ydzc1.top/gtwvcxpmbu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinghuilouyu.cn/gtpgkseykq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.aibaodan.cn/gtbsaspgnq.html

Go:   // 手写循环
来源：http://hz.wangshuangyany.cn/gtjyqjeexa.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.ywan-chungtsiang.top/gtermoqqbd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.aibaodan.cn/gtcbzooohg.html

[D24] 字典 / Map 基本操作
来源：http://hz.yj20258888.top/gtwpuwujfq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.ydzc1.top/gtfqvqhaar.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yj202588.top/gtaxeyqkye.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.ehwqpu.com/gtxxrbmpsu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.jyoumei.cn/gtvprchqwq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.shangyingyoupin.top/gtslhocuvj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yanxiufei.cn/gtlvidoedb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.yongpay.top/gtuxazqvbv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yj202588.top/gtskintriu.html

[D25] Set 集合去重与交并差
来源：http://hz.jinqigfzy.top/gtibtiqjev.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.shanyushiyangkeji.top/gtuokqghyo.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.ivvv.top/gtstdaxmhi.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.gaohongyu789.top/gtrujdhlaz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jinyuanbaomall.cn/gtpkehjlex.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.zhaomingkeji.xyz/gtgxztjjbk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.xinyue.icu/gtrjcqshkf.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.sufxvd.cn/gtedkmuppm.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.0kj1m.cn/gtkkrbezwl.html

[D26] 数组转字符串
来源：http://hz.wangshuangyany.cn/gtoqgkhvua.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zhiwuduotai.top/gtkujcouhw.html

PHP:  implode(", ", $arr);
来源：http://hz.ydjk.org.cn/gtqmeehhtn.html

JS:   arr.join(", ")
来源：http://hz.snrcjt.cn/gtsubdkbgm.html

TS:   arr.join(", ")
来源：http://hz.yangfankeji.com/gtsljyfbfq.html

Java: String.join(", ", list)
来源：http://hz.zhaomingkeji.xyz/gtpyhwmltw.html

Go:   strings.Join(strs, ", ")
来源：http://hz.gaohongyu789.top/gtlqqanulw.html

Ruby: arr.join(", ")
来源：http://hz.c1oappe.top/gtlpoaomyc.html

C#:   string.Join(", ", list)
来源：http://hz.jiagoushi.top/gtqfrylefh.html

================================================================================
来源：http://hz.cucudq.cn/gtyogaowcs.html

E. 字符串处理
来源：http://hz.vqdsnc.cn/gtcqctheqh.html

================================================================================
来源：http://hz.guannengcc.top/gtqlhxpdui.html

[E01] 拼接字符串
来源：http://hz.yangfankeji.com/gtsrxoehne.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.zhengqikj.top/gtfypucuoz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.jlsjyb.cn/gtefyfnkao.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ydjk.org.cn/gtqzjbndwk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.tanke756.top/gtoqburahb.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.cashguo.top/gtdhsjsxom.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.redwolf501.top/gthsumhtly.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.cucudq.cn/gtvzshbrhk.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yj20258888.top/gtgggcpcjk.html

[E02] 重复字符串
来源：http://hz.aizwys.cn/gttetkkukj.html

Py:   "ab" * 3
来源：http://hz.dianchejie.cn/gtscirhwwd.html

PHP:  str_repeat("ab", 3);
来源：http://hz.birdmap.top/gtzymwolea.html

JS:   "ab".repeat(3)
来源：http://hz.sysykeji.top/gtezllzdri.html

TS:   "ab".repeat(3)
来源：http://hz.iojbl.cn/gtdprcphfg.html

Java: "ab".repeat(3)
来源：http://hz.cucudq.cn/gthhwifjwv.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.iojbl.cn/gtlammroxy.html

Ruby: "ab" * 3
来源：http://hz.dashuyun.cn/gtkhfwyulh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.jiagoushi.top/gtdvhreitt.html

[E03] 截取子串
来源：http://hz.jinqigfzy.top/gthhkebhnx.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.meibo888.top/gtgasmhxdi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.c1oappe.top/gtivdnzoip.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.hfpthk.cn/gtwtcbteoc.html

TS:   s.slice(1, 4)
来源：http://hz.vqdsnc.cn/gtbhbixkpq.html

Java: s.substring(1, 4)
来源：http://hz.gaohongyu789.top/gtqnogwjfj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.nwbrower.top/gtsgalpywj.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.andypj.xyz/gtggedxlkn.html

C#:   s.Substring(1, 3)
来源：http://hz.hammf.cn/gtcksijgax.html

[E04] 查找子串位置
来源：http://hz.ywan-chungtsiang.top/gtuopdzwbl.html

Py:   s.find("x");  s.index("x")
来源：http://hz.andypj.xyz/gthdyaierd.html

PHP:  strpos($s, "x");
来源：http://hz.chenlongwang.top/gtndqbcpht.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zycfv.cn/gtcevwjhbh.html

TS:   s.indexOf("x")
来源：http://hz.gaohongyu789.top/gtzuqikoej.html

Java: s.indexOf("x")
来源：http://hz.zhaomingkeji.xyz/gtypancgqv.html

Go:   strings.Index(s, "x")
来源：http://hz.zycfv.cn/gtfogustir.html

Ruby: s.index("x")
来源：http://hz.xuanzx.com/gtmglwlrtt.html

C#:   s.IndexOf("x")
来源：http://hz.iojbl.cn/gthafexsuc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.316326.xyz/gtabkziorw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.xziqi.cn/gtrmsnlcxw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.chenlongwang.top/gtwnmuuxvj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yj20258888.top/gtqofclkep.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.ivvv.top/gtbktnlzoc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.dianchejie.cn/gtdpipnyeu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.redwolf501.top/gtcokqcfnq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.316326.xyz/gtbludvild.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.shuidangran.top/gtwltddrys.html

[E06] 替换子串
来源：http://hz.316326.xyz/gtganaruqf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.daxiang520.top/gtiojhgtwg.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.316326.xyz/gtorswwzuq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.fzhhl.top/gteoynuijd.html

TS:   s.replaceAll("a", "b")
来源：http://hz.sxryk.cn/gtkftmbwby.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jqgufenzy.top/gtpaxylzfz.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.feifeiyinyue.top/gtpmsygcuo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.sxryk.cn/gtkdyxlkcg.html

C#:   s.Replace("a", "b")
来源：http://hz.yvedp.cn/gtbiuupbqc.html

[E07] 按分隔符拆分
来源：http://hz.tian-w.cn/gtggollztr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.zhiwuduotai.top/gtsvjhrybp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.dashuyun.cn/gteokojtbt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.daria6918.cn/gtuydipjoj.html

TS:   s.split(",")
来源：http://hz.dianchejie.cn/gtdtgujrhv.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.iojbl.cn/gtbritcrum.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zycfv.cn/gtlfvhpqru.html

Ruby: s.split(",");  s.split
来源：http://hz.pycfn.com/gtmqplnywg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.zycfv.cn/gtwqujmqpj.html

[E08] 数组按分隔符合并
来源：http://hz.ivvv.top/gtbzkfsaxd.html

Py:   ",".join(items)
来源：http://hz.xuanzx.com/gtwmkvvmvr.html

PHP:  implode(",", $items);
来源：http://hz.c1oappe.top/gtkvfzmfgu.html

JS:   items.join(",")
来源：http://hz.hongshengwenyu.top/gtkukgbmvd.html

TS:   items.join(",")
来源：http://hz.zhengqikj.top/gtbdjohxbu.html

Java: String.join(",", items)
来源：http://hz.pycfn.com/gtznqluxvx.html

Go:   strings.Join(items, ",")
来源：http://hz.haohaochexian.top/gtmfukzvll.html

Ruby: items.join(",")
来源：http://hz.0kj1m.cn/gtsrpchpel.html

C#:   string.Join(",", items)
来源：http://hz.yongpay.top/gthxykzdqc.html

[E09] 去除所有空白字符
来源：http://hz.gaohongyu789.top/gtxhuqylxy.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.yanxiufei.cn/gtdjcpscgs.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.meibo888.top/gtpovrfchm.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.cashguo.top/gtsdrvcadl.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.chenjidiqi.icu/gtfnggnswh.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.shanyushiyangkeji.top/gtbcdstrpn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xylfe.cn/gtujnwwmiw.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.zycfv.cn/gtzhkghsnw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.sufxvd.cn/gthrliceyd.html

[E10] 左侧补零 / 定长填充
来源：http://hz.sxryk.cn/gtsvjgalfz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.shuidangran.top/gtyooygfpx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.guannengcc.top/gtzjzxzdvg.html

JS:   "7".padStart(3, "0")
来源：http://hz.sysykeji.top/gtxbgidhux.html

TS:   "7".padStart(3, "0")
来源：http://hz.guannengcc.top/gtccqszneg.html

Java: String.format("%03d", 7)
来源：http://hz.yuanzhike.top/gtvagxpzha.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jiagoushi.top/gtgqfjpfxc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.ydzc1.top/gtmuatmlkp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.sufxvd.cn/gtyzcfopdp.html

[E11] 反转字符串
来源：http://hz.sysykeji.top/gtltsbdlmu.html

Py:   s[::-1]
来源：http://hz.cdnleiting.top/gtrwtqvavd.html

PHP:  strrev($s);
来源：http://hz.tian-w.cn/gtpjvdlbpc.html


<!-- 参考信息 -->