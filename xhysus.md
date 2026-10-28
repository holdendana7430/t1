代发 wailian999

Java: list.size();
来源：http://hz.jqgfzy.top/gtapifqtdr.html

Go:   len(arr)
来源：http://hz.0kj1m.cn/gtlrawwkjf.html

Ruby: arr.length; arr.size
来源：http://hz.yuanzhike.top/gtxqygoolf.html

C#:   list.Count;
来源：http://hz.gogol.net.cn/gtskhmjkvz.html

[D07] 切片 / 取子数组
来源：http://hz.aibaodan.cn/gtlatkvagy.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zycfv.cn/gtippexnuq.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.nanxinkj.top/gtvbiwyoyr.html

JS:   arr.slice(1, 4);
来源：http://hz.gaohongyu789.top/gtbrskmlwi.html

TS:   arr.slice(1, 4);
来源：http://hz.zhaomingkeji.xyz/gtnytkcbcz.html

Java: list.subList(1, 4);
来源：http://hz.hongshengwenyu.top/gtssphhric.html

Go:   arr[1:4]
来源：http://hz.316326.xyz/gtawdinurp.html

Ruby: arr[1, 3]
来源：http://hz.ppjwa.cn/gthgkdbmyv.html

C#:   list.GetRange(1, 3);
来源：http://hz.shuidangran.top/gtnrxtxvti.html

[D08] 合并两个数组
来源：http://hz.yonumen.top/gthohtuwno.html

Py:   a + b;  a.extend(b)
来源：http://hz.316326.xyz/gtgfonrfoi.html

PHP:  array_merge($a, $b);
来源：http://hz.sxryk.cn/gtazwtstli.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.cdnleiting.top/gtdnbgunbo.html

TS:   [...a, ...b];
来源：http://hz.daxiang520.top/gtzmwufpuv.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.svipenyu.cn/gtrbkcynym.html

Go:   append(a, b...)
来源：http://hz.cdnleiting.top/gtsagbzjgq.html

Ruby: a + b;  a.concat(b)
来源：http://hz.ehwqpu.com/gtrcarzshs.html

C#:   a.Concat(b).ToList()
来源：http://hz.hammf.cn/gtmtdmpqkw.html

[D09] 排序（升序）
来源：http://hz.sxryk.cn/gtctaahbfp.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xingfuxueyuan.xyz/gtbcufaxym.html

PHP:  sort($arr);
来源：http://hz.jinyuanbaomall.cn/gtttgksszt.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hnxiangtu.top/gtxpmopxxq.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zdqjudy.top/gtckgextuj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.hysaishi.cn/gtkczxqdmw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.jiagoushi.top/gtogyofyjl.html

Ruby: arr.sort
来源：http://hz.jyoumei.cn/gtkadbmsca.html

C#:   list.Sort();
来源：http://hz.ybcxt.top/gtmjpwksig.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.sufxvd.cn/gtqluggxev.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.cheryme.top/gtrnopkqvg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.wangdashe.top/gtejkudknc.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.nwbrower.top/gtlczhlwxz.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cucudq.cn/gtpliglftz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.kuanghao11.cn/gtksxyjssm.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.shangyingyoupin.top/gthwkiyhlu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.316326.xyz/gtmghirwen.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.ppjwa.cn/gtjjhllboy.html

[D11] 反转数组
来源：http://hz.sxryk.cn/gtswzynbqb.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.pengpengdd.cyou/gtuujdjxcy.html

PHP:  array_reverse($arr);
来源：http://hz.yueranfly.top/gtwnugyler.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.shuidangran.top/gtboaffccd.html

TS:   [...arr].reverse();
来源：http://hz.yanxiufei.cn/gtghgejnfl.html

Java: Collections.reverse(list);
来源：http://hz.yj20258888.top/gtyycqxhdl.html

Go:   slices.Reverse(arr)
来源：http://hz.daria6918.cn/gtpuuhkhci.html

