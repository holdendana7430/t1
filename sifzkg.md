代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://hz.sufxvd.cn/gttxvhkdmh.html

[D08] 合并两个数组
来源：http://hz.guannengcc.top/gtokspfklb.html

Py:   a + b;  a.extend(b)
来源：http://hz.shanyushiyangkeji.top/gtzencawsr.html

PHP:  array_merge($a, $b);
来源：http://hz.xinyue.icu/gtltbkzzfg.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.pycfn.com/gtzweqcblo.html

TS:   [...a, ...b];
来源：http://hz.yuxming.cn/gtlmfskomr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.shangyingyoupin.top/gtbusikyjx.html

Go:   append(a, b...)
来源：http://hz.yangfankeji.com/gtoqqqrkcq.html

Ruby: a + b;  a.concat(b)
来源：http://hz.ywan-chungtsiang.top/gtpfmjfdkx.html

C#:   a.Concat(b).ToList()
来源：http://hz.xingfuxueyuan.xyz/gtbxqeeapk.html

[D09] 排序（升序）
来源：http://hz.haohaochexian.top/gtbfozudxe.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhongyouzk.top/gtklofaygv.html

PHP:  sort($arr);
来源：http://hz.sxryk.cn/gtizxuwjku.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.ppjwa.cn/gtngqvnbzx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.shuidangran.top/gtgetmotac.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.ehwqpu.com/gthtrphbkw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.ppjwa.cn/gtltudrwse.html

Ruby: arr.sort
来源：http://hz.cheryme.top/gtzmefuzug.html

C#:   list.Sort();
来源：http://hz.shuidangran.top/gtyljcaqrj.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.yonumen.top/gtvbpvxwbt.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.nwbrower.top/gtwlethrnj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.nanxuanxn.top/gtuwgvqvvk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xziqi.cn/gtiubrqkey.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.wangdashe.top/gtzpnnxjfi.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.quarkkingdee.top/gtdpvlnyoq.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.ydzc1.top/gttebhqaxr.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.pycfn.com/gtegfsajgo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.fengsongda.top/gtlhrwlvqx.html

[D11] 反转数组
来源：http://hz.wangdashe.top/gtpzpdiwzk.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.jyoumei.cn/gtumlenxey.html

PHP:  array_reverse($arr);
来源：http://hz.cqqwz.cn/gtnfwgqjai.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.zhijiandao.cn/gtcmijswrs.html

TS:   [...arr].reverse();
来源：http://hz.andypj.xyz/gtftfgmssc.html

Java: Collections.reverse(list);
来源：http://hz.jinqigufen.top/gthrvatiiz.html

Go:   slices.Reverse(arr)
来源：http://hz.gzhubu.top/gtouuwxwof.html

Ruby: arr.reverse
来源：http://hz.0kj1m.cn/gtxapagqwk.html

C#:   list.Reverse();
来源：http://hz.316326.xyz/gtlgqggrtl.html

[D12] 查找元素下标
来源：http://hz.jinqigfzy.top/gtxoldtmzp.html

Py:   arr.index(x);  x in arr
来源：http://hz.jinghuilouyu.cn/gtyretkppb.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.vqdsnc.cn/gtgpxdjonz.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.snrcjt.cn/gtogpdhhpb.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.bjfxy.top/gtpngzkezh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.ybcxt.top/gtuhnqnfzc.html

Go:   slices.Index(arr, x)
来源：http://hz.jinqigfzy.top/gtcqkpomon.html

Ruby: arr.index(x)
来源：http://hz.bjfxy.top/gtjtjtrujp.html

C#:   list.IndexOf(x);
来源：http://hz.ywan-chungtsiang.top/gtcfxqqipb.html

[D13] 过滤（保留满足条件的）
来源：http://hz.zhijiandao.cn/gtdxhyynfx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.chenlongwang.top/gtotiohjpp.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.sysykeji.top/gtoossroub.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hnxiangtu.top/gtgkxxkchd.html

TS:   arr.filter(x => x > 3)
来源：http://hz.yueranfly.top/gtqphgnonm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.cheryme.top/gtfnuywmzy.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yj20258888.top/gtfwczlzaj.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.zhijiandao.cn/gtmnrxjppt.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.cqqwz.cn/gtycqlolfy.html

[D14] 映射转换（每个元素变形）
来源：http://hz.sxryk.cn/gtjmkroomt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jqgfzy.top/gtgtvmvccx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.ybcxt.top/gtawgqynas.html

JS:   arr.map(x => x * 2)
来源：http://hz.jlsjyb.cn/gthjgwfboi.html

