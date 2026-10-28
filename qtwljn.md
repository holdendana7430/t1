代发 wailian999

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.tanke756.top/gtojbznnhp.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.hfpthk.cn/gtfuvpcypn.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.shangyingyoupin.top/gtmjgshrsb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.dashuyun.cn/gtknwinoae.html

[D11] 反转数组
来源：http://hz.gotoacloud.top/gthkqhqjaw.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.iojbl.cn/gtsuqipnmh.html

PHP:  array_reverse($arr);
来源：http://hz.hammf.cn/gtfmnmoang.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.ydzc1.top/gttcbmohqz.html

TS:   [...arr].reverse();
来源：http://hz.wangdashe.top/gtfbvqmyrz.html

Java: Collections.reverse(list);
来源：http://hz.jinyuanbaomall.cn/gtvfpakskg.html

Go:   slices.Reverse(arr)
来源：http://hz.sysykeji.top/gtmexshkew.html

Ruby: arr.reverse
来源：http://hz.jyoumei.cn/gtekqsacpj.html

C#:   list.Reverse();
来源：http://hz.zhoulong.xyz/gtimqeqtjl.html

[D12] 查找元素下标
来源：http://hz.hysaishi.cn/gtdtgtouzd.html

Py:   arr.index(x);  x in arr
来源：http://hz.yj20258888.top/gtylfgcakf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yuxming.cn/gtmcykbixb.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.pycfn.com/gtoetscplg.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.pycfn.com/gtfvehpvut.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.smart0.xyz/gtntkdfvji.html

Go:   slices.Index(arr, x)
来源：http://hz.cucudq.cn/gtywbscckd.html

Ruby: arr.index(x)
来源：http://hz.zhoulong.xyz/gtasamfgvo.html

C#:   list.IndexOf(x);
来源：http://hz.cashguo.top/gttevihipw.html

[D13] 过滤（保留满足条件的）
来源：http://hz.vqdsnc.cn/gtvwohgzup.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.yj20258888.top/gtxpgrlduc.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.bjfxy.top/gtmwhjyqaz.html

JS:   arr.filter(x => x > 3)
来源：http://hz.mhx1999.top/gtaujrinoy.html

TS:   arr.filter(x => x > 3)
来源：http://hz.0kj1m.cn/gtworjwzun.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.jlsjyb.cn/gtssncmgdj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.ehwqpu.com/gtkkxocims.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.sysykeji.top/gtujriaufc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.yonumen.top/gtphactses.html

[D14] 映射转换（每个元素变形）
来源：http://hz.cashguo.top/gtuncklcox.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.c1oappe.top/gtlwnegukh.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.aibaodan.cn/gtyxhsyoth.html

JS:   arr.map(x => x * 2)
来源：http://hz.xziqi.cn/gtdzqarchs.html

TS:   arr.map(x => x * 2)
来源：http://hz.bjfxy.top/gtjyoyqkdy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.tian-w.cn/gtgrdvdvpk.html

Go:   // 手写循环
来源：http://hz.ydzc1.top/gthpoqkkxg.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.redwolf501.top/gtfzbvprrm.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.316326.xyz/gtnutowqzf.html

[D15] 去重
来源：http://hz.gotoacloud.top/gtulqdwojp.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yonumen.top/gtofeckvqw.html

PHP:  array_unique($arr);
来源：http://hz.hfpthk.cn/gtupckmosf.html

JS:   [...new Set(arr)]
来源：http://hz.hnqzz.top/gtyjadalvk.html

TS:   [...new Set(arr)]
来源：http://hz.jinghuilouyu.cn/gtsknawjro.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.gogol.net.cn/gtkudrwzcx.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.ybcxt.top/gtylrluhep.html

Ruby: arr.uniq
来源：http://hz.tian-w.cn/gthvoezdbh.html

C#:   list.Distinct().ToList()
来源：http://hz.dianchejie.cn/gtpywiijrl.html

[D16] 求和与平均值
来源：http://hz.yonumen.top/gtpmaafuky.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.shanyushiyangkeji.top/gtugowozjx.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.hysaishi.cn/gtckcrpfiu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jinqigfzy.top/gtskvjlpvv.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.guannengcc.top/gtkbgbcyrx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yanxiufei.cn/gtvgxoemca.html

Go:   // 手写循环累加
来源：http://hz.ehwqpu.com/gtdcqfenkt.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jqgufenzy.top/gtdhxlpser.html

C#:   list.Sum();  list.Average()
来源：http://hz.vqdsnc.cn/gturnyfncc.html

