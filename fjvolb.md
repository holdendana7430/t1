代发 wailian999

PHP:  sort($arr);
来源：http://hz.sweek.top/gthrtbchfc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.chenlongwang.top/gtvhgpppnb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zhongyouzk.top/gtfiihypcc.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.meibo888.top/gtkkrayzax.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.dianchejie.cn/gtnkgzahsh.html

Ruby: arr.sort
来源：http://hz.ydjk.org.cn/gtpdmrsesp.html

C#:   list.Sort();
来源：http://hz.hnxiangtu.top/gteosbepcp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zhijiandao.cn/gtojilotnl.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zhengqikj.top/gtnjukbtwb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.chenlongwang.top/gtmlksbcfi.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.kuanghao11.cn/gtvugnpvij.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.fengsongda.top/gtgnmlrlhb.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.sweek.top/gtojuzsums.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.bjfxy.top/gtukeqbolf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.chenzaomai.com/gtrmqveagz.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jlsjyb.cn/gtwsgjhdny.html

[D11] 反转数组
来源：http://hz.shanyushiyangtech.top/gthxrfevzj.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yueranfly.top/gtmtyppejq.html

PHP:  array_reverse($arr);
来源：http://hz.jiagoushi.top/gtkbrkzucl.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.dashuyun.cn/gtarbbfpeh.html

TS:   [...arr].reverse();
来源：http://hz.redwolf501.top/gtibafnptv.html

Java: Collections.reverse(list);
来源：http://hz.smart0.xyz/gtbyzvzahx.html

Go:   slices.Reverse(arr)
来源：http://hz.zhengqikj.top/gtjstpclka.html

Ruby: arr.reverse
来源：http://hz.dashuyun.cn/gtedoxjegl.html

C#:   list.Reverse();
来源：http://hz.guowangkeji.top/gtdzmqrnep.html

[D12] 查找元素下标
来源：http://hz.quarkkingdee.top/gtivwkkvyt.html

Py:   arr.index(x);  x in arr
来源：http://hz.hnqzz.top/gtohcvvzik.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yuanzhike.top/gtulzvvskr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yueranfly.top/gtcxjswmji.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hysaishi.cn/gtgozdpiya.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.xziqi.cn/gtiwtqawhi.html

Go:   slices.Index(arr, x)
来源：http://hz.ydzc1.top/gtqiimynrw.html

Ruby: arr.index(x)
来源：http://hz.yj20258888.top/gtckjxogpd.html

C#:   list.IndexOf(x);
来源：http://hz.vqdsnc.cn/gtzqekjlqy.html

[D13] 过滤（保留满足条件的）
来源：http://hz.fengsongda.top/gtkcubdqwt.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.nanxuanxn.top/gtvgoknfxf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.0kj1m.cn/gtnnsjqlwr.html

JS:   arr.filter(x => x > 3)
来源：http://hz.kuanghao11.cn/gtcibqigtb.html

TS:   arr.filter(x => x > 3)
来源：http://hz.iojbl.cn/gtdmdwfldl.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.guowangkeji.top/gtobmjdimc.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.tanke756.top/gtjlgtyihr.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.sufxvd.cn/gtqurufwwl.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.zhoulong.xyz/gtjftbnujw.html

[D14] 映射转换（每个元素变形）
来源：http://hz.xingfuxueyuan.xyz/gtzksdxhof.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.sweek.top/gtcorckscq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.meibo888.top/gtulkwsbri.html

JS:   arr.map(x => x * 2)
来源：http://hz.birdmap.top/gtyrirkdiy.html

TS:   arr.map(x => x * 2)
来源：http://hz.cucudq.cn/gtfrlrdgtp.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.gzhubu.top/gtajjhmkiq.html

Go:   // 手写循环
来源：http://hz.sxryk.cn/gtnqxckhsa.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.xylfe.cn/gtnskzgzfb.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.quarkkingdee.top/gtziutvvpm.html

[D15] 去重
来源：http://hz.cashguo.top/gtbuankvzw.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.nanxuanxn.top/gtsyaiijfl.html

PHP:  array_unique($arr);
来源：http://hz.yanxiufei.cn/gtbqaciaut.html

JS:   [...new Set(arr)]
来源：http://hz.jyoumei.cn/gtcxeyvzzs.html

TS:   [...new Set(arr)]
来源：http://hz.wangdashe.top/gtouuwaxgf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.redwolf501.top/gtyxhkvkie.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.daria6918.cn/gtrnavabqu.html

Ruby: arr.uniq
来源：http://hz.hnqzz.top/gtsfxucebt.html

