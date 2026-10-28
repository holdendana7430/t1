代发 wailian999

[D07] 切片 / 取子数组
来源：http://hz.nwbrower.top/gtxaghwfnl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yvedp.cn/gtttjxrpbw.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.xziqi.cn/gtbdzlqawv.html

JS:   arr.slice(1, 4);
来源：http://hz.meibo888.top/gthugzqunr.html

TS:   arr.slice(1, 4);
来源：http://hz.kuanghao11.cn/gtpbksryou.html

Java: list.subList(1, 4);
来源：http://hz.ppjwa.cn/gthkfgxwxs.html

Go:   arr[1:4]
来源：http://hz.zhoulong.xyz/gtmwecnyfn.html

Ruby: arr[1, 3]
来源：http://hz.nanxinkj.top/gtqhnrhsnp.html

C#:   list.GetRange(1, 3);
来源：http://hz.iojbl.cn/gtbvcrsqqt.html

[D08] 合并两个数组
来源：http://hz.havefunace.top/gtsozbvyuq.html

Py:   a + b;  a.extend(b)
来源：http://hz.zycfv.cn/gtmmsrhhrb.html

PHP:  array_merge($a, $b);
来源：http://hz.hnqzz.top/gtwgpevqhp.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.shangyingyoupin.top/gthwfzbbai.html

TS:   [...a, ...b];
来源：http://hz.snrcjt.cn/gtfewbpvrj.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.nanxinkj.top/gtipscjkax.html

Go:   append(a, b...)
来源：http://hz.shanyushiyangkeji.top/gtqzlrzzvr.html

Ruby: a + b;  a.concat(b)
来源：http://hz.xziqi.cn/gtkvsgklga.html

C#:   a.Concat(b).ToList()
来源：http://hz.shuidangran.top/gtjnfugczg.html

[D09] 排序（升序）
来源：http://hz.zhijiandao.cn/gtmsmbmnsa.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.yj202588.top/gtzjdkxhjy.html

PHP:  sort($arr);
来源：http://hz.0kj1m.cn/gtrorzqvwc.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.hysaishi.cn/gtaggjcjhv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.zhixingplan.top/gtcwjzvyix.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.daxiang520.top/gtoofzhwan.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.dianchejie.cn/gthyghsaly.html

Ruby: arr.sort
来源：http://hz.yonumen.top/gtxgqxxchl.html

C#:   list.Sort();
来源：http://hz.jyoumei.cn/gtdpcwtuaq.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.gogol.net.cn/gtylpoxxfa.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.sysykeji.top/gtvdiotiyh.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.pycfn.com/gtknxzhtya.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhijiandao.cn/gttzvdqffb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zdqjudy.top/gtxomclzgf.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zhengqikj.top/gtyewbymao.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.zhiwuduotai.top/gtczppbuhf.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.ybcxt.top/gtqzmpyeud.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.bjfxy.top/gtgweqgaqn.html

[D11] 反转数组
来源：http://hz.0kj1m.cn/gtdmevlila.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.iojbl.cn/gtxygtfjqm.html

PHP:  array_reverse($arr);
来源：http://hz.jyoumei.cn/gtddkmijwt.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.sysykeji.top/gtzniscbvl.html

TS:   [...arr].reverse();
来源：http://hz.gotoacloud.top/gtoxggyqjd.html

Java: Collections.reverse(list);
来源：http://hz.snrcjt.cn/gtmcfzqufj.html

Go:   slices.Reverse(arr)
来源：http://hz.gotoacloud.top/gtvrhzwfdd.html

Ruby: arr.reverse
来源：http://hz.jyoumei.cn/gtbwlkwhyr.html

C#:   list.Reverse();
来源：http://hz.fengsongda.top/gtxlrgoege.html

[D12] 查找元素下标
来源：http://hz.xinyue.icu/gtfrjbsido.html

