代发 wailian999

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.gzhubu.top/gtycmvsgiz.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.jinqigfzy.top/gtwbdszccf.html

[D05] 访问与修改元素
来源：http://hz.jianghu66.top/gtkhwmqeqe.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.aibaodan.cn/gtiiitciib.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.gzhubu.top/gtvsixwhxg.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.316326.xyz/gttrocjslq.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.jlsjyb.cn/gtocvpduwn.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.ehwqpu.com/gtzrsbvhuh.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.hfpthk.cn/gtvnabscoo.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.zycfv.cn/gtbaimwcii.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jinyuanbaomall.cn/gtdulslxld.html

[D06] 数组长度
来源：http://hz.zhiwuduotai.top/gttlhtyoij.html

Py:   len(arr)
来源：http://hz.ywan-chungtsiang.top/gteqmqfrnd.html

PHP:  count($arr);
来源：http://hz.sysykeji.top/gtjnhdnfyu.html

JS:   arr.length
来源：http://hz.zhixingplan.top/gtvvlckxch.html

TS:   arr.length
来源：http://hz.xylfe.cn/gtgxkmidbm.html

Java: list.size();
来源：http://hz.jyoumei.cn/gtbtdufdhf.html

Go:   len(arr)
来源：http://hz.nwbrower.top/gtavngmocg.html

Ruby: arr.length; arr.size
来源：http://hz.shzxlz.cn/gttgyzvbak.html

C#:   list.Count;
来源：http://hz.zycfv.cn/gtgjzrcxxn.html

[D07] 切片 / 取子数组
来源：http://hz.ppjwa.cn/gtvtqdtxcc.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.cheryme.top/gtzrivjrfp.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.cqqwz.cn/gtbmwzcjxv.html

JS:   arr.slice(1, 4);
来源：http://hz.sufxvd.cn/gtyzcxeygt.html

TS:   arr.slice(1, 4);
来源：http://hz.dianchejie.cn/gtvadqanwr.html

Java: list.subList(1, 4);
来源：http://hz.shuidangran.top/gtzgmqlwhn.html

Go:   arr[1:4]
来源：http://hz.xinyue.icu/gtckuhhtqw.html

Ruby: arr[1, 3]
来源：http://hz.guowangkeji.top/gtgmnyynlp.html

C#:   list.GetRange(1, 3);
来源：http://hz.ppjwa.cn/gtbpkgjvuc.html

[D08] 合并两个数组
来源：http://hz.shanyushiyangtech.top/gtiytofoyd.html

Py:   a + b;  a.extend(b)
来源：http://hz.ehwqpu.com/gtmfjvqaln.html

PHP:  array_merge($a, $b);
来源：http://hz.vqdsnc.cn/gtgromleyj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.316326.xyz/gtdmwwnunq.html

TS:   [...a, ...b];
来源：http://hz.nwbrower.top/gtcebnzeds.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.shangyingyoupin.top/gthvflcbop.html

Go:   append(a, b...)
来源：http://hz.sysykeji.top/gtusozhzxz.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jinqigfzy.top/gtadyqcsqu.html

C#:   a.Concat(b).ToList()
来源：http://hz.aibaodan.cn/gtqnwczuvh.html

[D09] 排序（升序）
来源：http://hz.jqgfzy.top/gtotdlmpxp.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cqqwz.cn/gtucqcqrlh.html

PHP:  sort($arr);
来源：http://hz.nwbrower.top/gtupqugnxp.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.cashguo.top/gtogeazfij.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.guannengcc.top/gtsmeicpnr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.jqgfzy.top/gtnavigqgx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.gaohongyu789.top/gttcuozclx.html

Ruby: arr.sort
来源：http://hz.zhengqikj.top/gteiqitqdf.html