C#:   list.Distinct().ToList()
来源：http://hz.cqqwz.cn/gtqxndapwt.html

[D16] 求和与平均值
来源：http://hz.birdmap.top/gthrgbbbdf.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.c1oappe.top/gtoawvluat.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.zhixingplan.top/gtmjcaxlcm.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yuxming.cn/gthlzpigmu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.chenjidiqi.icu/gtfkrgobme.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yueranfly.top/gtmvbbdqvm.html

Go:   // 手写循环累加
来源：http://hz.c1oappe.top/gtkqiccgnr.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.hysaishi.cn/gthbyjpfdu.html

C#:   list.Sum();  list.Average()
来源：http://hz.xinyue.icu/gtunwhyhoc.html

[D17] 最大值与最小值
来源：http://hz.zhoulong.xyz/gturinjtpq.html

Py:   max(arr);  min(arr)
来源：http://hz.yj20258888.top/gtbcjglowu.html

PHP:  max($arr);  min($arr);
来源：http://hz.yj202588.top/gtyqivhshl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.xingfuxueyuan.xyz/gtxkzezwun.html

TS:   Math.max(...arr);
来源：http://hz.gogol.net.cn/gtcajsvqws.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.hywenlv.cn/gtzwzozklt.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zdqjudy.top/gtnyjrrelr.html

Ruby: arr.max;  arr.min
来源：http://hz.yuxming.cn/gtgzkvzelz.html

C#:   list.Max();  list.Min()
来源：http://hz.daria6918.cn/gtztlmtbmp.html

[D18] 扁平化嵌套数组
来源：http://hz.nanxinkj.top/gtgxndskxm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.dashuyun.cn/gtxeqiilre.html

PHP:  array_merge(...$nested);
来源：http://hz.daxiang520.top/gtbaezixoe.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.sweek.top/gtbnvgutqa.html

TS:   nested.flat();
来源：http://hz.xylfe.cn/gtlgukfesu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yongpay.top/gtzzwggmym.html

Go:   // 手写双层循环
来源：http://hz.zhongyouzk.top/gtamuwbnue.html

Ruby: nested.flatten
来源：http://hz.316326.xyz/gtkutrsstd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zhengqikj.top/gtbifzpmcr.html

[D19] 按字段分组
来源：http://hz.52xcode.cn/gtdbeseovy.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.fengsongda.top/gtndwfcjcd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.dianchejie.cn/gtqyhxzxag.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.iojbl.cn/gtgzbtyalj.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.vqdsnc.cn/gtxlfsdcjd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.xuetiantiany.cn/gtynfccklx.html

Go:   // 手写 map[string][]T
来源：http://hz.yvedp.cn/gttjszrwra.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.yj20258888.top/gtvzrnuahu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yvedp.cn/gtdaioygcs.html

[D20] 统计每个元素出现次数
来源：http://hz.jinqigfzy.top/gtfojyppvv.html

Py:   Counter(arr)
来源：http://hz.52xcode.cn/gtokahnzud.html

PHP:  array_count_values($arr);
来源：http://hz.nwbrower.top/gtxnitxlpp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.chenzaomai.com/gtofoagvpo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ivvv.top/gtxygzystu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ivvv.top/gtltnbjpjn.html

Go:   // 手写 map[T]int
来源：http://hz.yanxiufei.cn/gtxnorfqhq.html

Ruby: arr.tally
来源：http://hz.cashguo.top/gtyhavwzfi.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.hammf.cn/gtyofsjkvo.html

[D21] 判断是否包含某元素
来源：http://hz.feifeiyinyue.top/gtgyersicd.html

Py:   x in arr
来源：http://hz.dianchejie.cn/gtjztgrofi.html

PHP:  in_array($x, $arr, true);
来源：http://hz.jinyuanbaomall.cn/gtrvgcnglt.html

JS:   arr.includes(x)
来源：http://hz.nwbrower.top/gttlivkvnt.html

TS:   arr.includes(x)
来源：http://hz.9152youxi.cn/gtgigkkezh.html

Java: list.contains(x)
来源：http://hz.yj20258.top/gtrpxyoles.html

Go:   slices.Contains(arr, x)
来源：http://hz.yuanzhike.top/gtenfvajyf.html

Ruby: arr.include?(x)
来源：http://hz.316326.xyz/gtrnvssrhq.html

C#:   list.Contains(x)
来源：http://hz.zhaomingkeji.xyz/gtbldgnyio.html

