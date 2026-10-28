代发 wailian999

C#:   list.Insert(0, 0);
来源：http://hz.yuxming.cn/gtwnfshmnf.html

[D04] 删除元素
来源：http://hz.zhaomingkeji.xyz/gtytrxcxrr.html

Py:   del arr[0]; arr.pop(); arr.remove(3)
来源：http://hz.hywenlv.cn/gtvohvglzb.html

PHP:  array_splice($arr, 0, 1); array_pop($arr);
来源：http://hz.jyoumei.cn/gtayttpsao.html

JS:   arr.splice(0, 1); arr.pop(); arr.shift();
来源：http://hz.yuanzhike.top/gteivxefrx.html

TS:   arr.splice(0, 1);
来源：http://hz.9152youxi.cn/gttdsqxvkf.html

Java: list.remove(0); list.removeIf(x -> x == 3);
来源：http://hz.sweek.top/gtwrsrskaf.html

Go:   arr = append(arr[:0], arr[1:]...)
来源：http://hz.shanyushiyangkeji.top/gtwchndpjg.html

Ruby: arr.delete_at(0); arr.delete(3)
来源：http://hz.tianlin.xyz/gtzttbfbmb.html

C#:   list.RemoveAt(0); list.Remove(3);
来源：http://hz.nanxuanxn.top/gtxliiktpd.html

[D05] 访问与修改元素
来源：http://hz.jinqigfzy.top/gtbgyushdu.html

Py:   arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.9152youxi.cn/gtbyizuyqn.html

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.chenlongwang.top/gtlqtbxzfa.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.sweek.top/gtmhuirpqo.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.mhx1999.top/gtcqvhntze.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.daria6918.cn/gtecvydfpc.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.hongshengwenyu.top/gtjcnvwkag.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.hywenlv.cn/gtrniqlakp.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.jqgfzy.top/gtpatudrtx.html

[D06] 数组长度
来源：http://hz.zdqjudy.top/gtyjcqkpnc.html

Py:   len(arr)
来源：http://hz.meibo888.top/gtwwjiwlls.html

PHP:  count($arr);
来源：http://hz.aizwys.cn/gtfqayzzgi.html

JS:   arr.length
来源：http://hz.hysaishi.cn/gtgxjzuhpb.html

TS:   arr.length
来源：http://hz.yanxiufei.cn/gtfvlrknsd.html

Java: list.size();
来源：http://hz.hnxiangtu.top/gtxdecgajp.html

Go:   len(arr)
来源：http://hz.birdmap.top/gtuzhsaevr.html

Ruby: arr.length; arr.size
来源：http://hz.aizwys.cn/gtkmuhvufl.html

C#:   list.Count;
来源：http://hz.52xcode.cn/gtdgxkfiyt.html

[D07] 切片 / 取子数组
来源：http://hz.tian-w.cn/gtwmrdgfkz.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.ehwqpu.com/gtodsavtll.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.gzhubu.top/gttazzhqlp.html

JS:   arr.slice(1, 4);
来源：http://hz.snrcjt.cn/gtioflyhes.html

TS:   arr.slice(1, 4);
来源：http://hz.hywenlv.cn/gtifiwtnvm.html

Java: list.subList(1, 4);
来源：http://hz.daria6918.cn/gtmiwyoswr.html

Go:   arr[1:4]
来源：http://hz.redwolf501.top/gthiqgxujr.html

Ruby: arr[1, 3]
来源：http://hz.jqgufenzy.top/gtpyngbcdg.html

C#:   list.GetRange(1, 3);
来源：http://hz.aibaodan.cn/gtrxiwbnfq.html

[D08] 合并两个数组
来源：http://hz.xuanzx.com/gtrtygdcpf.html

Py:   a + b;  a.extend(b)
来源：http://hz.ppjwa.cn/gtwkmlwzwl.html

PHP:  array_merge($a, $b);
来源：http://hz.birdmap.top/gtgjepcdyw.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.xinyue.icu/gtvvmbyerw.html