[D17] 最大值与最小值
来源：http://hz.wangdashe.top/gtkrsdmucg.html

Py:   max(arr);  min(arr)
来源：http://hz.xingfuxueyuan.xyz/gthxomikbu.html

PHP:  max($arr);  min($arr);
来源：http://hz.jlsjyb.cn/gtkloelijr.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.9152youxi.cn/gtbbrcguwh.html

TS:   Math.max(...arr);
来源：http://hz.hfpthk.cn/gtcmsevhdj.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.smart0.xyz/gtsoktogdf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.xingfuxueyuan.xyz/gtcnmmfuif.html

Ruby: arr.max;  arr.min
来源：http://hz.jinyuanbaomall.cn/gtprqfnpue.html

C#:   list.Max();  list.Min()
来源：http://hz.jyoumei.cn/gtvkghagnd.html

[D18] 扁平化嵌套数组
来源：http://hz.jinqigfzy.top/gtbdppvwbv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zhiwuduotai.top/gtwqjusish.html

PHP:  array_merge(...$nested);
来源：http://hz.iojbl.cn/gtjwfddqol.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yueranfly.top/gtpjgpoche.html

TS:   nested.flat();
来源：http://hz.gzhubu.top/gtkyyxfixp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.shzxlz.cn/gtmtmzcdvf.html

Go:   // 手写双层循环
来源：http://hz.yangfankeji.com/gtlcgduiex.html

Ruby: nested.flatten
来源：http://hz.gotoacloud.top/gtuxpvflpc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.pycfn.com/gttnlokllo.html

[D19] 按字段分组
来源：http://hz.52xcode.cn/gtsubgdfbv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.dashuyun.cn/gtzdqicsri.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.tian-w.cn/gthgostkon.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.xylfe.cn/gttchtkeeu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.shanyushiyangtech.top/gtibhrtbia.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.hywenlv.cn/gtdqrrgovi.html

Go:   // 手写 map[string][]T
来源：http://hz.shangyingyoupin.top/gtbdtiumev.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.nwbrower.top/gtfjurnmlg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.aizwys.cn/gtlkhaiylh.html

[D20] 统计每个元素出现次数
来源：http://hz.zhaomingkeji.xyz/gtgikaziso.html

Py:   Counter(arr)
来源：http://hz.hfpthk.cn/gteuogjngb.html

PHP:  array_count_values($arr);
来源：http://hz.meibo888.top/gtcuhmcicp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.mhx1999.top/gttbepxnib.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jinqigfzy.top/gtmqxappgo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.shanyushiyangkeji.top/gtpuwjabro.html

Go:   // 手写 map[T]int
来源：http://hz.jiagoushi.top/gthxearviq.html

Ruby: arr.tally
来源：http://hz.dianchejie.cn/gtmtgehvbl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.ydjk.org.cn/gtkvzuulpf.html

[D21] 判断是否包含某元素
来源：http://hz.hfpthk.cn/gtaqkrrdsp.html

Py:   x in arr
来源：http://hz.xziqi.cn/gtvbyqyigj.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yvedp.cn/gtackwvyci.html

JS:   arr.includes(x)
来源：http://hz.tianlin.xyz/gtvhovciea.html

TS:   arr.includes(x)
来源：http://hz.c1oappe.top/gtegjbvggk.html

Java: list.contains(x)
来源：http://hz.quarkkingdee.top/gtxiogjehi.html

Go:   slices.Contains(arr, x)
来源：http://hz.yuanzhike.top/gtmlfyvlqd.html

Ruby: arr.include?(x)
来源：http://hz.nanxuanxn.top/gtssehjdgl.html

C#:   list.Contains(x)
来源：http://hz.fengsongda.top/gtmvdbwfgv.html

[D22] 复制数组（避免共享引用）
来源：http://hz.sxryk.cn/gtyzlczpaj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yangfankeji.com/gtpwuccoby.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jinqigufen.top/gtveghppdf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jlsjyb.cn/gtlnpxdumb.html

TS:   [...arr];
来源：http://hz.pengpengdd.cyou/gtfczzqixk.html

Java: new ArrayList<>(list);
来源：http://hz.316326.xyz/gtonepbmlz.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.meibo888.top/gtmbqkmiub.html

Ruby: arr.dup;  arr.clone
来源：http://hz.guannengcc.top/gtmkwebjlf.html

C#:   new List<int>(list);
来源：http://hz.svipenyu.cn/gtlqoltqbf.html

