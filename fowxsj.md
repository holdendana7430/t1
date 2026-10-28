代发 wailian999

TS:   arr.slice(1, 4);
来源：http://hz.redwolf501.top/gtirfefoka.html

Java: list.subList(1, 4);
来源：http://hz.zhoulong.xyz/gthmgseutp.html

Go:   arr[1:4]
来源：http://hz.zycfv.cn/gtrvntgexo.html

Ruby: arr[1, 3]
来源：http://hz.zhixingplan.top/gtlnagbyfo.html

C#:   list.GetRange(1, 3);
来源：http://hz.shanyushiyangkeji.top/gtlgqvyvkm.html

[D08] 合并两个数组
来源：http://hz.ppjwa.cn/gtxrhoprlj.html

Py:   a + b;  a.extend(b)
来源：http://hz.redwolf501.top/gtexnzbhpc.html

PHP:  array_merge($a, $b);
来源：http://hz.andypj.xyz/gtrglummfl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yongpay.top/gtjuhwszjx.html

TS:   [...a, ...b];
来源：http://hz.shangyingyoupin.top/gtmchagayr.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.snrcjt.cn/gtfytxiscf.html

Go:   append(a, b...)
来源：http://hz.jinghuilouyu.cn/gtpzmxpkge.html

Ruby: a + b;  a.concat(b)
来源：http://hz.shzxlz.cn/gtpnxclhwe.html

C#:   a.Concat(b).ToList()
来源：http://hz.tian-w.cn/gtyklwknrz.html

[D09] 排序（升序）
来源：http://hz.aibaodan.cn/gtmynaszyk.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.gzhubu.top/gthjeluigl.html

PHP:  sort($arr);
来源：http://hz.nwbrower.top/gtkiyjvqsp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.ydjk.org.cn/gtdcapddod.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.chenjidiqi.icu/gtrsmlpeqm.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.pengpengdd.cyou/gtnjencmeb.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.nanxinkj.top/gtoocqunmc.html

Ruby: arr.sort
来源：http://hz.zycfv.cn/gtzyrmfqro.html

C#:   list.Sort();
来源：http://hz.316326.xyz/gtjphlqzxe.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.c1oappe.top/gtmbscbylm.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yj20258888.top/gtkyadylxf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.smart0.xyz/gtvscaheqd.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zdqjudy.top/gtwcvdlxwx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yuxming.cn/gtgwrwsqxw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.quarkkingdee.top/gtjsaknfna.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.c1oappe.top/gtisyvhira.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.shanyushiyangkeji.top/gtttqqzuwm.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.hfpthk.cn/gtvjpyhozm.html

[D11] 反转数组
来源：http://hz.pengpengdd.cyou/gtfibmttxp.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.jiagoushi.top/gtsxrrfcji.html

PHP:  array_reverse($arr);
来源：http://hz.cucudq.cn/gtdxgsuktk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jyoumei.cn/gtifvbauyd.html

TS:   [...arr].reverse();
来源：http://hz.hywenlv.cn/gtdrvfeqfh.html

Java: Collections.reverse(list);
来源：http://hz.gogol.net.cn/gtujuyfdnh.html

Go:   slices.Reverse(arr)
来源：http://hz.aibaodan.cn/gtvaapasmh.html

Ruby: arr.reverse
来源：http://hz.xinyue.icu/gtxbaqxqbw.html

C#:   list.Reverse();
来源：http://hz.zhijiandao.cn/gtgxoxxxuo.html

[D12] 查找元素下标
来源：http://hz.ydjk.org.cn/gtiuuohghr.html

Py:   arr.index(x);  x in arr
来源：http://hz.smart0.xyz/gtcamexzfs.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jqgufenzy.top/gtuxapzykr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ehwqpu.com/gtlluaiwix.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhongyouzk.top/gtqhwhxtjz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.gaohongyu789.top/gtkkueqofe.html