C#:   list.Sort();
来源：http://hz.kuanghao11.cn/gtfsccbnim.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.mhx1999.top/gtmmyomzll.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.hywenlv.cn/gtjeqygqje.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zdqjudy.top/gtnzpunlgz.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ybcxt.top/gtcyjnoxxk.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.guowangkeji.top/gtruqviwej.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.xziqi.cn/gtmubkfkri.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.dianchejie.cn/gtkaccvbbq.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.ehwqpu.com/gtklrvgfzn.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.yj202588.top/gtqsrrhtkw.html

[D11] 反转数组
来源：http://hz.guannengcc.top/gtjpxzjokv.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zhixingplan.top/gtrepiznsn.html

PHP:  array_reverse($arr);
来源：http://hz.dianchejie.cn/gtmesqhfaz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.xuanzx.com/gtmvjnyohm.html

TS:   [...arr].reverse();
来源：http://hz.xingfuxueyuan.xyz/gtwmsomxro.html

Java: Collections.reverse(list);
来源：http://hz.sufxvd.cn/gtabveztim.html

Go:   slices.Reverse(arr)
来源：http://hz.jqgufenzy.top/gtjfiupquo.html

Ruby: arr.reverse
来源：http://hz.shzxlz.cn/gtnklfihif.html

C#:   list.Reverse();
来源：http://hz.xinyue.icu/gteokrtclk.html

[D12] 查找元素下标
来源：http://hz.hnxiangtu.top/gtkuwwghqk.html

Py:   arr.index(x);  x in arr
来源：http://hz.jqgufenzy.top/gtbiwqhkwn.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.tianlin.xyz/gtzprriisr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yj20258.top/gtnqcrdsuk.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yongpay.top/gtwmrwqvmu.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yj20258888.top/gtheqiqqgk.html

Go:   slices.Index(arr, x)
来源：http://hz.zhengqikj.top/gtvcigaprc.html

Ruby: arr.index(x)
来源：http://hz.birdmap.top/gtntnpwncq.html

C#:   list.IndexOf(x);
来源：http://hz.aizwys.cn/gtysqpckgg.html

[D13] 过滤（保留满足条件的）
来源：http://hz.birdmap.top/gttykopsvu.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.yvedp.cn/gtkoabxqld.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.wangshuangyany.cn/gtzepmreja.html

JS:   arr.filter(x => x > 3)
来源：http://hz.quarkkingdee.top/gtbhrstjnd.html

TS:   arr.filter(x => x > 3)
来源：http://hz.shuidangran.top/gteblmeoye.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.9152youxi.cn/gtnipwbuzn.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.sysykeji.top/gtmvokgcmp.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.bjfxy.top/gthlewiedb.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.pengpengdd.cyou/gtcvfzvaan.html

[D14] 映射转换（每个元素变形）
来源：http://hz.zhengqikj.top/gttulsfvsu.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jianghu66.top/gtgxxlkrqg.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.birdmap.top/gtzwohnegy.html

JS:   arr.map(x => x * 2)
来源：http://hz.wangdashe.top/gtsifkgzoe.html

TS:   arr.map(x => x * 2)
来源：http://hz.smart0.xyz/gtrxztqhdk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.xuetiantiany.cn/gtuxzlnawc.html

Go:   // 手写循环
来源：http://hz.yonumen.top/gtpqvsxhjp.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.shangyingyoupin.top/gtzwxskbtu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.9152youxi.cn/gtwnmqqrsj.html

[D15] 去重
来源：http://hz.sweek.top/gttfgfxlaz.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yj20258888.top/gtekeyblkw.html

PHP:  array_unique($arr);
来源：http://hz.shuidangran.top/gtkjxlmadp.html

JS:   [...new Set(arr)]
来源：http://hz.yj20258.top/gtvumbitaa.html

TS:   [...new Set(arr)]
来源：http://hz.xuetiantiany.cn/gtdivzuxbe.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.birdmap.top/gtynepqddh.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.jinghuilouyu.cn/gtkdkgrxia.html