[D23] reduce 累积计算
来源：http://hz.gotoacloud.top/gteubjurwv.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.cashguo.top/gtdachqrvk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.gogol.net.cn/gtyjwqeuxg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.guannengcc.top/gtaqtqdwzz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cdnleiting.top/gtbavdwjnh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jinqigufen.top/gtcutdncgo.html

Go:   // 手写循环
来源：http://hz.jinqigfzy.top/gtaxqwpafo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.aizwys.cn/gtbjyeqcid.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.c1oappe.top/gtznodixlp.html

[D24] 字典 / Map 基本操作
来源：http://hz.xziqi.cn/gtqztyldlw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.nanxuanxn.top/gtiesuocsd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.zhoulong.xyz/gtpdxlpbpx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.xziqi.cn/gtubhzargg.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.xylfe.cn/gtgbmiafol.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yj202588.top/gtqouewrui.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.yvedp.cn/gtojfvtxna.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.sweek.top/gtganvgerq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yueranfly.top/gthnfbsijn.html

[D25] Set 集合去重与交并差
来源：http://hz.redwolf501.top/gtcowkgone.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.meibo888.top/gthwacgssl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.cheryme.top/gtbwegwbeh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.ppjwa.cn/gtjnijkncw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.zdqjudy.top/gtxwhsphkz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.redwolf501.top/gtwltfnoya.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.pycfn.com/gtklokofvg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.xinyue.icu/gtfyrtlowt.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.dashuyun.cn/gtasjbcuap.html

[D26] 数组转字符串
来源：http://hz.cucudq.cn/gtwypiedcv.html

Py:   ", ".join(map(str, arr))
来源：http://hz.havefunace.top/gthpxdjlyt.html

PHP:  implode(", ", $arr);
来源：http://hz.wangshuangyany.cn/gtzmrdtpyb.html

JS:   arr.join(", ")
来源：http://hz.shangyingyoupin.top/gtulzzrjce.html

TS:   arr.join(", ")
来源：http://hz.yongpay.top/gtffmxpfcx.html

Java: String.join(", ", list)
来源：http://hz.hnxiangtu.top/gtptbupoha.html

Go:   strings.Join(strs, ", ")
来源：http://hz.snrcjt.cn/gtzadkpuec.html

Ruby: arr.join(", ")
来源：http://hz.haohaochexian.top/gtdnywlhbw.html

C#:   string.Join(", ", list)
来源：http://hz.yongpay.top/gtauskdfls.html

================================================================================
来源：http://hz.hysaishi.cn/gteprunlfh.html

E. 字符串处理
来源：http://hz.jinyuanbaomall.cn/gtxhrmfhaa.html

================================================================================
来源：http://hz.haohaochexian.top/gttgbbrlge.html

[E01] 拼接字符串
来源：http://hz.gotoacloud.top/gtfqthgxwt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.shuidangran.top/gtnkkibgxi.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zdqjudy.top/gtcqblshkl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.guowangkeji.top/gtxgwljhgk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.gaohongyu789.top/gtwwwlmoen.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yj20258888.top/gtauakqxfi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jyoumei.cn/gtgbumuqzh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.wangshuangyany.cn/gtccowhdpo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.sysykeji.top/gtkyqcswhz.html

[E02] 重复字符串
来源：http://hz.kuanghao11.cn/gtpbfgpnka.html

Py:   "ab" * 3
来源：http://hz.bjfxy.top/gthoaqzlpq.html

PHP:  str_repeat("ab", 3);
来源：http://hz.cashguo.top/gtsaouxvxj.html

JS:   "ab".repeat(3)
来源：http://hz.bjfxy.top/gtnraqjddo.html

TS:   "ab".repeat(3)
来源：http://hz.ydzc1.top/gtafioiepg.html

Java: "ab".repeat(3)
来源：http://hz.chenlongwang.top/gtyztdyjbs.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jinqigufen.top/gtdyzjewdu.html

Ruby: "ab" * 3
来源：http://hz.jinqigfzy.top/gtpsbugzqy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.fzhhl.top/gtjhhvgrjz.html

[E03] 截取子串
来源：http://hz.fzhhl.top/gtnpmmcvgi.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jiagoushi.top/gtvayjantg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.iojbl.cn/gtccmhtmcx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.tanke756.top/gtzggbipsn.html

TS:   s.slice(1, 4)
来源：http://hz.hfpthk.cn/gtxuxkdzoo.html

Java: s.substring(1, 4)
来源：http://hz.xuanzx.com/gtyvnxyczt.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.havefunace.top/gtpuotjmfa.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jyoumei.cn/gtpspehqzf.html