TS:   [...a, ...b];
来源：http://hz.zhijiandao.cn/gtycpyqbav.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.zhixingplan.top/gtpzqrbrnf.html

Go:   append(a, b...)
来源：http://hz.ehwqpu.com/gtuscnkweh.html

Ruby: a + b;  a.concat(b)
来源：http://hz.xinyue.icu/gtntjhmzdt.html

C#:   a.Concat(b).ToList()
来源：http://hz.9152youxi.cn/gtoroaqhui.html

[D09] 排序（升序）
来源：http://hz.yueranfly.top/gtetbtregr.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.snrcjt.cn/gtwrdabqsy.html

PHP:  sort($arr);
来源：http://hz.zhongyouzk.top/gtdqpgqluh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.jqgfzy.top/gtuzloogtk.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.fengsongda.top/gtfwokmlet.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yanxiufei.cn/gttgpfogmd.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.cucudq.cn/gthhqpywdp.html

Ruby: arr.sort
来源：http://hz.ywan-chungtsiang.top/gtiaplizix.html

C#:   list.Sort();
来源：http://hz.tianlin.xyz/gttqizgizi.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.snrcjt.cn/gtzothntrr.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.gotoacloud.top/gtjvflodwn.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cucudq.cn/gtybedvhur.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.cdnleiting.top/gtenfedoja.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xziqi.cn/gtcgufsfpr.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.fengsongda.top/gtfdqtqfwk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.nanxuanxn.top/gtmhtofwwu.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.nanxinkj.top/gtpamzvtpp.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zhijiandao.cn/gtmdwclbvg.html

[D11] 反转数组
来源：http://hz.mhx1999.top/gtjehknpnj.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.jqgfzy.top/gtwoeatrlz.html

PHP:  array_reverse($arr);
来源：http://hz.hammf.cn/gthftnwzkq.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.redwolf501.top/gtogemisno.html

TS:   [...arr].reverse();
来源：http://hz.52xcode.cn/gtvekioywl.html

Java: Collections.reverse(list);
来源：http://hz.tanke756.top/gtzodnekns.html

Go:   slices.Reverse(arr)
来源：http://hz.xylfe.cn/gtbxcvysgg.html

Ruby: arr.reverse
来源：http://hz.9152youxi.cn/gtxzrucqlj.html

C#:   list.Reverse();
来源：http://hz.wangshuangyany.cn/gtbwthyfdt.html

[D12] 查找元素下标
来源：http://hz.sysykeji.top/gtscgobbop.html

Py:   arr.index(x);  x in arr
来源：http://hz.andypj.xyz/gturujyxqc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.smart0.xyz/gtwcobahac.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shuidangran.top/gtonoivmqx.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.nwbrower.top/gtcvaspsrl.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yongpay.top/gtotzeunic.html

Go:   slices.Index(arr, x)
来源：http://hz.zhongyouzk.top/gtprjguwly.html

Ruby: arr.index(x)
来源：http://hz.dashuyun.cn/gtiaurxpjk.html

C#:   list.IndexOf(x);
来源：http://hz.tanke756.top/gtuvafojqy.html

[D13] 过滤（保留满足条件的）
来源：http://hz.mhx1999.top/gtquspzbuv.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.meibo888.top/gthncsngkf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.sxryk.cn/gtfaxenhvn.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jianghu66.top/gtcnfywphe.html

TS:   arr.filter(x => x > 3)
来源：http://hz.c1oappe.top/gtvmpffjii.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.mhx1999.top/gtijemnevz.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.xziqi.cn/gtyiwgfetj.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.vqdsnc.cn/gterqnwxjz.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.hysaishi.cn/gttnmxaezu.html

[D14] 映射转换（每个元素变形）
来源：http://hz.chenzaomai.com/gtdtwvoiwj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.tanke756.top/gtislhdmcv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.hysaishi.cn/gtoflrazso.html

