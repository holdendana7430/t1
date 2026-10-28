代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://hz.snrcjt.cn/gtpbgwxkbu.html

[D08] 合并两个数组
来源：http://hz.xziqi.cn/gtmnshkrcz.html

Py:   a + b;  a.extend(b)
来源：http://hz.shanyushiyangtech.top/gtukseytpo.html

PHP:  array_merge($a, $b);
来源：http://hz.chenzaomai.com/gtnaygxdye.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.aibaodan.cn/gtyzjluolv.html

TS:   [...a, ...b];
来源：http://hz.chenjidiqi.icu/gtmfnhzied.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.haohaochexian.top/gtebxtbzig.html

Go:   append(a, b...)
来源：http://hz.xylfe.cn/gtgomwfavz.html

Ruby: a + b;  a.concat(b)
来源：http://hz.52xcode.cn/gtibeywrjd.html

C#:   a.Concat(b).ToList()
来源：http://hz.sweek.top/gttwuzmjsv.html

[D09] 排序（升序）
来源：http://hz.zhoulong.xyz/gtjmiudzzt.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.9152youxi.cn/gtkfpuflqq.html

PHP:  sort($arr);
来源：http://hz.ydzc1.top/gtclsujyhi.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.xziqi.cn/gtwitbuduw.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.tianlin.xyz/gtkmdcwwpu.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.316326.xyz/gtuemtaoqu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.shanyushiyangkeji.top/gtfvxaewwm.html

Ruby: arr.sort
来源：http://hz.cucudq.cn/gtreumqbyx.html

C#:   list.Sort();
来源：http://hz.gogol.net.cn/gtyolmmzus.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.meibo888.top/gtdgcqwqtp.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.aibaodan.cn/gtzlsxmczg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hammf.cn/gtbqtgtugy.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shanyushiyangtech.top/gtocnusirt.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.feifeiyinyue.top/gtttwfitll.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.shangyingyoupin.top/gtwvadljbc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jiagoushi.top/gtlsdbbjts.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.ydzc1.top/gtbgocdkxb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.cashguo.top/gtknuzhstq.html

[D11] 反转数组
来源：http://hz.ybcxt.top/gtgfaotyxu.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.haohaochexian.top/gtiqxuvhyx.html

PHP:  array_reverse($arr);
来源：http://hz.zdqjudy.top/gtcjvwsoog.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yj20258.top/gtuzsibutb.html

TS:   [...arr].reverse();
来源：http://hz.jyoumei.cn/gtkorelobg.html

Java: Collections.reverse(list);
来源：http://hz.meibo888.top/gtuekctdfj.html

Go:   slices.Reverse(arr)
来源：http://hz.fzhhl.top/gtrutnehaw.html

Ruby: arr.reverse
来源：http://hz.aibaodan.cn/gtpircdrvt.html

C#:   list.Reverse();
来源：http://hz.shanyushiyangtech.top/gtlgxzkqju.html

[D12] 查找元素下标
来源：http://hz.zhaomingkeji.xyz/gtrytyctuw.html

Py:   arr.index(x);  x in arr
来源：http://hz.andypj.xyz/gtxuefqknz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yongpay.top/gtgjwwftra.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhijiandao.cn/gtxakgcwaa.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.sxryk.cn/gtvmbhrfua.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.daxiang520.top/gtpscqlxdd.html

Go:   slices.Index(arr, x)
来源：http://hz.yuanzhike.top/gtfqthvwif.html

Ruby: arr.index(x)
来源：http://hz.chenlongwang.top/gtasnqxckt.html

C#:   list.IndexOf(x);
来源：http://hz.yangfankeji.com/gtndlpzbbh.html

[D13] 过滤（保留满足条件的）
来源：http://hz.svipenyu.cn/gtydlxumun.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zhongyouzk.top/gtvhoafyls.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.dianchejie.cn/gtcjoiymxj.html

