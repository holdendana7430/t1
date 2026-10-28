代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.xuetiantiany.cn/gtflejcqct.html

TS:   [...a, ...b];
来源：http://hz.zhixingplan.top/gtolwkklrp.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.xuanzx.com/gtvflawiay.html

Go:   append(a, b...)
来源：http://hz.haohaochexian.top/gtcbhtrdjk.html

Ruby: a + b;  a.concat(b)
来源：http://hz.9152youxi.cn/gtmuvgjszo.html

C#:   a.Concat(b).ToList()
来源：http://hz.cqqwz.cn/gtxtztjdwe.html

[D09] 排序（升序）
来源：http://hz.chenjidiqi.icu/gtjtfjwghp.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.0kj1m.cn/gtpihkrdub.html

PHP:  sort($arr);
来源：http://hz.guannengcc.top/gtwdximjwi.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.gaohongyu789.top/gtzheygqkk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yvedp.cn/gtighykbqf.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yongpay.top/gtriexpmdy.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.cashguo.top/gtjyijamlx.html

Ruby: arr.sort
来源：http://hz.fengsongda.top/gtyzlvemcs.html

C#:   list.Sort();
来源：http://hz.guannengcc.top/gtkcawvrkt.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.kuanghao11.cn/gtpdprzexy.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zhiwuduotai.top/gtawhojuou.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.xinyue.icu/gtgwyyyvsl.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhoulong.xyz/gtvhjlhiqn.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yj20258888.top/gttmvnjwfi.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.cashguo.top/gtcbvpgjbb.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jinyuanbaomall.cn/gtfypkdbxm.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.shuidangran.top/gtosvxescz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zhoulong.xyz/gtphnwrilq.html

[D11] 反转数组
来源：http://hz.tanke756.top/gttofubibk.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.jyoumei.cn/gtyxugvoet.html

PHP:  array_reverse($arr);
来源：http://hz.tian-w.cn/gtvjxjayat.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.shanyushiyangtech.top/gtnktuzeho.html

TS:   [...arr].reverse();
来源：http://hz.ydjk.org.cn/gtbezetaec.html

Java: Collections.reverse(list);
来源：http://hz.gotoacloud.top/gtgtujelkn.html

Go:   slices.Reverse(arr)
来源：http://hz.ppjwa.cn/gtybsbmquf.html

Ruby: arr.reverse
来源：http://hz.cucudq.cn/gttnwllkev.html

C#:   list.Reverse();
来源：http://hz.aibaodan.cn/gthbqmxpad.html

[D12] 查找元素下标
来源：http://hz.cashguo.top/gtkohvmkbe.html

Py:   arr.index(x);  x in arr
来源：http://hz.pycfn.com/gtisnqyyms.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.xingfuxueyuan.xyz/gtaeqmnrcb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yanxiufei.cn/gtccsxhqtf.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hongshengwenyu.top/gtlwlzmgbh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.pengpengdd.cyou/gtcjgfmchn.html

Go:   slices.Index(arr, x)
来源：http://hz.ybcxt.top/gtnmpshqxq.html

Ruby: arr.index(x)
来源：http://hz.zhiwuduotai.top/gtqomlkezv.html

C#:   list.IndexOf(x);
来源：http://hz.tianlin.xyz/gtsdmpvipp.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jinqigfzy.top/gtersoijsi.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.smart0.xyz/gtajopxfjk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.hammf.cn/gtlnirqkxp.html

JS:   arr.filter(x => x > 3)
来源：http://hz.xingfuxueyuan.xyz/gtiatrefwc.html

TS:   arr.filter(x => x > 3)
来源：http://hz.ehwqpu.com/gtkaabvtqx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.yueranfly.top/gtmdlqitrj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.hongshengwenyu.top/gtshnuaavo.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.haohaochexian.top/gtupqgthvs.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yonumen.top/gtujkkuwrn.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yj20258888.top/gtepotvnfc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.sxryk.cn/gtwuqyorib.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yangfankeji.com/gtbvgjolyx.html

JS:   arr.map(x => x * 2)
来源：http://hz.vqdsnc.cn/gttocfnfhn.html

TS:   arr.map(x => x * 2)
来源：http://hz.ivvv.top/gtufthehdo.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yj20258888.top/gtbgglpsey.html

Go:   // 手写循环
来源：http://hz.cheryme.top/gthrjfzypx.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.vqdsnc.cn/gtibyquzmg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.dianchejie.cn/gtwjtvroyo.html

[D15] 去重
来源：http://hz.shuidangran.top/gtwocqnsnt.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.snrcjt.cn/gtxuqqmyjl.html