JS:   arr.map(x => x * 2)
来源：http://hz.yueranfly.top/gtezvhwwfd.html

TS:   arr.map(x => x * 2)
来源：http://hz.pycfn.com/gtgsbivqvz.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.sufxvd.cn/gtpvlrekjb.html

Go:   // 手写循环
来源：http://hz.shuidangran.top/gtfzvgckab.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.nwbrower.top/gtzltbjkfh.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.chenzaomai.com/gttpfxjrsw.html

[D15] 去重
来源：http://hz.birdmap.top/gtrbjnazze.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.chenjidiqi.icu/gtkkvajber.html

PHP:  array_unique($arr);
来源：http://hz.yonumen.top/gtbumcvtoi.html

JS:   [...new Set(arr)]
来源：http://hz.jyoumei.cn/gttzgswxnh.html

TS:   [...new Set(arr)]
来源：http://hz.sweek.top/gtzdoulbvz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.iojbl.cn/gtpcujmvse.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.52xcode.cn/gtsjizrdyq.html

Ruby: arr.uniq
来源：http://hz.dianchejie.cn/gtcfvnxgwc.html

C#:   list.Distinct().ToList()
来源：http://hz.hnxiangtu.top/gtnmctmznc.html

[D16] 求和与平均值
来源：http://hz.birdmap.top/gthlgaftbp.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jqgufenzy.top/gtpjyqdrcl.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.guannengcc.top/gtbrpkaapw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.pycfn.com/gtgmejlszm.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.dashuyun.cn/gtkvilavex.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.cqqwz.cn/gtptbjxjdb.html

Go:   // 手写循环累加
来源：http://hz.zhaomingkeji.xyz/gtuxbqtaph.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.ehwqpu.com/gtobmlefzm.html

C#:   list.Sum();  list.Average()
来源：http://hz.xylfe.cn/gtgsuaztaa.html

[D17] 最大值与最小值
来源：http://hz.cheryme.top/gtvgtcwcio.html

Py:   max(arr);  min(arr)
来源：http://hz.ywan-chungtsiang.top/gtclgafglh.html

PHP:  max($arr);  min($arr);
来源：http://hz.cucudq.cn/gtoyhxfwak.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yueranfly.top/gthlxfodqv.html

TS:   Math.max(...arr);
来源：http://hz.andypj.xyz/gtqvqbicjf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zdqjudy.top/gtlyhnhyky.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.0kj1m.cn/gttswzejif.html

Ruby: arr.max;  arr.min
来源：http://hz.ivvv.top/gtgunbmzie.html

C#:   list.Max();  list.Min()
来源：http://hz.zhijiandao.cn/gtunrwjsvs.html

[D18] 扁平化嵌套数组
来源：http://hz.9152youxi.cn/gtovjavukx.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.sysykeji.top/gtypwhrrdf.html

PHP:  array_merge(...$nested);
来源：http://hz.redwolf501.top/gtamyhyxhv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.xingfuxueyuan.xyz/gttszciofn.html

TS:   nested.flat();
来源：http://hz.zhongyouzk.top/gtaltwdzcf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.c1oappe.top/gtslfmqqeg.html

Go:   // 手写双层循环
来源：http://hz.zhaomingkeji.xyz/gtjgaltvxb.html

Ruby: nested.flatten
来源：http://hz.cashguo.top/gttygsqvvk.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.yanxiufei.cn/gtzskgohxa.html

[D19] 按字段分组
来源：http://hz.52xcode.cn/gtwujncmem.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.hammf.cn/gtlfhogfpv.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.yuxming.cn/gtzasjvbaa.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.aibaodan.cn/gtcajesrzk.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.haohaochexian.top/gteyouvifn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.jinqigufen.top/gtspsyxqph.html

Go:   // 手写 map[string][]T
来源：http://hz.pengpengdd.cyou/gttrcirbfn.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.zhongyouzk.top/gteytwqsez.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.cdnleiting.top/gttghglqtg.html