Py:   arr.index(x);  x in arr
来源：http://hz.sweek.top/gtddyvpdem.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.yonumen.top/gtntwgrlhc.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.dianchejie.cn/gtxfpqaior.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.316326.xyz/gtllgvvndg.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yanxiufei.cn/gtjrrctuxt.html

Go:   slices.Index(arr, x)
来源：http://hz.chenzaomai.com/gtbncihfxz.html

Ruby: arr.index(x)
来源：http://hz.shzxlz.cn/gthqqzgjpl.html

C#:   list.IndexOf(x);
来源：http://hz.pycfn.com/gtmfxrafqh.html

[D13] 过滤（保留满足条件的）
来源：http://hz.svipenyu.cn/gtaiudjpxn.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.gogol.net.cn/gtwvgdntrk.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.hongshengwenyu.top/gtgjfbgnka.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jyoumei.cn/gtgkcxwppj.html

TS:   arr.filter(x => x > 3)
来源：http://hz.ivvv.top/gtvzjkwbax.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.shangyingyoupin.top/gteidmzjhj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.chenlongwang.top/gtwwivysfc.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.shangyingyoupin.top/gtohyvsote.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.aizwys.cn/gtyuhkqtcn.html

[D14] 映射转换（每个元素变形）
来源：http://hz.haohaochexian.top/gthqvlzqsd.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.nanxuanxn.top/gtdrjpoyrx.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.bjfxy.top/gtethrnrce.html

JS:   arr.map(x => x * 2)
来源：http://hz.gaohongyu789.top/gtygxsvdth.html

TS:   arr.map(x => x * 2)
来源：http://hz.haohaochexian.top/gtuxinhvpc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.aizwys.cn/gtscpnmzuo.html

Go:   // 手写循环
来源：http://hz.birdmap.top/gtwsxdnsvg.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.yangfankeji.com/gtaoyiddad.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.vqdsnc.cn/gttihwvufw.html

[D15] 去重
来源：http://hz.sufxvd.cn/gtkxhckzxe.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.xylfe.cn/gtpatfgwtf.html

PHP:  array_unique($arr);
来源：http://hz.snrcjt.cn/gtucteiylj.html

JS:   [...new Set(arr)]
来源：http://hz.sysykeji.top/gtjjykhlie.html

TS:   [...new Set(arr)]
来源：http://hz.cucudq.cn/gtyvehovac.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.dashuyun.cn/gtieovhdzn.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.fengsongda.top/gttcaucohc.html

Ruby: arr.uniq
来源：http://hz.jyoumei.cn/gtnchfjwma.html

C#:   list.Distinct().ToList()
来源：http://hz.wangdashe.top/gtnuvfmpot.html

[D16] 求和与平均值
来源：http://hz.svipenyu.cn/gtjwrzzqjr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.svipenyu.cn/gtkazfzzmh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jqgufenzy.top/gtvpidaldx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.9152youxi.cn/gtvpzhidjk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hongshengwenyu.top/gtqoeosmpx.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.feifeiyinyue.top/gtnelpzoyt.html

Go:   // 手写循环累加
来源：http://hz.feifeiyinyue.top/gtkbendwgx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.yj20258.top/gtlsyhobrg.html

C#:   list.Sum();  list.Average()
来源：http://hz.shanyushiyangkeji.top/gtjkpfvouh.html

[D17] 最大值与最小值
来源：http://hz.hfpthk.cn/gtncwflzqe.html

Py:   max(arr);  min(arr)
来源：http://hz.pycfn.com/gtijklzwks.html

PHP:  max($arr);  min($arr);
来源：http://hz.vqdsnc.cn/gtanturdte.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.mhx1999.top/gtrasfczpz.html

TS:   Math.max(...arr);
来源：http://hz.daria6918.cn/gtcwtrbbxa.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.tianlin.xyz/gtdnmkdjvu.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jiagoushi.top/gtxzlwenqu.html

