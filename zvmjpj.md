代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://hz.shanyushiyangkeji.top/gtzjvfqdhb.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.xuanzx.com/gtzimjiidk.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.birdmap.top/gtrzpqxajl.html

[D06] 数组长度
来源：http://hz.jinqigfzy.top/gtlkuudktk.html

Py:   len(arr)
来源：http://hz.yj20258.top/gtbbgwoffr.html

PHP:  count($arr);
来源：http://hz.nwbrower.top/gtqrtlywwk.html

JS:   arr.length
来源：http://hz.cqqwz.cn/gttofgrzoh.html

TS:   arr.length
来源：http://hz.haohaochexian.top/gtigxfigyb.html

Java: list.size();
来源：http://hz.chenzaomai.com/gttwerebzg.html

Go:   len(arr)
来源：http://hz.zhoulong.xyz/gtqqxjwvak.html

Ruby: arr.length; arr.size
来源：http://hz.shzxlz.cn/gthhdmwyuk.html

C#:   list.Count;
来源：http://hz.ydjk.org.cn/gtfcpapaqe.html

[D07] 切片 / 取子数组
来源：http://hz.dashuyun.cn/gtuwpcqvkn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.jlsjyb.cn/gttimlwqwq.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.jqgfzy.top/gtgzttzwhq.html

JS:   arr.slice(1, 4);
来源：http://hz.hongshengwenyu.top/gteccdjbiq.html

TS:   arr.slice(1, 4);
来源：http://hz.ehwqpu.com/gtoczxebnp.html

Java: list.subList(1, 4);
来源：http://hz.yuxming.cn/gtorudbiwd.html

Go:   arr[1:4]
来源：http://hz.tanke756.top/gtzttrsubn.html

Ruby: arr[1, 3]
来源：http://hz.ybcxt.top/gtozbzufhe.html

C#:   list.GetRange(1, 3);
来源：http://hz.yj20258.top/gtrvjyolxj.html

[D08] 合并两个数组
来源：http://hz.hongshengwenyu.top/gtzqbfwztx.html

Py:   a + b;  a.extend(b)
来源：http://hz.yueranfly.top/gtsqwlpuhc.html

PHP:  array_merge($a, $b);
来源：http://hz.jinqigufen.top/gtkhkyetql.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.zhiwuduotai.top/gthugjxcet.html

TS:   [...a, ...b];
来源：http://hz.dianchejie.cn/gtvnzqtvpn.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yj202588.top/gtjwpvlfoy.html

Go:   append(a, b...)
来源：http://hz.yvedp.cn/gtpqnyssuv.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yonumen.top/gtacradnou.html

C#:   a.Concat(b).ToList()
来源：http://hz.yueranfly.top/gtmeupmzia.html

[D09] 排序（升序）
来源：http://hz.jinqigufen.top/gthlvnnjkx.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.ivvv.top/gtoqkdmoij.html

PHP:  sort($arr);
来源：http://hz.yuxming.cn/gtfpivacnq.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.fzhhl.top/gtlecpwbia.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yuxming.cn/gtuddcujgt.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yuanzhike.top/gtbvmtnxpz.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yanxiufei.cn/gtujyawpwn.html

Ruby: arr.sort
来源：http://hz.smart0.xyz/gtuhjjuztt.html

C#:   list.Sort();
来源：http://hz.xinyue.icu/gtzvkxvulf.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.nwbrower.top/gtzhqjekvj.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zhijiandao.cn/gtkdfmeyap.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zhengqikj.top/gtestzzcaa.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.sxryk.cn/gtmpivgkfn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shzxlz.cn/gtvizbkyuu.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.quarkkingdee.top/gtnydjjocy.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.shanyushiyangtech.top/gtqaknsjtw.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.cucudq.cn/gtxvdcvsnf.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.xziqi.cn/gtxsggvpik.html

[D11] 反转数组
来源：http://hz.zhengqikj.top/gtvdarzaok.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.feifeiyinyue.top/gtkdywbtaa.html

PHP:  array_reverse($arr);
来源：http://hz.chenzaomai.com/gtgjzoaxzn.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.shanyushiyangkeji.top/gtmzwfgekz.html

TS:   [...arr].reverse();
来源：http://hz.yangfankeji.com/gtqeasfyip.html

Java: Collections.reverse(list);
来源：http://hz.guannengcc.top/gtjiztumvm.html

Go:   slices.Reverse(arr)
来源：http://hz.xingfuxueyuan.xyz/gtjezgvprl.html

Ruby: arr.reverse
来源：http://hz.dianchejie.cn/gtffzkosye.html