[D20] 统计每个元素出现次数
来源：http://hz.kuanghao11.cn/gtuqoqdptg.html

Py:   Counter(arr)
来源：http://hz.redwolf501.top/gtduxlwsiy.html

PHP:  array_count_values($arr);
来源：http://hz.guowangkeji.top/gtavjfmjny.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yj20258888.top/gtdribhnaj.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.dashuyun.cn/gtfoitcgmn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yj20258888.top/gtdhyzxtrj.html

Go:   // 手写 map[T]int
来源：http://hz.ywan-chungtsiang.top/gtqjnmlegk.html

Ruby: arr.tally
来源：http://hz.jyoumei.cn/gtdlmakbsq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.svipenyu.cn/gtnxzhzmwb.html

[D21] 判断是否包含某元素
来源：http://hz.chenlongwang.top/gtekohnmil.html

Py:   x in arr
来源：http://hz.iojbl.cn/gtwtbjrets.html

PHP:  in_array($x, $arr, true);
来源：http://hz.52xcode.cn/gtjxbtnzpl.html

JS:   arr.includes(x)
来源：http://hz.shanyushiyangkeji.top/gtoewfxryh.html

TS:   arr.includes(x)
来源：http://hz.sufxvd.cn/gtycfshqog.html

Java: list.contains(x)
来源：http://hz.ybcxt.top/gtlwihgxgz.html

Go:   slices.Contains(arr, x)
来源：http://hz.yj202588.top/gtifpjhwey.html

Ruby: arr.include?(x)
来源：http://hz.zhiwuduotai.top/gtapwnvscu.html

C#:   list.Contains(x)
来源：http://hz.hysaishi.cn/gtgnojqhah.html

[D22] 复制数组（避免共享引用）
来源：http://hz.gogol.net.cn/gtegagngis.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.feifeiyinyue.top/gtsprnebjd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.jqgfzy.top/gtpizuqgov.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.ppjwa.cn/gtfnmdjdox.html

TS:   [...arr];
来源：http://hz.yangfankeji.com/gtlhngnjdk.html

Java: new ArrayList<>(list);
来源：http://hz.smart0.xyz/gtymehjqkl.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.iojbl.cn/gtphxsbpnd.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yj20258.top/gtxmzrtffw.html

C#:   new List<int>(list);
来源：http://hz.c1oappe.top/gtvxzpsyti.html

[D23] reduce 累积计算
来源：http://hz.xuetiantiany.cn/gtldwwhfhl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.hnqzz.top/gthadujsgc.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.c1oappe.top/gtosuzulgk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinyuanbaomall.cn/gtbyvhhulj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yangfankeji.com/gtckcilkut.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.aibaodan.cn/gtnkhgfhtm.html

Go:   // 手写循环
来源：http://hz.jiagoushi.top/gtwrrmvcvy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.nanxuanxn.top/gtypkzfopa.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.jqgufenzy.top/gtpycxgcpi.html

[D24] 字典 / Map 基本操作
来源：http://hz.hfpthk.cn/gtyfwyaqnz.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.jyoumei.cn/gtedapxcye.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.tanke756.top/gtldmyfxwy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.shangyingyoupin.top/gtciqorxze.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.ydjk.org.cn/gtfqoizxvb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.ydjk.org.cn/gtyalbtaaj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.shanyushiyangtech.top/gttmrkisgf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.hfpthk.cn/gtbzoztdaw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.daria6918.cn/gtwwgctbtm.html

[D25] Set 集合去重与交并差
来源：http://hz.aibaodan.cn/gtufcmqecs.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.xziqi.cn/gtiuppfnas.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.hfpthk.cn/gtlwhosscg.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.snrcjt.cn/gtakrgxivr.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.yj20258888.top/gtrpiefxrm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.shanyushiyangtech.top/gtfcaqespx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.hnxiangtu.top/gtukwbwvre.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.mhx1999.top/gtnuxbqiyc.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yuxming.cn/gtwieixljw.html