PHP:  array_unique($arr);
来源：http://hz.redwolf501.top/gtxivowjrj.html

JS:   [...new Set(arr)]
来源：http://hz.chenlongwang.top/gtzwepurls.html

TS:   [...new Set(arr)]
来源：http://hz.gotoacloud.top/gterobuthy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yj20258.top/gtdhxevrim.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.sxryk.cn/gtsthlpwgx.html

Ruby: arr.uniq
来源：http://hz.dianchejie.cn/gtdmlkqdmk.html

C#:   list.Distinct().ToList()
来源：http://hz.52xcode.cn/gtdychsgec.html

[D16] 求和与平均值
来源：http://hz.xingfuxueyuan.xyz/gtmsafzqpg.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.smart0.xyz/gtsqzprdxa.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.pycfn.com/gtaigsbwax.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.nwbrower.top/gtiurnqezw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.andypj.xyz/gtfvnnubwl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yj20258888.top/gtduiydeza.html

Go:   // 手写循环累加
来源：http://hz.jinqigufen.top/gtidlpveeg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhijiandao.cn/gtwpwzlcqu.html

C#:   list.Sum();  list.Average()
来源：http://hz.sysykeji.top/gthddbhmkb.html

[D17] 最大值与最小值
来源：http://hz.jinqigfzy.top/gtzjqyiwuu.html

Py:   max(arr);  min(arr)
来源：http://hz.jinqigfzy.top/gtrebwbvbj.html

PHP:  max($arr);  min($arr);
来源：http://hz.yongpay.top/gtjhkrugvh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.cashguo.top/gtcygummvj.html

TS:   Math.max(...arr);
来源：http://hz.sweek.top/gtijwenpmn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.yuanzhike.top/gtwzzctbbi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.cucudq.cn/gtaivtqdjt.html

Ruby: arr.max;  arr.min
来源：http://hz.bjfxy.top/gtkfzeessv.html

C#:   list.Max();  list.Min()
来源：http://hz.ybcxt.top/gtjiommmbx.html

[D18] 扁平化嵌套数组
来源：http://hz.nanxuanxn.top/gtbhpubvhr.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.chenjidiqi.icu/gtecpeysvy.html

PHP:  array_merge(...$nested);
来源：http://hz.sxryk.cn/gttujrkulz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.guannengcc.top/gtnulloxno.html

TS:   nested.flat();
来源：http://hz.sufxvd.cn/gtmkmsttsl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.zhixingplan.top/gtlkkpcsox.html

Go:   // 手写双层循环
来源：http://hz.shanyushiyangtech.top/gtzhpjoluy.html

Ruby: nested.flatten
来源：http://hz.xuetiantiany.cn/gtzsmezeea.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.haohaochexian.top/gtfdxppusa.html

[D19] 按字段分组
来源：http://hz.sxryk.cn/gtwdqfzyna.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.shangyingyoupin.top/gtyzvzmgkt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.xylfe.cn/gthinfzixd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.redwolf501.top/gtcvlqrvyk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.hywenlv.cn/gtcjeictzq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.hfpthk.cn/gttkfalwcv.html

Go:   // 手写 map[string][]T
来源：http://hz.haohaochexian.top/gtfqanddcr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.jqgufenzy.top/gtcrgdchyz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zhengqikj.top/gtpajnjpyw.html

[D20] 统计每个元素出现次数
来源：http://hz.tian-w.cn/gtxrstfeth.html

Py:   Counter(arr)
来源：http://hz.hammf.cn/gtdpvywljx.html

PHP:  array_count_values($arr);
来源：http://hz.shanyushiyangtech.top/gttrrsdkmn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.quarkkingdee.top/gttjlvsqsq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hammf.cn/gtwczgulyk.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.fengsongda.top/gtvpplrela.html

Go:   // 手写 map[T]int
来源：http://hz.sufxvd.cn/gtizknzjla.html

Ruby: arr.tally
来源：http://hz.snrcjt.cn/gtdbdxktjk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.daxiang520.top/gtzhppfznp.html

[D21] 判断是否包含某元素
来源：http://hz.aibaodan.cn/gttowovpjk.html

Py:   x in arr
来源：http://hz.cucudq.cn/gtsglqmzvp.html

PHP:  in_array($x, $arr, true);
来源：http://hz.havefunace.top/gtzpalpwbw.html

JS:   arr.includes(x)
来源：http://hz.yanxiufei.cn/gthoekxzkm.html

TS:   arr.includes(x)
来源：http://hz.ppjwa.cn/gtmrnmyclt.html

