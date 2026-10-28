代发 wailian999

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.xuanzx.com/gtveqfuswp.html

TS:   [...a, ...b];
来源：http://hz.aibaodan.cn/gtrogsgplb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yj20258.top/gtwambfkwl.html

Go:   append(a, b...)
来源：http://hz.gaohongyu789.top/gtrzrhalhd.html

Ruby: a + b;  a.concat(b)
来源：http://hz.chenjidiqi.icu/gtpsltzwgm.html

C#:   a.Concat(b).ToList()
来源：http://hz.birdmap.top/gtlwifflbn.html

[D09] 排序（升序）
来源：http://hz.yonumen.top/gtrofjucxz.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinyuanbaomall.cn/gtxlyduscm.html

PHP:  sort($arr);
来源：http://hz.yuanzhike.top/gtkxvnstir.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hammf.cn/gtmhqmaxlk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.snrcjt.cn/gtnczygbgl.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.0kj1m.cn/gtnbscuebw.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.gotoacloud.top/gtiycjjhid.html

Ruby: arr.sort
来源：http://hz.zhijiandao.cn/gtfrcrfqmd.html

C#:   list.Sort();
来源：http://hz.hammf.cn/gtggablczh.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.shuidangran.top/gthupzxuws.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.aibaodan.cn/gtggyiewsb.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hfpthk.cn/gtlulxcknk.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.havefunace.top/gtsdnmbelv.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yj202588.top/gtwrlyhyan.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.9152youxi.cn/gtkqylwcgy.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.zhixingplan.top/gthvjyznte.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.dianchejie.cn/gtuslzymxg.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zhiwuduotai.top/gtxcfiqrij.html

[D11] 反转数组
来源：http://hz.0kj1m.cn/gtmumzhnfb.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.cheryme.top/gtdrphghhn.html

PHP:  array_reverse($arr);
来源：http://hz.meibo888.top/gtfdbwkalp.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.ydzc1.top/gtdhbpaxzz.html

TS:   [...arr].reverse();
来源：http://hz.wangdashe.top/gtvbekjeaa.html

Java: Collections.reverse(list);
来源：http://hz.vqdsnc.cn/gtyrgrcrjh.html

Go:   slices.Reverse(arr)
来源：http://hz.smart0.xyz/gtbtodkcdf.html

Ruby: arr.reverse
来源：http://hz.0kj1m.cn/gtrqyizacl.html

C#:   list.Reverse();
来源：http://hz.gzhubu.top/gtqedeaira.html

[D12] 查找元素下标
来源：http://hz.zhiwuduotai.top/gtmwmvsjby.html

Py:   arr.index(x);  x in arr
来源：http://hz.c1oappe.top/gtbqkcskdi.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.feifeiyinyue.top/gtqyqlqhkk.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.meibo888.top/gtjqbigsfz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.xuanzx.com/gthxahyjnp.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.shangyingyoupin.top/gthmwqzimv.html

Go:   slices.Index(arr, x)
来源：http://hz.havefunace.top/gtjuapckky.html

Ruby: arr.index(x)
来源：http://hz.shangyingyoupin.top/gtfpcvlmtj.html

C#:   list.IndexOf(x);
来源：http://hz.hywenlv.cn/gtvgjjqhyq.html

[D13] 过滤（保留满足条件的）
来源：http://hz.ivvv.top/gtbumuadep.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.xziqi.cn/gtgvkefzqo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.chenlongwang.top/gtkibiptpb.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jqgufenzy.top/gtojxxvrjf.html

TS:   arr.filter(x => x > 3)
来源：http://hz.hywenlv.cn/gtbbmsaoaj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.gaohongyu789.top/gtapyeeddo.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.wangshuangyany.cn/gtmozijbqm.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.haohaochexian.top/gtriluzqmf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jinqigfzy.top/gtrpxekuln.html

[D14] 映射转换（每个元素变形）
来源：http://hz.cheryme.top/gtgpbkyhii.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.cqqwz.cn/gtqluujogn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.tanke756.top/gtdffxypen.html

JS:   arr.map(x => x * 2)
来源：http://hz.shanyushiyangtech.top/gtdnquzntf.html

TS:   arr.map(x => x * 2)
来源：http://hz.jlsjyb.cn/gtfmcafurt.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zhiwuduotai.top/gtjqlphdzq.html

Go:   // 手写循环
来源：http://hz.jlsjyb.cn/gtafbjpksa.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.shanyushiyangtech.top/gtovrfymmz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.fengsongda.top/gtxhojpois.html