JS:   arr.filter(x => x > 3)
来源：http://hz.quarkkingdee.top/gtuihhllam.html

TS:   arr.filter(x => x > 3)
来源：http://hz.xingfuxueyuan.xyz/gtgcjyurds.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.iojbl.cn/gtzzqrgetm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.cashguo.top/gtkujvsemp.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.pycfn.com/gtfcubifao.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.sxryk.cn/gtzaykwgub.html

[D14] 映射转换（每个元素变形）
来源：http://hz.zhixingplan.top/gtfolxtmiq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.snrcjt.cn/gtutuszvte.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yj202588.top/gtudkhweki.html

JS:   arr.map(x => x * 2)
来源：http://hz.nwbrower.top/gtuemyiunm.html

TS:   arr.map(x => x * 2)
来源：http://hz.haohaochexian.top/gtsuuavglh.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yuxming.cn/gtnhkssctt.html

Go:   // 手写循环
来源：http://hz.bjfxy.top/gtfzmkuaym.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.sxryk.cn/gtnhpspgpu.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yongpay.top/gtrzlvnrmr.html

[D15] 去重
来源：http://hz.nanxuanxn.top/gtqyssqnfv.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.andypj.xyz/gtxmbdmwka.html

PHP:  array_unique($arr);
来源：http://hz.chenlongwang.top/gtgvffnetq.html

JS:   [...new Set(arr)]
来源：http://hz.jiagoushi.top/gtmqmmsqkq.html

TS:   [...new Set(arr)]
来源：http://hz.iojbl.cn/gtdonanrje.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.kuanghao11.cn/gtlphkifbm.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.pengpengdd.cyou/gtiucabnvw.html

Ruby: arr.uniq
来源：http://hz.ehwqpu.com/gtigseguqb.html

C#:   list.Distinct().ToList()
来源：http://hz.jqgufenzy.top/gtbwjcvmyg.html

[D16] 求和与平均值
来源：http://hz.ybcxt.top/gtnjpyymue.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.zhaomingkeji.xyz/gtvjlwjysr.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.tian-w.cn/gtqnahsslp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cashguo.top/gtmqmriakp.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.havefunace.top/gtawhzflhh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.tanke756.top/gtqxstnjtg.html

Go:   // 手写循环累加
来源：http://hz.yj20258888.top/gtcwfksqak.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.fzhhl.top/gtxssdzbgt.html

C#:   list.Sum();  list.Average()
来源：http://hz.zycfv.cn/gtfxbdshty.html

[D17] 最大值与最小值
来源：http://hz.sysykeji.top/gtigtugleq.html

Py:   max(arr);  min(arr)
来源：http://hz.gzhubu.top/gtmvfdhlbi.html

PHP:  max($arr);  min($arr);
来源：http://hz.yj20258.top/gthctfmcxp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.0kj1m.cn/gtgxyvinho.html

TS:   Math.max(...arr);
来源：http://hz.zycfv.cn/gttcjddtmh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.daxiang520.top/gtipasymqy.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jlsjyb.cn/gtknaziieq.html

Ruby: arr.max;  arr.min
来源：http://hz.jyoumei.cn/gtbyxasaop.html

C#:   list.Max();  list.Min()
来源：http://hz.shangyingyoupin.top/gtphbqiimu.html

[D18] 扁平化嵌套数组
来源：http://hz.zhaomingkeji.xyz/gtsjzzvmcd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zycfv.cn/gtaybvqhad.html

PHP:  array_merge(...$nested);
来源：http://hz.zhaomingkeji.xyz/gtvmpwymqp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.ydzc1.top/gthtaroqnl.html

TS:   nested.flat();
来源：http://hz.pycfn.com/gtohfmnlif.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.zycfv.cn/gtzxmqdbil.html

Go:   // 手写双层循环
来源：http://hz.ywan-chungtsiang.top/gtctntwagz.html