Go:   slices.Index(arr, x)
来源：http://hz.gogol.net.cn/gtzaewkwyw.html

Ruby: arr.index(x)
来源：http://hz.hfpthk.cn/gtwjuarzca.html

C#:   list.IndexOf(x);
来源：http://hz.yuanzhike.top/gtubnnjpra.html

[D13] 过滤（保留满足条件的）
来源：http://hz.hywenlv.cn/gtulxxngdn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.tian-w.cn/gtwvzsvcql.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.smart0.xyz/gtnakohsoa.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zhoulong.xyz/gtdptergeg.html

TS:   arr.filter(x => x > 3)
来源：http://hz.xuanzx.com/gtxavgybkz.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.guannengcc.top/gtsicnhdqp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yangfankeji.com/gttmpywqiu.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.chenlongwang.top/gtxjgkzega.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.daxiang520.top/gtywbqwxhf.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yj20258888.top/gtaypkwzbq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.cucudq.cn/gtpdpgurfy.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.xylfe.cn/gtcavyfhnu.html

JS:   arr.map(x => x * 2)
来源：http://hz.zdqjudy.top/gtfxqiltcv.html

TS:   arr.map(x => x * 2)
来源：http://hz.daxiang520.top/gtbiskpzfc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.aibaodan.cn/gtmrxzsqhr.html

Go:   // 手写循环
来源：http://hz.jinqigfzy.top/gtachzdorb.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.tianlin.xyz/gtatenpmxr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.hongshengwenyu.top/gtwvruebes.html

[D15] 去重
来源：http://hz.wangshuangyany.cn/gtzecselsp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.zhoulong.xyz/gtijcritwh.html

PHP:  array_unique($arr);
来源：http://hz.nanxuanxn.top/gtmxucrnui.html

JS:   [...new Set(arr)]
来源：http://hz.quarkkingdee.top/gtdhchemgi.html

TS:   [...new Set(arr)]
来源：http://hz.iojbl.cn/gtcuhimzap.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.wangshuangyany.cn/gtiqyisgvx.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.snrcjt.cn/gttlhvunon.html

Ruby: arr.uniq
来源：http://hz.wangshuangyany.cn/gtzjjhggju.html

C#:   list.Distinct().ToList()
来源：http://hz.52xcode.cn/gtdxqsisue.html

[D16] 求和与平均值
来源：http://hz.zhiwuduotai.top/gthsjnwfji.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jlsjyb.cn/gtlpkdvbmu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.ydjk.org.cn/gtfslhqbdb.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.haohaochexian.top/gtgcmteakn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.havefunace.top/gtojijfqaw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yj20258888.top/gtuodhacha.html

Go:   // 手写循环累加
来源：http://hz.ydzc1.top/gtccsjwrwd.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.ywan-chungtsiang.top/gtlqnwrwae.html

C#:   list.Sum();  list.Average()
来源：http://hz.cucudq.cn/gtjzrvptsf.html

[D17] 最大值与最小值
来源：http://hz.zhongyouzk.top/gtmtwczxwe.html

Py:   max(arr);  min(arr)
来源：http://hz.ppjwa.cn/gtmainyiqb.html

PHP:  max($arr);  min($arr);
来源：http://hz.chenzaomai.com/gtogndkngv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.gaohongyu789.top/gtikhjddsx.html

TS:   Math.max(...arr);
来源：http://hz.cashguo.top/gtrfuowtxo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.cdnleiting.top/gtnperxkss.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.dashuyun.cn/gtkifqelnh.html

Ruby: arr.max;  arr.min
来源：http://hz.ydjk.org.cn/gtsxhzcnoh.html

C#:   list.Max();  list.Min()
来源：http://hz.0kj1m.cn/gthyimnreg.html

[D18] 扁平化嵌套数组
来源：http://hz.birdmap.top/gtkbasqdno.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.redwolf501.top/gtaziyzeex.html