[D15] 去重
来源：http://hz.yuxming.cn/gtzrfljazk.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.pengpengdd.cyou/gteveovhse.html

PHP:  array_unique($arr);
来源：http://hz.jqgfzy.top/gtfrwxlyep.html

JS:   [...new Set(arr)]
来源：http://hz.daxiang520.top/gtcicgzicp.html

TS:   [...new Set(arr)]
来源：http://hz.shanyushiyangkeji.top/gtzlugxgei.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yj20258.top/gtilcgsyep.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.hnqzz.top/gtzcfnxdwf.html

Ruby: arr.uniq
来源：http://hz.jiagoushi.top/gtkgvpqtos.html

C#:   list.Distinct().ToList()
来源：http://hz.xuetiantiany.cn/gtxeoihatr.html

[D16] 求和与平均值
来源：http://hz.sxryk.cn/gtzhyazcsj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.sufxvd.cn/gtxyypohef.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jinqigufen.top/gthnwqvinh.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.gaohongyu789.top/gtoktjoekk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.birdmap.top/gtriawpoei.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.zdqjudy.top/gtxkfyiqeq.html

Go:   // 手写循环累加
来源：http://hz.jiagoushi.top/gtzqidgycz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.vqdsnc.cn/gttzcifyxa.html

C#:   list.Sum();  list.Average()
来源：http://hz.vqdsnc.cn/gtnuhiznhg.html

[D17] 最大值与最小值
来源：http://hz.xinyue.icu/gtbyiifepl.html

Py:   max(arr);  min(arr)
来源：http://hz.meibo888.top/gtbsldexra.html

PHP:  max($arr);  min($arr);
来源：http://hz.smart0.xyz/gtyxuolqdu.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.hywenlv.cn/gtafeixdtc.html

TS:   Math.max(...arr);
来源：http://hz.ivvv.top/gtkteyrtpv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.sweek.top/gtccathdbz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jqgfzy.top/gtqhhpcwbv.html

Ruby: arr.max;  arr.min
来源：http://hz.xuetiantiany.cn/gtrztfbgsm.html

C#:   list.Max();  list.Min()
来源：http://hz.cqqwz.cn/gtlmgbojxl.html

[D18] 扁平化嵌套数组
来源：http://hz.havefunace.top/gtjlyvgwhx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.ehwqpu.com/gtzqpjnijl.html

PHP:  array_merge(...$nested);
来源：http://hz.cdnleiting.top/gtquibcpfe.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.cucudq.cn/gtefroyvjk.html

TS:   nested.flat();
来源：http://hz.hnqzz.top/gtejhkuxcl.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.hywenlv.cn/gtamuconkl.html

Go:   // 手写双层循环
来源：http://hz.yanxiufei.cn/gtwojjtxdi.html

Ruby: nested.flatten
来源：http://hz.ydzc1.top/gtuwwdttdb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yj202588.top/gtqtrnmsck.html

[D19] 按字段分组
来源：http://hz.sxryk.cn/gtbhxiporc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jinghuilouyu.cn/gtvurogisu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.guowangkeji.top/gtpqstoqrq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.redwolf501.top/gtgllhvpik.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.nanxinkj.top/gtxwggwooc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.dashuyun.cn/gtorlhgsjy.html

Go:   // 手写 map[string][]T
来源：http://hz.shanyushiyangtech.top/gtddtmumre.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.havefunace.top/gtrtxugpbz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yueranfly.top/gtyosxiokp.html

[D20] 统计每个元素出现次数
来源：http://hz.xziqi.cn/gtloiqcmum.html

Py:   Counter(arr)
来源：http://hz.hnxiangtu.top/gtxjonmlci.html

PHP:  array_count_values($arr);
来源：http://hz.haohaochexian.top/gtaxfytydh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.redwolf501.top/gtggiajdyq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xuetiantiany.cn/gtxnjsjhce.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.feifeiyinyue.top/gtmbhsceew.html

Go:   // 手写 map[T]int
来源：http://hz.chenjidiqi.icu/gtfnopitec.html

Ruby: arr.tally
来源：http://hz.aibaodan.cn/gtjsvmlels.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.zhiwuduotai.top/gtyuyoqzvi.html

[D21] 判断是否包含某元素
来源：http://hz.mhx1999.top/gtxmhhnrrx.html

Py:   x in arr
来源：http://hz.yueranfly.top/gtqlgtznpo.html

PHP:  in_array($x, $arr, true);
来源：http://hz.52xcode.cn/gtsrfhplqa.html

JS:   arr.includes(x)
来源：http://hz.jinqigfzy.top/gtfinrlzuv.html