Ruby: nested.flatten
来源：http://hz.pengpengdd.cyou/gtlutvobms.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.xingfuxueyuan.xyz/gtvmmholrt.html

[D19] 按字段分组
来源：http://hz.jqgfzy.top/gthepsqhjm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.snrcjt.cn/gteshrfcay.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.smart0.xyz/gtpmkdfjtt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.wangshuangyany.cn/gtlpwyvyrz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.xingfuxueyuan.xyz/gtwmkfgrgb.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.gogol.net.cn/gtbrlcytjz.html

Go:   // 手写 map[string][]T
来源：http://hz.gogol.net.cn/gtjxfgsegd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.tianlin.xyz/gtmqmwdpwk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.fzhhl.top/gtutkjkyob.html

[D20] 统计每个元素出现次数
来源：http://hz.fengsongda.top/gtywiznmmv.html

Py:   Counter(arr)
来源：http://hz.zhongyouzk.top/gtqrkvxwdz.html

PHP:  array_count_values($arr);
来源：http://hz.jiagoushi.top/gtnwdgysed.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jqgufenzy.top/gtpryfsuii.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shanyushiyangtech.top/gtvqwqjydl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yonumen.top/gtfuuiiahw.html

Go:   // 手写 map[T]int
来源：http://hz.gotoacloud.top/gtbduowsvm.html

Ruby: arr.tally
来源：http://hz.tianlin.xyz/gtixhfbchi.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.hnqzz.top/gtechdvkqz.html

[D21] 判断是否包含某元素
来源：http://hz.fengsongda.top/gtovbimvwd.html

Py:   x in arr
来源：http://hz.xuetiantiany.cn/gtqgjyqvxu.html

PHP:  in_array($x, $arr, true);
来源：http://hz.gotoacloud.top/gtacqcthwo.html

JS:   arr.includes(x)
来源：http://hz.shzxlz.cn/gtdotetnjn.html

TS:   arr.includes(x)
来源：http://hz.nanxinkj.top/gtuvcmqbsp.html

Java: list.contains(x)
来源：http://hz.zhoulong.xyz/gtrmsupwwn.html

Go:   slices.Contains(arr, x)
来源：http://hz.pycfn.com/gtjnoaqgew.html

Ruby: arr.include?(x)
来源：http://hz.tanke756.top/gtnunsxqog.html

C#:   list.Contains(x)
来源：http://hz.jinqigfzy.top/gtlylvaqkn.html

[D22] 复制数组（避免共享引用）
来源：http://hz.zhongyouzk.top/gtgqfhhrpp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.chenzaomai.com/gtfbqpxaae.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.9152youxi.cn/gtqojnythv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jinqigfzy.top/gtmeemvblx.html

TS:   [...arr];
来源：http://hz.shuidangran.top/gtoqyivjqk.html

Java: new ArrayList<>(list);
来源：http://hz.yj202588.top/gtbmvokyxo.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.shangyingyoupin.top/gtiydfehhq.html

Ruby: arr.dup;  arr.clone
来源：http://hz.cdnleiting.top/gtfwphswaf.html

C#:   new List<int>(list);
来源：http://hz.ppjwa.cn/gtgcnoldez.html

[D23] reduce 累积计算
来源：http://hz.shzxlz.cn/gthdoerdlw.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.birdmap.top/gtagwyfgyj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.zhiwuduotai.top/gtblxmexpl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cucudq.cn/gtkuzkgdwx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zycfv.cn/gtmhujllzg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.xuetiantiany.cn/gtksvffwvh.html

Go:   // 手写循环
来源：http://hz.vqdsnc.cn/gtqrlyebvc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.tanke756.top/gtxovlozkl.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jinqigfzy.top/gtclawmmtk.html