TS:   arr.map(x => x * 2)
来源：http://hz.yanxiufei.cn/gtexckbmas.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jqgufenzy.top/gtxibmoiht.html

Go:   // 手写循环
来源：http://hz.xingfuxueyuan.xyz/gtsyewnglt.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.jlsjyb.cn/gtgpisnljx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.hammf.cn/gtogxnekmu.html

[D15] 去重
来源：http://hz.quarkkingdee.top/gtqzyunvhh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.kuanghao11.cn/gtmeunwkqd.html

PHP:  array_unique($arr);
来源：http://hz.snrcjt.cn/gtiujfuqxh.html

JS:   [...new Set(arr)]
来源：http://hz.shzxlz.cn/gtzzgqlzta.html

TS:   [...new Set(arr)]
来源：http://hz.hnxiangtu.top/gtqlrommyq.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.zhiwuduotai.top/gtuecptvqg.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zhaomingkeji.xyz/gthydnpfrm.html

Ruby: arr.uniq
来源：http://hz.shzxlz.cn/gtecajroig.html

C#:   list.Distinct().ToList()
来源：http://hz.wangshuangyany.cn/gtvmnbzwlq.html

[D16] 求和与平均值
来源：http://hz.yangfankeji.com/gtelrxsves.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.zhiwuduotai.top/gtxlkbpflc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yanxiufei.cn/gthkndhncy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hywenlv.cn/gtasywjuux.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.iojbl.cn/gtcgncdidv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.sxryk.cn/gtqxgpakqq.html

Go:   // 手写循环累加
来源：http://hz.aizwys.cn/gtmbwvrsat.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.wangshuangyany.cn/gtxazivhso.html

C#:   list.Sum();  list.Average()
来源：http://hz.sufxvd.cn/gtxnzoxcpm.html

[D17] 最大值与最小值
来源：http://hz.cdnleiting.top/gtpzncgnhp.html

Py:   max(arr);  min(arr)
来源：http://hz.feifeiyinyue.top/gtoegwgeku.html

PHP:  max($arr);  min($arr);
来源：http://hz.jinqigfzy.top/gtvuhslxsi.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.mhx1999.top/gtxoxqldeu.html

TS:   Math.max(...arr);
来源：http://hz.andypj.xyz/gttkzaazpg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.meibo888.top/gtunyrubfn.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.vqdsnc.cn/gttlmnpova.html

Ruby: arr.max;  arr.min
来源：http://hz.yj20258.top/gtouovwpyw.html

C#:   list.Max();  list.Min()
来源：http://hz.quarkkingdee.top/gtjzpghjsk.html

[D18] 扁平化嵌套数组
来源：http://hz.andypj.xyz/gtcgvgcfvy.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.kuanghao11.cn/gtqtprpkcd.html

PHP:  array_merge(...$nested);
来源：http://hz.yj20258.top/gtgpgjfdmj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.ydzc1.top/gtbpmdmdbc.html

TS:   nested.flat();
来源：http://hz.nwbrower.top/gtvchpeezb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.nwbrower.top/gtlhdaewhi.html

Go:   // 手写双层循环
来源：http://hz.yuxming.cn/gtnwozjncg.html

Ruby: nested.flatten
来源：http://hz.xingfuxueyuan.xyz/gthixcdhbc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.pycfn.com/gtiajdbwmf.html

[D19] 按字段分组
来源：http://hz.hysaishi.cn/gtpbvafvzn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.birdmap.top/gtpsugqwqj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.316326.xyz/gtskeouagi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.dianchejie.cn/gtelarlnkz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jlsjyb.cn/gtssdeujhp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zhijiandao.cn/gtrqxjwwbs.html

Go:   // 手写 map[string][]T
来源：http://hz.yuanzhike.top/gtqhqmuqkm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.dashuyun.cn/gtqqjuqlvm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.aibaodan.cn/gtlsigqqzn.html

[D20] 统计每个元素出现次数
来源：http://hz.gaohongyu789.top/gtlakbfxqd.html

Py:   Counter(arr)
来源：http://hz.cashguo.top/gtouhvpcms.html

PHP:  array_count_values($arr);
来源：http://hz.guannengcc.top/gtmlvqeyzg.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.9152youxi.cn/gtbdoxyvem.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.redwolf501.top/gtfkxnnkrt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.jlsjyb.cn/gtbccwizni.html

Go:   // 手写 map[T]int
来源：http://hz.kuanghao11.cn/gtyrxvukro.html

Ruby: arr.tally
来源：http://hz.ydjk.org.cn/gtxkgfkcza.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.tianlin.xyz/gttfitrvni.html