Ruby: arr.reverse
来源：http://hz.xingfuxueyuan.xyz/gttppsjtql.html

C#:   list.Reverse();
来源：http://hz.cucudq.cn/gtceuuyngm.html

[D12] 查找元素下标
来源：http://hz.fzhhl.top/gtxwkhprzg.html

Py:   arr.index(x);  x in arr
来源：http://hz.sufxvd.cn/gtovipadcs.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.xziqi.cn/gtgppgityf.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.tian-w.cn/gtibbdgahw.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.jqgfzy.top/gtvmzlncrz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.9152youxi.cn/gtkgexcwnu.html

Go:   slices.Index(arr, x)
来源：http://hz.sysykeji.top/gtovbzwdmr.html

Ruby: arr.index(x)
来源：http://hz.xingfuxueyuan.xyz/gtekgqwmbk.html

C#:   list.IndexOf(x);
来源：http://hz.zhongyouzk.top/gtmknvjmty.html

[D13] 过滤（保留满足条件的）
来源：http://hz.c1oappe.top/gtjgpmwgbg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.vqdsnc.cn/gtufrwlkqv.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yj20258.top/gtskraobkn.html

JS:   arr.filter(x => x > 3)
来源：http://hz.guannengcc.top/gtmyfpgmnv.html

TS:   arr.filter(x => x > 3)
来源：http://hz.hongshengwenyu.top/gtleiuxtvi.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jlsjyb.cn/gthdasqcdo.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.ydjk.org.cn/gtfrjvmnwh.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.jyoumei.cn/gteicowqto.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.0kj1m.cn/gtrvrjzehy.html

[D14] 映射转换（每个元素变形）
来源：http://hz.dianchejie.cn/gtiypxumra.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yangfankeji.com/gtfsgijwhk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.jinyuanbaomall.cn/gtdoqiijba.html

JS:   arr.map(x => x * 2)
来源：http://hz.andypj.xyz/gtxfhtjhow.html

TS:   arr.map(x => x * 2)
来源：http://hz.meibo888.top/gtsiypenzq.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yj202588.top/gtcfpywias.html

Go:   // 手写循环
来源：http://hz.ywan-chungtsiang.top/gtxneuefss.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.guannengcc.top/gtkzdenvem.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zycfv.cn/gtiadfftmj.html

[D15] 去重
来源：http://hz.chenlongwang.top/gttecnvyng.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yonumen.top/gtaxuyekih.html

PHP:  array_unique($arr);
来源：http://hz.ydzc1.top/gtqckhocjj.html

JS:   [...new Set(arr)]
来源：http://hz.yuxming.cn/gtttiuufsr.html

TS:   [...new Set(arr)]
来源：http://hz.zhoulong.xyz/gtxusxjtaf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.xuetiantiany.cn/gtleqbobmz.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.shzxlz.cn/gtgsvosmtx.html

Ruby: arr.uniq
来源：http://hz.hammf.cn/gtirupovua.html

C#:   list.Distinct().ToList()
来源：http://hz.cucudq.cn/gtlokswany.html

[D16] 求和与平均值
来源：http://hz.jinqigfzy.top/gtnlmcpztf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.meibo888.top/gtsuspywma.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.gotoacloud.top/gtprashrfz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hammf.cn/gtrafsybpd.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ppjwa.cn/gtqmngefui.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.cashguo.top/gttsuakymz.html

Go:   // 手写循环累加
来源：http://hz.gogol.net.cn/gtfjybeggt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhaomingkeji.xyz/gtomslwedx.html

C#:   list.Sum();  list.Average()
来源：http://hz.zhengqikj.top/gtnlumdmrx.html

[D17] 最大值与最小值
来源：http://hz.quarkkingdee.top/gtomvaoixz.html

Py:   max(arr);  min(arr)
来源：http://hz.yangfankeji.com/gtvppefrlk.html

