代发 wailian999

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.shangyingyoupin.top/gtjpuoifsg.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.ydzc1.top/gtbxrmrdzn.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.svipenyu.cn/gtmbkhwsjx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.tian-w.cn/gtxclqjxmy.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.shzxlz.cn/gtcvecpdjg.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.xinyue.icu/gtachnsceh.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.guannengcc.top/gtsgkbiyxo.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jyoumei.cn/gtxtxpatef.html

[D11] 反转数组
来源：http://hz.yanxiufei.cn/gtrvisazgu.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.xylfe.cn/gtsiglapro.html

PHP:  array_reverse($arr);
来源：http://hz.cashguo.top/gtssoybzhf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.jqgfzy.top/gtwdrmivoc.html

TS:   [...arr].reverse();
来源：http://hz.cheryme.top/gtwwkobufi.html

Java: Collections.reverse(list);
来源：http://hz.chenjidiqi.icu/gtjqbikkpn.html

Go:   slices.Reverse(arr)
来源：http://hz.chenzaomai.com/gtlstrsjeb.html

Ruby: arr.reverse
来源：http://hz.zdqjudy.top/gtbcyziwey.html

C#:   list.Reverse();
来源：http://hz.feifeiyinyue.top/gtauwdbkon.html

[D12] 查找元素下标
来源：http://hz.ivvv.top/gtadtsdhmh.html

Py:   arr.index(x);  x in arr
来源：http://hz.iojbl.cn/gtxuztqybo.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.andypj.xyz/gtbwpsqxqc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.c1oappe.top/gtmnvgoymc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.chenzaomai.com/gtrappwfbq.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.cashguo.top/gtmzayxsvh.html

Go:   slices.Index(arr, x)
来源：http://hz.aibaodan.cn/gtciwjhorg.html

Ruby: arr.index(x)
来源：http://hz.ydjk.org.cn/gtsnsxmchi.html

C#:   list.IndexOf(x);
来源：http://hz.ehwqpu.com/gtoytdlhas.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jqgufenzy.top/gthwrihoeo.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.wangdashe.top/gtktinjlqr.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.yonumen.top/gtomielzjf.html

JS:   arr.filter(x => x > 3)
来源：http://hz.quarkkingdee.top/gtriyprxxr.html

TS:   arr.filter(x => x > 3)
来源：http://hz.ivvv.top/gtpvsfswyb.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.sxryk.cn/gtyanjhiav.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.pycfn.com/gtygoojeai.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.chenjidiqi.icu/gtuevhfjdz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.smart0.xyz/gtsaxsqeft.html

[D14] 映射转换（每个元素变形）
来源：http://hz.tianlin.xyz/gtpmozpxmb.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.0kj1m.cn/gtupvgbtkx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.shzxlz.cn/gtrubycpko.html

JS:   arr.map(x => x * 2)
来源：http://hz.wangshuangyany.cn/gtlgmtwrbo.html

TS:   arr.map(x => x * 2)
来源：http://hz.sxryk.cn/gttsjgsvcl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jiagoushi.top/gtynfyrhtv.html

Go:   // 手写循环
来源：http://hz.hongshengwenyu.top/gtuwhyqudn.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.tanke756.top/gtqxpkeikx.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jinqigfzy.top/gtuprqsodr.html

[D15] 去重
来源：http://hz.hnqzz.top/gtquvtuewa.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.jqgfzy.top/gtrvyrxkjs.html

PHP:  array_unique($arr);
来源：http://hz.yj20258888.top/gtykdrymhn.html

JS:   [...new Set(arr)]
来源：http://hz.9152youxi.cn/gtraugkmjo.html

TS:   [...new Set(arr)]
来源：http://hz.jinqigfzy.top/gtsjctgjww.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.shuidangran.top/gtubtgxlda.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.jqgufenzy.top/gtpzndoiqk.html

Ruby: arr.uniq
来源：http://hz.gaohongyu789.top/gtenbkxzwx.html

C#:   list.Distinct().ToList()
来源：http://hz.pengpengdd.cyou/gtyuzlcqsg.html

[D16] 求和与平均值
来源：http://hz.sweek.top/gtloavkmwu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.zhoulong.xyz/gtfvvxrmuf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.nanxuanxn.top/gthcpaoozi.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.gaohongyu789.top/gthsbfuxrw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.wangshuangyany.cn/gtnqgfregl.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.guowangkeji.top/gtyajxhhfd.html

Go:   // 手写循环累加
来源：http://hz.cdnleiting.top/gtjjkyeesa.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.sufxvd.cn/gtjqlzrcii.html

