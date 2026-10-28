代发 wailian999

Java: list.size();
来源：http://hz.jqgfzy.top/gtgwtoxgbd.html

Go:   len(arr)
来源：http://hz.meibo888.top/gtkklzsufq.html

Ruby: arr.length; arr.size
来源：http://hz.chenjidiqi.icu/gtlwqrztov.html

C#:   list.Count;
来源：http://hz.gotoacloud.top/gtpsucgnqw.html

[D07] 切片 / 取子数组
来源：http://hz.316326.xyz/gtvlbgvqnl.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.52xcode.cn/gtphelxtbo.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.kuanghao11.cn/gtimldqtim.html

JS:   arr.slice(1, 4);
来源：http://hz.ehwqpu.com/gtzqsubwii.html

TS:   arr.slice(1, 4);
来源：http://hz.hysaishi.cn/gtqllocckb.html

Java: list.subList(1, 4);
来源：http://hz.ydjk.org.cn/gtwdxfitap.html

Go:   arr[1:4]
来源：http://hz.zhixingplan.top/gtluzbsgzy.html

Ruby: arr[1, 3]
来源：http://hz.svipenyu.cn/gtwyvozkvw.html

C#:   list.GetRange(1, 3);
来源：http://hz.yanxiufei.cn/gtictgdyqw.html

[D08] 合并两个数组
来源：http://hz.zhengqikj.top/gtepfjfjom.html

Py:   a + b;  a.extend(b)
来源：http://hz.shangyingyoupin.top/gtpqulrkrh.html

PHP:  array_merge($a, $b);
来源：http://hz.cucudq.cn/gtpruhnxud.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.zhixingplan.top/gtfvuioglz.html

TS:   [...a, ...b];
来源：http://hz.sxryk.cn/gtimxvfxfq.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.birdmap.top/gtnicfhdfb.html

Go:   append(a, b...)
来源：http://hz.shuidangran.top/gtxsanixud.html

Ruby: a + b;  a.concat(b)
来源：http://hz.shanyushiyangkeji.top/gtfdrgtfgj.html

C#:   a.Concat(b).ToList()
来源：http://hz.ydjk.org.cn/gtzbtgumwh.html

[D09] 排序（升序）
来源：http://hz.ppjwa.cn/gtjpprwcjs.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jinyuanbaomall.cn/gttuscaxge.html

PHP:  sort($arr);
来源：http://hz.hnxiangtu.top/gtdtqfrmaz.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.havefunace.top/gtptqjiqrv.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.guannengcc.top/gtftjyoxep.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yongpay.top/gtqdqqkhpp.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.fengsongda.top/gtuayjjdiu.html

Ruby: arr.sort
来源：http://hz.tian-w.cn/gtrnpiyhmr.html

C#:   list.Sort();
来源：http://hz.cqqwz.cn/gtmaiygxcp.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.birdmap.top/gtjlfensdn.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.smart0.xyz/gthefvdenq.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cucudq.cn/gtjvlahecx.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.guannengcc.top/gtsgyvpbzx.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yj20258.top/gtbzkfxvio.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zhiwuduotai.top/gtwzajktil.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.zhoulong.xyz/gtkzwytscz.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.ivvv.top/gtyzjpinhk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.c1oappe.top/gtsrzrnmwv.html

[D11] 反转数组
来源：http://hz.hywenlv.cn/gtpllbpupl.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.jlsjyb.cn/gtxdlytusb.html

PHP:  array_reverse($arr);
来源：http://hz.fzhhl.top/gtatofzlyi.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.tianlin.xyz/gtcwcwehta.html

TS:   [...arr].reverse();
来源：http://hz.xinyue.icu/gtvqxdxixd.html

Java: Collections.reverse(list);
来源：http://hz.nanxuanxn.top/gtyzfdtqgx.html

Go:   slices.Reverse(arr)
来源：http://hz.zhongyouzk.top/gththzirml.html