C#:   s.Substring(1, 3)
来源：http://hz.cdnleiting.top/gttkypgbje.html

[E04] 查找子串位置
来源：http://hz.gzhubu.top/gtjitxamgg.html

Py:   s.find("x");  s.index("x")
来源：http://hz.shanyushiyangkeji.top/gtreujdoqp.html

PHP:  strpos($s, "x");
来源：http://hz.ydzc1.top/gtwnzcdimd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.havefunace.top/gtimtmbfmq.html

TS:   s.indexOf("x")
来源：http://hz.havefunace.top/gthblcrzhb.html

Java: s.indexOf("x")
来源：http://hz.chenjidiqi.icu/gttwytdaox.html

Go:   strings.Index(s, "x")
来源：http://hz.kuanghao11.cn/gtroelqjao.html

Ruby: s.index("x")
来源：http://hz.nanxuanxn.top/gttyvgjajw.html

C#:   s.IndexOf("x")
来源：http://hz.jinyuanbaomall.cn/gtcmikpwxl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.sxryk.cn/gtktplahwb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.dashuyun.cn/gtuvaaynqn.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.tanke756.top/gtgvyqhiqj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hongshengwenyu.top/gtfuuyosvc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.nanxuanxn.top/gtjuhruqne.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.shangyingyoupin.top/gtghdbckyu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.quarkkingdee.top/gttqbuokmq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.cqqwz.cn/gtcyfgfuaq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jyoumei.cn/gtnxgrbhuk.html

[E06] 替换子串
来源：http://hz.hnqzz.top/gtfanlllsw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jinghuilouyu.cn/gtopimzgub.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.cdnleiting.top/gthgasdxyh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.ybcxt.top/gtlqtimqvq.html

TS:   s.replaceAll("a", "b")
来源：http://hz.yonumen.top/gtfdgwvmjv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hongshengwenyu.top/gtjqbfdlhu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.havefunace.top/gtclaguwcb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.hongshengwenyu.top/gtnxbuwodb.html

C#:   s.Replace("a", "b")
来源：http://hz.jqgufenzy.top/gtuhdtbvse.html

[E07] 按分隔符拆分
来源：http://hz.c1oappe.top/gtfiamgffq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.ybcxt.top/gtypdizzwc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.316326.xyz/gtrvbqfrlu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.wangshuangyany.cn/gtgheetapd.html

TS:   s.split(",")
来源：http://hz.wangdashe.top/gtsmlpayjd.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.sysykeji.top/gtfwvdvnrs.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.jinqigfzy.top/gtmxleiubt.html

Ruby: s.split(",");  s.split
来源：http://hz.shangyingyoupin.top/gtczjbjzzt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.aibaodan.cn/gtsobygyab.html

[E08] 数组按分隔符合并
来源：http://hz.yj20258.top/gtvkudooyw.html

Py:   ",".join(items)
来源：http://hz.ywan-chungtsiang.top/gtufjhsfql.html

PHP:  implode(",", $items);
来源：http://hz.fengsongda.top/gtikhuugsr.html

JS:   items.join(",")
来源：http://hz.daxiang520.top/gttqphefwp.html

TS:   items.join(",")
来源：http://hz.haohaochexian.top/gtyrkcindi.html

Java: String.join(",", items)
来源：http://hz.sysykeji.top/gtphgydlje.html

Go:   strings.Join(items, ",")
来源：http://hz.xinyue.icu/gtntacumbm.html

Ruby: items.join(",")
来源：http://hz.jqgufenzy.top/gtqhjldxpp.html

C#:   string.Join(",", items)
来源：http://hz.cashguo.top/gtzawlnrnv.html

[E09] 去除所有空白字符
来源：http://hz.cucudq.cn/gtwdlocsyl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.gotoacloud.top/gtcigzobtx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.wangdashe.top/gtlpfefqnb.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.yongpay.top/gtsnnoehbe.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.haohaochexian.top/gthucswoma.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yj20258888.top/gtbvwlmhlw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.fzhhl.top/gthrovrnrz.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.hfpthk.cn/gtyaxwqyno.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.hnxiangtu.top/gthxjmbjnp.html

[E10] 左侧补零 / 定长填充
来源：http://hz.sxryk.cn/gtljuthwgi.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.xuetiantiany.cn/gtmjsbnlcr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.pengpengdd.cyou/gtvmhamjlv.html

JS:   "7".padStart(3, "0")
来源：http://hz.dianchejie.cn/gtogttdwuv.html

TS:   "7".padStart(3, "0")
来源：http://hz.yj202588.top/gtyzetexfz.html

