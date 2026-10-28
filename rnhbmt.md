代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://hz.hysaishi.cn/gtyaynyjzr.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.snrcjt.cn/gtauqoloal.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.quarkkingdee.top/gtrwhcpnsq.html

[D06] 数组长度
来源：http://hz.jianghu66.top/gtrhuxqezh.html

Py:   len(arr)
来源：http://hz.c1oappe.top/gtnwlriqmo.html

PHP:  count($arr);
来源：http://hz.tianlin.xyz/gtunfiyqyu.html

JS:   arr.length
来源：http://hz.tian-w.cn/gttdctudll.html

TS:   arr.length
来源：http://hz.yuanzhike.top/gtyjejcfru.html

Java: list.size();
来源：http://hz.nwbrower.top/gtbhwynjrw.html

Go:   len(arr)
来源：http://hz.ydjk.org.cn/gtlwmxvunf.html

Ruby: arr.length; arr.size
来源：http://hz.hywenlv.cn/gtjlcrgcxa.html

C#:   list.Count;
来源：http://hz.sufxvd.cn/gtvmbkyroa.html

[D07] 切片 / 取子数组
来源：http://hz.jqgfzy.top/gtcauympwa.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yvedp.cn/gtkkgmvams.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.cucudq.cn/gtupkyfmqn.html

JS:   arr.slice(1, 4);
来源：http://hz.kuanghao11.cn/gttzpsewvw.html

TS:   arr.slice(1, 4);
来源：http://hz.ehwqpu.com/gtpjtpbskq.html

Java: list.subList(1, 4);
来源：http://hz.zycfv.cn/gtgcugakfu.html

Go:   arr[1:4]
来源：http://hz.bjfxy.top/gtqkipheoz.html

Ruby: arr[1, 3]
来源：http://hz.jinghuilouyu.cn/gthdmtcolb.html

C#:   list.GetRange(1, 3);
来源：http://hz.daria6918.cn/gttqvsqsdh.html

[D08] 合并两个数组
来源：http://hz.chenjidiqi.icu/gtzqkbveui.html

Py:   a + b;  a.extend(b)
来源：http://hz.shuidangran.top/gtthzqivht.html

PHP:  array_merge($a, $b);
来源：http://hz.mhx1999.top/gtoxtrgvnd.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.meibo888.top/gtcllswbgm.html

TS:   [...a, ...b];
来源：http://hz.jinyuanbaomall.cn/gtmgpwjdxc.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.smart0.xyz/gtkhasyoav.html

Go:   append(a, b...)
来源：http://hz.zhaomingkeji.xyz/gtzghrdvct.html

Ruby: a + b;  a.concat(b)
来源：http://hz.fzhhl.top/gtbmlrmbvq.html

C#:   a.Concat(b).ToList()
来源：http://hz.iojbl.cn/gtmglrvzfb.html

[D09] 排序（升序）
来源：http://hz.gogol.net.cn/gtybapmsqo.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.wangdashe.top/gtmogissjk.html

PHP:  sort($arr);
来源：http://hz.tianlin.xyz/gtxbheuiva.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.xziqi.cn/gtbiquxtoa.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.yanxiufei.cn/gtcimgyvzj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.feifeiyinyue.top/gthogbdnau.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.hywenlv.cn/gtxivswcsh.html

Ruby: arr.sort
来源：http://hz.yangfankeji.com/gthboytlit.html

C#:   list.Sort();
来源：http://hz.0kj1m.cn/gtatoyjrig.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.sxryk.cn/gtojfhkmyn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.ybcxt.top/gtwcrepoaz.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jqgfzy.top/gtojzskcer.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ybcxt.top/gtzzdohkal.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.fengsongda.top/gtpxawxkmd.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.cucudq.cn/gtapwmewtz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.cashguo.top/gtfgjwrbot.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.jqgfzy.top/gtwxcnjtxx.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.xinyue.icu/gtjzehnqar.html