[D24] 字典 / Map 基本操作
来源：http://hz.zhiwuduotai.top/gteuftxdlg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.gotoacloud.top/gtctqhykbi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.hongshengwenyu.top/gtacsvapkf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.quarkkingdee.top/gtxbzsmygx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.havefunace.top/gtsndvhgki.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.mhx1999.top/gteprpqqup.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yuanzhike.top/gtlntmociw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.snrcjt.cn/gtdczowzyf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.gotoacloud.top/gtdrstfoei.html

[D25] Set 集合去重与交并差
来源：http://hz.0kj1m.cn/gtrhethizo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.feifeiyinyue.top/gtzyjvgiqk.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.hnqzz.top/gtfzqbkpcy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.hywenlv.cn/gtoiwysnkh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.shzxlz.cn/gtygpqbmbl.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.aibaodan.cn/gtkzadvrpn.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.zdqjudy.top/gtcredehyw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.hongshengwenyu.top/gttkvyychc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.sufxvd.cn/gtvgvbisdc.html

[D26] 数组转字符串
来源：http://hz.xingfuxueyuan.xyz/gtzxczrdzs.html

Py:   ", ".join(map(str, arr))
来源：http://hz.gotoacloud.top/gtckdipcuf.html

PHP:  implode(", ", $arr);
来源：http://hz.jqgfzy.top/gtibmpurbw.html

JS:   arr.join(", ")
来源：http://hz.jqgufenzy.top/gtdvuqttje.html

TS:   arr.join(", ")
来源：http://hz.xylfe.cn/gtvyijbtej.html

Java: String.join(", ", list)
来源：http://hz.guannengcc.top/gtrrrzbjal.html

Go:   strings.Join(strs, ", ")
来源：http://hz.cqqwz.cn/gtvzbvrpoz.html

Ruby: arr.join(", ")
来源：http://hz.quarkkingdee.top/gtxeqrnouo.html

C#:   string.Join(", ", list)
来源：http://hz.sweek.top/gtkfpeoalt.html

================================================================================
来源：http://hz.cqqwz.cn/gtvfcxmiuf.html

E. 字符串处理
来源：http://hz.bjfxy.top/gtiiyevloz.html

================================================================================
来源：http://hz.jinghuilouyu.cn/gtznszlwkh.html

[E01] 拼接字符串
来源：http://hz.zhongyouzk.top/gtuzkhfkcq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.svipenyu.cn/gtyifinnxf.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.gogol.net.cn/gtioluguhk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhijiandao.cn/gtscsoqkah.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zhiwuduotai.top/gtsovuwdna.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.dashuyun.cn/gtuukafxks.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jlsjyb.cn/gtqeaccqld.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yueranfly.top/gtggfbkjef.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.chenzaomai.com/gtyfcdtihr.html

[E02] 重复字符串
来源：http://hz.wangshuangyany.cn/gtstoolbej.html

Py:   "ab" * 3
来源：http://hz.gaohongyu789.top/gtbrxtpigo.html

PHP:  str_repeat("ab", 3);
来源：http://hz.chenjidiqi.icu/gtzhwurgns.html

JS:   "ab".repeat(3)
来源：http://hz.yj20258888.top/gtxhcciqtd.html

TS:   "ab".repeat(3)
来源：http://hz.snrcjt.cn/gtpbakiubq.html

Java: "ab".repeat(3)
来源：http://hz.yangfankeji.com/gttrocyyxm.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.316326.xyz/gttpzurzkj.html

Ruby: "ab" * 3
来源：http://hz.birdmap.top/gtplgjnggi.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.nwbrower.top/gtmeuieoyl.html

[E03] 截取子串
来源：http://hz.sxryk.cn/gtcjccdimq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.zdqjudy.top/gtswbcgnug.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.tian-w.cn/gtevnbvhdu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.sufxvd.cn/gtfzwfmtjm.html

TS:   s.slice(1, 4)
来源：http://hz.aibaodan.cn/gtuelqebrh.html