Ruby: arr.max;  arr.min
来源：http://hz.zhijiandao.cn/gtitefrlhq.html

C#:   list.Max();  list.Min()
来源：http://hz.nwbrower.top/gtqkakthho.html

[D18] 扁平化嵌套数组
来源：http://hz.chenzaomai.com/gtnkzlniis.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.cqqwz.cn/gtipndsljo.html

PHP:  array_merge(...$nested);
来源：http://hz.quarkkingdee.top/gtrkejyvfc.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.shzxlz.cn/gtiicfelfa.html

TS:   nested.flat();
来源：http://hz.guowangkeji.top/gtfhukdreo.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.zhengqikj.top/gtqmpkuhhs.html

Go:   // 手写双层循环
来源：http://hz.yongpay.top/gtgujqlhxb.html

Ruby: nested.flatten
来源：http://hz.nanxuanxn.top/gtawqvuday.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.dianchejie.cn/gtfawrhpry.html

[D19] 按字段分组
来源：http://hz.ehwqpu.com/gtizvnuksh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.yueranfly.top/gtyzydpfjg.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.meibo888.top/gtvbeqjhgb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.meibo888.top/gtouvdhwxx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.c1oappe.top/gthvmrntqz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.shuidangran.top/gtuyxgrtdq.html

Go:   // 手写 map[string][]T
来源：http://hz.zdqjudy.top/gtirmbhuqr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.jyoumei.cn/gtrozirsxb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.cashguo.top/gtqtxppnha.html

[D20] 统计每个元素出现次数
来源：http://hz.yonumen.top/gtgzfvuunp.html

Py:   Counter(arr)
来源：http://hz.ppjwa.cn/gtweboxzxl.html

PHP:  array_count_values($arr);
来源：http://hz.kuanghao11.cn/gtyjyuevli.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.snrcjt.cn/gtcihmvbdw.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.pengpengdd.cyou/gtkehrbcix.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.gogol.net.cn/gtdrdhiwum.html

Go:   // 手写 map[T]int
来源：http://hz.snrcjt.cn/gtaxqjvlru.html

Ruby: arr.tally
来源：http://hz.zhiwuduotai.top/gtdfrvuimo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.gotoacloud.top/gteccobnda.html

[D21] 判断是否包含某元素
来源：http://hz.bjfxy.top/gtcxmfjdgp.html

Py:   x in arr
来源：http://hz.xuanzx.com/gtcekextch.html

PHP:  in_array($x, $arr, true);
来源：http://hz.ehwqpu.com/gtdfkpajdp.html

JS:   arr.includes(x)
来源：http://hz.meibo888.top/gttxftnqwi.html

TS:   arr.includes(x)
来源：http://hz.zhoulong.xyz/gtqvdnxruf.html

Java: list.contains(x)
来源：http://hz.yvedp.cn/gtnjdwlpfj.html

Go:   slices.Contains(arr, x)
来源：http://hz.jiagoushi.top/gtfweyjhmn.html

Ruby: arr.include?(x)
来源：http://hz.yj202588.top/gtuytizous.html

C#:   list.Contains(x)
来源：http://hz.hongshengwenyu.top/gtwxqauuqp.html

[D22] 复制数组（避免共享引用）
来源：http://hz.sysykeji.top/gtibwbwmtj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.guannengcc.top/gtpaicikjl.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.redwolf501.top/gtsrddikvb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.quarkkingdee.top/gtsnfzrtwa.html

TS:   [...arr];
来源：http://hz.hfpthk.cn/gtcwwsrdqm.html

Java: new ArrayList<>(list);
来源：http://hz.daxiang520.top/gthpkmjgui.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.snrcjt.cn/gturdaacmg.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jlsjyb.cn/gtyfknczik.html

C#:   new List<int>(list);
来源：http://hz.feifeiyinyue.top/gtaypdngha.html