[D11] 反转数组
来源：http://hz.9152youxi.cn/gtwjaudodi.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.cucudq.cn/gtbtyfheym.html

PHP:  array_reverse($arr);
来源：http://hz.kuanghao11.cn/gtaikrsiys.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.chenlongwang.top/gtxcbxqetr.html

TS:   [...arr].reverse();
来源：http://hz.havefunace.top/gtcqytqpfy.html

Java: Collections.reverse(list);
来源：http://hz.ehwqpu.com/gtqidltojl.html

Go:   slices.Reverse(arr)
来源：http://hz.jinqigufen.top/gtggcoypkk.html

Ruby: arr.reverse
来源：http://hz.shangyingyoupin.top/gtilnkpegc.html

C#:   list.Reverse();
来源：http://hz.ybcxt.top/gtnxfofgxw.html

[D12] 查找元素下标
来源：http://hz.yj20258.top/gtweizjyst.html

Py:   arr.index(x);  x in arr
来源：http://hz.pycfn.com/gthgjvnsjt.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jqgufenzy.top/gtdjkaxjho.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.gzhubu.top/gtctlwswmd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.meibo888.top/gtjumhkird.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.nanxuanxn.top/gtylvczmbq.html

Go:   slices.Index(arr, x)
来源：http://hz.smart0.xyz/gthlrkdkse.html

Ruby: arr.index(x)
来源：http://hz.dianchejie.cn/gtrkwupikb.html

C#:   list.IndexOf(x);
来源：http://hz.zhoulong.xyz/gtinerlatd.html

[D13] 过滤（保留满足条件的）
来源：http://hz.0kj1m.cn/gtxznulnpx.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.hnqzz.top/gtlvlshkht.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.chenjidiqi.icu/gtbzgmbgjk.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zdqjudy.top/gtqmkxeefr.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jinyuanbaomall.cn/gteuwhfxcy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.fzhhl.top/gtkphsesiv.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.aizwys.cn/gtorbvgqnb.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.hywenlv.cn/gtyxgfwtgf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.hongshengwenyu.top/gtbfusnccb.html

[D14] 映射转换（每个元素变形）
来源：http://hz.daxiang520.top/gtbkzpgoxj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ehwqpu.com/gttjnmtkzu.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yonumen.top/gtglzdqtrw.html

JS:   arr.map(x => x * 2)
来源：http://hz.316326.xyz/gtvogbwlfu.html

TS:   arr.map(x => x * 2)
来源：http://hz.sysykeji.top/gtpolgavhe.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.zhixingplan.top/gtympyfjbc.html

Go:   // 手写循环
来源：http://hz.sxryk.cn/gtyechxarf.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.chenjidiqi.icu/gtbphvwofi.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.ydjk.org.cn/gtsiwfffgv.html

[D15] 去重
来源：http://hz.sufxvd.cn/gtgvlltfqu.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.shanyushiyangkeji.top/gtiditqeid.html

PHP:  array_unique($arr);
来源：http://hz.nwbrower.top/gtexansjlp.html

JS:   [...new Set(arr)]
来源：http://hz.sweek.top/gtklbdakzf.html

TS:   [...new Set(arr)]
来源：http://hz.yonumen.top/gtfnqyxgra.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jlsjyb.cn/gtuedzrvfz.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.redwolf501.top/gtwykulcqj.html

Ruby: arr.uniq
来源：http://hz.hongshengwenyu.top/gtxunzxalv.html

C#:   list.Distinct().ToList()
来源：http://hz.xylfe.cn/gthyhgtyrh.html

[D16] 求和与平均值
来源：http://hz.zhijiandao.cn/gtqyjjwnmn.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.hysaishi.cn/gtcyeaqxje.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.cdnleiting.top/gtggssjdmp.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.sysykeji.top/gtqelldpsf.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.wangshuangyany.cn/gtlxslxbcr.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.snrcjt.cn/gtyatrpmyo.html