PHP:  array_merge(...$nested);
来源：http://hz.ydjk.org.cn/gtnqmrqfgb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.zdqjudy.top/gtbakpqyop.html

TS:   nested.flat();
来源：http://hz.xingfuxueyuan.xyz/gtqntotfyi.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.xziqi.cn/gtytnwehtq.html

Go:   // 手写双层循环
来源：http://hz.cdnleiting.top/gtbdvmrksd.html

Ruby: nested.flatten
来源：http://hz.cucudq.cn/gtyhvmioei.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zhengqikj.top/gthkclaldi.html

[D19] 按字段分组
来源：http://hz.jinqigufen.top/gtmpddyrwd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.chenjidiqi.icu/gtovkmnmkh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yj20258.top/gtphgsadsk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.yonumen.top/gtgdtcxwmw.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.kuanghao11.cn/gtpjoezozt.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.tanke756.top/gtizdfzwbt.html

Go:   // 手写 map[string][]T
来源：http://hz.wangshuangyany.cn/gtgeasrujh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.vqdsnc.cn/gtwexbvfvg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yuxming.cn/gtwntbuwzn.html

[D20] 统计每个元素出现次数
来源：http://hz.xuetiantiany.cn/gtlraueyle.html

Py:   Counter(arr)
来源：http://hz.hfpthk.cn/gtvdmvpjln.html

PHP:  array_count_values($arr);
来源：http://hz.zhijiandao.cn/gtaupuhlpj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yuanzhike.top/gtqfhrwtuj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.svipenyu.cn/gtckadrdhg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.chenzaomai.com/gtkqeaynkd.html

Go:   // 手写 map[T]int
来源：http://hz.yuanzhike.top/gthxhakist.html

Ruby: arr.tally
来源：http://hz.yueranfly.top/gtgjcspulv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.chenlongwang.top/gtteguhvlm.html

[D21] 判断是否包含某元素
来源：http://hz.xingfuxueyuan.xyz/gtfubyxrls.html

Py:   x in arr
来源：http://hz.pengpengdd.cyou/gtulxdjrmn.html

PHP:  in_array($x, $arr, true);
来源：http://hz.sufxvd.cn/gttliboonj.html

JS:   arr.includes(x)
来源：http://hz.gotoacloud.top/gtxyzprdug.html

TS:   arr.includes(x)
来源：http://hz.zycfv.cn/gtxhozkikd.html

Java: list.contains(x)
来源：http://hz.feifeiyinyue.top/gtyuqwtcpt.html

Go:   slices.Contains(arr, x)
来源：http://hz.iojbl.cn/gtgncijsss.html

Ruby: arr.include?(x)
来源：http://hz.sysykeji.top/gtxcmovntk.html

C#:   list.Contains(x)
来源：http://hz.cqqwz.cn/gtpjukseih.html

[D22] 复制数组（避免共享引用）
来源：http://hz.mhx1999.top/gtxbfwxzal.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.0kj1m.cn/gttlradzyw.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jinghuilouyu.cn/gtudjvwudn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.cucudq.cn/gtfkmiedii.html

TS:   [...arr];
来源：http://hz.xuanzx.com/gtfmmkwdkc.html

Java: new ArrayList<>(list);
来源：http://hz.hnxiangtu.top/gtbmadmudo.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.tian-w.cn/gttjavydxb.html

Ruby: arr.dup;  arr.clone
来源：http://hz.svipenyu.cn/gtjauvckcj.html

C#:   new List<int>(list);
来源：http://hz.aibaodan.cn/gtbdtvpcoq.html

[D23] reduce 累积计算
来源：http://hz.xylfe.cn/gtovlvrnnh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jiagoushi.top/gtbpqjehos.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.cdnleiting.top/gtxifanruh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.aizwys.cn/gtmnouyopt.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jyoumei.cn/gtdhqkjcld.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.0kj1m.cn/gtkrxjrdys.html