Ruby: arr.uniq
来源：http://hz.tianlin.xyz/gtzugcjwii.html

C#:   list.Distinct().ToList()
来源：http://hz.yongpay.top/gttwjqepkx.html

[D16] 求和与平均值
来源：http://hz.yj202588.top/gtwjjrvbpr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.birdmap.top/gthqzjkade.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.chenjidiqi.icu/gtbehahtks.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jyoumei.cn/gtkvfviwwk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yongpay.top/gtowtwwpgf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.xuetiantiany.cn/gtbxducfru.html

Go:   // 手写循环累加
来源：http://hz.aibaodan.cn/gtvynrcyiq.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jiagoushi.top/gtyqiywjmh.html

C#:   list.Sum();  list.Average()
来源：http://hz.52xcode.cn/gtnemyjcxm.html

[D17] 最大值与最小值
来源：http://hz.jianghu66.top/gtwezljmhe.html

Py:   max(arr);  min(arr)
来源：http://hz.jianghu66.top/gtvbdpyxst.html

PHP:  max($arr);  min($arr);
来源：http://hz.ydzc1.top/gtgetbjqnd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.andypj.xyz/gtkrhruzga.html

TS:   Math.max(...arr);
来源：http://hz.wangshuangyany.cn/gtirbqugbt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.guannengcc.top/gttaxpzluo.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yangfankeji.com/gtikabawam.html

Ruby: arr.max;  arr.min
来源：http://hz.316326.xyz/gtkhvxvtjx.html

C#:   list.Max();  list.Min()
来源：http://hz.zhaomingkeji.xyz/gtesmvalyr.html

[D18] 扁平化嵌套数组
来源：http://hz.tianlin.xyz/gtvlwizjxz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zhoulong.xyz/gttgyfriun.html

PHP:  array_merge(...$nested);
来源：http://hz.zhijiandao.cn/gtbgbkugvf.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.haohaochexian.top/gthbjwefis.html

TS:   nested.flat();
来源：http://hz.kuanghao11.cn/gtpvqcfvwy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.gzhubu.top/gtkuspuyhz.html

Go:   // 手写双层循环
来源：http://hz.jinyuanbaomall.cn/gtgftmpvpy.html

Ruby: nested.flatten
来源：http://hz.xinyue.icu/gtbrvqqrxy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.jinqigfzy.top/gtzzumhgtq.html

[D19] 按字段分组
来源：http://hz.ybcxt.top/gtbqbksgwa.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.kuanghao11.cn/gtshtgapnb.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.iojbl.cn/gtecbohrhz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.zhoulong.xyz/gtxcgqeipr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.daxiang520.top/gtmoklswjy.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zdqjudy.top/gtjhqdiwpo.html

Go:   // 手写 map[string][]T
来源：http://hz.xylfe.cn/gtxvbnkfax.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.jinqigfzy.top/gtglnfguvp.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.chenjidiqi.icu/gtrmktzckv.html

[D20] 统计每个元素出现次数
来源：http://hz.shuidangran.top/gtlwixdngm.html

Py:   Counter(arr)
来源：http://hz.jinghuilouyu.cn/gtveitbsme.html

PHP:  array_count_values($arr);
来源：http://hz.haohaochexian.top/gtmbcpxxru.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jqgufenzy.top/gtmsoolwjc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhaomingkeji.xyz/gtnkqicazh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.zhongyouzk.top/gtqlovxjrh.html

Go:   // 手写 map[T]int
来源：http://hz.dianchejie.cn/gtqritacmm.html

Ruby: arr.tally
来源：http://hz.dianchejie.cn/gtarnrnnig.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.nanxinkj.top/gtccaqojjn.html

[D21] 判断是否包含某元素
来源：http://hz.hfpthk.cn/gtxeliksdf.html

Py:   x in arr
来源：http://hz.yueranfly.top/gtqjzhrjnq.html

