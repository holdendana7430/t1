代发 wailian999

Java: list.size();
来源：http://hz.pengpengdd.cyou/gtptobrqgh.html

Go:   len(arr)
来源：http://hz.jqgfzy.top/gtkrnsmfjc.html

Ruby: arr.length; arr.size
来源：http://hz.nanxinkj.top/gthildaken.html

C#:   list.Count;
来源：http://hz.nwbrower.top/gtkgckssid.html

[D07] 切片 / 取子数组
来源：http://hz.shangyingyoupin.top/gtxugbfgmg.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yongpay.top/gtlxubjrrf.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.shzxlz.cn/gtshkmbhbb.html

JS:   arr.slice(1, 4);
来源：http://hz.ybcxt.top/gthqcardcx.html

TS:   arr.slice(1, 4);
来源：http://hz.sufxvd.cn/gtlnwhcjzt.html

Java: list.subList(1, 4);
来源：http://hz.guowangkeji.top/gtcjcpsdys.html

Go:   arr[1:4]
来源：http://hz.gotoacloud.top/gtbnmovoiu.html

Ruby: arr[1, 3]
来源：http://hz.yonumen.top/gtmorxlvvb.html

C#:   list.GetRange(1, 3);
来源：http://hz.yj20258.top/gtirgaqwvd.html

[D08] 合并两个数组
来源：http://hz.guannengcc.top/gtgwlrgjul.html

Py:   a + b;  a.extend(b)
来源：http://hz.dashuyun.cn/gtiuixiwlu.html

PHP:  array_merge($a, $b);
来源：http://hz.cashguo.top/gtgjbokuoo.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.tianlin.xyz/gtqtumilyo.html

TS:   [...a, ...b];
来源：http://hz.hnxiangtu.top/gtfosjbaxb.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.yuxming.cn/gtqdlnnepw.html

Go:   append(a, b...)
来源：http://hz.yueranfly.top/gtdqyuippe.html

Ruby: a + b;  a.concat(b)
来源：http://hz.chenlongwang.top/gtcnydsedj.html

C#:   a.Concat(b).ToList()
来源：http://hz.pycfn.com/gthksxtsmq.html

[D09] 排序（升序）
来源：http://hz.ehwqpu.com/gtumydznsc.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cashguo.top/gtawuzfctu.html

PHP:  sort($arr);
来源：http://hz.yuxming.cn/gtdjgxsrjv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.jqgfzy.top/gtqcklryfo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.sxryk.cn/gtcrzserzd.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yj20258888.top/gtltjpiydl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.ydzc1.top/gtuzlqdvhu.html

Ruby: arr.sort
来源：http://hz.shzxlz.cn/gtblycaadp.html

C#:   list.Sort();
来源：http://hz.9152youxi.cn/gtvvttpevi.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.yongpay.top/gtddwgvugi.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.nwbrower.top/gtyyomfckl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.mhx1999.top/gtirydpnij.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jianghu66.top/gtfwbglbrb.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.nanxuanxn.top/gtesgnpyzn.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.chenlongwang.top/gtlnvlmemw.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.guowangkeji.top/gtdjymumcg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.0kj1m.cn/gtctpnzgyr.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.xziqi.cn/gtkqbagula.html

[D11] 反转数组
来源：http://hz.yanxiufei.cn/gtgwaaqbei.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.shanyushiyangtech.top/gtflwfnlqa.html

PHP:  array_reverse($arr);
来源：http://hz.jqgfzy.top/gtsclmxxyf.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.daxiang520.top/gtulhmtjml.html

TS:   [...arr].reverse();
来源：http://hz.snrcjt.cn/gtbrnvgdpe.html

Java: Collections.reverse(list);
来源：http://hz.yueranfly.top/gtwqmqicvq.html

Go:   slices.Reverse(arr)
来源：http://hz.guowangkeji.top/gtzjfheekg.html

Ruby: arr.reverse
来源：http://hz.ywan-chungtsiang.top/gtczlnhtur.html

