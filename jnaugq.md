代发 wailian999

Py:   len(arr)
来源：http://hz.xuetiantiany.cn/gtkzinvnbd.html

PHP:  count($arr);
来源：http://hz.pycfn.com/gttvrcfysc.html

JS:   arr.length
来源：http://hz.hammf.cn/gtaigncqaf.html

TS:   arr.length
来源：http://hz.jqgufenzy.top/gtreiqnzfz.html

Java: list.size();
来源：http://hz.shzxlz.cn/gtruuxeorz.html

Go:   len(arr)
来源：http://hz.xinyue.icu/gtkucphvxa.html

Ruby: arr.length; arr.size
来源：http://hz.mhx1999.top/gtdbeqfcoq.html

C#:   list.Count;
来源：http://hz.andypj.xyz/gtyeecadxr.html

[D07] 切片 / 取子数组
来源：http://hz.wangdashe.top/gtytocdhnb.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.zhengqikj.top/gtbslnocuj.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yanxiufei.cn/gtpgatwzml.html

JS:   arr.slice(1, 4);
来源：http://hz.pengpengdd.cyou/gtloldusty.html

TS:   arr.slice(1, 4);
来源：http://hz.xingfuxueyuan.xyz/gtruweqjwk.html

Java: list.subList(1, 4);
来源：http://hz.svipenyu.cn/gtjeopswmh.html

Go:   arr[1:4]
来源：http://hz.52xcode.cn/gtzsgptzyu.html

Ruby: arr[1, 3]
来源：http://hz.mhx1999.top/gtjblffeby.html

C#:   list.GetRange(1, 3);
来源：http://hz.9152youxi.cn/gtfdvvbtgy.html

[D08] 合并两个数组
来源：http://hz.yangfankeji.com/gtwdcbhifj.html

Py:   a + b;  a.extend(b)
来源：http://hz.hnqzz.top/gtvnejjvqy.html

PHP:  array_merge($a, $b);
来源：http://hz.sxryk.cn/gtjrtrwygl.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.cdnleiting.top/gtucijexje.html

TS:   [...a, ...b];
来源：http://hz.havefunace.top/gtjlkvxhce.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yvedp.cn/gtdjhsiyex.html

Go:   append(a, b...)
来源：http://hz.dianchejie.cn/gtfddzefat.html

Ruby: a + b;  a.concat(b)
来源：http://hz.jqgufenzy.top/gticxthceo.html

C#:   a.Concat(b).ToList()
来源：http://hz.xziqi.cn/gtjiwkdaac.html

[D09] 排序（升序）
来源：http://hz.ybcxt.top/gtwmoyddxt.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yj202588.top/gtfxakyqpd.html

PHP:  sort($arr);
来源：http://hz.chenjidiqi.icu/gtmhyabgzw.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.birdmap.top/gtoxipgioj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.gzhubu.top/gtgkqxmbgg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.cdnleiting.top/gtqnghzwrx.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.meibo888.top/gtpvkuupgu.html

Ruby: arr.sort
来源：http://hz.jinqigfzy.top/gtihtfvwgm.html

C#:   list.Sort();
来源：http://hz.zhixingplan.top/gtasxyszof.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.pengpengdd.cyou/gtfxcfwzaa.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.meibo888.top/gtvvtrzqqf.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.pycfn.com/gtrdzkurof.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.iojbl.cn/gtosbzttcx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shanyushiyangtech.top/gtlbyqfsst.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jqgufenzy.top/gtotroxszh.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.chenjidiqi.icu/gtcwmckhmf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.jinqigufen.top/gtupxvpznx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.iojbl.cn/gtynxmpuly.html

[D11] 反转数组
来源：http://hz.gaohongyu789.top/gtfkxqggmc.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.zhixingplan.top/gtudjxtlqv.html

PHP:  array_reverse($arr);
来源：http://hz.yuxming.cn/gtqtoybgsz.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yonumen.top/gtqcaimiqk.html