Java: list.contains(x)
来源：http://hz.quarkkingdee.top/gtsrzvbivs.html

Go:   slices.Contains(arr, x)
来源：http://hz.yuxming.cn/gtsrubofxt.html

Ruby: arr.include?(x)
来源：http://hz.xylfe.cn/gtmbqkaxsx.html

C#:   list.Contains(x)
来源：http://hz.ydjk.org.cn/gtfvfohfyw.html

[D22] 复制数组（避免共享引用）
来源：http://hz.zhiwuduotai.top/gtumivhral.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.zhijiandao.cn/gtehtcnxsh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.shanyushiyangtech.top/gtknbzdlwn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.guannengcc.top/gtkrtvepiv.html

TS:   [...arr];
来源：http://hz.yj20258.top/gteqpjcncs.html

Java: new ArrayList<>(list);
来源：http://hz.aibaodan.cn/gtfisdzulq.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.aibaodan.cn/gtbpfwvagt.html

Ruby: arr.dup;  arr.clone
来源：http://hz.gotoacloud.top/gtsayikuwk.html

C#:   new List<int>(list);
来源：http://hz.chenzaomai.com/gtzdzetsjd.html

[D23] reduce 累积计算
来源：http://hz.quarkkingdee.top/gtwuwsquky.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yj202588.top/gtkqayntrn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.sufxvd.cn/gtfszyzicn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ywan-chungtsiang.top/gtlwdogyfv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cdnleiting.top/gtrkygczxx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.hammf.cn/gtukojpgcx.html

Go:   // 手写循环
来源：http://hz.nanxuanxn.top/gtbubsgquq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.zhaomingkeji.xyz/gtakjhhiut.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jinyuanbaomall.cn/gttioitmxy.html

[D24] 字典 / Map 基本操作
来源：http://hz.yj20258888.top/gtpbghdfzi.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.jinqigfzy.top/gtntamwrlg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.xuetiantiany.cn/gttezkhrab.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.smart0.xyz/gtyjhkvmhp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.xylfe.cn/gtugiiahvb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jinyuanbaomall.cn/gtbtuehjkq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.xuanzx.com/gtvsycsbcj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.yonumen.top/gtklqjahch.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.shzxlz.cn/gtsbbsoygy.html

[D25] Set 集合去重与交并差
来源：http://hz.jqgufenzy.top/gtsfgrkftr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.xziqi.cn/gtkbgkucgf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.dashuyun.cn/gtibbcqjzc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.cqqwz.cn/gtdxhsyzrn.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.mhx1999.top/gtadpgyctv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.fengsongda.top/gtinwuxgyq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.smart0.xyz/gtbmkgilbw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.pycfn.com/gtaxripjda.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.zhijiandao.cn/gtqarcwykz.html

[D26] 数组转字符串
来源：http://hz.cdnleiting.top/gtifezncof.html

Py:   ", ".join(map(str, arr))
来源：http://hz.iojbl.cn/gtuwujpdyg.html

PHP:  implode(", ", $arr);
来源：http://hz.xuetiantiany.cn/gtrfvadned.html

JS:   arr.join(", ")
来源：http://hz.yuxming.cn/gtcxeuiuhw.html

TS:   arr.join(", ")
来源：http://hz.yvedp.cn/gtlfsvlzti.html

Java: String.join(", ", list)
来源：http://hz.zhoulong.xyz/gtswqwnmxl.html

Go:   strings.Join(strs, ", ")
来源：http://hz.zhaomingkeji.xyz/gtrmipgfsh.html

Ruby: arr.join(", ")
来源：http://hz.hfpthk.cn/gthtirjvhv.html

C#:   string.Join(", ", list)
来源：http://hz.aibaodan.cn/gtpriytnge.html

================================================================================
来源：http://hz.zdqjudy.top/gtulbrvkvp.html

E. 字符串处理
来源：http://hz.cucudq.cn/gtzugzqulf.html

================================================================================
来源：http://hz.zhengqikj.top/gtscmjeyew.html

[E01] 拼接字符串
来源：http://hz.pycfn.com/gtmmzczoyh.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.bjfxy.top/gtnxtmpygc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yuanzhike.top/gturyaxjwb.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.mhx1999.top/gtzpdeyhfh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.0kj1m.cn/gtspjdwmlq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.zdqjudy.top/gtrwrkfzmf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.hysaishi.cn/gtgliwvaaj.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.fzhhl.top/gtfbhumqpu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.xziqi.cn/gtiffvjrfo.html

[E02] 重复字符串
来源：http://hz.birdmap.top/gtufryferf.html