Go:   // 手写循环
来源：http://hz.gaohongyu789.top/gtfjvccplx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.ybcxt.top/gtsiscbxhg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.0kj1m.cn/gtguwitble.html

[D24] 字典 / Map 基本操作
来源：http://hz.yj20258.top/gtmcdbetji.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.nanxinkj.top/gtiqyxwwta.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yj20258888.top/gtwdlulzfq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.zhiwuduotai.top/gtwlzzzfbt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.xuetiantiany.cn/gtmvpxradr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.gzhubu.top/gtcvpkdhit.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.cqqwz.cn/gtljlvxjjx.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.nwbrower.top/gtlrbuttef.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zhijiandao.cn/gtslfrerdv.html

[D25] Set 集合去重与交并差
来源：http://hz.gotoacloud.top/gtflgynadf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.cucudq.cn/gtpccffjng.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.ywan-chungtsiang.top/gtehknbiki.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.guannengcc.top/gtoxrtugzk.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.ywan-chungtsiang.top/gtkxvptypx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.nanxuanxn.top/gtbcmjvery.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.daria6918.cn/gtkdxvbgep.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.mhx1999.top/gtrbzdzxsh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.dashuyun.cn/gtliahranu.html

[D26] 数组转字符串
来源：http://hz.gaohongyu789.top/gtdjdkuqyl.html

Py:   ", ".join(map(str, arr))
来源：http://hz.nwbrower.top/gtyisdisaz.html

PHP:  implode(", ", $arr);
来源：http://hz.ppjwa.cn/gttmdrcwvi.html

JS:   arr.join(", ")
来源：http://hz.xziqi.cn/gtwutowdjm.html

TS:   arr.join(", ")
来源：http://hz.zhengqikj.top/gttnstdsrg.html

Java: String.join(", ", list)
来源：http://hz.ppjwa.cn/gtolvwrphf.html

Go:   strings.Join(strs, ", ")
来源：http://hz.fzhhl.top/gtthdegozq.html

Ruby: arr.join(", ")
来源：http://hz.zhixingplan.top/gtbvoamitj.html

C#:   string.Join(", ", list)
来源：http://hz.chenjidiqi.icu/gtpfdgqmyo.html

================================================================================
来源：http://hz.mhx1999.top/gtaksylfga.html

E. 字符串处理
来源：http://hz.gotoacloud.top/gthlwdmvfd.html

================================================================================
来源：http://hz.yonumen.top/gtieqhomyc.html

[E01] 拼接字符串
来源：http://hz.ehwqpu.com/gthqajmavf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yanxiufei.cn/gtjfivosjz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yj20258888.top/gtycbtpxsz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.wangdashe.top/gtipqgkebg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.nanxinkj.top/gtvbswtuef.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.hnqzz.top/gtsqkhqvbf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.havefunace.top/gtghazkboz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yj20258.top/gtezqrhhjz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.hywenlv.cn/gtbgepmmqa.html

[E02] 重复字符串
来源：http://hz.redwolf501.top/gtikvxvoaf.html

Py:   "ab" * 3
来源：http://hz.yuxming.cn/gtndcltbnw.html

PHP:  str_repeat("ab", 3);
来源：http://hz.chenlongwang.top/gtookbanqs.html

JS:   "ab".repeat(3)
来源：http://hz.birdmap.top/gtmhrpndxe.html

TS:   "ab".repeat(3)
来源：http://hz.mhx1999.top/gthfnvwwry.html

Java: "ab".repeat(3)
来源：http://hz.shangyingyoupin.top/gtabjxvkjo.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.smart0.xyz/gtvzrcxzft.html

Ruby: "ab" * 3
来源：http://hz.iojbl.cn/gtauprskzo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.feifeiyinyue.top/gtootuwghi.html

[E03] 截取子串
来源：http://hz.yueranfly.top/gtbdewimrt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.wangdashe.top/gtovcnepek.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.hammf.cn/gtkdhqntra.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.aibaodan.cn/gtgpzeyigm.html