Ruby: arr.reverse
来源：http://hz.hammf.cn/gtfucvtask.html

C#:   list.Reverse();
来源：http://hz.ydjk.org.cn/gtxxxkvjzd.html

[D12] 查找元素下标
来源：http://hz.jqgufenzy.top/gtdxkjkqsu.html

Py:   arr.index(x);  x in arr
来源：http://hz.hywenlv.cn/gtjwkurdin.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.cucudq.cn/gtizfprlyp.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.dianchejie.cn/gtzcdglhqy.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zdqjudy.top/gtznarjceo.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.xuetiantiany.cn/gtkhnuqkhn.html

Go:   slices.Index(arr, x)
来源：http://hz.yueranfly.top/gtpfvlkiuc.html

Ruby: arr.index(x)
来源：http://hz.jqgufenzy.top/gtclfexzka.html

C#:   list.IndexOf(x);
来源：http://hz.tian-w.cn/gthpfaflhh.html

[D13] 过滤（保留满足条件的）
来源：http://hz.jinyuanbaomall.cn/gtinxkvocf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.gogol.net.cn/gtocebagkd.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.birdmap.top/gtrmvnkuhz.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jqgfzy.top/gtpabjkzdh.html

TS:   arr.filter(x => x > 3)
来源：http://hz.dianchejie.cn/gtvpykxhdt.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.sufxvd.cn/gtmvqmmmmj.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.ydzc1.top/gtezfptiro.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.vqdsnc.cn/gtmezjvemi.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.ybcxt.top/gtufrxgpsy.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yonumen.top/gtffocnwsz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.nwbrower.top/gturcvtrlf.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.ywan-chungtsiang.top/gtmubypbmh.html

JS:   arr.map(x => x * 2)
来源：http://hz.52xcode.cn/gtjzabkcme.html

TS:   arr.map(x => x * 2)
来源：http://hz.tianlin.xyz/gtigmmomzf.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.gotoacloud.top/gtvzdlzyvc.html

Go:   // 手写循环
来源：http://hz.wangshuangyany.cn/gtolsrceco.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.nanxuanxn.top/gternrtmox.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.shanyushiyangkeji.top/gtnxhurelx.html

[D15] 去重
来源：http://hz.tanke756.top/gtijfarjsj.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.cucudq.cn/gtcrvmblsn.html

PHP:  array_unique($arr);
来源：http://hz.zhijiandao.cn/gtilmmmcsk.html

JS:   [...new Set(arr)]
来源：http://hz.wangshuangyany.cn/gtfvzvlihd.html

TS:   [...new Set(arr)]
来源：http://hz.yonumen.top/gtuiteubmf.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.yueranfly.top/gtlaqgnmpd.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.c1oappe.top/gtsgoyqvyj.html

Ruby: arr.uniq
来源：http://hz.guowangkeji.top/gtkglmdkkw.html

C#:   list.Distinct().ToList()
来源：http://hz.sweek.top/gtknukxebw.html

[D16] 求和与平均值
来源：http://hz.aizwys.cn/gtljiikphl.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.shanyushiyangtech.top/gtostxcpsd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yj202588.top/gtxoskkbpx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ppjwa.cn/gtnenmntsb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.dianchejie.cn/gtbsokgpvw.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.gotoacloud.top/gtloifilrm.html

Go:   // 手写循环累加
来源：http://hz.fzhhl.top/gtyhfvsylw.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.iojbl.cn/gtvsgcvors.html

C#:   list.Sum();  list.Average()
来源：http://hz.meibo888.top/gtbyowkptx.html

[D17] 最大值与最小值
来源：http://hz.yongpay.top/gtcasqapmt.html

Py:   max(arr);  min(arr)
来源：http://hz.zhaomingkeji.xyz/gtyjaldorf.html

PHP:  max($arr);  min($arr);
来源：http://hz.dianchejie.cn/gtddusjvqy.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.hysaishi.cn/gtfmvqsgof.html