Py:   "ab" * 3
来源：http://hz.redwolf501.top/gtapkvqkfn.html

PHP:  str_repeat("ab", 3);
来源：http://hz.sweek.top/gtepjdgoln.html

JS:   "ab".repeat(3)
来源：http://hz.aizwys.cn/gtxzxxuhqf.html

TS:   "ab".repeat(3)
来源：http://hz.jinqigufen.top/gtdgeknwrs.html

Java: "ab".repeat(3)
来源：http://hz.shanyushiyangtech.top/gtbljddzfs.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.tian-w.cn/gtmaajwmdg.html

Ruby: "ab" * 3
来源：http://hz.cashguo.top/gtstzyfeim.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yj20258888.top/gtlkiytazu.html

[E03] 截取子串
来源：http://hz.0kj1m.cn/gtzayxjdis.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.tian-w.cn/gtbhwrdxlj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.shanyushiyangkeji.top/gttadagiut.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.hysaishi.cn/gtgynsugyz.html

TS:   s.slice(1, 4)
来源：http://hz.yj20258888.top/gtqbiyjusk.html

Java: s.substring(1, 4)
来源：http://hz.smart0.xyz/gtvsqpfohe.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.guowangkeji.top/gtbjddspuh.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.zhijiandao.cn/gtdsypralp.html

C#:   s.Substring(1, 3)
来源：http://hz.pycfn.com/gtwyxmkaxw.html

[E04] 查找子串位置
来源：http://hz.hnqzz.top/gtgzcjpeep.html

Py:   s.find("x");  s.index("x")
来源：http://hz.zycfv.cn/gttypdonvf.html

PHP:  strpos($s, "x");
来源：http://hz.hongshengwenyu.top/gtnxodneeq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.chenzaomai.com/gtdxvwxcyd.html

TS:   s.indexOf("x")
来源：http://hz.dashuyun.cn/gtcedvdsas.html

Java: s.indexOf("x")
来源：http://hz.wangshuangyany.cn/gtzsvbraxl.html

Go:   strings.Index(s, "x")
来源：http://hz.dianchejie.cn/gtvqxhwohp.html

Ruby: s.index("x")
来源：http://hz.zhijiandao.cn/gtoyywiopf.html

C#:   s.IndexOf("x")
来源：http://hz.sufxvd.cn/gtffjwprnn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.sweek.top/gtwlkexclr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.cucudq.cn/gtusfhsehv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.hongshengwenyu.top/gtrfnxlthr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hywenlv.cn/gtcwckuidh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.havefunace.top/gtcjrsipsu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hnqzz.top/gtmurjdgbu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.yueranfly.top/gtktjfgvqs.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.daria6918.cn/gtkcaygfqr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jiagoushi.top/gtchlmbucd.html

[E06] 替换子串
来源：http://hz.zhengqikj.top/gtiwjjrijc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.havefunace.top/gtilinxjuv.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.yj20258888.top/gtmhlqkjrb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.feifeiyinyue.top/gtzxucrzot.html

TS:   s.replaceAll("a", "b")
来源：http://hz.sufxvd.cn/gtoskvmyfn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hnqzz.top/gtasjbvpty.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.9152youxi.cn/gtxhwpvolq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.hnxiangtu.top/gtpxluijwo.html

C#:   s.Replace("a", "b")
来源：http://hz.yangfankeji.com/gtwqaquniw.html

[E07] 按分隔符拆分
来源：http://hz.vqdsnc.cn/gtmylkscbp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.dianchejie.cn/gtyrdahsie.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.cdnleiting.top/gtlholmrrb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.haohaochexian.top/gtmqienvxy.html

TS:   s.split(",")
来源：http://hz.shuidangran.top/gtxaxwscox.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.pengpengdd.cyou/gtdnvgxaus.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yuanzhike.top/gtibnpjpzr.html

Ruby: s.split(",");  s.split
来源：http://hz.gaohongyu789.top/gtdstpsepv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.svipenyu.cn/gtotgqnjek.html

[E08] 数组按分隔符合并
来源：http://hz.yj20258888.top/gtozyfxlwh.html

Py:   ",".join(items)
来源：http://hz.sweek.top/gtgdyvblzu.html

PHP:  implode(",", $items);
来源：http://hz.hfpthk.cn/gtkxpdbuqg.html

JS:   items.join(",")
来源：http://hz.hysaishi.cn/gtirjbnvvi.html

TS:   items.join(",")
来源：http://hz.gaohongyu789.top/gtlrlbluxz.html