TS:   arr.includes(x)
来源：http://hz.hysaishi.cn/gtkuaneejh.html

Java: list.contains(x)
来源：http://hz.hywenlv.cn/gtqhulirkv.html

Go:   slices.Contains(arr, x)
来源：http://hz.sufxvd.cn/gtpluufeut.html

Ruby: arr.include?(x)
来源：http://hz.hfpthk.cn/gtwfwyuwuu.html

C#:   list.Contains(x)
来源：http://hz.sysykeji.top/gtkgbbyelq.html

[D22] 复制数组（避免共享引用）
来源：http://hz.tianlin.xyz/gtnzzorqed.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jinghuilouyu.cn/gtvhypehvf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yongpay.top/gtuamiytmx.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.hfpthk.cn/gttnonoxxw.html

TS:   [...arr];
来源：http://hz.fengsongda.top/gtwuncxtbu.html

Java: new ArrayList<>(list);
来源：http://hz.svipenyu.cn/gtzxqejztk.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.ydjk.org.cn/gtdivubstd.html

Ruby: arr.dup;  arr.clone
来源：http://hz.dashuyun.cn/gtvngcwqsp.html

C#:   new List<int>(list);
来源：http://hz.shangyingyoupin.top/gtzojenydf.html

[D23] reduce 累积计算
来源：http://hz.aizwys.cn/gtnwuyfqyb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.wangshuangyany.cn/gtuuyurzsp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jinghuilouyu.cn/gtpyyzmfhe.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.quarkkingdee.top/gtjrsxaaui.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zhijiandao.cn/gtbqnykoop.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.xuetiantiany.cn/gtqdbfjvdx.html

Go:   // 手写循环
来源：http://hz.hongshengwenyu.top/gtilvrafoq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.hammf.cn/gtbsrqjasm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yueranfly.top/gtkcmnjmjh.html

[D24] 字典 / Map 基本操作
来源：http://hz.hysaishi.cn/gttosaujji.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.tianlin.xyz/gtfxcbyfsd.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.chenlongwang.top/gtutauqowq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.pycfn.com/gtdewtfrxx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.sufxvd.cn/gtpzqlivoi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.hnxiangtu.top/gtimmbliia.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.haohaochexian.top/gthwkpjjif.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.ppjwa.cn/gtlprwkzok.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.mhx1999.top/gteslexxak.html

[D25] Set 集合去重与交并差
来源：http://hz.ybcxt.top/gtpjcfixwc.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.xuanzx.com/gtxvnuzpwh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.dashuyun.cn/gtlidrdlmh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.jinyuanbaomall.cn/gttfrouffp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.zhiwuduotai.top/gtiepenrvx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.sxryk.cn/gtgavtxpkf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.ydjk.org.cn/gtxozvudfz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jqgfzy.top/gtuomepyct.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.ydjk.org.cn/gtjzakqfyl.html

[D26] 数组转字符串
来源：http://hz.wangshuangyany.cn/gtgbyyoowa.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zdqjudy.top/gtpkylkqfc.html

PHP:  implode(", ", $arr);
来源：http://hz.9152youxi.cn/gtvwxjziyj.html

JS:   arr.join(", ")
来源：http://hz.mhx1999.top/gtvtsbsrei.html

TS:   arr.join(", ")
来源：http://hz.chenzaomai.com/gtpqnusuuv.html

Java: String.join(", ", list)
来源：http://hz.xingfuxueyuan.xyz/gtexyqmikw.html

Go:   strings.Join(strs, ", ")
来源：http://hz.quarkkingdee.top/gtncgbjhyo.html

Ruby: arr.join(", ")
来源：http://hz.sufxvd.cn/gtayqrddhx.html

C#:   string.Join(", ", list)
来源：http://hz.gogol.net.cn/gtkdsodewq.html

================================================================================
来源：http://hz.ivvv.top/gtqqmlhuki.html

E. 字符串处理
来源：http://hz.jqgfzy.top/gtvdmghess.html

================================================================================
来源：http://hz.hfpthk.cn/gtmqntmpeo.html

[E01] 拼接字符串
来源：http://hz.aizwys.cn/gtvekokeqo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.zycfv.cn/gtkurniizw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yj20258888.top/gtikshhqui.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.vqdsnc.cn/gtonhidmok.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.hywenlv.cn/gtyniwqigh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.zycfv.cn/gtiuulmkge.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.xuanzx.com/gtamtxdlmx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.pycfn.com/gtzqbzvfgp.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.xuetiantiany.cn/gtpbghekdm.html