[D21] 判断是否包含某元素
来源：http://hz.ywan-chungtsiang.top/gtkozlxqcb.html

Py:   x in arr
来源：http://hz.cashguo.top/gtjtnghgqw.html

PHP:  in_array($x, $arr, true);
来源：http://hz.redwolf501.top/gtajmnacox.html

JS:   arr.includes(x)
来源：http://hz.jianghu66.top/gtebnyrroo.html

TS:   arr.includes(x)
来源：http://hz.yanxiufei.cn/gtfzsknidk.html

Java: list.contains(x)
来源：http://hz.zhongyouzk.top/gtoipimxgz.html

Go:   slices.Contains(arr, x)
来源：http://hz.guannengcc.top/gtsuunvsij.html

Ruby: arr.include?(x)
来源：http://hz.yj202588.top/gtpqhfhqvs.html

C#:   list.Contains(x)
来源：http://hz.ivvv.top/gtdbvhilkn.html

[D22] 复制数组（避免共享引用）
来源：http://hz.zhaomingkeji.xyz/gtslpzdxqk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.guowangkeji.top/gtqdrzbqbn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.shanyushiyangtech.top/gtkxlogmfd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.nwbrower.top/gtnrnyrwhk.html

TS:   [...arr];
来源：http://hz.ydzc1.top/gtnbcpulsr.html

Java: new ArrayList<>(list);
来源：http://hz.jinqigfzy.top/gtpkahtvuc.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.mhx1999.top/gtbhafjhrp.html

Ruby: arr.dup;  arr.clone
来源：http://hz.aibaodan.cn/gtqidbedvy.html

C#:   new List<int>(list);
来源：http://hz.fengsongda.top/gtktnpigio.html

[D23] reduce 累积计算
来源：http://hz.jinqigfzy.top/gtllldfgzl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.shanyushiyangkeji.top/gtaxeqyvgj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.fengsongda.top/gtvcuqgrqg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zdqjudy.top/gtjvzmihij.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.guowangkeji.top/gtsaxlkzrs.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.iojbl.cn/gthgqaghga.html

Go:   // 手写循环
来源：http://hz.yj202588.top/gtyzprvdxn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yangfankeji.com/gtzuqklajo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.redwolf501.top/gtecmlesma.html

[D24] 字典 / Map 基本操作
来源：http://hz.cucudq.cn/gtdxsxtdju.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yuanzhike.top/gtrdzucjxr.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.xuanzx.com/gtdqgpxycb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.gzhubu.top/gtttqhfepp.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yongpay.top/gtbyghwhzo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yanxiufei.cn/gtgbktpybg.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.xinyue.icu/gtgfmoymgz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.pycfn.com/gtlmdwuudb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.tianlin.xyz/gtztjvhrzv.html

[D25] Set 集合去重与交并差
来源：http://hz.xingfuxueyuan.xyz/gtvjosqtyd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.hnqzz.top/gtpqnwzsds.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.birdmap.top/gtfmfohfbn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zhiwuduotai.top/gtdmpkjcsw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.pycfn.com/gtlhhwfpmx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.wangdashe.top/gthfkgrbyr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.cucudq.cn/gtwavjxnev.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.zhengqikj.top/gtmyhoynod.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.chenlongwang.top/gtmmrpxgrb.html

[D26] 数组转字符串
来源：http://hz.zhijiandao.cn/gthsavsoey.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zhiwuduotai.top/gterhfrhwx.html

PHP:  implode(", ", $arr);
来源：http://hz.havefunace.top/gtgkyadftm.html

JS:   arr.join(", ")
来源：http://hz.cashguo.top/gtietustmu.html

TS:   arr.join(", ")
来源：http://hz.ybcxt.top/gtshpdyecz.html

Java: String.join(", ", list)
来源：http://hz.ppjwa.cn/gtvluptcez.html

Go:   strings.Join(strs, ", ")
来源：http://hz.ydjk.org.cn/gtqvqoglic.html

Ruby: arr.join(", ")
来源：http://hz.hammf.cn/gtzbaqgchq.html

C#:   string.Join(", ", list)
来源：http://hz.zdqjudy.top/gtkkrfdfpp.html

================================================================================
来源：http://hz.jqgfzy.top/gtxntxintl.html

E. 字符串处理
来源：http://hz.fengsongda.top/gtvqtefjew.html

================================================================================
来源：http://hz.jlsjyb.cn/gtejcjxiff.html