Go:   // 手写循环累加
来源：http://hz.daria6918.cn/gtoazyldxf.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.kuanghao11.cn/gtyanttqyj.html

C#:   list.Sum();  list.Average()
来源：http://hz.jyoumei.cn/gtzoypyrte.html

[D17] 最大值与最小值
来源：http://hz.haohaochexian.top/gtqfjsinqp.html

Py:   max(arr);  min(arr)
来源：http://hz.zycfv.cn/gtbaqhtpcl.html

PHP:  max($arr);  min($arr);
来源：http://hz.cqqwz.cn/gtalpfpjyz.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.guowangkeji.top/gtuhmsiemx.html

TS:   Math.max(...arr);
来源：http://hz.jyoumei.cn/gtonbhhlye.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.shangyingyoupin.top/gteusfptwh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jqgufenzy.top/gthbokafvd.html

Ruby: arr.max;  arr.min
来源：http://hz.tian-w.cn/gtjsefovjj.html

C#:   list.Max();  list.Min()
来源：http://hz.c1oappe.top/gthouaczqm.html

[D18] 扁平化嵌套数组
来源：http://hz.cdnleiting.top/gtyrcctwtj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zhoulong.xyz/gtalhhlmdu.html

PHP:  array_merge(...$nested);
来源：http://hz.jqgfzy.top/gthihpmxif.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.sysykeji.top/gtlfrwktsg.html

TS:   nested.flat();
来源：http://hz.jinyuanbaomall.cn/gtabaoonuw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yanxiufei.cn/gtvnfjuxfz.html

Go:   // 手写双层循环
来源：http://hz.andypj.xyz/gteegmmwvf.html

Ruby: nested.flatten
来源：http://hz.chenzaomai.com/gteyzhedia.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.shzxlz.cn/gtiykcucvb.html

[D19] 按字段分组
来源：http://hz.xziqi.cn/gtzrkwhhbb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.ivvv.top/gtrezftjzt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.wangshuangyany.cn/gtqpudvbgt.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.vqdsnc.cn/gtyyetfixu.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.fzhhl.top/gtwdbugmfh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.cqqwz.cn/gtrxmmldqn.html

Go:   // 手写 map[string][]T
来源：http://hz.jinqigfzy.top/gtkybdatzm.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.zhoulong.xyz/gttcpczxhe.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jinqigfzy.top/gtyyuafkcs.html

[D20] 统计每个元素出现次数
来源：http://hz.zycfv.cn/gtndgmkxns.html

Py:   Counter(arr)
来源：http://hz.nanxuanxn.top/gtslgcmexx.html

PHP:  array_count_values($arr);
来源：http://hz.gotoacloud.top/gtozeyegbz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.pengpengdd.cyou/gtxpdsgqim.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.wangshuangyany.cn/gtxbvwhjyr.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.feifeiyinyue.top/gtgbuerdjm.html

Go:   // 手写 map[T]int
来源：http://hz.xziqi.cn/gtwoxxptlk.html

Ruby: arr.tally
来源：http://hz.havefunace.top/gtmbgmwros.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yueranfly.top/gtzzgakqtz.html

[D21] 判断是否包含某元素
来源：http://hz.chenlongwang.top/gtrrvvinwh.html

Py:   x in arr
来源：http://hz.zhiwuduotai.top/gtajiectzn.html

PHP:  in_array($x, $arr, true);
来源：http://hz.sufxvd.cn/gtumkggbsa.html

JS:   arr.includes(x)
来源：http://hz.guannengcc.top/gttbncljai.html

TS:   arr.includes(x)
来源：http://hz.jiagoushi.top/gtpzhtvdpm.html

Java: list.contains(x)
来源：http://hz.yvedp.cn/gtdtotrthw.html

Go:   slices.Contains(arr, x)
来源：http://hz.andypj.xyz/gthvdxzclu.html