C#:   list.Sum();  list.Average()
来源：http://hz.jqgfzy.top/gtwszabcbo.html

[D17] 最大值与最小值
来源：http://hz.svipenyu.cn/gtvwnhpxvz.html

Py:   max(arr);  min(arr)
来源：http://hz.cashguo.top/gtoxgygnoe.html

PHP:  max($arr);  min($arr);
来源：http://hz.daria6918.cn/gtjdrcwpje.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.zhongyouzk.top/gtpffveavl.html

TS:   Math.max(...arr);
来源：http://hz.cdnleiting.top/gtzxssorgm.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zhoulong.xyz/gtkgjusdbe.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hammf.cn/gtukdlompr.html

Ruby: arr.max;  arr.min
来源：http://hz.yangfankeji.com/gtapufanmc.html

C#:   list.Max();  list.Min()
来源：http://hz.cdnleiting.top/gtjbflspbv.html

[D18] 扁平化嵌套数组
来源：http://hz.zhoulong.xyz/gtucaaozmw.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.shuidangran.top/gtveletnba.html

PHP:  array_merge(...$nested);
来源：http://hz.zhongyouzk.top/gtjawlespt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.wangdashe.top/gtgggjxqar.html

TS:   nested.flat();
来源：http://hz.yvedp.cn/gtactyfdfp.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.ppjwa.cn/gtaxxxizia.html

Go:   // 手写双层循环
来源：http://hz.cdnleiting.top/gtgedoqixa.html

Ruby: nested.flatten
来源：http://hz.ybcxt.top/gtkvpekwap.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zhijiandao.cn/gtnzxpogrk.html

[D19] 按字段分组
来源：http://hz.jiagoushi.top/gtimarqdnh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.sufxvd.cn/gtruthupna.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.shanyushiyangkeji.top/gteiezyxok.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.vqdsnc.cn/gtoshpousc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.gaohongyu789.top/gtzgibjcso.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jlsjyb.cn/gtwvkeskhu.html

Go:   // 手写 map[string][]T
来源：http://hz.hnqzz.top/gtgivtmgsg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.xingfuxueyuan.xyz/gtpcuxzoic.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.guowangkeji.top/gtgquhvvsy.html

[D20] 统计每个元素出现次数
来源：http://hz.9152youxi.cn/gtwgvtrekw.html

Py:   Counter(arr)
来源：http://hz.ybcxt.top/gtruxzdpxo.html

PHP:  array_count_values($arr);
来源：http://hz.yj202588.top/gtsxhdyvgr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.fzhhl.top/gtbnntkaba.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ybcxt.top/gtpbbqtuhe.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.dianchejie.cn/gteooifooc.html

Go:   // 手写 map[T]int
来源：http://hz.haohaochexian.top/gtnfzdwyzl.html

Ruby: arr.tally
来源：http://hz.yvedp.cn/gtlzfxdvij.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yuanzhike.top/gtwhogcfrr.html

[D21] 判断是否包含某元素
来源：http://hz.zhongyouzk.top/gtjtkkgcnk.html

Py:   x in arr
来源：http://hz.sysykeji.top/gtztkqdmlr.html

PHP:  in_array($x, $arr, true);
来源：http://hz.chenjidiqi.icu/gtgjvydfup.html

JS:   arr.includes(x)
来源：http://hz.yuanzhike.top/gtmpsiliei.html

TS:   arr.includes(x)
来源：http://hz.sxryk.cn/gtrwslskms.html

Java: list.contains(x)
来源：http://hz.haohaochexian.top/gtfdadxoeu.html

Go:   slices.Contains(arr, x)
来源：http://hz.zhaomingkeji.xyz/gtthpmelco.html

Ruby: arr.include?(x)
来源：http://hz.nanxuanxn.top/gtuavwewtk.html

C#:   list.Contains(x)
来源：http://hz.ydzc1.top/gtvvwcwmqm.html

[D22] 复制数组（避免共享引用）
来源：http://hz.bjfxy.top/gtvarcdsdv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.pycfn.com/gtuqoipfnp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.daxiang520.top/gtsttqvnas.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jinghuilouyu.cn/gtimmlnqet.html

TS:   [...arr];
来源：http://hz.jinghuilouyu.cn/gthxsgswbn.html

Java: new ArrayList<>(list);
来源：http://hz.zhiwuduotai.top/gtybluxwha.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.0kj1m.cn/gtneanyfxz.html

Ruby: arr.dup;  arr.clone
来源：http://hz.hongshengwenyu.top/gtfprauzfa.html