[D26] 数组转字符串
来源：http://hz.ivvv.top/gtfcykcmbe.html

Py:   ", ".join(map(str, arr))
来源：http://hz.hfpthk.cn/gtosptiyay.html

PHP:  implode(", ", $arr);
来源：http://hz.zhiwuduotai.top/gtbelgspiw.html

JS:   arr.join(", ")
来源：http://hz.wangshuangyany.cn/gtwkdzhzej.html

TS:   arr.join(", ")
来源：http://hz.wangshuangyany.cn/gtqwrxzwrt.html

Java: String.join(", ", list)
来源：http://hz.mhx1999.top/gtvqnqwosq.html

Go:   strings.Join(strs, ", ")
来源：http://hz.hammf.cn/gtkuvjijiu.html

Ruby: arr.join(", ")
来源：http://hz.xuetiantiany.cn/gthpaugvcz.html

C#:   string.Join(", ", list)
来源：http://hz.zdqjudy.top/gtntbhtexz.html

================================================================================
来源：http://hz.fengsongda.top/gtysrychak.html

E. 字符串处理
来源：http://hz.kuanghao11.cn/gtaxjoffst.html

================================================================================
来源：http://hz.xuetiantiany.cn/gthrfnbihw.html

[E01] 拼接字符串
来源：http://hz.0kj1m.cn/gtnsdltpku.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.shanyushiyangtech.top/gtdltymjsc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.pycfn.com/gtboryhzvx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jyoumei.cn/gtiicgtswv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.birdmap.top/gtillprymr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.xziqi.cn/gtrmjpnjfj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.wangshuangyany.cn/gtcywkgmmr.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jiagoushi.top/gtbspetcik.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.tianlin.xyz/gtjwmgcchr.html

[E02] 重复字符串
来源：http://hz.zhaomingkeji.xyz/gtxvdqajfw.html

Py:   "ab" * 3
来源：http://hz.hysaishi.cn/gtwrniyirs.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jiagoushi.top/gtoslgapvb.html

JS:   "ab".repeat(3)
来源：http://hz.xuetiantiany.cn/gtioeiailb.html

TS:   "ab".repeat(3)
来源：http://hz.xuanzx.com/gtccolcuad.html

Java: "ab".repeat(3)
来源：http://hz.sufxvd.cn/gtbogsteac.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.yj20258.top/gtaychynsr.html

Ruby: "ab" * 3
来源：http://hz.ydjk.org.cn/gtqtomwufy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.shuidangran.top/gtspangmae.html

[E03] 截取子串
来源：http://hz.tianlin.xyz/gtfhevhupo.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.yj202588.top/gtoqypzfma.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.cdnleiting.top/gtqwqmkdbg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.tianlin.xyz/gtlwstqscq.html

TS:   s.slice(1, 4)
来源：http://hz.jinghuilouyu.cn/gtfbtvwnww.html

Java: s.substring(1, 4)
来源：http://hz.cdnleiting.top/gtrstsjwaf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.hnxiangtu.top/gtizefbhrv.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.zhongyouzk.top/gtfftesqcf.html

C#:   s.Substring(1, 3)
来源：http://hz.nanxuanxn.top/gtiennwtyo.html

[E04] 查找子串位置
来源：http://hz.wangdashe.top/gtbscwfxjk.html

Py:   s.find("x");  s.index("x")
来源：http://hz.ywan-chungtsiang.top/gtmibmngmw.html

PHP:  strpos($s, "x");
来源：http://hz.tian-w.cn/gtlwikltda.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zhixingplan.top/gthgvwerbt.html

TS:   s.indexOf("x")
来源：http://hz.dianchejie.cn/gtsndpkhfq.html

Java: s.indexOf("x")
来源：http://hz.guannengcc.top/gtvxrwjzhk.html

Go:   strings.Index(s, "x")
来源：http://hz.ppjwa.cn/gtjlecnwfr.html