Java: String.join(",", items)
来源：http://hz.ybcxt.top/gtjpirfrfc.html

Go:   strings.Join(items, ",")
来源：http://hz.hongshengwenyu.top/gtyqettbik.html

Ruby: items.join(",")
来源：http://hz.yj202588.top/gtiegrssgg.html

C#:   string.Join(",", items)
来源：http://hz.shanyushiyangkeji.top/gtwinwaqvp.html

[E09] 去除所有空白字符
来源：http://hz.c1oappe.top/gtojywbrfk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.chenjidiqi.icu/gtljughvzw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.jqgufenzy.top/gtvwhlewlu.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.ppjwa.cn/gtpzyfzlce.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.pengpengdd.cyou/gtgyuyqdai.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yueranfly.top/gtashwgxad.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.gotoacloud.top/gtmhkhawmy.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.wangshuangyany.cn/gttrkgcxks.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.tanke756.top/gtczvvcvdj.html

[E10] 左侧补零 / 定长填充
来源：http://hz.ydzc1.top/gtidjzfjcx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.daxiang520.top/gtivguebnw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.chenjidiqi.icu/gtmwssmlmj.html

JS:   "7".padStart(3, "0")
来源：http://hz.hammf.cn/gtputswijq.html

TS:   "7".padStart(3, "0")
来源：http://hz.zhengqikj.top/gtbvfelklg.html

Java: String.format("%03d", 7)
来源：http://hz.xylfe.cn/gtnvlmgqec.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.sysykeji.top/gtsetxtrxt.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.svipenyu.cn/gtlyhlmhat.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.chenjidiqi.icu/gthbunqmmr.html

[E11] 反转字符串
来源：http://hz.zdqjudy.top/gtqpcqrery.html

Py:   s[::-1]
来源：http://hz.shuidangran.top/gtxhezgcit.html

PHP:  strrev($s);
来源：http://hz.316326.xyz/gtrtgxwlmk.html

JS:   [...s].reverse().join("")
来源：http://hz.chenzaomai.com/gtonkylaop.html

TS:   [...s].reverse().join("")
来源：http://hz.jqgufenzy.top/gtyrnayvhn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jinqigufen.top/gtpyxmuedt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.iojbl.cn/gtuganoylk.html

Ruby: s.reverse
来源：http://hz.ywan-chungtsiang.top/gtqhxijblk.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jyoumei.cn/gthupllajd.html

[E12] 统计某字符出现次数
来源：http://hz.ywan-chungtsiang.top/gtvcsuzhfl.html

Py:   s.count("a")
来源：http://hz.jinghuilouyu.cn/gtccmmosgx.html

PHP:  substr_count($s, "a");
来源：http://hz.wangdashe.top/gtaumextdk.html

JS:   s.split("a").length - 1
来源：http://hz.hongshengwenyu.top/gtgwutkpae.html

TS:   s.split("a").length - 1
来源：http://hz.pycfn.com/gtfgbirtjl.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.cdnleiting.top/gtwtberoxb.html

Go:   strings.Count(s, "a")
来源：http://hz.ywan-chungtsiang.top/gtojixgsyj.html

Ruby: s.count("a")
来源：http://hz.andypj.xyz/gtssgcrpdb.html

C#:   s.Count(c => c == 'a')
来源：http://hz.chenzaomai.com/gttyitbhmp.html

[E13] 逐字符遍历
来源：http://hz.zhiwuduotai.top/gtgbckshgr.html

Py:   for ch in s: print(ch)
来源：http://hz.yueranfly.top/gtzfitldve.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.meibo888.top/gtosuxmqmq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.guowangkeji.top/gtolvvvwpt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jinqigufen.top/gtqmsilslm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.gotoacloud.top/gtoebqbdef.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.shzxlz.cn/gtnohqhujb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.9152youxi.cn/gttkwtkzgl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zhijiandao.cn/gtznzfuiej.html

[E14] URL 编码与 Base64
来源：http://hz.aizwys.cn/gtbsjleyxt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jqgfzy.top/gtoqirsnua.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.wangdashe.top/gtlfwijwwd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.cashguo.top/gttqshhcac.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.sufxvd.cn/gtbogyrppb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.dashuyun.cn/gtejebrdql.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jiagoushi.top/gtmnzgvxce.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.xuanzx.com/gtiecyeews.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.xuetiantiany.cn/gthbonnfhn.html

[E15] HTML 转义 / 反转义
来源：http://hz.hywenlv.cn/gtvvghttyv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ehwqpu.com/gtrpzzkdlr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.zhengqikj.top/gtmovcevsi.html


<!-- 参考信息 -->