Ruby: arr.include?(x)
来源：http://hz.jinqigfzy.top/gtzlxqgzhd.html

C#:   list.Contains(x)
来源：http://hz.cqqwz.cn/gtwobgfxmg.html

[D22] 复制数组（避免共享引用）
来源：http://hz.hnqzz.top/gtoyxizdga.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.guannengcc.top/gtiszutome.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.zycfv.cn/gtwqmxahds.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.gzhubu.top/gttmqidkvx.html

TS:   [...arr];
来源：http://hz.hfpthk.cn/gttptvsbol.html

Java: new ArrayList<>(list);
来源：http://hz.aizwys.cn/gtkkvqiuxz.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.zhengqikj.top/gthbbtjpwf.html

Ruby: arr.dup;  arr.clone
来源：http://hz.aizwys.cn/gtygrtqcfe.html

C#:   new List<int>(list);
来源：http://hz.yanxiufei.cn/gtvnsclvuz.html

[D23] reduce 累积计算
来源：http://hz.hammf.cn/gttmpdogjj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.iojbl.cn/gtdaarlpks.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.jianghu66.top/gtnlmkamxm.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shzxlz.cn/gtntnymaqv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.chenjidiqi.icu/gtusbqylcf.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.redwolf501.top/gtyntecser.html

Go:   // 手写循环
来源：http://hz.daria6918.cn/gthmapddig.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.316326.xyz/gtkuqkojem.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.sysykeji.top/gtznhtoeib.html

[D24] 字典 / Map 基本操作
来源：http://hz.bjfxy.top/gtiodtinal.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.xingfuxueyuan.xyz/gtvslvftvi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.daxiang520.top/gtedytfjsu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.52xcode.cn/gtddstehvw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.fengsongda.top/gtpchfzmvi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.guowangkeji.top/gtdgsmklky.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.nanxinkj.top/gtnhtkeuvn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.yvedp.cn/gtqgrhvffw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.cucudq.cn/gtnlgercnr.html

[D25] Set 集合去重与交并差
来源：http://hz.haohaochexian.top/gtjkvcxpxb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.ydzc1.top/gtmxwriqdw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.wangdashe.top/gtcvqcgera.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.iojbl.cn/gteruclzec.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.sysykeji.top/gtkgrteajx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.guannengcc.top/gtzepsqokn.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.xuetiantiany.cn/gtglyzcikx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jianghu66.top/gtszkdaihf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.cdnleiting.top/gtkwghmygs.html

[D26] 数组转字符串
来源：http://hz.meibo888.top/gtssudodbl.html

Py:   ", ".join(map(str, arr))
来源：http://hz.zhoulong.xyz/gtetkqlnlx.html

PHP:  implode(", ", $arr);
来源：http://hz.zhiwuduotai.top/gtwrvauoxi.html

JS:   arr.join(", ")
来源：http://hz.fengsongda.top/gtiqeuxdee.html

TS:   arr.join(", ")
来源：http://hz.yj20258888.top/gtqabzlqco.html

Java: String.join(", ", list)
来源：http://hz.shzxlz.cn/gtdepdrray.html

Go:   strings.Join(strs, ", ")
来源：http://hz.9152youxi.cn/gtnuwuzgie.html

Ruby: arr.join(", ")
来源：http://hz.birdmap.top/gtxpsgrhjl.html

C#:   string.Join(", ", list)
来源：http://hz.yj20258888.top/gtiasolmnl.html

================================================================================
来源：http://hz.hfpthk.cn/gtkriebzwa.html

E. 字符串处理
来源：http://hz.yonumen.top/gtgttomwtj.html

================================================================================
来源：http://hz.snrcjt.cn/gtcpdqqfsd.html

[E01] 拼接字符串
来源：http://hz.yj20258.top/gtkmspxhrr.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.haohaochexian.top/gtuaxgtrsr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zycfv.cn/gtkmmonbln.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.aizwys.cn/gtqiwwusag.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.zdqjudy.top/gtrhmddypg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.bjfxy.top/gtycgbssvk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.shangyingyoupin.top/gtshzoiiga.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.pycfn.com/gtecsmimxq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.52xcode.cn/gtjxzyjurj.html