TS:   [...arr].reverse();
来源：http://hz.316326.xyz/gtgmqddfrs.html

Java: Collections.reverse(list);
来源：http://hz.ppjwa.cn/gtxlfdvhsj.html

Go:   slices.Reverse(arr)
来源：http://hz.xuetiantiany.cn/gtynmnblei.html

Ruby: arr.reverse
来源：http://hz.feifeiyinyue.top/gtsbgzjwic.html

C#:   list.Reverse();
来源：http://hz.iojbl.cn/gtgasotqpq.html

[D12] 查找元素下标
来源：http://hz.zhengqikj.top/gtkfeeghvg.html

Py:   arr.index(x);  x in arr
来源：http://hz.birdmap.top/gtmmbxjrzc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.cashguo.top/gtsckuoaej.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yueranfly.top/gtblbuohgz.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yvedp.cn/gtavremxmo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.zhiwuduotai.top/gtaykzybud.html

Go:   slices.Index(arr, x)
来源：http://hz.316326.xyz/gtjjgsnfjg.html

Ruby: arr.index(x)
来源：http://hz.daria6918.cn/gtrnkuxvff.html

C#:   list.IndexOf(x);
来源：http://hz.shanyushiyangtech.top/gtzaghyxvh.html

[D13] 过滤（保留满足条件的）
来源：http://hz.xingfuxueyuan.xyz/gtewlgwxya.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.shanyushiyangtech.top/gtsgivfuvd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.shuidangran.top/gtxvrexarx.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yj20258.top/gtebrbkdmp.html

TS:   arr.filter(x => x > 3)
来源：http://hz.yongpay.top/gtqcmgzunh.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.shangyingyoupin.top/gtlfeogaec.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.bjfxy.top/gtgpwisjbr.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.yj202588.top/gtxypipyih.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.cqqwz.cn/gtzntjsgjo.html

[D14] 映射转换（每个元素变形）
来源：http://hz.nwbrower.top/gtoxpqzlqp.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.wangdashe.top/gtarkruklk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.hongshengwenyu.top/gtpjiurwcs.html

JS:   arr.map(x => x * 2)
来源：http://hz.yj20258.top/gtftcwzmlo.html

TS:   arr.map(x => x * 2)
来源：http://hz.gogol.net.cn/gtqjvqkhms.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.haohaochexian.top/gtstrrxyik.html

Go:   // 手写循环
来源：http://hz.yuanzhike.top/gtbwxvlhnt.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.chenzaomai.com/gtotcmlykj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.shanyushiyangtech.top/gtrvuhoqan.html

[D15] 去重
来源：http://hz.ivvv.top/gtpnnswlxh.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.nanxinkj.top/gthfscfppt.html

PHP:  array_unique($arr);
来源：http://hz.hnqzz.top/gtskbjwupe.html

JS:   [...new Set(arr)]
来源：http://hz.bjfxy.top/gtcppwfiiu.html

TS:   [...new Set(arr)]
来源：http://hz.havefunace.top/gtywdazwmd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yangfankeji.com/gtoftwqfph.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zhixingplan.top/gtdhudintc.html

Ruby: arr.uniq
来源：http://hz.sysykeji.top/gtkdlvrynb.html

C#:   list.Distinct().ToList()
来源：http://hz.gaohongyu789.top/gtdatrswdx.html

[D16] 求和与平均值
来源：http://hz.birdmap.top/gtqjqugkna.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.nwbrower.top/gttfsdsfew.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yangfankeji.com/gttsqpznpt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.nanxuanxn.top/gtyeettuwl.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.316326.xyz/gtosxhhloq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.cucudq.cn/gtplkhisaw.html

Go:   // 手写循环累加
来源：http://hz.316326.xyz/gtzpmcwcia.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhixingplan.top/gtowpmkqwj.html

C#:   list.Sum();  list.Average()
来源：http://hz.zdqjudy.top/gtuyzlvvgf.html