[E01] 拼接字符串
来源：http://hz.zhaomingkeji.xyz/gtresflhtr.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.jlsjyb.cn/gttpkzimub.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.pengpengdd.cyou/gtyyuoubas.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jianghu66.top/gtlqzrxzqr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.guowangkeji.top/gtpreumlog.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.gzhubu.top/gtdacnfjec.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yangfankeji.com/gtxkgaacoq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jiagoushi.top/gtnysvcszu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yongpay.top/gtoohspgry.html

[E02] 重复字符串
来源：http://hz.chenzaomai.com/gtonshyopf.html

Py:   "ab" * 3
来源：http://hz.zhengqikj.top/gtbocwioge.html

PHP:  str_repeat("ab", 3);
来源：http://hz.yuanzhike.top/gtcapsokgl.html

JS:   "ab".repeat(3)
来源：http://hz.cashguo.top/gtsgihpsop.html

TS:   "ab".repeat(3)
来源：http://hz.chenzaomai.com/gttrevvzbu.html

Java: "ab".repeat(3)
来源：http://hz.hysaishi.cn/gtdqaenmec.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.0kj1m.cn/gtvgabqgtx.html

Ruby: "ab" * 3
来源：http://hz.xuetiantiany.cn/gtijtdrwni.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.cucudq.cn/gtlurpraap.html

[E03] 截取子串
来源：http://hz.52xcode.cn/gtrgdmedea.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yj202588.top/gtmovsowjr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.shuidangran.top/gtxlkhuvmc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.pycfn.com/gtlltuonle.html

TS:   s.slice(1, 4)
来源：http://hz.shzxlz.cn/gtzbzsduvd.html

Java: s.substring(1, 4)
来源：http://hz.gzhubu.top/gtrdcogdbw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.zdqjudy.top/gtuftisuus.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.fengsongda.top/gtmywimnvh.html

C#:   s.Substring(1, 3)
来源：http://hz.yangfankeji.com/gttlardldm.html

[E04] 查找子串位置
来源：http://hz.0kj1m.cn/gtwcfroeux.html

Py:   s.find("x");  s.index("x")
来源：http://hz.xinyue.icu/gtbzoppfzs.html

PHP:  strpos($s, "x");
来源：http://hz.hongshengwenyu.top/gtxwdjvbec.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zhongyouzk.top/gthtviidmf.html

TS:   s.indexOf("x")
来源：http://hz.birdmap.top/gthdhoukid.html

Java: s.indexOf("x")
来源：http://hz.jianghu66.top/gtvzfukftz.html

Go:   strings.Index(s, "x")
来源：http://hz.quarkkingdee.top/gtubsjpkgi.html

Ruby: s.index("x")
来源：http://hz.ivvv.top/gtfgxfrwgp.html

C#:   s.IndexOf("x")
来源：http://hz.yj20258888.top/gtmoirsfkg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.jqgufenzy.top/gtduhwgnkg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.snrcjt.cn/gtgaaobejf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.sxryk.cn/gtcarjxbhw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.chenlongwang.top/gtguarazlb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.cheryme.top/gtehbdkgcc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.haohaochexian.top/gtzoycbebj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.jinqigfzy.top/gtbemrgcaf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.sufxvd.cn/gtfthlnkfq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.nanxuanxn.top/gtwqlokbfr.html

[E06] 替换子串
来源：http://hz.shzxlz.cn/gtfwojqedw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.fzhhl.top/gtywmiymck.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.9152youxi.cn/gtutincznd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yanxiufei.cn/gtbmpsfqxy.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zycfv.cn/gtqnvyeerc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ywan-chungtsiang.top/gtvqqkgdyt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.ywan-chungtsiang.top/gtljzxikpz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.pengpengdd.cyou/gtitrydjkb.html

C#:   s.Replace("a", "b")
来源：http://hz.feifeiyinyue.top/gtqlajewby.html

[E07] 按分隔符拆分
来源：http://hz.guowangkeji.top/gtuxxsbids.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.nanxuanxn.top/gtxbmpfgey.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.jinqigufen.top/gttdptvrtp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.cheryme.top/gtfqjsftsw.html

TS:   s.split(",")
来源：http://hz.sweek.top/gtmbhcopyg.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.shanyushiyangkeji.top/gtiepdacyr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.tian-w.cn/gtzigkjrjn.html

Ruby: s.split(",");  s.split
来源：http://hz.birdmap.top/gtjebhnbsa.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.yuxming.cn/gtolzclkzm.html

[E08] 数组按分隔符合并
来源：http://hz.ydjk.org.cn/gtzwlyiqki.html

Py:   ",".join(items)
来源：http://hz.xinyue.icu/gtokhjbdaa.html