[D22] 复制数组（避免共享引用）
来源：http://hz.cashguo.top/gtzqjeurqn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yuanzhike.top/gtexitxrwh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.dashuyun.cn/gtkcnpsfyc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.9152youxi.cn/gtrlerpbkp.html

TS:   [...arr];
来源：http://hz.aibaodan.cn/gtdtumarxx.html

Java: new ArrayList<>(list);
来源：http://hz.zhongyouzk.top/gtuijvigjz.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.xylfe.cn/gtjlojsfcl.html

Ruby: arr.dup;  arr.clone
来源：http://hz.zhongyouzk.top/gtoqlcgcjp.html

C#:   new List<int>(list);
来源：http://hz.nanxuanxn.top/gtnxwrcdxh.html

[D23] reduce 累积计算
来源：http://hz.yj202588.top/gtpktnxnwr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yuxming.cn/gtjcyqocjl.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.sysykeji.top/gtzzixyzgv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.dashuyun.cn/gthrabxlaz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.nanxuanxn.top/gtdpzycbye.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.chenjidiqi.icu/gtngtxdplm.html

Go:   // 手写循环
来源：http://hz.xinyue.icu/gtueygqnyt.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yongpay.top/gtpbgmonhx.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.ydzc1.top/gtnusycnqv.html

[D24] 字典 / Map 基本操作
来源：http://hz.xinyue.icu/gtklmwqisd.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.yuanzhike.top/gtkigmutsd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yongpay.top/gtwgcqywge.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.svipenyu.cn/gteccbidwz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.xingfuxueyuan.xyz/gtofyfvtii.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.hnxiangtu.top/gtqeorkjfd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.daria6918.cn/gtefmbnftg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.xylfe.cn/gtlmvidrqn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.aibaodan.cn/gtptdzwtyk.html

[D25] Set 集合去重与交并差
来源：http://hz.cdnleiting.top/gtxnxtmmwu.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.smart0.xyz/gtpefxruwj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.xuetiantiany.cn/gtifdzmcob.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.shzxlz.cn/gtwlptcqnt.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.ydjk.org.cn/gtbnmboeml.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.hywenlv.cn/gtlzflcvpt.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yanxiufei.cn/gtlgckfqpk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jlsjyb.cn/gtwcvvtfpc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.zhixingplan.top/gtaurzuxgq.html

[D26] 数组转字符串
来源：http://hz.tian-w.cn/gtchaoayeu.html

Py:   ", ".join(map(str, arr))
来源：http://hz.xuetiantiany.cn/gtulzxdqpg.html

PHP:  implode(", ", $arr);
来源：http://hz.hysaishi.cn/gterupeugo.html

JS:   arr.join(", ")
来源：http://hz.zycfv.cn/gtlhndsusv.html

TS:   arr.join(", ")
来源：http://hz.jqgfzy.top/gtehzcogkf.html

Java: String.join(", ", list)
来源：http://hz.yangfankeji.com/gtcvhukdlw.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yj20258.top/gtvapvoymr.html

Ruby: arr.join(", ")
来源：http://hz.xziqi.cn/gtyshqvuot.html

C#:   string.Join(", ", list)
来源：http://hz.cqqwz.cn/gtvqtmctyv.html

================================================================================
来源：http://hz.daria6918.cn/gtssgsvndi.html

E. 字符串处理
来源：http://hz.tian-w.cn/gtgezyncrg.html

================================================================================
来源：http://hz.cucudq.cn/gtgsrjemkm.html

[E01] 拼接字符串
来源：http://hz.hnxiangtu.top/gtcqzblcnt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.xingfuxueyuan.xyz/gtliirazxx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.jianghu66.top/gtbounbqmp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.mhx1999.top/gtvzrpremf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.guannengcc.top/gtxzfilhwk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.ydjk.org.cn/gtmoskmeie.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.meibo888.top/gtqnpxvtsw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.aibaodan.cn/gtpxnkguhi.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.chenzaomai.com/gtlfvttxwe.html

[E02] 重复字符串
来源：http://hz.ivvv.top/gtdfnbmxqz.html

Py:   "ab" * 3
来源：http://hz.kuanghao11.cn/gtkvemxluj.html

PHP:  str_repeat("ab", 3);
来源：http://hz.hammf.cn/gtcaywnavs.html

JS:   "ab".repeat(3)
来源：http://hz.zhijiandao.cn/gtrsrykhay.html

TS:   "ab".repeat(3)
来源：http://hz.havefunace.top/gtdecmmzsu.html