TS:   Math.max(...arr);
来源：http://hz.fengsongda.top/gtugyypuiv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.sweek.top/gtixjtqpxh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.hfpthk.cn/gtwzxmdifr.html

Ruby: arr.max;  arr.min
来源：http://hz.yonumen.top/gtjkwnygsl.html

C#:   list.Max();  list.Min()
来源：http://hz.ywan-chungtsiang.top/gtkyebwlrz.html

[D18] 扁平化嵌套数组
来源：http://hz.gaohongyu789.top/gtoihrfggb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.quarkkingdee.top/gtwxcsmitk.html

PHP:  array_merge(...$nested);
来源：http://hz.jiagoushi.top/gtmjeubrqj.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.daxiang520.top/gtfrdzlghe.html

TS:   nested.flat();
来源：http://hz.xuanzx.com/gtsjppkiyf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.ydzc1.top/gtnolmwueh.html

Go:   // 手写双层循环
来源：http://hz.nwbrower.top/gtojovbvcc.html

Ruby: nested.flatten
来源：http://hz.9152youxi.cn/gttcbtqqta.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.birdmap.top/gtcgjfaujz.html

[D19] 按字段分组
来源：http://hz.zhongyouzk.top/gtbavedtea.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.tianlin.xyz/gtifuelnvu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yonumen.top/gtplbxouhs.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.hnqzz.top/gtjjswsbks.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jiagoushi.top/gteuuabyiz.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.ehwqpu.com/gtbyneotqp.html

Go:   // 手写 map[string][]T
来源：http://hz.hammf.cn/gtizxthfrs.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.pengpengdd.cyou/gtwjbxztgc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zhongyouzk.top/gtmkhvgtqw.html

[D20] 统计每个元素出现次数
来源：http://hz.zdqjudy.top/gtfljydhbm.html

Py:   Counter(arr)
来源：http://hz.yongpay.top/gtbbyfdogs.html

PHP:  array_count_values($arr);
来源：http://hz.iojbl.cn/gteofuoqmt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhiwuduotai.top/gtgeoizhft.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yj202588.top/gtqbpoziww.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.xziqi.cn/gtfqwoxdny.html

Go:   // 手写 map[T]int
来源：http://hz.sweek.top/gtwebpyhdd.html

Ruby: arr.tally
来源：http://hz.wangdashe.top/gtpepeisaz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.jqgufenzy.top/gtgwykmzjf.html

[D21] 判断是否包含某元素
来源：http://hz.xziqi.cn/gtfdrhhfnx.html

Py:   x in arr
来源：http://hz.ydzc1.top/gtyvtnutag.html

PHP:  in_array($x, $arr, true);
来源：http://hz.tian-w.cn/gtvuvgxavn.html

JS:   arr.includes(x)
来源：http://hz.jinyuanbaomall.cn/gtphakyioy.html

TS:   arr.includes(x)
来源：http://hz.zhongyouzk.top/gtsfnccaty.html

Java: list.contains(x)
来源：http://hz.jianghu66.top/gtckukvmxr.html

Go:   slices.Contains(arr, x)
来源：http://hz.ybcxt.top/gtmydedwvq.html

Ruby: arr.include?(x)
来源：http://hz.vqdsnc.cn/gttgfdcons.html

C#:   list.Contains(x)
来源：http://hz.yangfankeji.com/gtmlznnvwi.html

[D22] 复制数组（避免共享引用）
来源：http://hz.zhixingplan.top/gtgqavicmr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.hfpthk.cn/gtwyedxcmt.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.9152youxi.cn/gtjcyetvsr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jiagoushi.top/gtsipatpcp.html

TS:   [...arr];
来源：http://hz.nanxinkj.top/gtmkdovisy.html

Java: new ArrayList<>(list);
来源：http://hz.zdqjudy.top/gtdwtnzqts.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.yj20258.top/gtqzzbvrqf.html

Ruby: arr.dup;  arr.clone
来源：http://hz.xuanzx.com/gtinmndtat.html