PHP:  max($arr);  min($arr);
来源：http://hz.nanxuanxn.top/gtmetnclab.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zhixingplan.top/gtwbzlqdzr.html

TS:   Math.max(...arr);
来源：http://hz.xinyue.icu/gtvtkqvryq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.pycfn.com/gtqwypowsh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jiagoushi.top/gtqzryllue.html

Ruby: arr.max;  arr.min
来源：http://hz.yj202588.top/gtngjgnywf.html

C#:   list.Max();  list.Min()
来源：http://hz.pengpengdd.cyou/gtfqqwhowt.html

[D18] 扁平化嵌套数组
来源：http://hz.yuanzhike.top/gtmgnlninb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.shuidangran.top/gtuddqsaau.html

PHP:  array_merge(...$nested);
来源：http://hz.zhoulong.xyz/gtrwndhfbc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.hnxiangtu.top/gtgkpgbgqn.html

TS:   nested.flat();
来源：http://hz.zhoulong.xyz/gtbdtwpcgt.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.gogol.net.cn/gtgznpnwam.html

Go:   // 手写双层循环
来源：http://hz.ywan-chungtsiang.top/gtstjfrepd.html

Ruby: nested.flatten
来源：http://hz.shzxlz.cn/gtxfrdrkkn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.ydzc1.top/gtrfcbkbgc.html

[D19] 按字段分组
来源：http://hz.yangfankeji.com/gtpsxjmcqh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.zycfv.cn/gtxxjtbqkn.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.316326.xyz/gtcnweyycb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.316326.xyz/gtljoewrov.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.zhixingplan.top/gtmupundtl.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.c1oappe.top/gtsewjbpun.html

Go:   // 手写 map[string][]T
来源：http://hz.chenjidiqi.icu/gtwpyzbypt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.fengsongda.top/gtfdsatmox.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.hfpthk.cn/gtmwaejgrv.html

[D20] 统计每个元素出现次数
来源：http://hz.cucudq.cn/gtlsunlych.html

Py:   Counter(arr)
来源：http://hz.zhongyouzk.top/gtaichthjk.html

PHP:  array_count_values($arr);
来源：http://hz.meibo888.top/gthjkuxhqw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.0kj1m.cn/gtdsskgabw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hysaishi.cn/gtyajxvxiv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.sweek.top/gtgpfnlkvz.html

Go:   // 手写 map[T]int
来源：http://hz.cashguo.top/gtqfxcnhnw.html

Ruby: arr.tally
来源：http://hz.yangfankeji.com/gtdelcxqzr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.meibo888.top/gtkzcpnbiy.html

[D21] 判断是否包含某元素
来源：http://hz.jinqigfzy.top/gtlkxclgaa.html

Py:   x in arr
来源：http://hz.jyoumei.cn/gtrjxnxnrx.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yangfankeji.com/gtzgtfobuq.html

JS:   arr.includes(x)
来源：http://hz.tian-w.cn/gtorciurqc.html

TS:   arr.includes(x)
来源：http://hz.ywan-chungtsiang.top/gtfzsnvbwq.html

Java: list.contains(x)
来源：http://hz.meibo888.top/gtuqnbzowk.html

Go:   slices.Contains(arr, x)
来源：http://hz.yj20258888.top/gtfdejjyvv.html

Ruby: arr.include?(x)
来源：http://hz.guannengcc.top/gtcephurvj.html

C#:   list.Contains(x)
来源：http://hz.zhiwuduotai.top/gtjzlomwbi.html

[D22] 复制数组（避免共享引用）
来源：http://hz.cdnleiting.top/gtvfcnjbtt.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jinqigfzy.top/gtrzkywoxu.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.snrcjt.cn/gtxycyacak.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.hammf.cn/gtiktzowji.html

TS:   [...arr];
来源：http://hz.316326.xyz/gtmaefnupy.html

Java: new ArrayList<>(list);
来源：http://hz.xinyue.icu/gtazvuusep.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.zycfv.cn/gtzbithudo.html