C#:   new List<int>(list);
来源：http://hz.hnqzz.top/gtnodtiyxy.html

[D23] reduce 累积计算
来源：http://hz.xylfe.cn/gtinxpyumt.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.redwolf501.top/gtcxulrvtt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.ywan-chungtsiang.top/gtncvmocom.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.chenlongwang.top/gteeartheg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ehwqpu.com/gtgpaujbkw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.feifeiyinyue.top/gtsgcglzoz.html

Go:   // 手写循环
来源：http://hz.9152youxi.cn/gtbnvixguc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.wangdashe.top/gtxkuijmet.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jinyuanbaomall.cn/gtgcbbxtfo.html

[D24] 字典 / Map 基本操作
来源：http://hz.zhongyouzk.top/gtenysbotb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.ivvv.top/gtfreevedi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.ppjwa.cn/gtmnjocflv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.aizwys.cn/gtxeoidifn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.cucudq.cn/gtkoyihedk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.yonumen.top/gthmhfyzzx.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jinghuilouyu.cn/gteygtyhuj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.smart0.xyz/gtqjccezra.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.fengsongda.top/gtslytiabq.html

[D25] Set 集合去重与交并差
来源：http://hz.hnxiangtu.top/gtejytdsbb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.vqdsnc.cn/gttowqtmzd.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.zhongyouzk.top/gtrlmupayc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yueranfly.top/gtjoukpwdo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.yanxiufei.cn/gtvuvsnltk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.andypj.xyz/gtltlrerfa.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.cucudq.cn/gtpuvahgbi.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.gaohongyu789.top/gtcttgxpmi.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yj20258.top/gtukpgdsbp.html

[D26] 数组转字符串
来源：http://hz.ehwqpu.com/gtauepbnyz.html

Py:   ", ".join(map(str, arr))
来源：http://hz.kuanghao11.cn/gtfdfarmev.html

PHP:  implode(", ", $arr);
来源：http://hz.daxiang520.top/gtulizbriv.html

JS:   arr.join(", ")
来源：http://hz.shzxlz.cn/gtajqzsixz.html

TS:   arr.join(", ")
来源：http://hz.yj202588.top/gtjcjqzxze.html

Java: String.join(", ", list)
来源：http://hz.guannengcc.top/gtctalsfmy.html

Go:   strings.Join(strs, ", ")
来源：http://hz.chenzaomai.com/gtonslrtxs.html

Ruby: arr.join(", ")
来源：http://hz.cdnleiting.top/gttbwrgmmn.html

C#:   string.Join(", ", list)
来源：http://hz.cqqwz.cn/gtfxmmixpt.html

================================================================================
来源：http://hz.zhijiandao.cn/gtpaeffxzi.html

E. 字符串处理
来源：http://hz.nanxinkj.top/gtexwtkaby.html

================================================================================
来源：http://hz.chenjidiqi.icu/gteomqzhbe.html

[E01] 拼接字符串
来源：http://hz.jyoumei.cn/gtxbvzpyre.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.shanyushiyangtech.top/gtyvzyglzm.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.chenzaomai.com/gtyuqurqmk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.sweek.top/gtsqrhcubm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.wangshuangyany.cn/gtjclqryjt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.guannengcc.top/gtoxqqofri.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.hongshengwenyu.top/gtykoygkyx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.dashuyun.cn/gtudbmxiwq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.52xcode.cn/gtjexypbmw.html

[E02] 重复字符串
来源：http://hz.shanyushiyangtech.top/gtkuldtcqv.html

Py:   "ab" * 3
来源：http://hz.xziqi.cn/gtanbgkwqq.html

PHP:  str_repeat("ab", 3);
来源：http://hz.zhijiandao.cn/gtmeplvuvl.html

JS:   "ab".repeat(3)
来源：http://hz.wangdashe.top/gthcaqlouc.html

TS:   "ab".repeat(3)
来源：http://hz.kuanghao11.cn/gtxwwbprzr.html

Java: "ab".repeat(3)
来源：http://hz.zdqjudy.top/gtisaldgvs.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.hongshengwenyu.top/gtcgastzdt.html

Ruby: "ab" * 3
来源：http://hz.aibaodan.cn/gtnsqjqsgl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.zhijiandao.cn/gtchmiygnd.html

[E03] 截取子串
来源：http://hz.52xcode.cn/gtggghomnj.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.zhiwuduotai.top/gtaeygygxp.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.xziqi.cn/gttxiorrdb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.zhaomingkeji.xyz/gtufwhoprl.html