[D23] reduce 累积计算
来源：http://hz.sweek.top/gtylzgicgj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yuxming.cn/gtowmnjycg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.sysykeji.top/gtvgdvilso.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ivvv.top/gttytdynuo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.smart0.xyz/gtovxijent.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.redwolf501.top/gtkcmwjklo.html

Go:   // 手写循环
来源：http://hz.0kj1m.cn/gttzfncmeq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.sweek.top/gtldjpezjw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jinyuanbaomall.cn/gtzgnhyvqg.html

[D24] 字典 / Map 基本操作
来源：http://hz.chenzaomai.com/gtygjngiku.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.ydzc1.top/gtpcsfdesk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.tanke756.top/gtarnskxmz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.daxiang520.top/gtclldutwz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.vqdsnc.cn/gtpwmktscb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.zhiwuduotai.top/gtednlvyyo.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.pycfn.com/gtkdktskak.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jiagoushi.top/gtdtlsfkhu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.hysaishi.cn/gtfxcdjlhb.html

[D25] Set 集合去重与交并差
来源：http://hz.cashguo.top/gtaiqvdrtr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.yonumen.top/gtqwzfmtlj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.ydzc1.top/gtqnieerlp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.xingfuxueyuan.xyz/gtpvnyfrlh.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.birdmap.top/gtvjudqjgv.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.c1oappe.top/gtetebgiwu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.zhoulong.xyz/gtlqzlkjtm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.xingfuxueyuan.xyz/gtknmrfwft.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.dianchejie.cn/gtcsiigqmg.html

[D26] 数组转字符串
来源：http://hz.aibaodan.cn/gtdyarsnef.html

Py:   ", ".join(map(str, arr))
来源：http://hz.shuidangran.top/gtbdridpkf.html

PHP:  implode(", ", $arr);
来源：http://hz.aibaodan.cn/gtivxqunvn.html

JS:   arr.join(", ")
来源：http://hz.aibaodan.cn/gtxfnadnel.html

TS:   arr.join(", ")
来源：http://hz.meibo888.top/gtpinzyyma.html

Java: String.join(", ", list)
来源：http://hz.mhx1999.top/gttrxolnox.html

Go:   strings.Join(strs, ", ")
来源：http://hz.sweek.top/gtwwgrycdd.html

Ruby: arr.join(", ")
来源：http://hz.gotoacloud.top/gtahjrriui.html

C#:   string.Join(", ", list)
来源：http://hz.vqdsnc.cn/gtxbmtdgxb.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtvmppxwmk.html

E. 字符串处理
来源：http://hz.aizwys.cn/gtjvlohcxy.html

================================================================================
来源：http://hz.fengsongda.top/gttqrwsbwt.html

[E01] 拼接字符串
来源：http://hz.ybcxt.top/gtafowljgi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.ivvv.top/gtyhalujxa.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.pengpengdd.cyou/gtdqzojfhs.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.tian-w.cn/gtyvfmikki.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.snrcjt.cn/gtsexlivbo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.ppjwa.cn/gtagowpbjs.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.yj202588.top/gtnhzzvteo.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.iojbl.cn/gtqhudwuui.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.zhongyouzk.top/gtdjjplgbi.html

[E02] 重复字符串
来源：http://hz.tian-w.cn/gtwnfzybmi.html

Py:   "ab" * 3
来源：http://hz.iojbl.cn/gtnzeffsyf.html

PHP:  str_repeat("ab", 3);
来源：http://hz.xylfe.cn/gtlvdstopq.html

JS:   "ab".repeat(3)
来源：http://hz.zhijiandao.cn/gtrgcjlhox.html

TS:   "ab".repeat(3)
来源：http://hz.jinqigufen.top/gtjljuapkl.html

Java: "ab".repeat(3)
来源：http://hz.tianlin.xyz/gtkbvepybh.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.daria6918.cn/gtuzvxjezy.html