PHP:  in_array($x, $arr, true);
来源：http://hz.zycfv.cn/gtcutwbgmx.html

JS:   arr.includes(x)
来源：http://hz.pengpengdd.cyou/gttvkdkkrd.html

TS:   arr.includes(x)
来源：http://hz.yangfankeji.com/gthpjesskv.html

Java: list.contains(x)
来源：http://hz.shanyushiyangtech.top/gtitkgyluq.html

Go:   slices.Contains(arr, x)
来源：http://hz.xinyue.icu/gtqfswjqtf.html

Ruby: arr.include?(x)
来源：http://hz.quarkkingdee.top/gtdukocnoj.html

C#:   list.Contains(x)
来源：http://hz.ydjk.org.cn/gtwviaemgx.html

[D22] 复制数组（避免共享引用）
来源：http://hz.xingfuxueyuan.xyz/gtatwktvor.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jinqigufen.top/gtvtqhusgk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yj20258888.top/gtipksvwns.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.nwbrower.top/gtfbhjjpfl.html

TS:   [...arr];
来源：http://hz.fzhhl.top/gtcxkdwjql.html

Java: new ArrayList<>(list);
来源：http://hz.aizwys.cn/gtuymhddjj.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yvedp.cn/gtwnplcoxa.html

Ruby: arr.dup;  arr.clone
来源：http://hz.redwolf501.top/gtvezdmckf.html

C#:   new List<int>(list);
来源：http://hz.ppjwa.cn/gtpiytufub.html

[D23] reduce 累积计算
来源：http://hz.zhijiandao.cn/gtslzkvxtl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.shanyushiyangkeji.top/gtgkxkfifc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.kuanghao11.cn/gtrznxvvlz.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhiwuduotai.top/gtgwdasyqh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.fengsongda.top/gtwsnqzzcu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.xylfe.cn/gthapwzfcv.html

Go:   // 手写循环
来源：http://hz.wangdashe.top/gtvzznwozn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.jqgfzy.top/gtlippicwg.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.quarkkingdee.top/gteldmktza.html

[D24] 字典 / Map 基本操作
来源：http://hz.hfpthk.cn/gthdlvgdqt.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.meibo888.top/gtuqwrpycq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.sxryk.cn/gtvczvwxzr.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jqgufenzy.top/gthuuaobvg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.sysykeji.top/gthqcsegig.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yuxming.cn/gtpcutkwfx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ehwqpu.com/gttglarbdy.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zycfv.cn/gtickrvgit.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.shanyushiyangtech.top/gtccksaenm.html

[D25] Set 集合去重与交并差
来源：http://hz.yongpay.top/gtogyfcznx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yj20258888.top/gtyuvoawzq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.ehwqpu.com/gtwbbbbofm.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.hammf.cn/gtiyypdugp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.9152youxi.cn/gtewxvwibr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.9152youxi.cn/gtbcmzspct.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.zycfv.cn/gtuqgoegli.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yueranfly.top/gtyzxxofdd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.sweek.top/gtidmubsqd.html

[D26] 数组转字符串
来源：http://hz.mhx1999.top/gtiwkqthpb.html

Py:   ", ".join(map(str, arr))
来源：http://hz.yuanzhike.top/gtrapqwkyt.html

PHP:  implode(", ", $arr);
来源：http://hz.gotoacloud.top/gteecnioia.html

JS:   arr.join(", ")
来源：http://hz.gaohongyu789.top/gtgsvsqtsf.html

TS:   arr.join(", ")
来源：http://hz.yj20258.top/gtrspsqkpa.html

Java: String.join(", ", list)
来源：http://hz.jqgfzy.top/gtwrunnotb.html

Go:   strings.Join(strs, ", ")
来源：http://hz.jiagoushi.top/gtvudkdnik.html

Ruby: arr.join(", ")
来源：http://hz.zhoulong.xyz/gtnnauzvkl.html