C#:   new List<int>(list);
来源：http://hz.dianchejie.cn/gtuvuhahgs.html

[D23] reduce 累积计算
来源：http://hz.shanyushiyangkeji.top/gtsvgoxioj.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.aizwys.cn/gtbpffvnjp.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.kuanghao11.cn/gtkhddwaaq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yj20258888.top/gttncneivh.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.meibo888.top/gtsntxjfyb.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.hongshengwenyu.top/gtiqwlsuag.html

Go:   // 手写循环
来源：http://hz.cheryme.top/gtknrjlaxc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.gaohongyu789.top/gtkvtjksdv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.pengpengdd.cyou/gtlhqfdpcz.html

[D24] 字典 / Map 基本操作
来源：http://hz.mhx1999.top/gtsoyidnmz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.jqgufenzy.top/gtcpzouuxs.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.sweek.top/gtqfbilcyg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jqgufenzy.top/gthakirbzw.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.ywan-chungtsiang.top/gtqydzavli.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.zycfv.cn/gtujulsjle.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.c1oappe.top/gtgfhbosxf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.fzhhl.top/gtekdvirfn.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.tian-w.cn/gttuvzxtaa.html

[D25] Set 集合去重与交并差
来源：http://hz.ydjk.org.cn/gtlzxtozvb.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zhengqikj.top/gtqxlzfsii.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.yuxming.cn/gtfysvyduk.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.hywenlv.cn/gtykhslmzm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.yuxming.cn/gtmylwqhds.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.sxryk.cn/gthapdgpar.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.tian-w.cn/gtcohrjdux.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yj20258.top/gtjgxrgpru.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.0kj1m.cn/gtmdtmotbi.html

[D26] 数组转字符串
来源：http://hz.shanyushiyangtech.top/gtgrkljexi.html

Py:   ", ".join(map(str, arr))
来源：http://hz.sysykeji.top/gtqrujtwfj.html

PHP:  implode(", ", $arr);
来源：http://hz.haohaochexian.top/gtdukbppsr.html

JS:   arr.join(", ")
来源：http://hz.snrcjt.cn/gtbbosoudt.html

TS:   arr.join(", ")
来源：http://hz.zhiwuduotai.top/gtmwfgtlcw.html

Java: String.join(", ", list)
来源：http://hz.fzhhl.top/gtkhzjiwnp.html

Go:   strings.Join(strs, ", ")
来源：http://hz.quarkkingdee.top/gtddhcrxoi.html

Ruby: arr.join(", ")
来源：http://hz.ppjwa.cn/gtlydlunqp.html

C#:   string.Join(", ", list)
来源：http://hz.fengsongda.top/gtikhbgyoa.html

================================================================================
来源：http://hz.hywenlv.cn/gtgnxcjvyv.html

E. 字符串处理
来源：http://hz.daxiang520.top/gtwbvskqlm.html

================================================================================
来源：http://hz.haohaochexian.top/gtopyskanw.html

[E01] 拼接字符串
来源：http://hz.vqdsnc.cn/gtacywmfpa.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.aibaodan.cn/gtoqjndnmh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yangfankeji.com/gttgygvzqu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.316326.xyz/gtmnqgosih.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.haohaochexian.top/gtxkdyasis.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.shangyingyoupin.top/gtivmofaco.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.shzxlz.cn/gtnjvwbhdx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.yj202588.top/gtnzikuufo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.gzhubu.top/gtbbdlvbeh.html

[E02] 重复字符串
来源：http://hz.ppjwa.cn/gtluwgbxyt.html

Py:   "ab" * 3
来源：http://hz.guannengcc.top/gtstvhzsux.html

PHP:  str_repeat("ab", 3);
来源：http://hz.havefunace.top/gtrjnkkwwd.html

JS:   "ab".repeat(3)
来源：http://hz.yueranfly.top/gteelmpmik.html

TS:   "ab".repeat(3)
来源：http://hz.zhijiandao.cn/gtqdtqcnzd.html