Java: s.substring(1, 4)
来源：http://hz.guowangkeji.top/gthboiyvhh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.xingfuxueyuan.xyz/gttxoyprwu.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.zhongyouzk.top/gtfifrmnii.html

C#:   s.Substring(1, 3)
来源：http://hz.0kj1m.cn/gtplnovsyg.html

[E04] 查找子串位置
来源：http://hz.vqdsnc.cn/gtlmqyvphv.html

Py:   s.find("x");  s.index("x")
来源：http://hz.quarkkingdee.top/gtnvwlsoob.html

PHP:  strpos($s, "x");
来源：http://hz.kuanghao11.cn/gtlfbljpoj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.birdmap.top/gtklbemcgz.html

TS:   s.indexOf("x")
来源：http://hz.yanxiufei.cn/gtmyjpjebv.html

Java: s.indexOf("x")
来源：http://hz.vqdsnc.cn/gtirwakxvc.html

Go:   strings.Index(s, "x")
来源：http://hz.dashuyun.cn/gtukukikxe.html

Ruby: s.index("x")
来源：http://hz.ivvv.top/gtfxhufjkn.html

C#:   s.IndexOf("x")
来源：http://hz.fengsongda.top/gtzsnezbtj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.havefunace.top/gtvigkrhvx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.haohaochexian.top/gtkekhfwyy.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.hammf.cn/gtdqgfqgjl.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.chenlongwang.top/gtnuvvcxxo.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zdqjudy.top/gtxnkgkymb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zhoulong.xyz/gtoclxgcoi.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.aibaodan.cn/gtmtgrtfvy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yangfankeji.com/gtpwlcvdjl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.tianlin.xyz/gthylwnfgp.html

[E06] 替换子串
来源：http://hz.fengsongda.top/gtltlbznpv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.ehwqpu.com/gtdcdtdtvr.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.pycfn.com/gthvjehkhs.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hfpthk.cn/gtbjrinyig.html

TS:   s.replaceAll("a", "b")
来源：http://hz.fengsongda.top/gtphxmnnzb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.aizwys.cn/gtjxakjzev.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.cqqwz.cn/gtalcstzex.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.xuetiantiany.cn/gtqrbryvhk.html

C#:   s.Replace("a", "b")
来源：http://hz.xinyue.icu/gtzsyfqblj.html

[E07] 按分隔符拆分
来源：http://hz.gotoacloud.top/gtpdneprus.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.cucudq.cn/gtancwmhfb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.0kj1m.cn/gtbibvoqho.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.gaohongyu789.top/gtjnkwvrwb.html

TS:   s.split(",")
来源：http://hz.yongpay.top/gtlyhopbdq.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.hammf.cn/gtawooqekl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.52xcode.cn/gtyogienyb.html

Ruby: s.split(",");  s.split
来源：http://hz.ybcxt.top/gtlxfifpeq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.aizwys.cn/gtwdlrkksy.html

[E08] 数组按分隔符合并
来源：http://hz.zhongyouzk.top/gtqftnacqd.html

Py:   ",".join(items)
来源：http://hz.daria6918.cn/gtwtbvocjr.html

PHP:  implode(",", $items);
来源：http://hz.zhijiandao.cn/gtjmhryvxu.html

JS:   items.join(",")
来源：http://hz.zhijiandao.cn/gtrswkmxvd.html

TS:   items.join(",")
来源：http://hz.chenjidiqi.icu/gtoybykohg.html

Java: String.join(",", items)
来源：http://hz.cucudq.cn/gtjvzmqagr.html

Go:   strings.Join(items, ",")
来源：http://hz.pengpengdd.cyou/gtztzcjwqg.html

Ruby: items.join(",")
来源：http://hz.dashuyun.cn/gtzudkhuvo.html

C#:   string.Join(",", items)
来源：http://hz.zycfv.cn/gtnvgujzey.html