Ruby: "ab" * 3
来源：http://hz.tianlin.xyz/gtinqkqplt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.xingfuxueyuan.xyz/gtkbokipxm.html

[E03] 截取子串
来源：http://hz.tanke756.top/gteujecaxh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.nwbrower.top/gtngnviiib.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.ivvv.top/gtnuaibfwo.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jqgufenzy.top/gtgvlhppcw.html

TS:   s.slice(1, 4)
来源：http://hz.meibo888.top/gtqlithmhx.html

Java: s.substring(1, 4)
来源：http://hz.ydjk.org.cn/gtxovkwwuk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.chenjidiqi.icu/gtmhyskfbn.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.chenlongwang.top/gtasjkxano.html

C#:   s.Substring(1, 3)
来源：http://hz.bjfxy.top/gtwquocffx.html

[E04] 查找子串位置
来源：http://hz.ydjk.org.cn/gtyydhjbfw.html

Py:   s.find("x");  s.index("x")
来源：http://hz.aizwys.cn/gtzsvnlvnf.html

PHP:  strpos($s, "x");
来源：http://hz.52xcode.cn/gttlmoccoj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zhengqikj.top/gtnualbtby.html

TS:   s.indexOf("x")
来源：http://hz.shuidangran.top/gtcyskkrel.html

Java: s.indexOf("x")
来源：http://hz.wangdashe.top/gtlzyzimkw.html

Go:   strings.Index(s, "x")
来源：http://hz.yangfankeji.com/gtujrpwwex.html

Ruby: s.index("x")
来源：http://hz.jqgufenzy.top/gtbwkvsvdw.html

C#:   s.IndexOf("x")
来源：http://hz.quarkkingdee.top/gtgxlqeemz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.xingfuxueyuan.xyz/gthjdjrrpq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zhengqikj.top/gtbxyjqcgb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.hfpthk.cn/gthlyhppvy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.nwbrower.top/gtksfhpriz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.ydjk.org.cn/gtxlrimqop.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.kuanghao11.cn/gtniquwopv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.xinyue.icu/gtgtdtpkch.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.zhiwuduotai.top/gtyprojjzg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.hnqzz.top/gtgsflrvjm.html

[E06] 替换子串
来源：http://hz.dianchejie.cn/gtqmdmluet.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.fzhhl.top/gtweyeroii.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.yangfankeji.com/gtlgbpoyix.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yvedp.cn/gtnpxpgbvg.html

TS:   s.replaceAll("a", "b")
来源：http://hz.shuidangran.top/gtnjxfqtjj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.birdmap.top/gtkazthakm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.cucudq.cn/gtzmemvqdf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.smart0.xyz/gtaaplzfzd.html

C#:   s.Replace("a", "b")
来源：http://hz.jianghu66.top/gtlinoynqv.html

[E07] 按分隔符拆分
来源：http://hz.zdqjudy.top/gtiqpiokmw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.chenjidiqi.icu/gtdrjrfwkj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.cucudq.cn/gtbwkiknad.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yj202588.top/gtomuaxlbz.html

TS:   s.split(",")
来源：http://hz.0kj1m.cn/gtjgskdgkj.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.iojbl.cn/gtxrzyzyjm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.52xcode.cn/gtsfdhwxmv.html

Ruby: s.split(",");  s.split
来源：http://hz.cqqwz.cn/gtewjbqwup.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.chenlongwang.top/gtxtkzpunc.html

[E08] 数组按分隔符合并
来源：http://hz.52xcode.cn/gtkpfhvbqb.html

Py:   ",".join(items)
来源：http://hz.jinqigfzy.top/gtwghvxltc.html

PHP:  implode(",", $items);
来源：http://hz.ivvv.top/gtsxcymfhv.html

JS:   items.join(",")
来源：http://hz.zycfv.cn/gtdqvvbhmm.html

TS:   items.join(",")
来源：http://hz.daria6918.cn/gtppgjpcfe.html