Ruby: arr.dup;  arr.clone
来源：http://hz.chenzaomai.com/gtatdgnrvo.html

C#:   new List<int>(list);
来源：http://hz.shangyingyoupin.top/gtyknxgmma.html

[D23] reduce 累积计算
来源：http://hz.shanyushiyangkeji.top/gtrjonlawk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.tianlin.xyz/gtflfdllej.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.hnxiangtu.top/gtwywnoyyd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hywenlv.cn/gtfshejegg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jlsjyb.cn/gtfngprgzn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.9152youxi.cn/gtaeqybjif.html

Go:   // 手写循环
来源：http://hz.aibaodan.cn/gtgrlwgzte.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.ivvv.top/gtagaqtemx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.daxiang520.top/gtdtydnyzq.html

[D24] 字典 / Map 基本操作
来源：http://hz.aibaodan.cn/gtjjbzptvv.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yj20258.top/gtioxzlfem.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.9152youxi.cn/gtszgbhoyy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.xylfe.cn/gtvqnuwrab.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.jinqigfzy.top/gtyamalaij.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jqgfzy.top/gtdjxammcz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.daria6918.cn/gtrjdfsdej.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.shanyushiyangtech.top/gtiopjyycw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zhengqikj.top/gtjrzpnvze.html

[D25] Set 集合去重与交并差
来源：http://hz.jqgfzy.top/gtzhevjrhe.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.cdnleiting.top/gtlalrkzgt.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jinqigfzy.top/gtpeovxgqt.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.hfpthk.cn/gtvnsvmfxl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.dashuyun.cn/gteyctegwu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.havefunace.top/gtyocozkej.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.daria6918.cn/gtfeyjmbvk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.pengpengdd.cyou/gtlxrhoaiu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jinqigufen.top/gtgmtngesd.html

[D26] 数组转字符串
来源：http://hz.yueranfly.top/gtnzlrtvgr.html

Py:   ", ".join(map(str, arr))
来源：http://hz.ivvv.top/gtpkqpvlss.html

PHP:  implode(", ", $arr);
来源：http://hz.cashguo.top/gtibznzfwf.html

JS:   arr.join(", ")
来源：http://hz.zycfv.cn/gtvfuwpljs.html

TS:   arr.join(", ")
来源：http://hz.yuxming.cn/gtbuagovny.html

Java: String.join(", ", list)
来源：http://hz.hysaishi.cn/gtekievwyo.html

Go:   strings.Join(strs, ", ")
来源：http://hz.pengpengdd.cyou/gtkuuelguk.html

Ruby: arr.join(", ")
来源：http://hz.shanyushiyangkeji.top/gtqhoqgrpj.html

C#:   string.Join(", ", list)
来源：http://hz.wangshuangyany.cn/gttiayirvt.html

================================================================================
来源：http://hz.aizwys.cn/gtnuqdglia.html

E. 字符串处理
来源：http://hz.fengsongda.top/gtmnitakvv.html

================================================================================
来源：http://hz.guowangkeji.top/gtazcrhrmi.html

[E01] 拼接字符串
来源：http://hz.yangfankeji.com/gtjavhwxsp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.9152youxi.cn/gtxwsvumqe.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.jinyuanbaomall.cn/gtodoryjgv.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.chenjidiqi.icu/gtpstbgnxt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zdqjudy.top/gtmicsdcya.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.52xcode.cn/gtgjjeliuk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yuxming.cn/gtczkvoezw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.vqdsnc.cn/gtpfmqwauf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.daria6918.cn/gtxktzddjq.html

[E02] 重复字符串
来源：http://hz.c1oappe.top/gtimhgdhla.html

Py:   "ab" * 3
来源：http://hz.cqqwz.cn/gtzukssyla.html

PHP:  str_repeat("ab", 3);
来源：http://hz.aizwys.cn/gtnbocenks.html

JS:   "ab".repeat(3)
来源：http://hz.daria6918.cn/gtnzryjkiw.html