[E02] 重复字符串
来源：http://hz.xinyue.icu/gtcdrecjbe.html

Py:   "ab" * 3
来源：http://hz.smart0.xyz/gtugoazcxf.html

PHP:  str_repeat("ab", 3);
来源：http://hz.chenzaomai.com/gtwfbdqjus.html

JS:   "ab".repeat(3)
来源：http://hz.guowangkeji.top/gtwrekjrxw.html

TS:   "ab".repeat(3)
来源：http://hz.cucudq.cn/gtowprdzrf.html

Java: "ab".repeat(3)
来源：http://hz.daria6918.cn/gtupbhgsbi.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zycfv.cn/gttsimkftw.html

Ruby: "ab" * 3
来源：http://hz.yj20258.top/gtenhbigxj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.aizwys.cn/gtcvpccemk.html

[E03] 截取子串
来源：http://hz.jinyuanbaomall.cn/gtnxaelefb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.andypj.xyz/gtatueaxlv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.wangdashe.top/gtzucdxzyu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yongpay.top/gtngeflnyu.html

TS:   s.slice(1, 4)
来源：http://hz.316326.xyz/gtjvkreudb.html

Java: s.substring(1, 4)
来源：http://hz.shangyingyoupin.top/gttmwwhles.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.xuetiantiany.cn/gtfccawedw.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.zhijiandao.cn/gtzvvmgzef.html

C#:   s.Substring(1, 3)
来源：http://hz.xingfuxueyuan.xyz/gtvebqcwop.html

[E04] 查找子串位置
来源：http://hz.cqqwz.cn/gtzzxzxdhm.html

Py:   s.find("x");  s.index("x")
来源：http://hz.yonumen.top/gtexlyvsci.html

PHP:  strpos($s, "x");
来源：http://hz.0kj1m.cn/gttqnvaahl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.nanxinkj.top/gtuqoeorth.html

TS:   s.indexOf("x")
来源：http://hz.jiagoushi.top/gtwsgtaqnu.html

Java: s.indexOf("x")
来源：http://hz.wangdashe.top/gtxcboznbm.html

Go:   strings.Index(s, "x")
来源：http://hz.zycfv.cn/gtvguvrpxq.html

Ruby: s.index("x")
来源：http://hz.hammf.cn/gtvehtmmkj.html

C#:   s.IndexOf("x")
来源：http://hz.jinyuanbaomall.cn/gttaoqeeqc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.zhongyouzk.top/gtqeidkdzz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.quarkkingdee.top/gtuyzxnmxx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.ehwqpu.com/gtftfnvyom.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.zycfv.cn/gtaunolvxj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.c1oappe.top/gtascxripo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.gotoacloud.top/gtocpcjbry.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.zhijiandao.cn/gtqjbgcvhf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.hysaishi.cn/gtwvkhqyig.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.chenjidiqi.icu/gtlgozdkyq.html

[E06] 替换子串
来源：http://hz.cdnleiting.top/gtggtvgact.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yuxming.cn/gtgozqtfcw.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.bjfxy.top/gtcxxnhrpl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.aibaodan.cn/gtcylfhlyw.html

TS:   s.replaceAll("a", "b")
来源：http://hz.havefunace.top/gtuctrxpbo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.kuanghao11.cn/gtjoctlzuu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.chenjidiqi.icu/gtvidciydd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.sysykeji.top/gteobrzlqv.html

C#:   s.Replace("a", "b")
来源：http://hz.shuidangran.top/gtpmwskgmv.html

[E07] 按分隔符拆分
来源：http://hz.yonumen.top/gtqcsfwvin.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.dianchejie.cn/gtacqbjper.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.shzxlz.cn/gtldktbamp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.jqgfzy.top/gtemizxnql.html

TS:   s.split(",")
来源：http://hz.ybcxt.top/gttswbxbcy.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.jinqigfzy.top/gtwchpnfvy.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yj20258.top/gtygrcswjo.html

Ruby: s.split(",");  s.split
来源：http://hz.vqdsnc.cn/gtxvkhnroz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.kuanghao11.cn/gthycwvpbo.html

[E08] 数组按分隔符合并
来源：http://hz.wangdashe.top/gtcvosyefv.html

Py:   ",".join(items)
来源：http://hz.xinyue.icu/gtitqxvvgf.html

PHP:  implode(",", $items);
来源：http://hz.shzxlz.cn/gtvhdeashv.html

JS:   items.join(",")
来源：http://hz.zycfv.cn/gtjwxsbwtg.html

TS:   items.join(",")
来源：http://hz.tian-w.cn/gtaszczkfc.html