C#:   list.Reverse();
来源：http://hz.zhongyouzk.top/gtvvjjtyyn.html

[D12] 查找元素下标
来源：http://hz.pycfn.com/gtfpfstwji.html

Py:   arr.index(x);  x in arr
来源：http://hz.yj202588.top/gtekznsmul.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.feifeiyinyue.top/gtxtcdniij.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.chenzaomai.com/gtlvmlwrdb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.guowangkeji.top/gtklfttnll.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yonumen.top/gtfemnkkgc.html

Go:   slices.Index(arr, x)
来源：http://hz.cashguo.top/gtvbttftvb.html

Ruby: arr.index(x)
来源：http://hz.iojbl.cn/gtyjvdmsna.html

C#:   list.IndexOf(x);
来源：http://hz.cheryme.top/gtujthngho.html

[D13] 过滤（保留满足条件的）
来源：http://hz.quarkkingdee.top/gtsknghvrf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.havefunace.top/gtlljinidl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.wangdashe.top/gtgarcycun.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yuxming.cn/gtweecrqmv.html

TS:   arr.filter(x => x > 3)
来源：http://hz.shzxlz.cn/gtbhgjmplv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.tianlin.xyz/gtpdnknfyp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jinqigufen.top/gtstdmxvnx.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.yonumen.top/gtynetesui.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.shanyushiyangtech.top/gtppdadbjl.html

[D14] 映射转换（每个元素变形）
来源：http://hz.ppjwa.cn/gtpmxnbhew.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.shangyingyoupin.top/gtpztsxrfo.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.redwolf501.top/gthmhpgqwm.html

JS:   arr.map(x => x * 2)
来源：http://hz.gotoacloud.top/gtkusuiyrh.html

TS:   arr.map(x => x * 2)
来源：http://hz.xuanzx.com/gtftgwxriv.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.daxiang520.top/gtchoduigr.html

Go:   // 手写循环
来源：http://hz.iojbl.cn/gtfwojylli.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.haohaochexian.top/gtpletxhps.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.9152youxi.cn/gtbzvppexn.html

[D15] 去重
来源：http://hz.dianchejie.cn/gtvffhwiox.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.xylfe.cn/gttphltmug.html

PHP:  array_unique($arr);
来源：http://hz.birdmap.top/gthfqhpnjr.html

JS:   [...new Set(arr)]
来源：http://hz.hywenlv.cn/gtzcevbnvs.html

TS:   [...new Set(arr)]
来源：http://hz.jlsjyb.cn/gtgvugcftk.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yangfankeji.com/gtjexiftkb.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zhijiandao.cn/gtctzlkymc.html

Ruby: arr.uniq
来源：http://hz.vqdsnc.cn/gtwzfohshl.html

C#:   list.Distinct().ToList()
来源：http://hz.jianghu66.top/gtqsbwhnmk.html

[D16] 求和与平均值
来源：http://hz.redwolf501.top/gtldqsnkod.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yuanzhike.top/gtnlehkump.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yuxming.cn/gtyfcrxzhd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.xuanzx.com/gtzeuxmmas.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinyuanbaomall.cn/gttrvzrwyh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.ivvv.top/gtpgnhuvma.html

Go:   // 手写循环累加
来源：http://hz.cqqwz.cn/gtzdtklijg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.daxiang520.top/gthrthhdva.html

C#:   list.Sum();  list.Average()
来源：http://hz.hammf.cn/gtrxobkazv.html

[D17] 最大值与最小值
来源：http://hz.xingfuxueyuan.xyz/gtmjfnvjha.html

Py:   max(arr);  min(arr)
来源：http://hz.yangfankeji.com/gtysfgbtdk.html

PHP:  max($arr);  min($arr);
来源：http://hz.yj202588.top/gtbrssyvnb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.iojbl.cn/gtenitxlmg.html

TS:   Math.max(...arr);
来源：http://hz.ydzc1.top/gtobvsjpcy.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.xuanzx.com/gthrtjoerc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.fengsongda.top/gtryxijzto.html

Ruby: arr.max;  arr.min
来源：http://hz.gaohongyu789.top/gtmyzolafc.html

C#:   list.Max();  list.Min()
来源：http://hz.yvedp.cn/gtjoflhemp.html

[D18] 扁平化嵌套数组
来源：http://hz.cashguo.top/gtosbtaxcg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yonumen.top/gtratksvoh.html

PHP:  array_merge(...$nested);
来源：http://hz.yj202588.top/gtamyfhsyk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yvedp.cn/gtzviunkvx.html

TS:   nested.flat();
来源：http://hz.tian-w.cn/gtmwsyanfk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.jiagoushi.top/gtwjvefqkc.html