TS:   s.slice(1, 4)
来源：http://hz.c1oappe.top/gtqzgexwyc.html

Java: s.substring(1, 4)
来源：http://hz.316326.xyz/gtddayintr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.hongshengwenyu.top/gtwdgsbzen.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yanxiufei.cn/gtrggwcley.html

C#:   s.Substring(1, 3)
来源：http://hz.zhijiandao.cn/gtjkhoyqgu.html

[E04] 查找子串位置
来源：http://hz.cdnleiting.top/gtnmhewvbi.html

Py:   s.find("x");  s.index("x")
来源：http://hz.aizwys.cn/gtfupzgqfi.html

PHP:  strpos($s, "x");
来源：http://hz.ppjwa.cn/gttplvakac.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.ivvv.top/gtlhrvvdvv.html

TS:   s.indexOf("x")
来源：http://hz.daxiang520.top/gtbgxbnycn.html

Java: s.indexOf("x")
来源：http://hz.0kj1m.cn/gtgsgjznte.html

Go:   strings.Index(s, "x")
来源：http://hz.gotoacloud.top/gtwlotwwtg.html

Ruby: s.index("x")
来源：http://hz.svipenyu.cn/gtpeufnqlo.html

C#:   s.IndexOf("x")
来源：http://hz.sufxvd.cn/gtlqsesnkn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.hfpthk.cn/gthrlaebnk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.fengsongda.top/gtmpsgpvim.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zhongyouzk.top/gtmtjbpjjr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.gotoacloud.top/gtgqndgajm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.0kj1m.cn/gtlbnxhmsr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.iojbl.cn/gttpdlrigh.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.aibaodan.cn/gtjcjjnidx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.gotoacloud.top/gtpfvubfqg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.aibaodan.cn/gtyszgikae.html

[E06] 替换子串
来源：http://hz.pycfn.com/gtuijcaxmz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.9152youxi.cn/gtegghvoeo.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.shangyingyoupin.top/gtyninxdke.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jinqigufen.top/gtlaxcuogv.html

TS:   s.replaceAll("a", "b")
来源：http://hz.yangfankeji.com/gttqgdpqwh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.xylfe.cn/gtkvpkcjby.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.9152youxi.cn/gtmabfjwoi.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.aizwys.cn/gtwgwncovd.html

C#:   s.Replace("a", "b")
来源：http://hz.feifeiyinyue.top/gtnsywsuuh.html

[E07] 按分隔符拆分
来源：http://hz.xziqi.cn/gtqlozpgvq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.zhijiandao.cn/gtavzjaxyh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.hnxiangtu.top/gtihjtinvi.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.jiagoushi.top/gthoyoweld.html

TS:   s.split(",")
来源：http://hz.fengsongda.top/gtxndqyqqr.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.cheryme.top/gtetztlmjm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.9152youxi.cn/gtxalswsci.html

Ruby: s.split(",");  s.split
来源：http://hz.cheryme.top/gtlhzqufue.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.cqqwz.cn/gtxixjzddz.html

[E08] 数组按分隔符合并
来源：http://hz.jinqigufen.top/gtmvsbngiy.html

Py:   ",".join(items)
来源：http://hz.sxryk.cn/gtrctagmbv.html

PHP:  implode(",", $items);
来源：http://hz.xziqi.cn/gtfaslocff.html

JS:   items.join(",")
来源：http://hz.ivvv.top/gtbcfxiwtd.html

TS:   items.join(",")
来源：http://hz.xinyue.icu/gtnznhqeeu.html

Java: String.join(",", items)
来源：http://hz.c1oappe.top/gtwoqlnezw.html

Go:   strings.Join(items, ",")
来源：http://hz.gotoacloud.top/gtotwgtkov.html

Ruby: items.join(",")
来源：http://hz.chenlongwang.top/gtcpllhohk.html

C#:   string.Join(",", items)
来源：http://hz.sufxvd.cn/gtgopxpbbt.html

[E09] 去除所有空白字符
来源：http://hz.yangfankeji.com/gtalplmmcz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zhijiandao.cn/gtjijmfkgr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.havefunace.top/gtxttdqrvt.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jianghu66.top/gtewubfgeo.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.chenlongwang.top/gtjxwpremp.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.tian-w.cn/gtnzjwmezi.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.gogol.net.cn/gtxeussrzt.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.ehwqpu.com/gtpwsemkca.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.ywan-chungtsiang.top/gtftlnyxhy.html

[E10] 左侧补零 / 定长填充
来源：http://hz.cashguo.top/gtzwutcprl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.bjfxy.top/gtjtfvfplm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jyoumei.cn/gtnhdihhew.html