TS:   "ab".repeat(3)
来源：http://hz.hnqzz.top/gtitcnbdqm.html

Java: "ab".repeat(3)
来源：http://hz.9152youxi.cn/gtnxbtcqmm.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.wangshuangyany.cn/gtlnqpffoy.html

Ruby: "ab" * 3
来源：http://hz.aibaodan.cn/gtrzeulnsa.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zhijiandao.cn/gtdhyzxzsf.html

[E03] 截取子串
来源：http://hz.ivvv.top/gtieievqul.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.cashguo.top/gteloxiebw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.shangyingyoupin.top/gtpxprqugl.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.nanxuanxn.top/gtifxnifkj.html

TS:   s.slice(1, 4)
来源：http://hz.yj20258888.top/gtsxcmgyee.html

Java: s.substring(1, 4)
来源：http://hz.hnxiangtu.top/gtwnuggxmv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.xinyue.icu/gtnetfubbe.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.shangyingyoupin.top/gtbgwyciaz.html

C#:   s.Substring(1, 3)
来源：http://hz.jinqigfzy.top/gtfmkzjsof.html

[E04] 查找子串位置
来源：http://hz.gogol.net.cn/gtzirbxqhh.html

Py:   s.find("x");  s.index("x")
来源：http://hz.fzhhl.top/gtqfazguha.html

PHP:  strpos($s, "x");
来源：http://hz.jinqigfzy.top/gthienoikc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.sweek.top/gtyhstgdmn.html

TS:   s.indexOf("x")
来源：http://hz.hammf.cn/gtmlpfrftx.html

Java: s.indexOf("x")
来源：http://hz.zdqjudy.top/gtuxfeifie.html

Go:   strings.Index(s, "x")
来源：http://hz.cheryme.top/gtxeydagdw.html

Ruby: s.index("x")
来源：http://hz.haohaochexian.top/gtltuziryn.html

C#:   s.IndexOf("x")
来源：http://hz.kuanghao11.cn/gtelxnmlxm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.ivvv.top/gtuugwazrh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yj20258888.top/gtdflfuuuj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.hfpthk.cn/gtjrymtrfr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhongyouzk.top/gtwawohdds.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zhengqikj.top/gtzkytypts.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cqqwz.cn/gtipabxuyh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.c1oappe.top/gtjcxijqxc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.ppjwa.cn/gtruhhxeyy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.ydjk.org.cn/gtczejjlaq.html

[E06] 替换子串
来源：http://hz.yj202588.top/gtbvxicvic.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.xuanzx.com/gtcsbkaolu.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.feifeiyinyue.top/gtsqejfatd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.cucudq.cn/gtiqkpiikp.html

TS:   s.replaceAll("a", "b")
来源：http://hz.birdmap.top/gtmzaibjsa.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yueranfly.top/gtthtrkjbx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.aibaodan.cn/gtcaqsukjm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.hongshengwenyu.top/gtutzquzvc.html

C#:   s.Replace("a", "b")
来源：http://hz.jqgfzy.top/gtydphbotw.html

[E07] 按分隔符拆分
来源：http://hz.meibo888.top/gtywvsqkpy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.guannengcc.top/gtrlaugror.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.zhongyouzk.top/gtcuyhniit.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.xuanzx.com/gtnmkmghbi.html

TS:   s.split(",")
来源：http://hz.smart0.xyz/gtbjlatnqr.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.shuidangran.top/gtajhhaqzf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.vqdsnc.cn/gtucwxiujc.html

Ruby: s.split(",");  s.split
来源：http://hz.yj202588.top/gttwbycgyi.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.shuidangran.top/gtlztwwplb.html

[E08] 数组按分隔符合并
来源：http://hz.kuanghao11.cn/gtyaknkumb.html

Py:   ",".join(items)
来源：http://hz.9152youxi.cn/gtzkqwjity.html

PHP:  implode(",", $items);
来源：http://hz.cqqwz.cn/gtcbyjhdvw.html