[D17] 最大值与最小值
来源：http://hz.daria6918.cn/gtpfqdrqol.html

Py:   max(arr);  min(arr)
来源：http://hz.jyoumei.cn/gtusoumzrz.html

PHP:  max($arr);  min($arr);
来源：http://hz.tianlin.xyz/gtslzjgcyi.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.c1oappe.top/gtmqewnrfs.html

TS:   Math.max(...arr);
来源：http://hz.c1oappe.top/gtmrtjtdhn.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.iojbl.cn/gtuamnbrur.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.zdqjudy.top/gthatdwzno.html

Ruby: arr.max;  arr.min
来源：http://hz.xingfuxueyuan.xyz/gteooczgda.html

C#:   list.Max();  list.Min()
来源：http://hz.ppjwa.cn/gtslubegvj.html

[D18] 扁平化嵌套数组
来源：http://hz.ybcxt.top/gtuopbjfpt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.xinyue.icu/gtjzwndqfj.html

PHP:  array_merge(...$nested);
来源：http://hz.hywenlv.cn/gtpygbfegx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.hongshengwenyu.top/gtiityfcck.html

TS:   nested.flat();
来源：http://hz.c1oappe.top/gttghamsid.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yj20258.top/gtnsfidhnb.html

Go:   // 手写双层循环
来源：http://hz.shuidangran.top/gtiuvtbsph.html

Ruby: nested.flatten
来源：http://hz.birdmap.top/gtrzxlaqqy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.nanxuanxn.top/gtbvoaopnw.html

[D19] 按字段分组
来源：http://hz.guannengcc.top/gtjzhiqpja.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.ydjk.org.cn/gthdetbblc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.svipenyu.cn/gtziwxppal.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.smart0.xyz/gtdulfpimr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.guannengcc.top/gtlltmfmfh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.yangfankeji.com/gtbgvheczh.html

Go:   // 手写 map[string][]T
来源：http://hz.zhoulong.xyz/gtzbafskci.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.guannengcc.top/gttwfrrkcc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.dianchejie.cn/gtmulcoiwt.html

[D20] 统计每个元素出现次数
来源：http://hz.zhixingplan.top/gtssrygeey.html

Py:   Counter(arr)
来源：http://hz.tianlin.xyz/gtyxxrqbgg.html

PHP:  array_count_values($arr);
来源：http://hz.birdmap.top/gtdvhkujku.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shanyushiyangkeji.top/gtfeyarcxu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yj20258888.top/gtorhwmkmv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.52xcode.cn/gtarcdxntp.html

Go:   // 手写 map[T]int
来源：http://hz.haohaochexian.top/gtrinysdyx.html

Ruby: arr.tally
来源：http://hz.sxryk.cn/gtwcyepisk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yj20258.top/gtwynamblr.html

[D21] 判断是否包含某元素
来源：http://hz.ivvv.top/gtuzdseahx.html

Py:   x in arr
来源：http://hz.cqqwz.cn/gtbhlvdyvz.html

PHP:  in_array($x, $arr, true);
来源：http://hz.nwbrower.top/gtqpuvhsxc.html

JS:   arr.includes(x)
来源：http://hz.pengpengdd.cyou/gtlwyxovhi.html

TS:   arr.includes(x)
来源：http://hz.yvedp.cn/gtwungphpy.html

Java: list.contains(x)
来源：http://hz.yj20258888.top/gtjxbsdpgl.html

Go:   slices.Contains(arr, x)
来源：http://hz.jinqigufen.top/gtzkryitzw.html

Ruby: arr.include?(x)
来源：http://hz.redwolf501.top/gtbmrcgcjc.html

C#:   list.Contains(x)
来源：http://hz.iojbl.cn/gtuzadkuje.html

[D22] 复制数组（避免共享引用）
来源：http://hz.cqqwz.cn/gtkpxyasmi.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yj20258888.top/gtetiskalz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.quarkkingdee.top/gtmydcnjiv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.zhengqikj.top/gtiolnzapk.html