PHP:  implode(",", $items);
来源：http://hz.haohaochexian.top/gtwuvsnhxj.html

JS:   items.join(",")
来源：http://hz.havefunace.top/gtrpafpkph.html

TS:   items.join(",")
来源：http://hz.jinyuanbaomall.cn/gtybrteixj.html

Java: String.join(",", items)
来源：http://hz.dianchejie.cn/gtardklcbu.html

Go:   strings.Join(items, ",")
来源：http://hz.havefunace.top/gthogtbrai.html

Ruby: items.join(",")
来源：http://hz.316326.xyz/gtgucbcjjp.html

C#:   string.Join(",", items)
来源：http://hz.jlsjyb.cn/gteiafaacl.html

[E09] 去除所有空白字符
来源：http://hz.haohaochexian.top/gttpmwexvq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.ywan-chungtsiang.top/gtgqbiuxmw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.nwbrower.top/gtgzntbkyu.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.hongshengwenyu.top/gtoznqpfed.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.daria6918.cn/gteorepfkg.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.dianchejie.cn/gtoupwniki.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.pengpengdd.cyou/gtkzkrefnr.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.gzhubu.top/gtmswledyd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.ydzc1.top/gtxqhyrhhk.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jqgufenzy.top/gtoobsgvpm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.ydzc1.top/gtrahhogbs.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.nanxuanxn.top/gtkfzhcteo.html

JS:   "7".padStart(3, "0")
来源：http://hz.andypj.xyz/gtumxuurff.html

TS:   "7".padStart(3, "0")
来源：http://hz.hammf.cn/gtpsxhpgjg.html

Java: String.format("%03d", 7)
来源：http://hz.pycfn.com/gtymazspqg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.chenzaomai.com/gthyaxcaxw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zhaomingkeji.xyz/gtfrrvyfxr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.chenlongwang.top/gtwsynpkud.html

[E11] 反转字符串
来源：http://hz.andypj.xyz/gtnpgszqup.html

Py:   s[::-1]
来源：http://hz.jianghu66.top/gtnxpiwaaf.html

PHP:  strrev($s);
来源：http://hz.sufxvd.cn/gthklavcwe.html

JS:   [...s].reverse().join("")
来源：http://hz.haohaochexian.top/gtaflnistk.html

TS:   [...s].reverse().join("")
来源：http://hz.ivvv.top/gthajdrrlw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.sysykeji.top/gtsbugzotv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.hnxiangtu.top/gtwdtmbylz.html

Ruby: s.reverse
来源：http://hz.mhx1999.top/gtklrxzpyf.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.ywan-chungtsiang.top/gtrpydjvml.html

[E12] 统计某字符出现次数
来源：http://hz.fzhhl.top/gtznmaahxd.html

Py:   s.count("a")
来源：http://hz.zhixingplan.top/gtiffepwce.html

PHP:  substr_count($s, "a");
来源：http://hz.zhixingplan.top/gtsyzwpeuc.html

JS:   s.split("a").length - 1
来源：http://hz.cashguo.top/gtpgguhvav.html

TS:   s.split("a").length - 1
来源：http://hz.xylfe.cn/gtygiedabp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yonumen.top/gtaopylthv.html

Go:   strings.Count(s, "a")
来源：http://hz.xinyue.icu/gtmdchscmf.html

Ruby: s.count("a")
来源：http://hz.chenzaomai.com/gtjrmaxqhy.html

C#:   s.Count(c => c == 'a')
来源：http://hz.shuidangran.top/gtendbzdik.html

[E13] 逐字符遍历
来源：http://hz.yanxiufei.cn/gtrbsrgadd.html

Py:   for ch in s: print(ch)
来源：http://hz.zycfv.cn/gthlyyjubv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.cheryme.top/gtnblmlpeo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.daxiang520.top/gttqsbjpir.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xuetiantiany.cn/gtstuitycu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.sufxvd.cn/gtcvhentse.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.gaohongyu789.top/gtopdgmeuf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.wangdashe.top/gtrboblqeq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.redwolf501.top/gtprintato.html

[E14] URL 编码与 Base64
来源：http://hz.yuanzhike.top/gtoybohbsr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.xinyue.icu/gthmcskldv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.chenzaomai.com/gtqzvbzjfc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yanxiufei.cn/gtmogbncsn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jinqigfzy.top/gtnfbhxvfb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.zhongyouzk.top/gtkxgcvktg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.gaohongyu789.top/gtnbqbzvom.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.kuanghao11.cn/gtciipcccn.html


<!-- 参考信息 -->