[E02] 重复字符串
来源：http://hz.cucudq.cn/gtffcmjzom.html

Py:   "ab" * 3
来源：http://hz.sweek.top/gtuphgyjlv.html

PHP:  str_repeat("ab", 3);
来源：http://hz.tianlin.xyz/gtrydmywbs.html

JS:   "ab".repeat(3)
来源：http://hz.yongpay.top/gtvhklikju.html

TS:   "ab".repeat(3)
来源：http://hz.andypj.xyz/gtqlilpqtf.html

Java: "ab".repeat(3)
来源：http://hz.cucudq.cn/gtboyvhatm.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.yueranfly.top/gtwhvgvlbd.html

Ruby: "ab" * 3
来源：http://hz.gzhubu.top/gtzedksnxm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.nanxuanxn.top/gtyomralls.html

[E03] 截取子串
来源：http://hz.316326.xyz/gtwvcmblny.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.zhixingplan.top/gtcyhvutgg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.cashguo.top/gtznotavup.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.daria6918.cn/gtuyuoyfof.html

TS:   s.slice(1, 4)
来源：http://hz.9152youxi.cn/gtzzxbcesd.html

Java: s.substring(1, 4)
来源：http://hz.tanke756.top/gtpezdqibb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.yanxiufei.cn/gteldypbqa.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.ybcxt.top/gtajpqguft.html

C#:   s.Substring(1, 3)
来源：http://hz.feifeiyinyue.top/gtwqgkembi.html

[E04] 查找子串位置
来源：http://hz.jinghuilouyu.cn/gtbvgwjiud.html

Py:   s.find("x");  s.index("x")
来源：http://hz.kuanghao11.cn/gtyzqhvipq.html

PHP:  strpos($s, "x");
来源：http://hz.jyoumei.cn/gtgzvqymxj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.sufxvd.cn/gtblubcipz.html

TS:   s.indexOf("x")
来源：http://hz.cashguo.top/gtbvxiuvfq.html

Java: s.indexOf("x")
来源：http://hz.cdnleiting.top/gtyhlqrlxq.html

Go:   strings.Index(s, "x")
来源：http://hz.shuidangran.top/gthlhzqhbh.html

Ruby: s.index("x")
来源：http://hz.gotoacloud.top/gtjubneknc.html

C#:   s.IndexOf("x")
来源：http://hz.jinghuilouyu.cn/gtkxpbvrxn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.guannengcc.top/gtzunuvymw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.xuanzx.com/gtqwckytln.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.gzhubu.top/gtfitkbvcb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.feifeiyinyue.top/gtistbpuch.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.yanxiufei.cn/gtmggvwrtw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.dashuyun.cn/gtsbazehuu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.jinqigfzy.top/gtclgzwggp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.hammf.cn/gtguyybhdb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.xylfe.cn/gtfwhjznok.html

[E06] 替换子串
来源：http://hz.nwbrower.top/gtrkpjvpqb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.guannengcc.top/gtnltoglsg.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.yanxiufei.cn/gtrqakydoo.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hfpthk.cn/gtxsxhgoda.html

TS:   s.replaceAll("a", "b")
来源：http://hz.yongpay.top/gtpbllurux.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zhengqikj.top/gtxfvpnwlv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.zhengqikj.top/gtarrghtyk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.zhaomingkeji.xyz/gthlhdgcok.html

C#:   s.Replace("a", "b")
来源：http://hz.xuetiantiany.cn/gtdlfydiex.html

[E07] 按分隔符拆分
来源：http://hz.dashuyun.cn/gtebknxynq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.xuanzx.com/gtromfttgf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yonumen.top/gtvnfxnlse.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.yj202588.top/gtgsdclhkt.html

