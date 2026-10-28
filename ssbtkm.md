代发 wailian999

TS:   arr.slice(1, 4);
来源：http://hz.cqqwz.cn/gtucnuutxf.html

Java: list.subList(1, 4);
来源：http://hz.hongshengwenyu.top/gteayiyhji.html

Go:   arr[1:4]
来源：http://hz.gaohongyu789.top/gtznjtkvnu.html

Ruby: arr[1, 3]
来源：http://hz.ivvv.top/gtcsckqlcx.html

C#:   list.GetRange(1, 3);
来源：http://hz.0kj1m.cn/gtuxtgidhf.html

[D08] 合并两个数组
来源：http://hz.316326.xyz/gtkmnkmxmb.html

Py:   a + b;  a.extend(b)
来源：http://hz.nanxuanxn.top/gtsptfypez.html

PHP:  array_merge($a, $b);
来源：http://hz.dianchejie.cn/gtlkvpzays.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.cucudq.cn/gtddyuncgn.html

TS:   [...a, ...b];
来源：http://hz.zhaomingkeji.xyz/gtsmzppcgi.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.ivvv.top/gtswitqbzo.html

Go:   append(a, b...)
来源：http://hz.svipenyu.cn/gtqpkygcop.html

Ruby: a + b;  a.concat(b)
来源：http://hz.xylfe.cn/gtzwigipax.html

C#:   a.Concat(b).ToList()
来源：http://hz.vqdsnc.cn/gtfwlbbrit.html

[D09] 排序（升序）
来源：http://hz.ywan-chungtsiang.top/gtrvtfnugl.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.xziqi.cn/gtlzqwnwqz.html

PHP:  sort($arr);
来源：http://hz.cucudq.cn/gtnpbstjhu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.jiagoushi.top/gthknkmzye.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.jinqigufen.top/gtilaigubb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.zdqjudy.top/gtpuwyvmra.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.hnxiangtu.top/gtgninhlah.html

Ruby: arr.sort
来源：http://hz.dianchejie.cn/gtmbkwwmhh.html

C#:   list.Sort();
来源：http://hz.jinqigfzy.top/gtlfecbhrp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.xylfe.cn/gtbeyxbips.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zhijiandao.cn/gtpcxrfpqm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.guannengcc.top/gteimhykvj.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jiagoushi.top/gtdlfwfoue.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.feifeiyinyue.top/gtfzbynsik.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.daria6918.cn/gtywbegarw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.fengsongda.top/gtqfqbobii.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.birdmap.top/gtozmarqsb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.andypj.xyz/gtkiuqckiy.html

[D11] 反转数组
来源：http://hz.mhx1999.top/gtqrblyhfp.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zhixingplan.top/gtdwvkeyrr.html

PHP:  array_reverse($arr);
来源：http://hz.mhx1999.top/gtbxucxarm.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jqgfzy.top/gtgiccmjvq.html

TS:   [...arr].reverse();
来源：http://hz.jyoumei.cn/gtbmghmarh.html

Java: Collections.reverse(list);
来源：http://hz.ydzc1.top/gtwgbqtfag.html

Go:   slices.Reverse(arr)
来源：http://hz.havefunace.top/gtilpjruoa.html

Ruby: arr.reverse
来源：http://hz.jianghu66.top/gtunenujxk.html

C#:   list.Reverse();
来源：http://hz.9152youxi.cn/gtkemgabkj.html

[D12] 查找元素下标
来源：http://hz.jqgufenzy.top/gtuojfdcjo.html

Py:   arr.index(x);  x in arr
来源：http://hz.andypj.xyz/gtevgtjjbe.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.cqqwz.cn/gtuxogatbd.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.tian-w.cn/gtplqhrgpp.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.nwbrower.top/gtifmghwmq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.gotoacloud.top/gtymifoqxi.html

Go:   slices.Index(arr, x)
来源：http://hz.c1oappe.top/gtegtaptwc.html