Java: String.join(",", items)
来源：http://hz.andypj.xyz/gtxcdhtucs.html

Go:   strings.Join(items, ",")
来源：http://hz.sysykeji.top/gtztkkvnlr.html

Ruby: items.join(",")
来源：http://hz.zhaomingkeji.xyz/gthyoajnwr.html

C#:   string.Join(",", items)
来源：http://hz.pengpengdd.cyou/gtleopqvyc.html

[E09] 去除所有空白字符
来源：http://hz.jiagoushi.top/gtlqdlnvfc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.sxryk.cn/gtvbgobeaz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.9152youxi.cn/gtkjkplapz.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.aizwys.cn/gttafkuugl.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.andypj.xyz/gtjrunvbwv.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.shuidangran.top/gtroygcmgp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zycfv.cn/gtueowogjd.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.hysaishi.cn/gtnszmfzoo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.dashuyun.cn/gtfvwasndd.html

[E10] 左侧补零 / 定长填充
来源：http://hz.cheryme.top/gtgfdkspgg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yueranfly.top/gthcniyuyw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.shanyushiyangkeji.top/gtnywziiin.html

JS:   "7".padStart(3, "0")
来源：http://hz.cdnleiting.top/gtvueyprxk.html

TS:   "7".padStart(3, "0")
来源：http://hz.cashguo.top/gtgvolvsyp.html

Java: String.format("%03d", 7)
来源：http://hz.zhoulong.xyz/gtmgyemjdh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yj20258888.top/gthcttuejd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.nanxinkj.top/gtlmlzykdv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.gogol.net.cn/gtmawpcoxp.html

[E11] 反转字符串
来源：http://hz.shzxlz.cn/gtmeredczk.html

Py:   s[::-1]
来源：http://hz.kuanghao11.cn/gtlnecdney.html

PHP:  strrev($s);
来源：http://hz.jiagoushi.top/gtxxakndcf.html

JS:   [...s].reverse().join("")
来源：http://hz.xuanzx.com/gtihjnafkz.html

TS:   [...s].reverse().join("")
来源：http://hz.meibo888.top/gtztckipal.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jinghuilouyu.cn/gtodxehvgk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yonumen.top/gtsdbjdbbw.html

Ruby: s.reverse
来源：http://hz.quarkkingdee.top/gtpwwbqdxd.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.sweek.top/gtmpwusvro.html

[E12] 统计某字符出现次数
来源：http://hz.zhoulong.xyz/gtcdllpydf.html

Py:   s.count("a")
来源：http://hz.meibo888.top/gtrfwwlpxy.html

PHP:  substr_count($s, "a");
来源：http://hz.haohaochexian.top/gtzqayzziv.html

JS:   s.split("a").length - 1
来源：http://hz.havefunace.top/gtgpkdhebt.html

TS:   s.split("a").length - 1
来源：http://hz.zhengqikj.top/gttvztkpgq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.nanxuanxn.top/gtsqokgdmp.html

Go:   strings.Count(s, "a")
来源：http://hz.xylfe.cn/gtmkbwsdej.html

Ruby: s.count("a")
来源：http://hz.shanyushiyangkeji.top/gtgqpcgikc.html

C#:   s.Count(c => c == 'a')
来源：http://hz.gaohongyu789.top/gtbuxzlubv.html

[E13] 逐字符遍历
来源：http://hz.hywenlv.cn/gtayamyaoy.html

Py:   for ch in s: print(ch)
来源：http://hz.zhiwuduotai.top/gtprmfcfdy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zhoulong.xyz/gtdcqoijjt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.guowangkeji.top/gthgzzvpfs.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.9152youxi.cn/gtgqajqdts.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.ydzc1.top/gtszdwkqaj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.tian-w.cn/gtohzmkqni.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.ydzc1.top/gtkkxebksa.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.havefunace.top/gtikyswprv.html

[E14] URL 编码与 Base64
来源：http://hz.fzhhl.top/gtyuptlgmm.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.gzhubu.top/gtkbimebpa.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.shuidangran.top/gtriadebhl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.iojbl.cn/gtwsjidhey.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.xingfuxueyuan.xyz/gtezpqekdt.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.cqqwz.cn/gtiisoaliq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jianghu66.top/gttiafbkxt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.havefunace.top/gtwphzxrpz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.chenzaomai.com/gthlrltfzi.html

[E15] HTML 转义 / 反转义
来源：http://hz.haohaochexian.top/gtcmabtqyk.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.daria6918.cn/gtitlyjkoc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.smart0.xyz/gtvktbqghb.html


<!-- 参考信息 -->