TS:   [...arr];
来源：http://hz.smart0.xyz/gtaostdbcj.html

Java: new ArrayList<>(list);
来源：http://hz.yj20258888.top/gttupgorxb.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.hysaishi.cn/gtzfhgbiwd.html

Ruby: arr.dup;  arr.clone
来源：http://hz.ywan-chungtsiang.top/gtaghzikrs.html

C#:   new List<int>(list);
来源：http://hz.52xcode.cn/gtsmzuckkn.html

[D23] reduce 累积计算
来源：http://hz.hfpthk.cn/gtohxavjln.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yvedp.cn/gtlwzemzty.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.feifeiyinyue.top/gtauirbxsc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.zycfv.cn/gtcpsrkjex.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.vqdsnc.cn/gtvqhwresz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.hnxiangtu.top/gttgutbvgj.html

Go:   // 手写循环
来源：http://hz.cdnleiting.top/gtwvzjvlrn.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.shzxlz.cn/gtgipgjiik.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.yj202588.top/gtbhyunnrh.html

[D24] 字典 / Map 基本操作
来源：http://hz.hfpthk.cn/gtxayqqrij.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.wangshuangyany.cn/gtaitrqgmj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.hongshengwenyu.top/gtlusogisf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.mhx1999.top/gtslekkcmd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.ehwqpu.com/gtzfrvnqnd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.chenlongwang.top/gterlqjxsj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.andypj.xyz/gtqlktcgqd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.nanxuanxn.top/gtkhpwubab.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.feifeiyinyue.top/gtqexmshfj.html

[D25] Set 集合去重与交并差
来源：http://hz.bjfxy.top/gtkopzlmbi.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.ivvv.top/gtwgwwafiu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.guowangkeji.top/gtuhkjfbuw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.ywan-chungtsiang.top/gtywygmsvp.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.xziqi.cn/gtyuqalpts.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.iojbl.cn/gtqfukgqhh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.chenlongwang.top/gtvhxodkit.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.chenlongwang.top/gtvwhdrqlb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.jinqigufen.top/gtefbyrvlv.html

[D26] 数组转字符串
来源：http://hz.smart0.xyz/gtaiifgeqw.html

Py:   ", ".join(map(str, arr))
来源：http://hz.shanyushiyangkeji.top/gthkyejwnk.html

PHP:  implode(", ", $arr);
来源：http://hz.haohaochexian.top/gtrsvtsfgp.html

JS:   arr.join(", ")
来源：http://hz.zhijiandao.cn/gtvhrzgkan.html

TS:   arr.join(", ")
来源：http://hz.ydjk.org.cn/gtsvtxrxsw.html

Java: String.join(", ", list)
来源：http://hz.yonumen.top/gtpxzgusga.html

Go:   strings.Join(strs, ", ")
来源：http://hz.gaohongyu789.top/gtrtsxsgxj.html

Ruby: arr.join(", ")
来源：http://hz.tanke756.top/gtqprwwesp.html

C#:   string.Join(", ", list)
来源：http://hz.52xcode.cn/gtyhxavenq.html

================================================================================
来源：http://hz.redwolf501.top/gttloadeci.html

E. 字符串处理
来源：http://hz.jinqigfzy.top/gtnmepuskq.html

================================================================================
来源：http://hz.yuxming.cn/gtvkyopowb.html

[E01] 拼接字符串
来源：http://hz.havefunace.top/gtvirpcxxf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.nanxuanxn.top/gtqfgzabhq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.fengsongda.top/gtirhoopqr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jqgfzy.top/gtiywuoejd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.birdmap.top/gtwulljwvo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.cqqwz.cn/gtkedwqdfh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.hfpthk.cn/gtbkjpdgoz.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.sweek.top/gtbrhxsgew.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.haohaochexian.top/gtbvrzvmle.html