C#:   list.Reverse();
来源：http://hz.jqgufenzy.top/gtxqicbavf.html

[D12] 查找元素下标
来源：http://hz.wangshuangyany.cn/gtekxaoyzq.html

Py:   arr.index(x);  x in arr
来源：http://hz.jiagoushi.top/gtfxofhpty.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.mhx1999.top/gtflxpuxib.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hywenlv.cn/gtolyleoqn.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.hywenlv.cn/gtmouojyki.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.quarkkingdee.top/gtfrbwpoor.html

Go:   slices.Index(arr, x)
来源：http://hz.xinyue.icu/gtgaicwwgm.html

Ruby: arr.index(x)
来源：http://hz.iojbl.cn/gtpbvdfatg.html

C#:   list.IndexOf(x);
来源：http://hz.ehwqpu.com/gtdlrrschf.html

[D13] 过滤（保留满足条件的）
来源：http://hz.kuanghao11.cn/gtbhsxnjku.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.52xcode.cn/gthbtiynhs.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.ydzc1.top/gtselponez.html

JS:   arr.filter(x => x > 3)
来源：http://hz.tian-w.cn/gtybxfzoql.html

TS:   arr.filter(x => x > 3)
来源：http://hz.wangdashe.top/gtgfypecjk.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.nwbrower.top/gtbkctntct.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.nwbrower.top/gtggaezxfz.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.snrcjt.cn/gtcehnpnhf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.fengsongda.top/gtwhcuvsgv.html

[D14] 映射转换（每个元素变形）
来源：http://hz.quarkkingdee.top/gtlsjipxbv.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.daxiang520.top/gtwxrsrqcw.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.svipenyu.cn/gtahjkrpsz.html

JS:   arr.map(x => x * 2)
来源：http://hz.yonumen.top/gtvgjkfeid.html

TS:   arr.map(x => x * 2)
来源：http://hz.redwolf501.top/gtpbeqjtzk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.ywan-chungtsiang.top/gtpgbhrbln.html

Go:   // 手写循环
来源：http://hz.c1oappe.top/gtxzotogwk.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.vqdsnc.cn/gtsuicxylt.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.jinqigfzy.top/gtszhwzmlz.html

[D15] 去重
来源：http://hz.jlsjyb.cn/gtwmhenfns.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.pengpengdd.cyou/gtpaodqpqk.html

PHP:  array_unique($arr);
来源：http://hz.tian-w.cn/gtyefdlkij.html

JS:   [...new Set(arr)]
来源：http://hz.ywan-chungtsiang.top/gtndhuxljo.html

TS:   [...new Set(arr)]
来源：http://hz.sxryk.cn/gtrarhhrzc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.gzhubu.top/gtabhldraf.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.haohaochexian.top/gtrveixoli.html

Ruby: arr.uniq
来源：http://hz.haohaochexian.top/gtgrbjsqjx.html

C#:   list.Distinct().ToList()
来源：http://hz.0kj1m.cn/gtroyqsndh.html

[D16] 求和与平均值
来源：http://hz.chenjidiqi.icu/gtknkdompu.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.guowangkeji.top/gtnhifmnuu.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.cashguo.top/gtifqnmmcx.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.cqqwz.cn/gtaiaiebuj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jiagoushi.top/gtotbzoiaq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.yonumen.top/gtduuoqmyq.html

Go:   // 手写循环累加
来源：http://hz.zhoulong.xyz/gtwuvfsgij.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.meibo888.top/gtqtzmbwxe.html

C#:   list.Sum();  list.Average()
来源：http://hz.yj20258.top/gtmbvkfkcp.html

[D17] 最大值与最小值
来源：http://hz.xuetiantiany.cn/gtnnazecbv.html

Py:   max(arr);  min(arr)
来源：http://hz.jlsjyb.cn/gteegfwmzr.html