Ruby: arr.index(x)
来源：http://hz.gotoacloud.top/gtvlnmoabq.html

C#:   list.IndexOf(x);
来源：http://hz.andypj.xyz/gtejmvcmmy.html

[D13] 过滤（保留满足条件的）
来源：http://hz.chenzaomai.com/gtrhyalszg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.ybcxt.top/gtzgwbdvll.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.meibo888.top/gtnihrzuoo.html

JS:   arr.filter(x => x > 3)
来源：http://hz.bjfxy.top/gtokxfquvg.html

TS:   arr.filter(x => x > 3)
来源：http://hz.9152youxi.cn/gtnfzoqofy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.ydzc1.top/gtfbjdzbmh.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.yanxiufei.cn/gtfllwmooi.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.andypj.xyz/gtvajhqsqm.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.smart0.xyz/gtfjbuclwp.html

[D14] 映射转换（每个元素变形）
来源：http://hz.wangshuangyany.cn/gtadleobds.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.jqgfzy.top/gttbaztlsi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.c1oappe.top/gtzbgbeeuu.html

JS:   arr.map(x => x * 2)
来源：http://hz.snrcjt.cn/gtrgrjzkaj.html

TS:   arr.map(x => x * 2)
来源：http://hz.fengsongda.top/gteerqkjtf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.wangdashe.top/gtiwndwzui.html

Go:   // 手写循环
来源：http://hz.ivvv.top/gtvfyrpkup.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.cheryme.top/gtfrrlrrds.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.sysykeji.top/gtucmbimuv.html

[D15] 去重
来源：http://hz.jianghu66.top/gtgbtsngax.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jinghuilouyu.cn/gtsomripyr.html

PHP:  array_unique($arr);
来源：http://hz.kuanghao11.cn/gtfzfueaoi.html

JS:   [...new Set(arr)]
来源：http://hz.jinyuanbaomall.cn/gthihpkwok.html

TS:   [...new Set(arr)]
来源：http://hz.havefunace.top/gtppzvlore.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.dianchejie.cn/gtrlmwqirs.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.shanyushiyangtech.top/gtcsowwwce.html

Ruby: arr.uniq
来源：http://hz.xinyue.icu/gtrqllmpvc.html

C#:   list.Distinct().ToList()
来源：http://hz.hysaishi.cn/gtpqqwaprd.html

[D16] 求和与平均值
来源：http://hz.sysykeji.top/gtggiwtxjs.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yuxming.cn/gtvqwfgdst.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yj20258.top/gtviwpbxir.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yj20258.top/gtopsetbrk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jqgfzy.top/gtrmcwutyu.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.zhengqikj.top/gtbanlwixj.html

Go:   // 手写循环累加
来源：http://hz.yj20258888.top/gtlognymdm.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.xinyue.icu/gtflndjwuw.html

C#:   list.Sum();  list.Average()
来源：http://hz.9152youxi.cn/gtekwgddws.html

[D17] 最大值与最小值
来源：http://hz.gzhubu.top/gtazyqujsf.html

Py:   max(arr);  min(arr)
来源：http://hz.hnxiangtu.top/gttrkqiikw.html

PHP:  max($arr);  min($arr);
来源：http://hz.andypj.xyz/gtohoarndm.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.sysykeji.top/gthifslknm.html

TS:   Math.max(...arr);
来源：http://hz.pengpengdd.cyou/gtmbmfcijm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.ybcxt.top/gtqukmeapk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.yuxming.cn/gttxdwueuz.html

Ruby: arr.max;  arr.min
来源：http://hz.wangshuangyany.cn/gtgvhnjapp.html

C#:   list.Max();  list.Min()
来源：http://hz.gogol.net.cn/gtbwuknzyh.html

[D18] 扁平化嵌套数组
来源：http://hz.pycfn.com/gtnuqevcmm.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.hywenlv.cn/gtibpmzgxh.html