Java: "ab".repeat(3)
来源：http://hz.aizwys.cn/gtfwkirtwt.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.nanxuanxn.top/gtsaobevxw.html

Ruby: "ab" * 3
来源：http://hz.yangfankeji.com/gtyvyihfao.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yangfankeji.com/gtcibidssz.html

[E03] 截取子串
来源：http://hz.sweek.top/gtdzmnqvrm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.cucudq.cn/gtjmplyiec.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.fengsongda.top/gtrxsgjkfm.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jyoumei.cn/gthcvmaftx.html

TS:   s.slice(1, 4)
来源：http://hz.jianghu66.top/gtvuftdypw.html

Java: s.substring(1, 4)
来源：http://hz.yj202588.top/gtxzlysvqy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.xingfuxueyuan.xyz/gthyyfsgtr.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.316326.xyz/gtnuhrfxdv.html

C#:   s.Substring(1, 3)
来源：http://hz.aibaodan.cn/gtwazbgmlw.html

[E04] 查找子串位置
来源：http://hz.hfpthk.cn/gtsuibzpuk.html

Py:   s.find("x");  s.index("x")
来源：http://hz.smart0.xyz/gtlozgrtwr.html

PHP:  strpos($s, "x");
来源：http://hz.hfpthk.cn/gtwjhxhcis.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.hfpthk.cn/gtbnfeerci.html

TS:   s.indexOf("x")
来源：http://hz.kuanghao11.cn/gthythuoyy.html

Java: s.indexOf("x")
来源：http://hz.c1oappe.top/gtssolwqci.html

Go:   strings.Index(s, "x")
来源：http://hz.jinghuilouyu.cn/gthnftapnm.html

Ruby: s.index("x")
来源：http://hz.9152youxi.cn/gtxjmwgjrk.html

C#:   s.IndexOf("x")
来源：http://hz.feifeiyinyue.top/gtiuwcuuwd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.aibaodan.cn/gtyrfrifrn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.fengsongda.top/gtalfpfxil.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.ehwqpu.com/gthjcsmiqv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hysaishi.cn/gtystgjtfs.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zhijiandao.cn/gtuxxpzryn.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yvedp.cn/gtkktrbmfj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.yj202588.top/gthdvvnkdj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.nanxuanxn.top/gtdvfdgztn.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.hongshengwenyu.top/gtqntqhepj.html

[E06] 替换子串
来源：http://hz.gogol.net.cn/gtpincuxkv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.sweek.top/gtavsdcnqt.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.9152youxi.cn/gtkigneqnm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yonumen.top/gtsmdwcftd.html

TS:   s.replaceAll("a", "b")
来源：http://hz.tianlin.xyz/gtxlsafydy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.jiagoushi.top/gtevyirtin.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.cashguo.top/gtwkuybegp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.iojbl.cn/gtzfuxixez.html

C#:   s.Replace("a", "b")
来源：http://hz.xuetiantiany.cn/gtzwzkzeaq.html

[E07] 按分隔符拆分
来源：http://hz.sweek.top/gtccubvyui.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.andypj.xyz/gtnlhmqluv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.hnxiangtu.top/gtwjjwtwpv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.shuidangran.top/gtjeysbgzh.html

TS:   s.split(",")
来源：http://hz.iojbl.cn/gtlngkaxib.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.ehwqpu.com/gtmymqdayc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zhaomingkeji.xyz/gtgecwextd.html

Ruby: s.split(",");  s.split
来源：http://hz.hongshengwenyu.top/gtvjhxxyze.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.hywenlv.cn/gtoqpurwko.html

[E08] 数组按分隔符合并
来源：http://hz.xuetiantiany.cn/gtgxukfspt.html

Py:   ",".join(items)
来源：http://hz.redwolf501.top/gtjbtuqean.html

PHP:  implode(",", $items);
来源：http://hz.zhoulong.xyz/gttfywgiwk.html