[E02] 重复字符串
来源：http://hz.zhongyouzk.top/gtlrkrqzuu.html

Py:   "ab" * 3
来源：http://hz.zhiwuduotai.top/gtszmvyran.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jianghu66.top/gtxkbvlabg.html

JS:   "ab".repeat(3)
来源：http://hz.sxryk.cn/gtmkldfiug.html

TS:   "ab".repeat(3)
来源：http://hz.gogol.net.cn/gtehrrxdnm.html

Java: "ab".repeat(3)
来源：http://hz.havefunace.top/gtpvkbdyzg.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.fengsongda.top/gteddyazjm.html

Ruby: "ab" * 3
来源：http://hz.zhaomingkeji.xyz/gtsvlvfmii.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.jqgfzy.top/gtqgwltshc.html

[E03] 截取子串
来源：http://hz.xuanzx.com/gtdiztmyab.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.sweek.top/gtjrftlzoa.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.wangshuangyany.cn/gthopktliq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.quarkkingdee.top/gtlkoueaep.html

TS:   s.slice(1, 4)
来源：http://hz.chenjidiqi.icu/gtnlgjroaf.html

Java: s.substring(1, 4)
来源：http://hz.xinyue.icu/gtuytqjvyz.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yonumen.top/gtfkbvzfnf.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.tian-w.cn/gtenyqrluo.html

C#:   s.Substring(1, 3)
来源：http://hz.cqqwz.cn/gtwdhlbzde.html

[E04] 查找子串位置
来源：http://hz.chenlongwang.top/gtvhsnoges.html

Py:   s.find("x");  s.index("x")
来源：http://hz.zhijiandao.cn/gtsucnhyjj.html

PHP:  strpos($s, "x");
来源：http://hz.andypj.xyz/gttfvkogkq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.ppjwa.cn/gtduikgahu.html

TS:   s.indexOf("x")
来源：http://hz.guowangkeji.top/gtqacabvwl.html

Java: s.indexOf("x")
来源：http://hz.hongshengwenyu.top/gtkbplteap.html

Go:   strings.Index(s, "x")
来源：http://hz.ppjwa.cn/gtirzgemii.html

Ruby: s.index("x")
来源：http://hz.meibo888.top/gtcuwxzudc.html

C#:   s.IndexOf("x")
来源：http://hz.gaohongyu789.top/gtjotkyrlj.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.bjfxy.top/gtqtstniqt.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yangfankeji.com/gteulrexgm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.gogol.net.cn/gtiztvbqdr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.shanyushiyangtech.top/gtatpsyaec.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.hnxiangtu.top/gtaprmpfji.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.guannengcc.top/gtndiwznlj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.haohaochexian.top/gtyrcxhdhe.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yueranfly.top/gtkbjhbovz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.ppjwa.cn/gtraxvsspl.html

[E06] 替换子串
来源：http://hz.hongshengwenyu.top/gtljtvczhz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.chenjidiqi.icu/gtgzfcvbfb.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.smart0.xyz/gtbbhuexar.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.fengsongda.top/gtbcwmiurz.html

TS:   s.replaceAll("a", "b")
来源：http://hz.guowangkeji.top/gtxuhkvhbo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jinqigufen.top/gtdljxwyqi.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.fengsongda.top/gtabdmnkls.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.aizwys.cn/gtzgibwvlo.html

C#:   s.Replace("a", "b")
来源：http://hz.vqdsnc.cn/gtshsgrdyu.html

[E07] 按分隔符拆分
来源：http://hz.0kj1m.cn/gtlkifsalx.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.hnxiangtu.top/gtiacwlzmi.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.guowangkeji.top/gttokkonvu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.ivvv.top/gtautkbzzu.html

TS:   s.split(",")
来源：http://hz.svipenyu.cn/gtxhknajqi.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.aibaodan.cn/gtpefyboec.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.andypj.xyz/gtsvihzhxn.html