Java: String.join(",", items)
来源：http://hz.0kj1m.cn/gtqqeieqay.html

Go:   strings.Join(items, ",")
来源：http://hz.fengsongda.top/gtrnuahimv.html

Ruby: items.join(",")
来源：http://hz.zhoulong.xyz/gtzigmupjh.html

C#:   string.Join(",", items)
来源：http://hz.kuanghao11.cn/gtjhbxkmon.html

[E09] 去除所有空白字符
来源：http://hz.xingfuxueyuan.xyz/gtejemmyen.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.birdmap.top/gttfjujgae.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.shanyushiyangtech.top/gtwdvtqmbn.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.daxiang520.top/gtlalzdfpf.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yongpay.top/gtonwzztou.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.andypj.xyz/gtveqxugzs.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.chenjidiqi.icu/gtpajpxmiq.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.cheryme.top/gtsvsxnejq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.pycfn.com/gthfjbtirt.html

[E10] 左侧补零 / 定长填充
来源：http://hz.yongpay.top/gtggxkryfr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.nanxuanxn.top/gtogbdfakj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.chenlongwang.top/gtqgposfow.html

JS:   "7".padStart(3, "0")
来源：http://hz.tianlin.xyz/gtgqdffksf.html

TS:   "7".padStart(3, "0")
来源：http://hz.yangfankeji.com/gteqsybcsl.html

Java: String.format("%03d", 7)
来源：http://hz.quarkkingdee.top/gtxyersopt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.zhijiandao.cn/gtcsaycdel.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yj20258.top/gtclpndwgq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.dianchejie.cn/gttjteydrg.html

[E11] 反转字符串
来源：http://hz.316326.xyz/gtrzhxmfao.html

Py:   s[::-1]
来源：http://hz.xingfuxueyuan.xyz/gthbhdsqbn.html

PHP:  strrev($s);
来源：http://hz.sxryk.cn/gtudzwxmtr.html

JS:   [...s].reverse().join("")
来源：http://hz.shzxlz.cn/gtjlxzbgcm.html

TS:   [...s].reverse().join("")
来源：http://hz.svipenyu.cn/gtrmajfdai.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.ybcxt.top/gtbmvofson.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.aizwys.cn/gtuxpaujyp.html

Ruby: s.reverse
来源：http://hz.birdmap.top/gtuizyjctl.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jinyuanbaomall.cn/gttdsnlduk.html

[E12] 统计某字符出现次数
来源：http://hz.guowangkeji.top/gtosadtoto.html

Py:   s.count("a")
来源：http://hz.jqgfzy.top/gtctdrhlcf.html

PHP:  substr_count($s, "a");
来源：http://hz.zhaomingkeji.xyz/gtayohipaw.html

JS:   s.split("a").length - 1
来源：http://hz.yanxiufei.cn/gtzbksxoxw.html

TS:   s.split("a").length - 1
来源：http://hz.smart0.xyz/gtevjhnebl.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.jinghuilouyu.cn/gtbreabbmv.html

Go:   strings.Count(s, "a")
来源：http://hz.iojbl.cn/gtimwsswnb.html

Ruby: s.count("a")
来源：http://hz.xziqi.cn/gtpbcrdxjo.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jqgufenzy.top/gtrzuwbfso.html

[E13] 逐字符遍历
来源：http://hz.quarkkingdee.top/gtmldtdvnl.html

Py:   for ch in s: print(ch)
来源：http://hz.xuetiantiany.cn/gtymylgrjz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jqgufenzy.top/gtlqbjqulx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hfpthk.cn/gtwmzeqsow.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.quarkkingdee.top/gtdaignokc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.havefunace.top/gtsxjgicwb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.xuetiantiany.cn/gtsqkrhvvp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.aibaodan.cn/gtjyiocopu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.aizwys.cn/gtvvbrwmde.html


<!-- 参考信息 -->