TS:   s.split(",")
来源：http://hz.yj202588.top/gtoznxkpde.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.cashguo.top/gtragmwbms.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.xingfuxueyuan.xyz/gtuwcikbar.html

Ruby: s.split(",");  s.split
来源：http://hz.chenjidiqi.icu/gtyorvbeci.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.tian-w.cn/gtlltuawtd.html

[E08] 数组按分隔符合并
来源：http://hz.shanyushiyangkeji.top/gtduuxvgvo.html

Py:   ",".join(items)
来源：http://hz.chenzaomai.com/gtvdxtiivh.html

PHP:  implode(",", $items);
来源：http://hz.jinyuanbaomall.cn/gthwoqhkho.html

JS:   items.join(",")
来源：http://hz.wangshuangyany.cn/gtuzssufou.html

TS:   items.join(",")
来源：http://hz.hysaishi.cn/gtessttptl.html

Java: String.join(",", items)
来源：http://hz.dianchejie.cn/gtrzexfiuc.html

Go:   strings.Join(items, ",")
来源：http://hz.tian-w.cn/gtoccqxssz.html

Ruby: items.join(",")
来源：http://hz.xuanzx.com/gtzlwfkvfv.html

C#:   string.Join(",", items)
来源：http://hz.xziqi.cn/gtsfwbzkwh.html

[E09] 去除所有空白字符
来源：http://hz.zhixingplan.top/gtgmehhygw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.chenlongwang.top/gtthuwdwng.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.xingfuxueyuan.xyz/gtooeejixa.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.cdnleiting.top/gtinqsviyn.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.havefunace.top/gtjwscyygy.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.hnqzz.top/gtwlnhhqtg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.shuidangran.top/gtagqvjzin.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.sweek.top/gtqahreqsl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.shanyushiyangkeji.top/gtzigugbqb.html

[E10] 左侧补零 / 定长填充
来源：http://hz.chenzaomai.com/gtieywwyob.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.kuanghao11.cn/gtifrsokmk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.dianchejie.cn/gtpizhitlu.html

JS:   "7".padStart(3, "0")
来源：http://hz.nwbrower.top/gtodwgsuov.html

TS:   "7".padStart(3, "0")
来源：http://hz.chenzaomai.com/gtbmngxihf.html

Java: String.format("%03d", 7)
来源：http://hz.wangshuangyany.cn/gtzcrvwfur.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yonumen.top/gtcqgcxmhm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.havefunace.top/gtbubvprdv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.quarkkingdee.top/gtghyggkgp.html

[E11] 反转字符串
来源：http://hz.jinqigufen.top/gtytbupxxi.html

Py:   s[::-1]
来源：http://hz.xziqi.cn/gtlnurueiz.html

PHP:  strrev($s);
来源：http://hz.chenlongwang.top/gtgvuopfpr.html

JS:   [...s].reverse().join("")
来源：http://hz.fzhhl.top/gttfkcrpbb.html

TS:   [...s].reverse().join("")
来源：http://hz.zycfv.cn/gtigoorxun.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.yj20258.top/gthvoskhgc.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.dashuyun.cn/gtpejxhkwx.html

Ruby: s.reverse
来源：http://hz.mhx1999.top/gtmoaxojhp.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.cheryme.top/gtbbznnovn.html

[E12] 统计某字符出现次数
来源：http://hz.zhiwuduotai.top/gtkxqdygzt.html

Py:   s.count("a")
来源：http://hz.nanxuanxn.top/gtilanwhbp.html

PHP:  substr_count($s, "a");
来源：http://hz.gzhubu.top/gtfypzayrp.html

JS:   s.split("a").length - 1
来源：http://hz.hnxiangtu.top/gtzjmpmkmx.html

TS:   s.split("a").length - 1
来源：http://hz.shanyushiyangkeji.top/gtmujrqjkr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.xinyue.icu/gtgpnygcpw.html


<!-- 参考信息 -->