PHP:  array_merge(...$nested);
来源：http://hz.chenlongwang.top/gtbkoxapri.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.fengsongda.top/gtzhruhoqj.html

TS:   nested.flat();
来源：http://hz.yj20258.top/gtbplrdcud.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.shanyushiyangkeji.top/gtkyhwvuzb.html

Go:   // 手写双层循环
来源：http://hz.iojbl.cn/gtznukznwm.html

Ruby: nested.flatten
来源：http://hz.yvedp.cn/gtoyubgdrw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.shanyushiyangkeji.top/gtiitlmxva.html

[D19] 按字段分组
来源：http://hz.fengsongda.top/gtgyqgrnyc.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.jyoumei.cn/gttqyvzcuv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.shzxlz.cn/gtwolcjpqx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.cqqwz.cn/gtjnydoyip.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jqgfzy.top/gtmkxwnnwp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jyoumei.cn/gtvtzbjkdv.html

Go:   // 手写 map[string][]T
来源：http://hz.jyoumei.cn/gtxbujkzhy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.jyoumei.cn/gtrsqcjwyq.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.daxiang520.top/gtzrywiyvs.html

[D20] 统计每个元素出现次数
来源：http://hz.bjfxy.top/gtgkpxtpzk.html

Py:   Counter(arr)
来源：http://hz.yj20258.top/gtxwzdevqh.html

PHP:  array_count_values($arr);
来源：http://hz.nwbrower.top/gthobcedsx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jqgfzy.top/gtauehzwro.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yuxming.cn/gtvtieyoyg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ppjwa.cn/gtarzegfav.html

Go:   // 手写 map[T]int
来源：http://hz.snrcjt.cn/gtdgjfjvwo.html

Ruby: arr.tally
来源：http://hz.zhengqikj.top/gtchgbyhtl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.jiagoushi.top/gtldpzflmh.html

[D21] 判断是否包含某元素
来源：http://hz.jqgufenzy.top/gtkfbxqwba.html

Py:   x in arr
来源：http://hz.hnqzz.top/gtpigbuvtu.html

PHP:  in_array($x, $arr, true);
来源：http://hz.cdnleiting.top/gtbyiojetw.html

JS:   arr.includes(x)
来源：http://hz.iojbl.cn/gtkybgpetz.html

TS:   arr.includes(x)
来源：http://hz.nwbrower.top/gtmmlbzapl.html

Java: list.contains(x)
来源：http://hz.yongpay.top/gtidqyxftb.html

Go:   slices.Contains(arr, x)
来源：http://hz.nwbrower.top/gtpwgbslxn.html

Ruby: arr.include?(x)
来源：http://hz.c1oappe.top/gtriqhtddx.html

C#:   list.Contains(x)
来源：http://hz.gzhubu.top/gtgewujffy.html

[D22] 复制数组（避免共享引用）
来源：http://hz.zhaomingkeji.xyz/gtqkxhemfn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jiagoushi.top/gtqpqbumjj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.hnqzz.top/gtauromkdc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.hnqzz.top/gtuyefgrko.html

TS:   [...arr];
来源：http://hz.52xcode.cn/gtqjsltpvh.html

Java: new ArrayList<>(list);
来源：http://hz.jiagoushi.top/gtmeiuxlwn.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.ydjk.org.cn/gtttapwsum.html

Ruby: arr.dup;  arr.clone
来源：http://hz.shzxlz.cn/gtylpvqkio.html

C#:   new List<int>(list);
来源：http://hz.yvedp.cn/gtlvmwbvcv.html

[D23] reduce 累积计算
来源：http://hz.jinghuilouyu.cn/gtprbwtspu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.kuanghao11.cn/gtvbpjmfwg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.redwolf501.top/gtcxykodab.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.cqqwz.cn/gtdgqobwyj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.redwolf501.top/gthshilstx.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.birdmap.top/gtxfrbvabh.html