Go:   // 手写双层循环
来源：http://hz.shzxlz.cn/gtkiopfrfb.html

Ruby: nested.flatten
来源：http://hz.quarkkingdee.top/gtvxccgvet.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.hammf.cn/gtxpiowntj.html

[D19] 按字段分组
来源：http://hz.sysykeji.top/gtrevtesii.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jinqigufen.top/gtwnsdspac.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.ydzc1.top/gttweyjmyf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yj20258.top/gtcoxciuqf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.cucudq.cn/gtvmyoogcb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jinghuilouyu.cn/gtoejwtlto.html

Go:   // 手写 map[string][]T
来源：http://hz.meibo888.top/gtsqejhqrq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.pycfn.com/gtvuzhnajw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yonumen.top/gtcotxepcr.html

[D20] 统计每个元素出现次数
来源：http://hz.birdmap.top/gtsoiowade.html

Py:   Counter(arr)
来源：http://hz.xingfuxueyuan.xyz/gtjohiedem.html

PHP:  array_count_values($arr);
来源：http://hz.cucudq.cn/gtfnflfgit.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.9152youxi.cn/gtgqcdylgs.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhengqikj.top/gtpuwcpsjo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yj202588.top/gtdlfqlcga.html

Go:   // 手写 map[T]int
来源：http://hz.chenlongwang.top/gtwxystluo.html

Ruby: arr.tally
来源：http://hz.nanxinkj.top/gtkbelmcku.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.ywan-chungtsiang.top/gtqcwgpiqy.html

[D21] 判断是否包含某元素
来源：http://hz.sufxvd.cn/gtpvlfanuv.html

Py:   x in arr
来源：http://hz.pengpengdd.cyou/gthuxyooxd.html

PHP:  in_array($x, $arr, true);
来源：http://hz.ydjk.org.cn/gttszbpszy.html

JS:   arr.includes(x)
来源：http://hz.pengpengdd.cyou/gtsvaqewed.html

TS:   arr.includes(x)
来源：http://hz.cashguo.top/gtihwravcy.html

Java: list.contains(x)
来源：http://hz.smart0.xyz/gtennqsilj.html

Go:   slices.Contains(arr, x)
来源：http://hz.sweek.top/gtcydpazlc.html

Ruby: arr.include?(x)
来源：http://hz.guannengcc.top/gtrekjqikj.html

C#:   list.Contains(x)
来源：http://hz.shanyushiyangkeji.top/gtghskdatq.html

[D22] 复制数组（避免共享引用）
来源：http://hz.yj20258.top/gtpeavnbhu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yueranfly.top/gtjynqpnvj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.sxryk.cn/gtidfwbxny.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.zhengqikj.top/gtjmconlvk.html

TS:   [...arr];
来源：http://hz.yanxiufei.cn/gtuocwbilz.html

Java: new ArrayList<>(list);
来源：http://hz.52xcode.cn/gtjqfeimia.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.zhiwuduotai.top/gtvsztcgft.html

Ruby: arr.dup;  arr.clone
来源：http://hz.guannengcc.top/gtsngsbayp.html

C#:   new List<int>(list);
来源：http://hz.feifeiyinyue.top/gtpqjottkb.html

[D23] reduce 累积计算
来源：http://hz.mhx1999.top/gtvbolvlhz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jlsjyb.cn/gtkenjmzvz.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jqgufenzy.top/gtvtszwqez.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.vqdsnc.cn/gtpcsuyski.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yj202588.top/gtaevkebxl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.hfpthk.cn/gttrqksern.html

Go:   // 手写循环
来源：http://hz.xziqi.cn/gtgjxuhney.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.zdqjudy.top/gtjgusbxyg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.xinyue.icu/gtkxrduocg.html

[D24] 字典 / Map 基本操作
来源：http://hz.jinqigfzy.top/gtjeqlztiv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.tianlin.xyz/gtwzsjvrua.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.smart0.xyz/gtssevitug.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.fengsongda.top/gtbrisjxzc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.chenjidiqi.icu/gthfbmcirb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.ehwqpu.com/gtkneuoxvh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.shanyushiyangtech.top/gtpbejensn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.andypj.xyz/gtyeiqattl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.jianghu66.top/gtajpzbrpa.html

[D25] Set 集合去重与交并差
来源：http://hz.snrcjt.cn/gtspqxqeou.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.jiagoushi.top/gtnmgenbom.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.cqqwz.cn/gtuhduhhra.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.daxiang520.top/gtcnnuknfn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jinqigfzy.top/gtomrfftnk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.ydjk.org.cn/gttxqthfzc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yj20258.top/gtjydcurnc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.xingfuxueyuan.xyz/gtkfisrxyw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.chenjidiqi.icu/gtwpyxywrp.html