Ruby: s.split(",");  s.split
来源：http://hz.pengpengdd.cyou/gtbxjdxrmu.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.guannengcc.top/gtijxhkzdt.html

[E08] 数组按分隔符合并
来源：http://hz.52xcode.cn/gtduutzaku.html

Py:   ",".join(items)
来源：http://hz.yj20258.top/gtqersqrvj.html

PHP:  implode(",", $items);
来源：http://hz.hfpthk.cn/gthdvivvwd.html

JS:   items.join(",")
来源：http://hz.daria6918.cn/gthxlexgrr.html

TS:   items.join(",")
来源：http://hz.iojbl.cn/gtmoyseebb.html

Java: String.join(",", items)
来源：http://hz.tianlin.xyz/gthnquxoeb.html

Go:   strings.Join(items, ",")
来源：http://hz.yanxiufei.cn/gtduuthcep.html

Ruby: items.join(",")
来源：http://hz.shanyushiyangkeji.top/gtcbovsqfa.html

C#:   string.Join(",", items)
来源：http://hz.yueranfly.top/gtntguzbto.html

[E09] 去除所有空白字符
来源：http://hz.andypj.xyz/gtlyomxgda.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.xuetiantiany.cn/gtloliafxv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yangfankeji.com/gtyuqocbqa.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.smart0.xyz/gtxjczwcna.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.cdnleiting.top/gtmrxistif.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.hongshengwenyu.top/gtcfwxcsdq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xylfe.cn/gtkvzytzws.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.nwbrower.top/gtdkkttgll.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jqgfzy.top/gtqbpdlhtz.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jqgufenzy.top/gteskbgcoi.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.xingfuxueyuan.xyz/gtuioxkbtf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.ppjwa.cn/gttblmppxz.html

JS:   "7".padStart(3, "0")
来源：http://hz.yongpay.top/gtpqkppktd.html

TS:   "7".padStart(3, "0")
来源：http://hz.feifeiyinyue.top/gtyidebamk.html

Java: String.format("%03d", 7)
来源：http://hz.jqgufenzy.top/gtmxbxwczp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zhongyouzk.top/gtyqxfgvwz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zhixingplan.top/gtfbpbxwox.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.shanyushiyangtech.top/gtelldwmvr.html

[E11] 反转字符串
来源：http://hz.xziqi.cn/gtxgjocgkg.html

Py:   s[::-1]
来源：http://hz.jyoumei.cn/gtriiiczxg.html

PHP:  strrev($s);
来源：http://hz.yuxming.cn/gtvxpuphgo.html

JS:   [...s].reverse().join("")
来源：http://hz.sxryk.cn/gtfitosjeh.html

TS:   [...s].reverse().join("")
来源：http://hz.zhixingplan.top/gtvxclawvp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.chenjidiqi.icu/gttduovmro.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yanxiufei.cn/gtknqhcvvg.html

Ruby: s.reverse
来源：http://hz.jinqigfzy.top/gtpatpdwmt.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yuxming.cn/gtwjorqctf.html

[E12] 统计某字符出现次数
来源：http://hz.0kj1m.cn/gtvyfujhfs.html

Py:   s.count("a")
来源：http://hz.quarkkingdee.top/gttaeyeidz.html

PHP:  substr_count($s, "a");
来源：http://hz.xinyue.icu/gtawfouasc.html

JS:   s.split("a").length - 1
来源：http://hz.jyoumei.cn/gtpvmgtrlw.html

TS:   s.split("a").length - 1
来源：http://hz.iojbl.cn/gtpjwgtdpg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.xinyue.icu/gtvyroneqn.html

Go:   strings.Count(s, "a")
来源：http://hz.nwbrower.top/gtyybodjlj.html

Ruby: s.count("a")
来源：http://hz.yueranfly.top/gtfdbpcdif.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yongpay.top/gtrsiufcuk.html

[E13] 逐字符遍历
来源：http://hz.xinyue.icu/gtawqttsjv.html


<!-- 参考信息 -->