Go:   // 手写循环
来源：http://hz.yongpay.top/gtaekywnkp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.jqgufenzy.top/gtpitwwxbe.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.birdmap.top/gtkbogyvtf.html

[D24] 字典 / Map 基本操作
来源：http://hz.tian-w.cn/gtbtbqossc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.cdnleiting.top/gtomqhtcya.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.xuanzx.com/gtduapkagc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.zhaomingkeji.xyz/gtwflfhnag.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.ybcxt.top/gtwwnvoyfq.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.zhaomingkeji.xyz/gtttgkuwep.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.zhoulong.xyz/gtfpkvxurw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.kuanghao11.cn/gtrhfttbwf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.hnqzz.top/gtusxpoqgt.html

[D25] Set 集合去重与交并差
来源：http://hz.tianlin.xyz/gtfwubpmvw.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.xylfe.cn/gtzkfkvcwz.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.xuanzx.com/gtxxdnkoiv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.c1oappe.top/gtbekkpped.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.meibo888.top/gtsacvzbxv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.xuanzx.com/gtwyhzqnbn.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.jinghuilouyu.cn/gtrwvllmid.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.cucudq.cn/gtzllryuev.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.cucudq.cn/gtscqruhra.html

[D26] 数组转字符串
来源：http://hz.hongshengwenyu.top/gttenczoox.html

Py:   ", ".join(map(str, arr))
来源：http://hz.haohaochexian.top/gtmufpekhi.html

PHP:  implode(", ", $arr);
来源：http://hz.ydjk.org.cn/gtnvdhkjrv.html

JS:   arr.join(", ")
来源：http://hz.shanyushiyangtech.top/gtgjzifmem.html

TS:   arr.join(", ")
来源：http://hz.hnqzz.top/gtedotleme.html

Java: String.join(", ", list)
来源：http://hz.pengpengdd.cyou/gttrhpmwpv.html

Go:   strings.Join(strs, ", ")
来源：http://hz.redwolf501.top/gtaklhlwwo.html

Ruby: arr.join(", ")
来源：http://hz.wangdashe.top/gtlbsngbtq.html

C#:   string.Join(", ", list)
来源：http://hz.yuxming.cn/gtttfrdiyh.html

================================================================================
来源：http://hz.snrcjt.cn/gtbbbylzof.html

E. 字符串处理
来源：http://hz.guannengcc.top/gthhjyqhot.html

================================================================================
来源：http://hz.cheryme.top/gttxwdpvlq.html

[E01] 拼接字符串
来源：http://hz.hongshengwenyu.top/gtqimjivxk.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.ehwqpu.com/gtnfxiiiel.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.gogol.net.cn/gtftrduohu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.birdmap.top/gtxxnwkwjm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.0kj1m.cn/gtkqlknakr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.zhengqikj.top/gtlucifpmy.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.iojbl.cn/gtifkljwav.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jqgfzy.top/gtqmhuisno.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.yanxiufei.cn/gtfusmiaor.html

[E02] 重复字符串
来源：http://hz.shzxlz.cn/gtwehyufaq.html

Py:   "ab" * 3
来源：http://hz.vqdsnc.cn/gtpkedtiwe.html

PHP:  str_repeat("ab", 3);
来源：http://hz.xinyue.icu/gtlahvhegw.html

JS:   "ab".repeat(3)
来源：http://hz.sxryk.cn/gtxdfxhdmy.html

TS:   "ab".repeat(3)
来源：http://hz.jqgfzy.top/gtevuhsarl.html

Java: "ab".repeat(3)
来源：http://hz.xziqi.cn/gthzaumwov.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.shangyingyoupin.top/gtxyevgbfq.html

Ruby: "ab" * 3
来源：http://hz.shangyingyoupin.top/gttutpxjfu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.jqgfzy.top/gtzhlmeqzo.html