[D26] 数组转字符串
来源：http://hz.kuanghao11.cn/gtfkodklnf.html

Py:   ", ".join(map(str, arr))
来源：http://hz.ybcxt.top/gtsoyygitn.html

PHP:  implode(", ", $arr);
来源：http://hz.guowangkeji.top/gtaotjznvs.html

JS:   arr.join(", ")
来源：http://hz.tianlin.xyz/gtzejskvyk.html

TS:   arr.join(", ")
来源：http://hz.fzhhl.top/gtnpirctza.html

Java: String.join(", ", list)
来源：http://hz.cdnleiting.top/gttaszjvkn.html

Go:   strings.Join(strs, ", ")
来源：http://hz.hnqzz.top/gtdykbndhi.html

Ruby: arr.join(", ")
来源：http://hz.jlsjyb.cn/gtuwimwbsj.html

C#:   string.Join(", ", list)
来源：http://hz.ivvv.top/gtxnaqfnot.html

================================================================================
来源：http://hz.xingfuxueyuan.xyz/gtpkxajuta.html

E. 字符串处理
来源：http://hz.gogol.net.cn/gtiaxhldvp.html

================================================================================
来源：http://hz.snrcjt.cn/gttilfpxwz.html

[E01] 拼接字符串
来源：http://hz.havefunace.top/gtsqjzpket.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.chenjidiqi.icu/gtakcrmfik.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.jyoumei.cn/gtlokafrvf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xylfe.cn/gtsjwvuzft.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ydzc1.top/gtcllibhlf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.cucudq.cn/gtlpjuekwg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yonumen.top/gtkvamhnse.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.nanxuanxn.top/gtbuiammio.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.daria6918.cn/gtcduiqsns.html

[E02] 重复字符串
来源：http://hz.nanxinkj.top/gtbfdkhvyy.html

Py:   "ab" * 3
来源：http://hz.shangyingyoupin.top/gtcmxurmru.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yuxming.cn/gtpylagmfo.html

JS:   "ab".repeat(3)
来源：http://hz.mhx1999.top/gtmeluyswh.html

TS:   "ab".repeat(3)
来源：http://hz.shanyushiyangkeji.top/gtzjuvugoc.html

Java: "ab".repeat(3)
来源：http://hz.hywenlv.cn/gttuhnwwem.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jianghu66.top/gtsshqvoce.html

Ruby: "ab" * 3
来源：http://hz.sufxvd.cn/gtoxkhethv.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.chenlongwang.top/gtivmrguzy.html

[E03] 截取子串
来源：http://hz.ydjk.org.cn/gtzhmraovc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.fengsongda.top/gtsjsfrccm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.fengsongda.top/gtaiozjsfh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.hysaishi.cn/gtewbsjmvb.html

TS:   s.slice(1, 4)
来源：http://hz.haohaochexian.top/gtfwnjgunr.html

Java: s.substring(1, 4)
来源：http://hz.xinyue.icu/gtsrtfcdhp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.andypj.xyz/gtzajpzyuc.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.ydzc1.top/gtfcexmemn.html

C#:   s.Substring(1, 3)
来源：http://hz.chenjidiqi.icu/gtdbqsmdax.html

[E04] 查找子串位置
来源：http://hz.zhongyouzk.top/gtsptvgmws.html

Py:   s.find("x");  s.index("x")
来源：http://hz.dashuyun.cn/gtydwlwefb.html

PHP:  strpos($s, "x");
来源：http://hz.iojbl.cn/gtszegrgxp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.jqgfzy.top/gtdrheknlh.html

TS:   s.indexOf("x")
来源：http://hz.hfpthk.cn/gtncxvqqzp.html

Java: s.indexOf("x")
来源：http://hz.shanyushiyangkeji.top/gtgvggqpsk.html

Go:   strings.Index(s, "x")
来源：http://hz.jiagoushi.top/gtpwtdxplz.html

Ruby: s.index("x")
来源：http://hz.pycfn.com/gthhogvggr.html

C#:   s.IndexOf("x")
来源：http://hz.chenlongwang.top/gtqsuhtxaq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.zhengqikj.top/gteyyvqtnj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zycfv.cn/gtlrsicbom.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.shangyingyoupin.top/gtgxshgfwg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.haohaochexian.top/gtvcyeiyfh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.dashuyun.cn/gtqhtqptzg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jqgufenzy.top/gtqhhbkalx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.yj20258.top/gtrgjnmhcr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.pengpengdd.cyou/gtylzsmmfo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.aibaodan.cn/gtgeswxwoc.html