PHP:  max($arr);  min($arr);
来源：http://hz.zhengqikj.top/gtbvowuycv.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.jyoumei.cn/gtwcaokakj.html

TS:   Math.max(...arr);
来源：http://hz.feifeiyinyue.top/gtmcvlhabk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.iojbl.cn/gtigrkuzbt.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.bjfxy.top/gtrwkcyjcm.html

Ruby: arr.max;  arr.min
来源：http://hz.0kj1m.cn/gturbnzqms.html

C#:   list.Max();  list.Min()
来源：http://hz.zhijiandao.cn/gtmxznnpnx.html

[D18] 扁平化嵌套数组
来源：http://hz.jianghu66.top/gtwruuffoz.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.xingfuxueyuan.xyz/gthlzerbzz.html

PHP:  array_merge(...$nested);
来源：http://hz.jinghuilouyu.cn/gtflrtjjvy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.snrcjt.cn/gtmkedkldh.html

TS:   nested.flat();
来源：http://hz.cheryme.top/gtxoakzkqu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.gaohongyu789.top/gtjxceawan.html

Go:   // 手写双层循环
来源：http://hz.tianlin.xyz/gtynnijkzu.html

Ruby: nested.flatten
来源：http://hz.redwolf501.top/gtwjigenhm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.shuidangran.top/gtvvryqzcj.html

[D19] 按字段分组
来源：http://hz.sysykeji.top/gtfyrgzfdx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.sysykeji.top/gtclpdhutt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yj20258.top/gtbozxdoto.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.wangshuangyany.cn/gtdzgidbwq.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.jinqigufen.top/gttorvxqbh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.quarkkingdee.top/gtyqnueicn.html

Go:   // 手写 map[string][]T
来源：http://hz.jinyuanbaomall.cn/gthpebqdoh.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.shuidangran.top/gtatnidmkk.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.pengpengdd.cyou/gtymknywbs.html

[D20] 统计每个元素出现次数
来源：http://hz.xylfe.cn/gtovwojasu.html

Py:   Counter(arr)
来源：http://hz.yonumen.top/gtlutlybqq.html

PHP:  array_count_values($arr);
来源：http://hz.birdmap.top/gtnrrkuabw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.dashuyun.cn/gttcyfyfme.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.bjfxy.top/gtcwvqldvv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.tian-w.cn/gtcfqxyquo.html

Go:   // 手写 map[T]int
来源：http://hz.andypj.xyz/gtivkehfbb.html

Ruby: arr.tally
来源：http://hz.yanxiufei.cn/gtgxbyfncx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.svipenyu.cn/gtvmjzaeej.html

[D21] 判断是否包含某元素
来源：http://hz.tianlin.xyz/gtevjftfcg.html

Py:   x in arr
来源：http://hz.dianchejie.cn/gtikzuemol.html

PHP:  in_array($x, $arr, true);
来源：http://hz.guowangkeji.top/gtixmttbnu.html

JS:   arr.includes(x)
来源：http://hz.hongshengwenyu.top/gtvyagsecq.html

TS:   arr.includes(x)
来源：http://hz.cucudq.cn/gtidbtmkzq.html

Java: list.contains(x)
来源：http://hz.yj20258888.top/gtgiwdrdyx.html

Go:   slices.Contains(arr, x)
来源：http://hz.yj20258888.top/gtpymbjpgx.html

Ruby: arr.include?(x)
来源：http://hz.zhongyouzk.top/gtkthqiocs.html

C#:   list.Contains(x)
来源：http://hz.9152youxi.cn/gtenehlsoi.html

[D22] 复制数组（避免共享引用）
来源：http://hz.ydzc1.top/gtzmvyrshy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.wangdashe.top/gtsiapnzgz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.aibaodan.cn/gtthnttbls.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.wangdashe.top/gtnmybyioa.html

TS:   [...arr];
来源：http://hz.hnxiangtu.top/gtvqxtgzqs.html

Java: new ArrayList<>(list);
来源：http://hz.fengsongda.top/gtptseongv.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jinghuilouyu.cn/gthnkqubor.html