TS:   s.slice(1, 4)
来源：http://hz.bjfxy.top/gteoamongc.html

Java: s.substring(1, 4)
来源：http://hz.yj202588.top/gthfnsuitk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.ydjk.org.cn/gtfsgudpiz.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.hnqzz.top/gtsrhynzli.html

C#:   s.Substring(1, 3)
来源：http://hz.gotoacloud.top/gtofucoher.html

[E04] 查找子串位置
来源：http://hz.ydzc1.top/gtwcligeoh.html

Py:   s.find("x");  s.index("x")
来源：http://hz.zhengqikj.top/gtcbwmgfxc.html

PHP:  strpos($s, "x");
来源：http://hz.ywan-chungtsiang.top/gtzwkeepos.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.bjfxy.top/gtxdsjsgtm.html

TS:   s.indexOf("x")
来源：http://hz.tian-w.cn/gtjwdwlomr.html

Java: s.indexOf("x")
来源：http://hz.yangfankeji.com/gtdrqkthso.html

Go:   strings.Index(s, "x")
来源：http://hz.xuanzx.com/gtoarhpgeb.html

Ruby: s.index("x")
来源：http://hz.ehwqpu.com/gtfievimkf.html

C#:   s.IndexOf("x")
来源：http://hz.zhiwuduotai.top/gtlfjfgcjf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.hongshengwenyu.top/gtbvskxmid.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.fzhhl.top/gtanrifocj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.yuanzhike.top/gtneovogqr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jqgufenzy.top/gteblqlnuh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.cheryme.top/gtnoaubdrp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hnqzz.top/gttdoleozy.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.yj20258.top/gtbbtdbseh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.gotoacloud.top/gtjbmyzntj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jiagoushi.top/gtzpzbicjm.html

[E06] 替换子串
来源：http://hz.xuetiantiany.cn/gtbjbeenwl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jinghuilouyu.cn/gtetwhwcet.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.jinyuanbaomall.cn/gteeiiemgj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.svipenyu.cn/gttordxuwf.html

TS:   s.replaceAll("a", "b")
来源：http://hz.yongpay.top/gtdrodlcxq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.cqqwz.cn/gtwxsgruyq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.vqdsnc.cn/gtzplqlxub.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.sxryk.cn/gtmhmjpgfi.html

C#:   s.Replace("a", "b")
来源：http://hz.hnxiangtu.top/gtcnfwcplg.html

[E07] 按分隔符拆分
来源：http://hz.ehwqpu.com/gtwwovxghk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.feifeiyinyue.top/gtotfepybj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.hammf.cn/gtygmvawlj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.hysaishi.cn/gtqqfikgjz.html

TS:   s.split(",")
来源：http://hz.hnqzz.top/gtfwjhgndj.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.zhoulong.xyz/gthqajjzpi.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yuanzhike.top/gtcnpmfgkx.html

Ruby: s.split(",");  s.split
来源：http://hz.52xcode.cn/gtbgrjbsau.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.cashguo.top/gtzcmnfxub.html

[E08] 数组按分隔符合并
来源：http://hz.cqqwz.cn/gtigjqicyb.html

Py:   ",".join(items)
来源：http://hz.yj202588.top/gtbimeeivo.html

PHP:  implode(",", $items);
来源：http://hz.nanxuanxn.top/gtufahaazh.html

JS:   items.join(",")
来源：http://hz.aibaodan.cn/gtymxhampy.html

TS:   items.join(",")
来源：http://hz.wangdashe.top/gtwzbeiexp.html

Java: String.join(",", items)
来源：http://hz.zhixingplan.top/gtkzikxzpz.html

Go:   strings.Join(items, ",")
来源：http://hz.hywenlv.cn/gtebwpoaiq.html

Ruby: items.join(",")
来源：http://hz.ydzc1.top/gtlyiwvnws.html