JS:   "7".padStart(3, "0")
来源：http://hz.feifeiyinyue.top/gtizhwagkh.html

TS:   "7".padStart(3, "0")
来源：http://hz.hongshengwenyu.top/gtaokpscnn.html

Java: String.format("%03d", 7)
来源：http://hz.hammf.cn/gtjhbetazn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.hfpthk.cn/gtnyhxbzee.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.dianchejie.cn/gtkafvxwda.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.gaohongyu789.top/gtjmnnxcjw.html

[E11] 反转字符串
来源：http://hz.ydzc1.top/gtdwhbqcvp.html

Py:   s[::-1]
来源：http://hz.cucudq.cn/gtgwpbokvf.html

PHP:  strrev($s);
来源：http://hz.hammf.cn/gtusqtghwk.html

JS:   [...s].reverse().join("")
来源：http://hz.chenlongwang.top/gtjjhwjsju.html

TS:   [...s].reverse().join("")
来源：http://hz.cdnleiting.top/gtvomnolgz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yongpay.top/gtulawjjmq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zhijiandao.cn/gtqddmwjmr.html

Ruby: s.reverse
来源：http://hz.cqqwz.cn/gtfcvxraii.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.ehwqpu.com/gtutdumzqj.html

[E12] 统计某字符出现次数
来源：http://hz.gzhubu.top/gtdglweddj.html

Py:   s.count("a")
来源：http://hz.pycfn.com/gtvkcoqzyj.html

PHP:  substr_count($s, "a");
来源：http://hz.daxiang520.top/gtlefriuof.html

JS:   s.split("a").length - 1
来源：http://hz.ywan-chungtsiang.top/gtjihimwfd.html

TS:   s.split("a").length - 1
来源：http://hz.yuxming.cn/gtccejyoae.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.hfpthk.cn/gtmfyxbxns.html

Go:   strings.Count(s, "a")
来源：http://hz.guannengcc.top/gtyttenlkb.html

Ruby: s.count("a")
来源：http://hz.yj202588.top/gtttwyhwtp.html

C#:   s.Count(c => c == 'a')
来源：http://hz.wangdashe.top/gtlocscffl.html

[E13] 逐字符遍历
来源：http://hz.xinyue.icu/gtcfqkeqhb.html

Py:   for ch in s: print(ch)
来源：http://hz.316326.xyz/gtbwifkafm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.fzhhl.top/gtnbqnprmk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shanyushiyangkeji.top/gtpytehgte.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.pycfn.com/gtwrxajglq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.c1oappe.top/gtvzsdfqyl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.cdnleiting.top/gtbaxdnfph.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.feifeiyinyue.top/gtdqizxmta.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.cdnleiting.top/gtdzertego.html

[E14] URL 编码与 Base64
来源：http://hz.jinqigufen.top/gtcrbsmhcu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.sufxvd.cn/gtwizzftad.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jinqigufen.top/gtmdbddqpc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.shuidangran.top/gtorteogqe.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.guowangkeji.top/gtbsspxiqq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.ybcxt.top/gtkimivfal.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.xuanzx.com/gtvatrkypg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.aibaodan.cn/gtikxujehs.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.cheryme.top/gtpyhdohek.html

[E15] HTML 转义 / 反转义
来源：http://hz.andypj.xyz/gtanznbuqx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.ydjk.org.cn/gtzixuygir.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.ivvv.top/gtjibpgmkf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.aizwys.cn/gtoqaiybmr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.sxryk.cn/gtcdvoiwst.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.cdnleiting.top/gtznjxngmb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.cheryme.top/gtiwejqxqc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.tanke756.top/gturbtlmyo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.aibaodan.cn/gtgxgbtzsw.html

[E16] 数字千分位
来源：http://hz.zhixingplan.top/gtilcotayq.html

Py:   f"{1234567:,}"
来源：http://hz.fengsongda.top/gtbcmjyuiz.html

PHP:  number_format(1234567);
来源：http://hz.xingfuxueyuan.xyz/gtesqshlmn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.gzhubu.top/gthklrhkpz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.dianchejie.cn/gtafoyeoor.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.havefunace.top/gtagelrbjr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.pycfn.com/gtrjwbxwxu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.guannengcc.top/gtsdaooshx.html

C#:   1234567.ToString("N0")
来源：http://hz.hnxiangtu.top/gtasxeoisd.html

[E17] 首字母大写
来源：http://hz.xziqi.cn/gtoyuscxbx.html


<!-- 参考信息 -->