Java: "ab".repeat(3)
来源：http://hz.meibo888.top/gtudoexlcr.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.xuanzx.com/gtkeakiglq.html

Ruby: "ab" * 3
来源：http://hz.jinghuilouyu.cn/gteirwjpkk.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.aibaodan.cn/gtuenjsuwr.html

[E03] 截取子串
来源：http://hz.jianghu66.top/gtexyhgtnc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jinqigufen.top/gtobfrhrll.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.hongshengwenyu.top/gtusuparuz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jinqigfzy.top/gthgezwxer.html

TS:   s.slice(1, 4)
来源：http://hz.tian-w.cn/gtuejwshrn.html

Java: s.substring(1, 4)
来源：http://hz.zycfv.cn/gtorioccfe.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.c1oappe.top/gtvomllriu.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.hysaishi.cn/gtzhocnoex.html

C#:   s.Substring(1, 3)
来源：http://hz.gogol.net.cn/gtzzvgqqfu.html

[E04] 查找子串位置
来源：http://hz.kuanghao11.cn/gtzbotzrzn.html

Py:   s.find("x");  s.index("x")
来源：http://hz.hnqzz.top/gtzcdtvocz.html

PHP:  strpos($s, "x");
来源：http://hz.andypj.xyz/gtslhegrvv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zdqjudy.top/gtwnbhihgo.html

TS:   s.indexOf("x")
来源：http://hz.xuetiantiany.cn/gtbbrzophs.html

Java: s.indexOf("x")
来源：http://hz.fzhhl.top/gtulzulpwc.html

Go:   strings.Index(s, "x")
来源：http://hz.nanxuanxn.top/gtnjulmllj.html

Ruby: s.index("x")
来源：http://hz.daxiang520.top/gtzslzbrfm.html

C#:   s.IndexOf("x")
来源：http://hz.meibo888.top/gtzalnacym.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.xuanzx.com/gtdjnjicps.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yj20258888.top/gtrotzapox.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zhongyouzk.top/gtlbygezle.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.smart0.xyz/gtcegeseyr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.fzhhl.top/gtvzfdlthy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.bjfxy.top/gtlzhdxquc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.redwolf501.top/gtuoxhhqot.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.316326.xyz/gtycdlsbfz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.kuanghao11.cn/gtajxkadyg.html

[E06] 替换子串
来源：http://hz.zhiwuduotai.top/gtozjfpsfs.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.cheryme.top/gtoaxmverr.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.sufxvd.cn/gtrvjvobzc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhoulong.xyz/gtyvvfplsk.html

TS:   s.replaceAll("a", "b")
来源：http://hz.zhaomingkeji.xyz/gtrkybfsfj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.shanyushiyangkeji.top/gtsajkewdr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.fzhhl.top/gtpmuatogi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.ivvv.top/gtlppnszrv.html

C#:   s.Replace("a", "b")
来源：http://hz.xziqi.cn/gtkmzpmkrb.html

[E07] 按分隔符拆分
来源：http://hz.shzxlz.cn/gtbbexwnpr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.fengsongda.top/gtbfwnjdun.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.shanyushiyangtech.top/gtuwoupofk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.redwolf501.top/gtghgmxbqw.html

TS:   s.split(",")
来源：http://hz.shanyushiyangkeji.top/gtgczmbgha.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.xziqi.cn/gtbqczldyv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.fzhhl.top/gthrdnqhoa.html

Ruby: s.split(",");  s.split
来源：http://hz.wangshuangyany.cn/gtcrsfofnf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.zdqjudy.top/gtwdxrrxdx.html

[E08] 数组按分隔符合并
来源：http://hz.chenlongwang.top/gtuqoizhqg.html

Py:   ",".join(items)
来源：http://hz.hongshengwenyu.top/gtnrqxyvko.html

PHP:  implode(",", $items);
来源：http://hz.zhijiandao.cn/gtcyenansl.html

JS:   items.join(",")
来源：http://hz.bjfxy.top/gthzmsjcbf.html

TS:   items.join(",")
来源：http://hz.aizwys.cn/gtxbmgnhme.html

Java: String.join(",", items)
来源：http://hz.nwbrower.top/gtrslvuemq.html

Go:   strings.Join(items, ",")
来源：http://hz.havefunace.top/gtawyvpepv.html

Ruby: items.join(",")
来源：http://hz.xziqi.cn/gtkbmnywjo.html

C#:   string.Join(",", items)
来源：http://hz.sufxvd.cn/gtkvkobfie.html