[E06] 替换子串
来源：http://hz.yvedp.cn/gtwkezztvu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.tian-w.cn/gtplefddqi.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.xuanzx.com/gtejezyaeu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.havefunace.top/gtuuhikcxh.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zhoulong.xyz/gtddcwbfqb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.bjfxy.top/gtmjonmpak.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.cheryme.top/gtlqsoidjm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.yj20258.top/gtiawqjpzu.html

C#:   s.Replace("a", "b")
来源：http://hz.zhongyouzk.top/gtecsdcggu.html

[E07] 按分隔符拆分
来源：http://hz.hysaishi.cn/gtiafywpcd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.sysykeji.top/gtjwvclqzp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.tianlin.xyz/gtidhwajxc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.jlsjyb.cn/gtldmxngfn.html

TS:   s.split(",")
来源：http://hz.bjfxy.top/gtgbtgtteb.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.jqgfzy.top/gtfrodniuj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.cqqwz.cn/gtewnyaqld.html

Ruby: s.split(",");  s.split
来源：http://hz.ppjwa.cn/gtlyrkxxpt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.jiagoushi.top/gtdvqpggzw.html

[E08] 数组按分隔符合并
来源：http://hz.yanxiufei.cn/gtklizoima.html

Py:   ",".join(items)
来源：http://hz.shzxlz.cn/gttqxlmbwf.html

PHP:  implode(",", $items);
来源：http://hz.snrcjt.cn/gtzamsusuy.html

JS:   items.join(",")
来源：http://hz.daxiang520.top/gtegntxkdf.html

TS:   items.join(",")
来源：http://hz.xinyue.icu/gtdwwtzuff.html

Java: String.join(",", items)
来源：http://hz.ybcxt.top/gthrduvehk.html

Go:   strings.Join(items, ",")
来源：http://hz.hfpthk.cn/gtrfolozww.html

Ruby: items.join(",")
来源：http://hz.ydjk.org.cn/gtdqvponqi.html

C#:   string.Join(",", items)
来源：http://hz.snrcjt.cn/gtjuztkobh.html

[E09] 去除所有空白字符
来源：http://hz.ydjk.org.cn/gtbmingblw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.dianchejie.cn/gtazsgnmah.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.hnqzz.top/gtqvzktktg.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jianghu66.top/gtxubvhcef.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zhiwuduotai.top/gtirbmallx.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.xziqi.cn/gtnlnbnngv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.svipenyu.cn/gtzontimaf.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.aizwys.cn/gtlcroeafz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jyoumei.cn/gtqjgnhgib.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zhijiandao.cn/gtfmaomfcm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zhixingplan.top/gtjbbuefef.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.hfpthk.cn/gtspnoldlt.html

JS:   "7".padStart(3, "0")
来源：http://hz.fzhhl.top/gtaepywkjr.html

TS:   "7".padStart(3, "0")
来源：http://hz.52xcode.cn/gtzmoshpmf.html

Java: String.format("%03d", 7)
来源：http://hz.xuanzx.com/gtomhkrcdw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.chenlongwang.top/gtzwccntsy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.gzhubu.top/gtsxqijppn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.cqqwz.cn/gtimulfoui.html

[E11] 反转字符串
来源：http://hz.havefunace.top/gtzohyttik.html

Py:   s[::-1]
来源：http://hz.haohaochexian.top/gtdhrivsyf.html

PHP:  strrev($s);
来源：http://hz.c1oappe.top/gtpynrkowu.html

JS:   [...s].reverse().join("")
来源：http://hz.xuanzx.com/gtcgvnfkzj.html

TS:   [...s].reverse().join("")
来源：http://hz.yj20258888.top/gthhbysryt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yonumen.top/gtajguworv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.ydzc1.top/gtgztwgqin.html

Ruby: s.reverse
来源：http://hz.daxiang520.top/gtssvayjxw.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.sxryk.cn/gtugaskdii.html

[E12] 统计某字符出现次数
来源：http://hz.cashguo.top/gtwtccpmnc.html

Py:   s.count("a")
来源：http://hz.jinqigufen.top/gteanintmq.html

PHP:  substr_count($s, "a");
来源：http://hz.ywan-chungtsiang.top/gtllqlsnmf.html

JS:   s.split("a").length - 1
来源：http://hz.yuxming.cn/gttrjumyjz.html

TS:   s.split("a").length - 1
来源：http://hz.chenjidiqi.icu/gtpukkkaqi.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.dianchejie.cn/gtzegjxwol.html


<!-- 参考信息 -->