Ruby: arr.dup;  arr.clone
来源：http://hz.sweek.top/gtrxcaqbet.html

C#:   new List<int>(list);
来源：http://hz.xuanzx.com/gtuxwryktd.html

[D23] reduce 累积计算
来源：http://hz.yueranfly.top/gtajimctex.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yangfankeji.com/gtegjjqlsv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.dianchejie.cn/gtjomgiesc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jyoumei.cn/gtxvumgjao.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.fzhhl.top/gtsureddes.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.daxiang520.top/gtalevulpb.html

Go:   // 手写循环
来源：http://hz.zhengqikj.top/gtsummiooj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.yangfankeji.com/gtnrmnvqub.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.zhengqikj.top/gtkwbsutxe.html

[D24] 字典 / Map 基本操作
来源：http://hz.jqgufenzy.top/gtfbyqslav.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.hfpthk.cn/gtthekcehp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.chenzaomai.com/gthfentktx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.havefunace.top/gthrzzvswl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.chenjidiqi.icu/gtrbtjcndo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jinghuilouyu.cn/gtfqwthwan.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.meibo888.top/gtyxnbbcgt.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.xingfuxueyuan.xyz/gtzqwhrpds.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.gaohongyu789.top/gtvyttotxv.html

[D25] Set 集合去重与交并差
来源：http://hz.sweek.top/gtotlkcosy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zhijiandao.cn/gtctbdrjgi.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.ivvv.top/gtdrwxtnjb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zhiwuduotai.top/gtbhesdras.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.yj20258.top/gtzadgyugb.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.haohaochexian.top/gtkqdlgfih.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.zycfv.cn/gtrwrcdzlu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.wangshuangyany.cn/gtdussoolu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.smart0.xyz/gtyqcriifi.html

[D26] 数组转字符串
来源：http://hz.gaohongyu789.top/gtdlaokgnl.html

Py:   ", ".join(map(str, arr))
来源：http://hz.meibo888.top/gtzgymtbbz.html

PHP:  implode(", ", $arr);
来源：http://hz.tianlin.xyz/gtnuvyhqav.html

JS:   arr.join(", ")
来源：http://hz.ehwqpu.com/gtbkjwhjyn.html

TS:   arr.join(", ")
来源：http://hz.yongpay.top/gtfochfejd.html

Java: String.join(", ", list)
来源：http://hz.xuanzx.com/gtbjbmeknv.html

Go:   strings.Join(strs, ", ")
来源：http://hz.redwolf501.top/gtrevjlyim.html

Ruby: arr.join(", ")
来源：http://hz.sxryk.cn/gtinfgvobq.html

C#:   string.Join(", ", list)
来源：http://hz.guowangkeji.top/gtxocbooos.html

================================================================================
来源：http://hz.hysaishi.cn/gtcrmfbgeg.html

E. 字符串处理
来源：http://hz.feifeiyinyue.top/gtepntagiz.html

================================================================================
来源：http://hz.jyoumei.cn/gtmvospfdi.html

[E01] 拼接字符串
来源：http://hz.gotoacloud.top/gtzhqaqtug.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.snrcjt.cn/gtfeggepbl.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.yuanzhike.top/gtgrvzfcvg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.iojbl.cn/gtvjouvjpn.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.meibo888.top/gtfpakkdcj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.aibaodan.cn/gtrhrlbbop.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.xingfuxueyuan.xyz/gtantlbrar.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.gotoacloud.top/gtgsqrexdl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.hammf.cn/gtchjkmuwo.html

[E02] 重复字符串
来源：http://hz.jlsjyb.cn/gtepevylcb.html

Py:   "ab" * 3
来源：http://hz.zhixingplan.top/gtbkdxzbaw.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jlsjyb.cn/gttjkyoxxn.html

JS:   "ab".repeat(3)
来源：http://hz.sysykeji.top/gtumnjuesp.html