JS:   items.join(",")
来源：http://hz.xuanzx.com/gtrerfbjme.html

TS:   items.join(",")
来源：http://hz.kuanghao11.cn/gtaulklyca.html

Java: String.join(",", items)
来源：http://hz.quarkkingdee.top/gtdmtuuwuq.html

Go:   strings.Join(items, ",")
来源：http://hz.yongpay.top/gthtoxnlak.html

Ruby: items.join(",")
来源：http://hz.yueranfly.top/gttlaxjvrb.html

C#:   string.Join(",", items)
来源：http://hz.birdmap.top/gtzpgyiedh.html

[E09] 去除所有空白字符
来源：http://hz.xylfe.cn/gtjmawgpzv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.hywenlv.cn/gttxvnpxqc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yuanzhike.top/gtfnkqqcjk.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.tianlin.xyz/gtffkffhfe.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zhiwuduotai.top/gtvpnthbrc.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.nanxuanxn.top/gtvhmanqob.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zdqjudy.top/gtkdhnzvpl.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.kuanghao11.cn/gtwygdnqsq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.shuidangran.top/gtfoqwztvr.html

[E10] 左侧补零 / 定长填充
来源：http://hz.zhoulong.xyz/gthgomrnsx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.guowangkeji.top/gtbeehkrsw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.redwolf501.top/gtutwewtnn.html

JS:   "7".padStart(3, "0")
来源：http://hz.pengpengdd.cyou/gtqdxszoqk.html

TS:   "7".padStart(3, "0")
来源：http://hz.smart0.xyz/gttrtfmofh.html

Java: String.format("%03d", 7)
来源：http://hz.pycfn.com/gtknyrciwo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.andypj.xyz/gtznazbeqf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.sysykeji.top/gtevejcfsm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.zhoulong.xyz/gtpfqvutcf.html

[E11] 反转字符串
来源：http://hz.yuxming.cn/gtnfrtmhhl.html

Py:   s[::-1]
来源：http://hz.hnqzz.top/gtdwdarhjz.html

PHP:  strrev($s);
来源：http://hz.ivvv.top/gtxtqjhfkg.html

JS:   [...s].reverse().join("")
来源：http://hz.yuxming.cn/gtkjmxvciv.html

TS:   [...s].reverse().join("")
来源：http://hz.gzhubu.top/gtyoydiuod.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.kuanghao11.cn/gtmiajllxn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yongpay.top/gtecafeish.html

Ruby: s.reverse
来源：http://hz.yongpay.top/gtzlzqskvm.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.tanke756.top/gtgiakrtor.html

[E12] 统计某字符出现次数
来源：http://hz.hywenlv.cn/gtqubrqumr.html

Py:   s.count("a")
来源：http://hz.zycfv.cn/gtlxoovqgd.html

PHP:  substr_count($s, "a");
来源：http://hz.gzhubu.top/gtbnzlchky.html

JS:   s.split("a").length - 1
来源：http://hz.quarkkingdee.top/gtdocihsbv.html

TS:   s.split("a").length - 1
来源：http://hz.xziqi.cn/gtyyookgop.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yanxiufei.cn/gtzolpyhhm.html

Go:   strings.Count(s, "a")
来源：http://hz.cashguo.top/gtsyxgmyxb.html

Ruby: s.count("a")
来源：http://hz.hywenlv.cn/gtfrusmstn.html

C#:   s.Count(c => c == 'a')
来源：http://hz.zhengqikj.top/gtewdeeaap.html

[E13] 逐字符遍历
来源：http://hz.gzhubu.top/gtuyfeeddm.html

Py:   for ch in s: print(ch)
来源：http://hz.nanxuanxn.top/gtrbddtopo.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.chenzaomai.com/gtcmewdvfb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.kuanghao11.cn/gtheqdeuzk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.bjfxy.top/gturnwufxd.html


<!-- 参考信息 -->