C#:   string.Join(", ", list)
来源：http://hz.nanxinkj.top/gtboxakqlj.html

================================================================================
来源：http://hz.redwolf501.top/gtiyrvxxnv.html

E. 字符串处理
来源：http://hz.andypj.xyz/gtpmceydtm.html

================================================================================
来源：http://hz.jyoumei.cn/gtsghqbjgf.html

[E01] 拼接字符串
来源：http://hz.jqgfzy.top/gtnpindtuu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.jqgfzy.top/gtowzqynbw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yangfankeji.com/gtmqkpofdk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hammf.cn/gttzacqygd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.0kj1m.cn/gtyvctoyrz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.gzhubu.top/gtasraetjb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.cheryme.top/gtmmrkmtva.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.shanyushiyangtech.top/gtxgrtqdri.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zycfv.cn/gtnuvxhflr.html

[E02] 重复字符串
来源：http://hz.ehwqpu.com/gtytfykthh.html

Py:   "ab" * 3
来源：http://hz.yuanzhike.top/gtekmtilbg.html

PHP:  str_repeat("ab", 3);
来源：http://hz.fengsongda.top/gtchdeavem.html

JS:   "ab".repeat(3)
来源：http://hz.zdqjudy.top/gtlkhervun.html

TS:   "ab".repeat(3)
来源：http://hz.haohaochexian.top/gtsdjrtsoo.html

Java: "ab".repeat(3)
来源：http://hz.ydzc1.top/gtspvhvsbe.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.nanxuanxn.top/gtxdgeueqd.html

Ruby: "ab" * 3
来源：http://hz.hnxiangtu.top/gtsoyloefm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.pycfn.com/gtktjkmosy.html

[E03] 截取子串
来源：http://hz.zhongyouzk.top/gthjesoqpd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.haohaochexian.top/gthdnznywa.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.jlsjyb.cn/gtmlcnnwsm.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yangfankeji.com/gtbwtxrofw.html

TS:   s.slice(1, 4)
来源：http://hz.aibaodan.cn/gtbvwqauqd.html

Java: s.substring(1, 4)
来源：http://hz.nwbrower.top/gtrhjwemsx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.mhx1999.top/gtaoalhjjy.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.hfpthk.cn/gtfpdqyfej.html

C#:   s.Substring(1, 3)
来源：http://hz.zhijiandao.cn/gthmczeyno.html

[E04] 查找子串位置
来源：http://hz.jiagoushi.top/gtebuhkrqo.html

Py:   s.find("x");  s.index("x")
来源：http://hz.vqdsnc.cn/gtndqxfjch.html

PHP:  strpos($s, "x");
来源：http://hz.jianghu66.top/gtfwijvdqe.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.ydjk.org.cn/gtjwnzgnpu.html

TS:   s.indexOf("x")
来源：http://hz.yj20258888.top/gtymbyfxvi.html

Java: s.indexOf("x")
来源：http://hz.9152youxi.cn/gtxjygvzuv.html

Go:   strings.Index(s, "x")
来源：http://hz.zhijiandao.cn/gtycssemov.html

Ruby: s.index("x")
来源：http://hz.chenlongwang.top/gtcbbhveyp.html

C#:   s.IndexOf("x")
来源：http://hz.c1oappe.top/gtsysvpvau.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.haohaochexian.top/gtfhoxhyks.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.shangyingyoupin.top/gtfqtcabzq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.fzhhl.top/gtofefgcdd.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.dashuyun.cn/gtjdsbrkjz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zhijiandao.cn/gtiuvwriet.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xingfuxueyuan.xyz/gtjfxyfwvu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.shanyushiyangkeji.top/gtywwtdjoc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.sysykeji.top/gtmvlzpnyt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.nanxuanxn.top/gtgzkqdbkc.html

[E06] 替换子串
来源：http://hz.andypj.xyz/gttnowzdbg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jinqigfzy.top/gtpsqxjzbc.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.fzhhl.top/gtlzeparjm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.andypj.xyz/gtprwhiuud.html