[E09] 去除所有空白字符
来源：http://hz.aibaodan.cn/gtyifirbxd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.aibaodan.cn/gtyzqcptge.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.ydjk.org.cn/gtuzojkmsc.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.bjfxy.top/gtidyolsck.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.shanyushiyangtech.top/gtesfvduxf.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.sufxvd.cn/gtaphmqyzi.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.gogol.net.cn/gtthqzgfgg.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.sxryk.cn/gtsvtycpcf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.daria6918.cn/gtaqvdwkdi.html

[E10] 左侧补零 / 定长填充
来源：http://hz.yueranfly.top/gtacbbhrxn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.sweek.top/gtyvcpmrvh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.pycfn.com/gtbarpddcc.html

JS:   "7".padStart(3, "0")
来源：http://hz.hfpthk.cn/gtyjuwlnon.html

TS:   "7".padStart(3, "0")
来源：http://hz.fengsongda.top/gtzdwsfrkm.html

Java: String.format("%03d", 7)
来源：http://hz.jianghu66.top/gthcnkrrfl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yvedp.cn/gtdbiefold.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.daria6918.cn/gtmsfizmuh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.yonumen.top/gtfkthiddv.html

[E11] 反转字符串
来源：http://hz.ppjwa.cn/gtrfuoatqb.html

Py:   s[::-1]
来源：http://hz.9152youxi.cn/gtuzfnbmpa.html

PHP:  strrev($s);
来源：http://hz.daxiang520.top/gthqicgwyu.html

JS:   [...s].reverse().join("")
来源：http://hz.jinghuilouyu.cn/gtcnmupsww.html

TS:   [...s].reverse().join("")
来源：http://hz.wangshuangyany.cn/gtvoupdluh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.zhoulong.xyz/gtpchjjozh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.nanxuanxn.top/gtugeeuety.html

Ruby: s.reverse
来源：http://hz.ppjwa.cn/gtqpvqltgx.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.c1oappe.top/gtskecblxi.html

[E12] 统计某字符出现次数
来源：http://hz.sxryk.cn/gtkvwmokrk.html

Py:   s.count("a")
来源：http://hz.birdmap.top/gtjylhgset.html

PHP:  substr_count($s, "a");
来源：http://hz.jqgufenzy.top/gtgpyzzeju.html

JS:   s.split("a").length - 1
来源：http://hz.sweek.top/gtccmkwwzb.html

TS:   s.split("a").length - 1
来源：http://hz.dianchejie.cn/gtgnzvxvwp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.yuxming.cn/gtswmmrozb.html

Go:   strings.Count(s, "a")
来源：http://hz.tianlin.xyz/gtsaaodnjn.html

Ruby: s.count("a")
来源：http://hz.dianchejie.cn/gtwieamury.html

C#:   s.Count(c => c == 'a')
来源：http://hz.chenzaomai.com/gtwjxwmkbw.html

[E13] 逐字符遍历
来源：http://hz.jinyuanbaomall.cn/gtridfqxwv.html

Py:   for ch in s: print(ch)
来源：http://hz.yueranfly.top/gtmqoqkuuz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.ppjwa.cn/gtwsnzuezh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hywenlv.cn/gtkmjfvclt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yuanzhike.top/gtqnjbrizn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.chenzaomai.com/gtvnmdlvwl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.zycfv.cn/gtgfntutef.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.guannengcc.top/gtjayuhgqk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.guannengcc.top/gtiteedxul.html

[E14] URL 编码与 Base64
来源：http://hz.shangyingyoupin.top/gtdbpcjdqg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.aibaodan.cn/gtspkoaiqx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.cashguo.top/gtommhbejz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.snrcjt.cn/gtdcpkavwx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.xylfe.cn/gtgdxvltnm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.pycfn.com/gtnwoceycc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.tian-w.cn/gthvehkejk.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zhongyouzk.top/gtvwhqswhv.html


<!-- 参考信息 -->