JS:   items.join(",")
来源：http://hz.52xcode.cn/gtvurcvicb.html

TS:   items.join(",")
来源：http://hz.chenlongwang.top/gtqgqepoes.html

Java: String.join(",", items)
来源：http://hz.hysaishi.cn/gtsgjoduxj.html

Go:   strings.Join(items, ",")
来源：http://hz.jinghuilouyu.cn/gtkiqcaxbm.html

Ruby: items.join(",")
来源：http://hz.zdqjudy.top/gtweocdbxb.html

C#:   string.Join(",", items)
来源：http://hz.kuanghao11.cn/gttsmbahbu.html

[E09] 去除所有空白字符
来源：http://hz.hongshengwenyu.top/gtwmspirjb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.tanke756.top/gtjvwyimig.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.ppjwa.cn/gthksaxwlx.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.cucudq.cn/gtyidwhamn.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.zhijiandao.cn/gtyatmhmmi.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.gzhubu.top/gtodqcxmni.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xuanzx.com/gtmgytfxnt.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.dashuyun.cn/gthinpgfud.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.gogol.net.cn/gtynhopkud.html

[E10] 左侧补零 / 定长填充
来源：http://hz.feifeiyinyue.top/gtxriwanwv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.zhoulong.xyz/gthizfjuua.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yanxiufei.cn/gthftmaill.html

JS:   "7".padStart(3, "0")
来源：http://hz.cheryme.top/gtkjbmiaby.html

TS:   "7".padStart(3, "0")
来源：http://hz.daria6918.cn/gtjenrdjyf.html

Java: String.format("%03d", 7)
来源：http://hz.haohaochexian.top/gtihzyjkqx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.dashuyun.cn/gtsdgafrvt.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.guowangkeji.top/gtbhatpbug.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.zhixingplan.top/gtlhjactpe.html

[E11] 反转字符串
来源：http://hz.zhaomingkeji.xyz/gtziwnuops.html

Py:   s[::-1]
来源：http://hz.meibo888.top/gtlldrtqfz.html

PHP:  strrev($s);
来源：http://hz.xziqi.cn/gtiwrsdznr.html

JS:   [...s].reverse().join("")
来源：http://hz.hfpthk.cn/gtcaahwrbe.html

TS:   [...s].reverse().join("")
来源：http://hz.jiagoushi.top/gtqpmegqcn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.zhengqikj.top/gtfjnplzem.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.gotoacloud.top/gtbsagcsqu.html

Ruby: s.reverse
来源：http://hz.52xcode.cn/gtgbgleqyi.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.cucudq.cn/gtwwwghcea.html

[E12] 统计某字符出现次数
来源：http://hz.haohaochexian.top/gtlpnvpevt.html

Py:   s.count("a")
来源：http://hz.hfpthk.cn/gtsikmvjof.html

PHP:  substr_count($s, "a");
来源：http://hz.xingfuxueyuan.xyz/gtfliwzwup.html

JS:   s.split("a").length - 1
来源：http://hz.cashguo.top/gtofzjbzmk.html

TS:   s.split("a").length - 1
来源：http://hz.gzhubu.top/gttoqtwxus.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.hnxiangtu.top/gtwxwxzwvd.html

Go:   strings.Count(s, "a")
来源：http://hz.ivvv.top/gtageynikr.html

Ruby: s.count("a")
来源：http://hz.chenjidiqi.icu/gtnwmvauaz.html

C#:   s.Count(c => c == 'a')
来源：http://hz.kuanghao11.cn/gttsnubfdn.html

[E13] 逐字符遍历
来源：http://hz.jinyuanbaomall.cn/gtnrvdjtod.html

Py:   for ch in s: print(ch)
来源：http://hz.birdmap.top/gtsdzqnmpb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.chenlongwang.top/gtqfbqpfnb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhaomingkeji.xyz/gtarowsnoa.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yangfankeji.com/gtsnxhetil.html


<!-- 参考信息 -->