TS:   s.replaceAll("a", "b")
来源：http://hz.cheryme.top/gtmzpmlaci.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hammf.cn/gtzuilimyq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.jinghuilouyu.cn/gtihpkcala.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.gaohongyu789.top/gteoiwrpsi.html

C#:   s.Replace("a", "b")
来源：http://hz.jinqigufen.top/gtyreiptrb.html

[E07] 按分隔符拆分
来源：http://hz.aibaodan.cn/gtrfgkdabo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.meibo888.top/gtcrqljkqc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.guowangkeji.top/gtjxqkplfw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.birdmap.top/gtekkegnhb.html

TS:   s.split(",")
来源：http://hz.yonumen.top/gtnkllzdzr.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.chenjidiqi.icu/gtshtbljbc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.bjfxy.top/gtpkbxjcxr.html

Ruby: s.split(",");  s.split
来源：http://hz.hammf.cn/gttuqhspqb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.guannengcc.top/gtowwjlmze.html

[E08] 数组按分隔符合并
来源：http://hz.feifeiyinyue.top/gtxazvmbxr.html

Py:   ",".join(items)
来源：http://hz.yuxming.cn/gtnoyvvqxy.html

PHP:  implode(",", $items);
来源：http://hz.yuxming.cn/gtdraldgon.html

JS:   items.join(",")
来源：http://hz.xuanzx.com/gtyxnksuad.html

TS:   items.join(",")
来源：http://hz.ppjwa.cn/gtylwzomvq.html

Java: String.join(",", items)
来源：http://hz.pycfn.com/gtgspzigbs.html

Go:   strings.Join(items, ",")
来源：http://hz.andypj.xyz/gtrtftgtdh.html

Ruby: items.join(",")
来源：http://hz.smart0.xyz/gtvvdodpvn.html

C#:   string.Join(",", items)
来源：http://hz.shzxlz.cn/gtqdkbmwth.html

[E09] 去除所有空白字符
来源：http://hz.yueranfly.top/gtsqblduuz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.tian-w.cn/gtiajxlyxa.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.chenjidiqi.icu/gtqznjatnj.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.hfpthk.cn/gtgoseqeju.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.nanxinkj.top/gtzyohpxog.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.wangshuangyany.cn/gthgfhqeuz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xinyue.icu/gtltoennrm.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.pengpengdd.cyou/gtteijocsc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yongpay.top/gtxjwnzlpv.html

[E10] 左侧补零 / 定长填充
来源：http://hz.shzxlz.cn/gtclbihtxa.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.tianlin.xyz/gtjhsbczqn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.dianchejie.cn/gtkivjaqvd.html

JS:   "7".padStart(3, "0")
来源：http://hz.yj20258888.top/gtiduupikn.html

TS:   "7".padStart(3, "0")
来源：http://hz.cucudq.cn/gtvckdqkbb.html

Java: String.format("%03d", 7)
来源：http://hz.jinqigfzy.top/gtrdipmfts.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.hongshengwenyu.top/gthaqjsyxr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.cdnleiting.top/gtwrewmtqs.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.shanyushiyangtech.top/gtunhfdigb.html

[E11] 反转字符串
来源：http://hz.tianlin.xyz/gtxowrelws.html

Py:   s[::-1]
来源：http://hz.svipenyu.cn/gtwjcmysuo.html

PHP:  strrev($s);
来源：http://hz.sxryk.cn/gthqtcemjn.html

JS:   [...s].reverse().join("")
来源：http://hz.xinyue.icu/gtzdgfuioz.html

TS:   [...s].reverse().join("")
来源：http://hz.yangfankeji.com/gtfpexmane.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.andypj.xyz/gtpshnuwkf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.hfpthk.cn/gtsdhswtke.html


<!-- 参考信息 -->