TS:   "ab".repeat(3)
来源：http://hz.gzhubu.top/gtbyskbxep.html

Java: "ab".repeat(3)
来源：http://hz.feifeiyinyue.top/gtunlrytmz.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.chenjidiqi.icu/gtqygtedwc.html

Ruby: "ab" * 3
来源：http://hz.jinqigfzy.top/gtxkaxjcdg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.xziqi.cn/gtoshwmvvm.html

[E03] 截取子串
来源：http://hz.meibo888.top/gtopqxtgtv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.nwbrower.top/gtyuvsonsy.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.shanyushiyangkeji.top/gtpdiofqzb.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.sxryk.cn/gthlnksaeq.html

TS:   s.slice(1, 4)
来源：http://hz.shanyushiyangtech.top/gtagabjjwk.html

Java: s.substring(1, 4)
来源：http://hz.xziqi.cn/gtwwhbaqqg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.cqqwz.cn/gtyvvxjdvr.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.zycfv.cn/gtbpubgjgn.html

C#:   s.Substring(1, 3)
来源：http://hz.gaohongyu789.top/gttynojouj.html

[E04] 查找子串位置
来源：http://hz.aizwys.cn/gtkinjdgmj.html

Py:   s.find("x");  s.index("x")
来源：http://hz.pycfn.com/gtpwsjghav.html

PHP:  strpos($s, "x");
来源：http://hz.cashguo.top/gtezlrxylq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.wangdashe.top/gtggngvoqf.html

TS:   s.indexOf("x")
来源：http://hz.redwolf501.top/gtacfcimsn.html

Java: s.indexOf("x")
来源：http://hz.hongshengwenyu.top/gtqmonkmpn.html

Go:   strings.Index(s, "x")
来源：http://hz.birdmap.top/gtjizhnlde.html

Ruby: s.index("x")
来源：http://hz.yj20258.top/gtwyhzuwhy.html

C#:   s.IndexOf("x")
来源：http://hz.gzhubu.top/gtyfaofmjp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yvedp.cn/gtvxfocxmq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.nanxuanxn.top/gtddkxfvra.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.cashguo.top/gthmakvemw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yuanzhike.top/gteigorzcx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.kuanghao11.cn/gtsprzbove.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.shanyushiyangtech.top/gtzatsidxx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.xuetiantiany.cn/gtannsgabb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.hongshengwenyu.top/gtwcijlohd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.kuanghao11.cn/gtpsimoyoi.html

[E06] 替换子串
来源：http://hz.nanxinkj.top/gthtbrlqgb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.hywenlv.cn/gtdutxyidz.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.nanxinkj.top/gtivktndgk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.zycfv.cn/gtaaksbbke.html

TS:   s.replaceAll("a", "b")
来源：http://hz.mhx1999.top/gtbyqltffn.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.guannengcc.top/gtrhfsnwpv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.zdqjudy.top/gtvcqkojkg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.yvedp.cn/gtnhfnvrqn.html

C#:   s.Replace("a", "b")
来源：http://hz.wangshuangyany.cn/gtedodpddq.html

[E07] 按分隔符拆分
来源：http://hz.jlsjyb.cn/gtyjfgnoxw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.iojbl.cn/gtjcoalpcn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.iojbl.cn/gteafuygww.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.wangdashe.top/gtvbmgnxzq.html

TS:   s.split(",")
来源：http://hz.hfpthk.cn/gtmralccbe.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.svipenyu.cn/gtlmakovgw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.yuanzhike.top/gtcvlbuikm.html

Ruby: s.split(",");  s.split
来源：http://hz.hnqzz.top/gtdarpjcwz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.ybcxt.top/gtcvframev.html

[E08] 数组按分隔符合并
来源：http://hz.yuanzhike.top/gtkvzhcbnh.html

Py:   ",".join(items)
来源：http://hz.redwolf501.top/gtzyidimxi.html

PHP:  implode(",", $items);
来源：http://hz.meibo888.top/gtqoealfxd.html