Ruby: s.index("x")
来源：http://hz.sufxvd.cn/gtbsepkksy.html

C#:   s.IndexOf("x")
来源：http://hz.yangfankeji.com/gtcgrlavlh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.hfpthk.cn/gtufkuehmt.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.ppjwa.cn/gtqdtjihra.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.yj20258.top/gtjarprsgf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.wangdashe.top/gtowzrlkym.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.cucudq.cn/gtcroirslj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jianghu66.top/gthppkfzgm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.andypj.xyz/gtdaipprtq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.shanyushiyangtech.top/gtpihfycff.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.pengpengdd.cyou/gtgrbxoiaw.html

[E06] 替换子串
来源：http://hz.jlsjyb.cn/gtohwbousu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.zhiwuduotai.top/gtfvvrasbp.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.aibaodan.cn/gtmbpannop.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.meibo888.top/gtbocccimo.html

TS:   s.replaceAll("a", "b")
来源：http://hz.ehwqpu.com/gtsjgfnqge.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yvedp.cn/gtwlupkbkt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.nanxinkj.top/gtrymbpfsm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.shzxlz.cn/gtakczwayk.html

C#:   s.Replace("a", "b")
来源：http://hz.jianghu66.top/gtzurcdazt.html

[E07] 按分隔符拆分
来源：http://hz.hnqzz.top/gtuytgefvc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.guannengcc.top/gtckhkejad.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.nwbrower.top/gtrgkdvgtg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.zhiwuduotai.top/gthmbjdoid.html

TS:   s.split(",")
来源：http://hz.52xcode.cn/gtgfinywxx.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.ppjwa.cn/gtcvuzouat.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.kuanghao11.cn/gtihvqxsyu.html

Ruby: s.split(",");  s.split
来源：http://hz.shuidangran.top/gttupthuaf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.shzxlz.cn/gtxjxepwvp.html

[E08] 数组按分隔符合并
来源：http://hz.fzhhl.top/gtvsbjscul.html

Py:   ",".join(items)
来源：http://hz.sxryk.cn/gthsvhfcbg.html

PHP:  implode(",", $items);
来源：http://hz.yj20258888.top/gtgjymkoft.html

JS:   items.join(",")
来源：http://hz.fengsongda.top/gtppvmfegy.html

TS:   items.join(",")
来源：http://hz.jlsjyb.cn/gtpdidruzv.html

Java: String.join(",", items)
来源：http://hz.smart0.xyz/gtqrvepzza.html

Go:   strings.Join(items, ",")
来源：http://hz.jinqigufen.top/gtsotznedn.html

Ruby: items.join(",")
来源：http://hz.fzhhl.top/gttqyavcdt.html

C#:   string.Join(",", items)
来源：http://hz.yvedp.cn/gtaburxsol.html

[E09] 去除所有空白字符
来源：http://hz.zhongyouzk.top/gtnxuhidxn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.wangshuangyany.cn/gtcmtajbac.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zycfv.cn/gthjqqxvhn.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.sysykeji.top/gtrffcjjgt.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.yueranfly.top/gtlkwigtwt.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.havefunace.top/gttgdsjhnt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.xylfe.cn/gtkdiqodmx.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.cucudq.cn/gtzhfziwgg.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zhongyouzk.top/gtabtknuxe.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jinghuilouyu.cn/gtjfawphvs.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.jianghu66.top/gtcsdxplbt.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.52xcode.cn/gtzgfzhrko.html

JS:   "7".padStart(3, "0")
来源：http://hz.ehwqpu.com/gtbyxtovfg.html

TS:   "7".padStart(3, "0")
来源：http://hz.bjfxy.top/gtyuccamzr.html

Java: String.format("%03d", 7)
来源：http://hz.zhaomingkeji.xyz/gtisbtguto.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.svipenyu.cn/gtbatftuzk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yongpay.top/gthtdecixs.html


<!-- 参考信息 -->