C#:   string.Join(",", items)
来源：http://hz.gotoacloud.top/gtazvdzrjl.html

[E09] 去除所有空白字符
来源：http://hz.cqqwz.cn/gttipvurtl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.sufxvd.cn/gtogerylcl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.cqqwz.cn/gtwdovcwiv.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.chenzaomai.com/gtruongguw.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.gotoacloud.top/gtnqehiyds.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.hfpthk.cn/gtmrtbatnu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.feifeiyinyue.top/gtrysphagd.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.aibaodan.cn/gtcapiplif.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.ywan-chungtsiang.top/gttdmaerdt.html

[E10] 左侧补零 / 定长填充
来源：http://hz.gogol.net.cn/gtyqbqdxmg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.wangdashe.top/gttgmppaki.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yangfankeji.com/gtlxunhtej.html

JS:   "7".padStart(3, "0")
来源：http://hz.xuetiantiany.cn/gtjrmovrtz.html

TS:   "7".padStart(3, "0")
来源：http://hz.daxiang520.top/gtwerdyswo.html

Java: String.format("%03d", 7)
来源：http://hz.vqdsnc.cn/gtnsvociva.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.daxiang520.top/gtkmirralt.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.ppjwa.cn/gtxwmqrwho.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.gaohongyu789.top/gtsjkqgppf.html

[E11] 反转字符串
来源：http://hz.chenlongwang.top/gtbchtnsjm.html

Py:   s[::-1]
来源：http://hz.ywan-chungtsiang.top/gtzbjftfso.html

PHP:  strrev($s);
来源：http://hz.guowangkeji.top/gtdovcyrva.html

JS:   [...s].reverse().join("")
来源：http://hz.hammf.cn/gtpzjktoey.html

TS:   [...s].reverse().join("")
来源：http://hz.sweek.top/gtxastzawm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.xingfuxueyuan.xyz/gttxvvlerm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.sufxvd.cn/gtumbvoqxc.html

Ruby: s.reverse
来源：http://hz.jinghuilouyu.cn/gtbpuxcgxe.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yuxming.cn/gtxyzrwgwu.html

[E12] 统计某字符出现次数
来源：http://hz.nanxuanxn.top/gtoqndyamv.html

Py:   s.count("a")
来源：http://hz.xuanzx.com/gtjkjjglqi.html

PHP:  substr_count($s, "a");
来源：http://hz.zhaomingkeji.xyz/gtynzxsufu.html

JS:   s.split("a").length - 1
来源：http://hz.c1oappe.top/gtlbyscysl.html

TS:   s.split("a").length - 1
来源：http://hz.sufxvd.cn/gtzzgvydlw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.xinyue.icu/gtvjzlkzyy.html

Go:   strings.Count(s, "a")
来源：http://hz.ehwqpu.com/gtjqdidjux.html

Ruby: s.count("a")
来源：http://hz.sweek.top/gtxjbvysmg.html

C#:   s.Count(c => c == 'a')
来源：http://hz.cdnleiting.top/gtfzdjiqzk.html

[E13] 逐字符遍历
来源：http://hz.sufxvd.cn/gtrfusvxjr.html

Py:   for ch in s: print(ch)
来源：http://hz.cdnleiting.top/gttmxonzwz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.ydjk.org.cn/gthetsngix.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.daxiang520.top/gtkjusgpxn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ppjwa.cn/gtwnoyyifv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jinqigufen.top/gtpgymaumy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.bjfxy.top/gtyhnwfnix.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.feifeiyinyue.top/gtrrghfgev.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.ydzc1.top/gthhtmnhhc.html

[E14] URL 编码与 Base64
来源：http://hz.yanxiufei.cn/gtigigsqys.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.redwolf501.top/gtdrsppgyz.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.iojbl.cn/gtaonovftu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.xuetiantiany.cn/gtzyrtvmch.html


<!-- 参考信息 -->