Java: String.format("%03d", 7)
来源：http://hz.chenzaomai.com/gtadwuqxuy.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.birdmap.top/gtyyjprekm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.chenjidiqi.icu/gtccquwgxa.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.snrcjt.cn/gtslypdpyo.html

[E11] 反转字符串
来源：http://hz.9152youxi.cn/gtyeesagaj.html

Py:   s[::-1]
来源：http://hz.yvedp.cn/gtsuqcrmhd.html

PHP:  strrev($s);
来源：http://hz.chenlongwang.top/gthbmmjgdn.html

JS:   [...s].reverse().join("")
来源：http://hz.nanxuanxn.top/gtnqyizxij.html

TS:   [...s].reverse().join("")
来源：http://hz.hnxiangtu.top/gturdasaeb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jinyuanbaomall.cn/gtxtbnogbw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.redwolf501.top/gtsiupewyl.html

Ruby: s.reverse
来源：http://hz.smart0.xyz/gtjnbsbecd.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.cucudq.cn/gtbptotqgk.html

[E12] 统计某字符出现次数
来源：http://hz.hammf.cn/gtejqkfdch.html

Py:   s.count("a")
来源：http://hz.dashuyun.cn/gtavylwslh.html

PHP:  substr_count($s, "a");
来源：http://hz.ybcxt.top/gtvotvojwh.html

JS:   s.split("a").length - 1
来源：http://hz.wangshuangyany.cn/gtpjqrwtqs.html

TS:   s.split("a").length - 1
来源：http://hz.yj20258.top/gtotuhziuk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jinyuanbaomall.cn/gtoqbqjbxb.html

Go:   strings.Count(s, "a")
来源：http://hz.birdmap.top/gtfslajbpa.html

Ruby: s.count("a")
来源：http://hz.fzhhl.top/gtmltsutvv.html

C#:   s.Count(c => c == 'a')
来源：http://hz.zhaomingkeji.xyz/gtvwoluzxo.html

[E13] 逐字符遍历
来源：http://hz.haohaochexian.top/gtqgfchqio.html

Py:   for ch in s: print(ch)
来源：http://hz.yj202588.top/gttacgetwv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jyoumei.cn/gtokludwit.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ppjwa.cn/gtxkqzgkst.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yj20258888.top/gtobibzbcg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.zhongyouzk.top/gtfrqugieq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.hfpthk.cn/gtsrteqcuw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zhoulong.xyz/gtdabnisfx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.daria6918.cn/gtqbclrfec.html

[E14] URL 编码与 Base64
来源：http://hz.ppjwa.cn/gtbrfshjxs.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.fengsongda.top/gtnpigbsrh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.daxiang520.top/gthlmmruxc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.mhx1999.top/gtwefwjnfn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.xuanzx.com/gtehupzbar.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.c1oappe.top/gtpsxjyxcb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.xziqi.cn/gtyhyinxlx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.wangdashe.top/gtrrqeoosw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.svipenyu.cn/gtweerqtga.html

[E15] HTML 转义 / 反转义
来源：http://hz.zhaomingkeji.xyz/gtoqoedphe.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.aibaodan.cn/gtviwgxmsa.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.chenlongwang.top/gtvrwjgste.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.aizwys.cn/gtxcgzkxpj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.ywan-chungtsiang.top/gtzwarnhyj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yj20258.top/gtmlwtfgxn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.sysykeji.top/gtkaknnqpr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.sweek.top/gtulfuyrgi.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jyoumei.cn/gthidyhsox.html

[E16] 数字千分位
来源：http://hz.shanyushiyangkeji.top/gtduxpwygd.html

Py:   f"{1234567:,}"
来源：http://hz.yueranfly.top/gtnnhbsvno.html

PHP:  number_format(1234567);
来源：http://hz.yuanzhike.top/gtqfafhaaf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.kuanghao11.cn/gtsvlhhzlr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.gogol.net.cn/gtpigzhcsz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.pengpengdd.cyou/gtqgzxyjdi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.hywenlv.cn/gtzmexjbrt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.chenzaomai.com/gtejdhiogv.html

C#:   1234567.ToString("N0")
来源：http://hz.xylfe.cn/gtgctxbfxo.html

[E17] 首字母大写
来源：http://hz.yj20258.top/gtlprynlrz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.fengsongda.top/gtnmepbuzg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jianghu66.top/gtdsrelzpx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xuanzx.com/gtngiruybg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.smart0.xyz/gtinpimdtb.html


<!-- 参考信息 -->