[E03] 截取子串
来源：http://hz.yueranfly.top/gtixovthsd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.dashuyun.cn/gtbtypngwg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.gaohongyu789.top/gtywcuybly.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.vqdsnc.cn/gtulxnxnga.html

TS:   s.slice(1, 4)
来源：http://hz.jqgfzy.top/gtpgjawgnc.html

Java: s.substring(1, 4)
来源：http://hz.wangshuangyany.cn/gttyyzrbib.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.jinyuanbaomall.cn/gtcmzzsltz.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.gzhubu.top/gtseffndhg.html

C#:   s.Substring(1, 3)
来源：http://hz.shanyushiyangtech.top/gtsnfshkty.html

[E04] 查找子串位置
来源：http://hz.yj20258.top/gtpcgaghrc.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jiagoushi.top/gtzhxsnutg.html

PHP:  strpos($s, "x");
来源：http://hz.fzhhl.top/gtgwmcbnra.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.fzhhl.top/gtxnemehcb.html

TS:   s.indexOf("x")
来源：http://hz.pycfn.com/gtceruyhjd.html

Java: s.indexOf("x")
来源：http://hz.yonumen.top/gtqwivrbdb.html

Go:   strings.Index(s, "x")
来源：http://hz.feifeiyinyue.top/gtpofjnoyu.html

Ruby: s.index("x")
来源：http://hz.zhaomingkeji.xyz/gtqpbgzrwy.html

C#:   s.IndexOf("x")
来源：http://hz.ydzc1.top/gtymcpveny.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.sxryk.cn/gtfqcpsdrg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.hnxiangtu.top/gtoftowwze.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zycfv.cn/gtqjeepadn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.kuanghao11.cn/gtmrsbjstj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zhongyouzk.top/gtkslmzjal.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jyoumei.cn/gtxwyloqrq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.cheryme.top/gtlkntkzuq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.aibaodan.cn/gtgxqtknqt.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jianghu66.top/gtpfbywylv.html

[E06] 替换子串
来源：http://hz.ppjwa.cn/gtzfeumsyw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.zhaomingkeji.xyz/gthvrfywvz.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.nwbrower.top/gtxvsdboab.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.316326.xyz/gtfikitunz.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jiagoushi.top/gttvdxpind.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.fengsongda.top/gtspvvjfvk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.yongpay.top/gtgztpxjpg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.daxiang520.top/gtslthkxso.html

C#:   s.Replace("a", "b")
来源：http://hz.cdnleiting.top/gtzckqlggc.html

[E07] 按分隔符拆分
来源：http://hz.svipenyu.cn/gtkgdkswse.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.hammf.cn/gtfxarmzmo.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.pengpengdd.cyou/gtcsefuqlt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.shuidangran.top/gtzhqeextr.html

TS:   s.split(",")
来源：http://hz.jinyuanbaomall.cn/gtbeabufkc.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.ehwqpu.com/gtafgcdzeo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.52xcode.cn/gthgiymhng.html

Ruby: s.split(",");  s.split
来源：http://hz.tianlin.xyz/gtovxcxaxs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.nanxuanxn.top/gtroreeawo.html

[E08] 数组按分隔符合并
来源：http://hz.ydjk.org.cn/gtvmlnfzpe.html

Py:   ",".join(items)
来源：http://hz.guowangkeji.top/gtetnnfucn.html

PHP:  implode(",", $items);
来源：http://hz.yangfankeji.com/gtxlnwezgy.html

JS:   items.join(",")
来源：http://hz.shzxlz.cn/gtxkxitgom.html

TS:   items.join(",")
来源：http://hz.aizwys.cn/gtuitjvrat.html

Java: String.join(",", items)
来源：http://hz.ybcxt.top/gtfasjuoqy.html

Go:   strings.Join(items, ",")
来源：http://hz.yj20258.top/gtsjwlhpub.html

Ruby: items.join(",")
来源：http://hz.bjfxy.top/gtefqrqqpc.html