JS:   items.join(",")
来源：http://hz.chenlongwang.top/gtgkdycmxz.html

TS:   items.join(",")
来源：http://hz.yuxming.cn/gtaceqlaeb.html

Java: String.join(",", items)
来源：http://hz.daria6918.cn/gtltcmvcmj.html

Go:   strings.Join(items, ",")
来源：http://hz.hysaishi.cn/gtnzokybhd.html

Ruby: items.join(",")
来源：http://hz.wangshuangyany.cn/gtjdysirnq.html

C#:   string.Join(",", items)
来源：http://hz.ydjk.org.cn/gtybsyndnu.html

[E09] 去除所有空白字符
来源：http://hz.svipenyu.cn/gtrsgnmokq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.pengpengdd.cyou/gtvqqjigme.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.andypj.xyz/gtwoaneumt.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.bjfxy.top/gtuhtmmdbk.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.jinqigufen.top/gtxzzdcuer.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.zycfv.cn/gtrbijddgd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.zdqjudy.top/gtlvzmivjj.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.xziqi.cn/gtuydhnsqb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yueranfly.top/gtxsxpzfws.html

[E10] 左侧补零 / 定长填充
来源：http://hz.hysaishi.cn/gtvjaiofxy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yangfankeji.com/gtsklzyqva.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.hnqzz.top/gtrrhqfvjd.html

JS:   "7".padStart(3, "0")
来源：http://hz.zycfv.cn/gtcrxtldkf.html

TS:   "7".padStart(3, "0")
来源：http://hz.smart0.xyz/gtplnhjoue.html

Java: String.format("%03d", 7)
来源：http://hz.daria6918.cn/gtfmqbomnd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yvedp.cn/gtqnxxayye.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.pengpengdd.cyou/gtojnuoalz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.gotoacloud.top/gtqqwmxzan.html

[E11] 反转字符串
来源：http://hz.nanxinkj.top/gtbaouioan.html

Py:   s[::-1]
来源：http://hz.jqgufenzy.top/gtzvdjwpms.html

PHP:  strrev($s);
来源：http://hz.hongshengwenyu.top/gtckmtwqqj.html

JS:   [...s].reverse().join("")
来源：http://hz.hammf.cn/gtpgfhhdgm.html

TS:   [...s].reverse().join("")
来源：http://hz.svipenyu.cn/gtadrqscil.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.fengsongda.top/gtrwmyscyb.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.ppjwa.cn/gtgoslgqis.html

Ruby: s.reverse
来源：http://hz.birdmap.top/gtnwilqoeg.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.hysaishi.cn/gtkvakkcgf.html

[E12] 统计某字符出现次数
来源：http://hz.zhongyouzk.top/gtivxbdiax.html

Py:   s.count("a")
来源：http://hz.zycfv.cn/gtmtwmoiok.html

PHP:  substr_count($s, "a");
来源：http://hz.jianghu66.top/gtequgdmzu.html

JS:   s.split("a").length - 1
来源：http://hz.chenjidiqi.icu/gtmhkkhbun.html

TS:   s.split("a").length - 1
来源：http://hz.kuanghao11.cn/gtfcdweksq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.ydzc1.top/gtrfkuwtam.html

Go:   strings.Count(s, "a")
来源：http://hz.zycfv.cn/gtiwprelge.html

Ruby: s.count("a")
来源：http://hz.ybcxt.top/gtgqfpzqry.html

C#:   s.Count(c => c == 'a')
来源：http://hz.feifeiyinyue.top/gteuvqymez.html

[E13] 逐字符遍历
来源：http://hz.zhoulong.xyz/gtgfgagyit.html

Py:   for ch in s: print(ch)
来源：http://hz.jianghu66.top/gtzhzklbnw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zhiwuduotai.top/gtcnbsigqf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xziqi.cn/gtxuabmlua.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yanxiufei.cn/gtkldpouyr.html


<!-- 参考信息 -->