[E09] 去除所有空白字符
来源：http://hz.ppjwa.cn/gtlinitwkl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.quarkkingdee.top/gtwyyptkpe.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.havefunace.top/gtkesloezg.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.9152youxi.cn/gtqcwhhqcg.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.wangshuangyany.cn/gtrgmmbogf.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.xylfe.cn/gtdfyaxxup.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zhongyouzk.top/gtmltazeyg.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.meibo888.top/gtcukfhcqa.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.meibo888.top/gtumppoafu.html

[E10] 左侧补零 / 定长填充
来源：http://hz.sysykeji.top/gtnogvuruu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zhengqikj.top/gteznkekft.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.zhengqikj.top/gtybwxwrce.html

JS:   "7".padStart(3, "0")
来源：http://hz.dianchejie.cn/gtpymhgahx.html

TS:   "7".padStart(3, "0")
来源：http://hz.bjfxy.top/gteyrajder.html

Java: String.format("%03d", 7)
来源：http://hz.ivvv.top/gtodsjlrso.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.jqgufenzy.top/gtvobuoyhm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.daria6918.cn/gtauehykwk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.mhx1999.top/gtiudvoxxh.html

[E11] 反转字符串
来源：http://hz.jyoumei.cn/gtvibflkev.html

Py:   s[::-1]
来源：http://hz.vqdsnc.cn/gtrqgafyyd.html

PHP:  strrev($s);
来源：http://hz.jqgfzy.top/gtwkfklhqx.html

JS:   [...s].reverse().join("")
来源：http://hz.yuxming.cn/gtnytlsqau.html

TS:   [...s].reverse().join("")
来源：http://hz.redwolf501.top/gtnctjuntf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.hfpthk.cn/gtqnsdlqlf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.jianghu66.top/gtktbkghab.html

Ruby: s.reverse
来源：http://hz.hnqzz.top/gthdbrvres.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.shangyingyoupin.top/gthadfljtp.html

[E12] 统计某字符出现次数
来源：http://hz.tianlin.xyz/gtdyvyzplt.html

Py:   s.count("a")
来源：http://hz.jinqigufen.top/gtizhuxpwh.html

PHP:  substr_count($s, "a");
来源：http://hz.dashuyun.cn/gtbmakksnc.html

JS:   s.split("a").length - 1
来源：http://hz.zhengqikj.top/gtkzgbjffg.html

TS:   s.split("a").length - 1
来源：http://hz.jinqigufen.top/gtusuuwkoh.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.hfpthk.cn/gtuocmdjto.html

Go:   strings.Count(s, "a")
来源：http://hz.aizwys.cn/gtblxtpgcg.html

Ruby: s.count("a")
来源：http://hz.yj202588.top/gtfgjouxmy.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jyoumei.cn/gtqtbslcxg.html

[E13] 逐字符遍历
来源：http://hz.sweek.top/gtxtcwtoro.html

Py:   for ch in s: print(ch)
来源：http://hz.cucudq.cn/gtwxnmxytm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.cdnleiting.top/gtwcoisdnh.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hnxiangtu.top/gtrjrhtdgm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ydjk.org.cn/gtizxjxbxu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jqgfzy.top/gtukgxinio.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.yuanzhike.top/gtcjzhauhj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.havefunace.top/gtszmocliv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jlsjyb.cn/gtgohppljr.html

[E14] URL 编码与 Base64
来源：http://hz.shanyushiyangtech.top/gtilfjgtmq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yuxming.cn/gtmaesjsuv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.tianlin.xyz/gttogjbsaa.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.bjfxy.top/gtjtrweueh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.xingfuxueyuan.xyz/gtgbimyaeb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.hongshengwenyu.top/gtljdnhdvl.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.xylfe.cn/gtjsbwcxuj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.xuetiantiany.cn/gtpxeknjtr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.chenjidiqi.icu/gtfenjmqym.html

[E15] HTML 转义 / 反转义
来源：http://hz.guowangkeji.top/gtapvxtecn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zhixingplan.top/gtpjgawyxa.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.meibo888.top/gtzulflmbm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.vqdsnc.cn/gtyfnvtehh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.cashguo.top/gtfkywmmfq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yuanzhike.top/gttxxsecuk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.gotoacloud.top/gtlhjzoulr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.zhengqikj.top/gtqkbosiuv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.daxiang520.top/gtxgjlvcap.html

[E16] 数字千分位
来源：http://hz.cqqwz.cn/gtlotrmcqg.html

Py:   f"{1234567:,}"
来源：http://hz.nanxuanxn.top/gtthhbiwtl.html


<!-- 参考信息 -->