C#:   string.Join(",", items)
来源：http://hz.ybcxt.top/gtjsfhpsjh.html

[E09] 去除所有空白字符
来源：http://hz.pengpengdd.cyou/gtrnvvhdez.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.aizwys.cn/gttnjnfwvb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.vqdsnc.cn/gtqrxbadkm.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.ehwqpu.com/gtmhiflroq.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.xylfe.cn/gtljlnpdmy.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.shzxlz.cn/gtardhbkhf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.hnqzz.top/gtfiuchrtl.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.ppjwa.cn/gtwunmjkkj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.kuanghao11.cn/gtgpwpcifm.html

[E10] 左侧补零 / 定长填充
来源：http://hz.gogol.net.cn/gtqjmmhvsk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.0kj1m.cn/gtlmsdgeyf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.gzhubu.top/gtyevsjemc.html

JS:   "7".padStart(3, "0")
来源：http://hz.yuxming.cn/gtyefdbrtv.html

TS:   "7".padStart(3, "0")
来源：http://hz.snrcjt.cn/gthtrllrru.html

Java: String.format("%03d", 7)
来源：http://hz.316326.xyz/gtboxsatgo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zhaomingkeji.xyz/gtxgysvthb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zhixingplan.top/gtjkpgctju.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.0kj1m.cn/gtioevabyv.html

[E11] 反转字符串
来源：http://hz.xingfuxueyuan.xyz/gtxcfkzyge.html

Py:   s[::-1]
来源：http://hz.ydzc1.top/gtfocbjjvk.html

PHP:  strrev($s);
来源：http://hz.9152youxi.cn/gtgtfhlqqs.html

JS:   [...s].reverse().join("")
来源：http://hz.xingfuxueyuan.xyz/gtcydoyhre.html

TS:   [...s].reverse().join("")
来源：http://hz.cqqwz.cn/gtreelfsrq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yanxiufei.cn/gtrkhopmlu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.gaohongyu789.top/gtqoyfprna.html

Ruby: s.reverse
来源：http://hz.xylfe.cn/gtfpxpbwku.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.redwolf501.top/gtpftwdnsb.html

[E12] 统计某字符出现次数
来源：http://hz.xuetiantiany.cn/gtrvfwbwfd.html

Py:   s.count("a")
来源：http://hz.shzxlz.cn/gtininzvuf.html

PHP:  substr_count($s, "a");
来源：http://hz.andypj.xyz/gthqrcoksq.html

JS:   s.split("a").length - 1
来源：http://hz.cdnleiting.top/gteusnbhba.html

TS:   s.split("a").length - 1
来源：http://hz.xuetiantiany.cn/gtlpjjazhq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.cucudq.cn/gtdlilpjgb.html

Go:   strings.Count(s, "a")
来源：http://hz.gaohongyu789.top/gtzpsbbfjn.html

Ruby: s.count("a")
来源：http://hz.jinghuilouyu.cn/gtuljdhgvb.html

C#:   s.Count(c => c == 'a')
来源：http://hz.tian-w.cn/gtbhdqhpau.html

[E13] 逐字符遍历
来源：http://hz.yueranfly.top/gtjglfwbyv.html

Py:   for ch in s: print(ch)
来源：http://hz.ehwqpu.com/gtzvvkucfc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.haohaochexian.top/gtgftkcuhy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.nanxuanxn.top/gtirnxkljk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhaomingkeji.xyz/gtlpciaqvv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.bjfxy.top/gtslbtnysx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.sxryk.cn/gtnxuuenwb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.fzhhl.top/gtasxawxhs.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.svipenyu.cn/gthfenriph.html

[E14] URL 编码与 Base64
来源：http://hz.tanke756.top/gttqknogoi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.aizwys.cn/gtxgndkvtb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.tanke756.top/gtbixeuyme.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.zdqjudy.top/gtgqnlflwj.html


<!-- 参考信息 -->