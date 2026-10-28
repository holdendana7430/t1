代发 wailian999

PHP:  $arr[0]; end($arr); $arr[0] = 9;
来源：http://hz.hnxiangtu.top/gtbrkokpot.html

JS:   arr[0]; arr.at(-1); arr[0] = 9;
来源：http://hz.yuanzhike.top/gtvqxavice.html

TS:   arr[0]; arr.at(-1);
来源：http://hz.hammf.cn/gtlxbgzeew.html

Java: list.get(0); list.set(0, 9);
来源：http://hz.tianlin.xyz/gtfskqcvwq.html

Go:   arr[0]; arr[0] = 9
来源：http://hz.gaohongyu789.top/gtqwbfhpbi.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.yongpay.top/gtlvwcxzmm.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.sxryk.cn/gtrdzrvlzf.html

[D06] 数组长度
来源：http://hz.yonumen.top/gtjqmgmfcl.html

Py:   len(arr)
来源：http://hz.smart0.xyz/gtogmkzyax.html

PHP:  count($arr);
来源：http://hz.hfpthk.cn/gtxjfsgmny.html

JS:   arr.length
来源：http://hz.chenjidiqi.icu/gtfkrixead.html

TS:   arr.length
来源：http://hz.yj20258888.top/gthyfcldrm.html

Java: list.size();
来源：http://hz.shanyushiyangtech.top/gtahnoydyd.html

Go:   len(arr)
来源：http://hz.jianghu66.top/gtfgdkveqy.html

Ruby: arr.length; arr.size
来源：http://hz.xylfe.cn/gtbgjpkool.html

C#:   list.Count;
来源：http://hz.gogol.net.cn/gtznqgvrvl.html

[D07] 切片 / 取子数组
来源：http://hz.yuxming.cn/gtkcmhogil.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.birdmap.top/gtatxabnnr.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.redwolf501.top/gtacjhdgga.html

JS:   arr.slice(1, 4);
来源：http://hz.ybcxt.top/gtstrqxuym.html

TS:   arr.slice(1, 4);
来源：http://hz.xuanzx.com/gtagjuznjx.html

Java: list.subList(1, 4);
来源：http://hz.ehwqpu.com/gtruarvdxj.html

Go:   arr[1:4]
来源：http://hz.yvedp.cn/gtimdwytur.html

Ruby: arr[1, 3]
来源：http://hz.ivvv.top/gtesnyhvrr.html

C#:   list.GetRange(1, 3);
来源：http://hz.vqdsnc.cn/gtlhznqxbi.html

[D08] 合并两个数组
来源：http://hz.tanke756.top/gthwbnjoql.html

Py:   a + b;  a.extend(b)
来源：http://hz.smart0.xyz/gtchyympxh.html

PHP:  array_merge($a, $b);
来源：http://hz.hfpthk.cn/gtxtfclhkh.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.dianchejie.cn/gtefwlnbjr.html

TS:   [...a, ...b];
来源：http://hz.xuetiantiany.cn/gtwvljkgun.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.jlsjyb.cn/gthoxabgde.html

Go:   append(a, b...)
来源：http://hz.sysykeji.top/gthazrdtfu.html

Ruby: a + b;  a.concat(b)
来源：http://hz.yuxming.cn/gtaiqugnyi.html

C#:   a.Concat(b).ToList()
来源：http://hz.nwbrower.top/gtnussdqfw.html

[D09] 排序（升序）
来源：http://hz.kuanghao11.cn/gtjwfbjtxz.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.fengsongda.top/gtfyhepetn.html

PHP:  sort($arr);
来源：http://hz.kuanghao11.cn/gtrqajyoqu.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.shuidangran.top/gtotofcqik.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.xylfe.cn/gtilubixrb.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.zhiwuduotai.top/gtbbjxjzwv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.quarkkingdee.top/gterdjtkev.html

Ruby: arr.sort
来源：http://hz.bjfxy.top/gtnaltwhqv.html

C#:   list.Sort();
来源：http://hz.jianghu66.top/gtdpgztvki.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.zhiwuduotai.top/gtqisezgcz.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.zhiwuduotai.top/gtasbsecbm.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.cqqwz.cn/gtlalvgvpf.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xziqi.cn/gtxhnnlwhf.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.sxryk.cn/gtjzlhsvxm.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.c1oappe.top/gtaflgfwes.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jlsjyb.cn/gtppcnzfgs.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.meibo888.top/gtqvfaiypt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jlsjyb.cn/gtfztmxnqb.html

[D11] 反转数组
来源：http://hz.dianchejie.cn/gthdmiwzao.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.nwbrower.top/gtwkglmamf.html

PHP:  array_reverse($arr);
来源：http://hz.cheryme.top/gtdzymfcji.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.ydjk.org.cn/gtfjcameol.html

TS:   [...arr].reverse();
来源：http://hz.sufxvd.cn/gtyjiehitn.html

Java: Collections.reverse(list);
来源：http://hz.jianghu66.top/gtmxhoiiav.html

Go:   slices.Reverse(arr)
来源：http://hz.shanyushiyangtech.top/gtkugevkke.html

Ruby: arr.reverse
来源：http://hz.yonumen.top/gtmnuccnva.html

C#:   list.Reverse();
来源：http://hz.ydjk.org.cn/gtmocyrwef.html

[D12] 查找元素下标
来源：http://hz.chenzaomai.com/gtfmprqviu.html

Py:   arr.index(x);  x in arr
来源：http://hz.yj202588.top/gtnsexkzpa.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.fzhhl.top/gtsdcvdlax.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.wangshuangyany.cn/gtxlkuioao.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.gaohongyu789.top/gtfmwchtyk.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.snrcjt.cn/gtatjfbybg.html

Go:   slices.Index(arr, x)
来源：http://hz.gotoacloud.top/gtamymikws.html

Ruby: arr.index(x)
来源：http://hz.xinyue.icu/gtuzooornz.html

C#:   list.IndexOf(x);
来源：http://hz.sxryk.cn/gtcdvenotu.html

[D13] 过滤（保留满足条件的）
来源：http://hz.tian-w.cn/gtbyjczkls.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.snrcjt.cn/gtxeszfiyf.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.cucudq.cn/gtmkgwnssg.html

JS:   arr.filter(x => x > 3)
来源：http://hz.nanxuanxn.top/gtarhqiami.html

TS:   arr.filter(x => x > 3)
来源：http://hz.zdqjudy.top/gtplhqzrss.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.redwolf501.top/gtuewrarba.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.pengpengdd.cyou/gtiimxfjyf.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.dianchejie.cn/gtbnqkbcfq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.cdnleiting.top/gtrocuolxe.html

[D14] 映射转换（每个元素变形）
来源：http://hz.316326.xyz/gtxpjzcbji.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.bjfxy.top/gtslprruzq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.gogol.net.cn/gtzhivhjpy.html

JS:   arr.map(x => x * 2)
来源：http://hz.zhongyouzk.top/gtcxzlnpit.html

TS:   arr.map(x => x * 2)
来源：http://hz.zdqjudy.top/gtozfdypqj.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jlsjyb.cn/gtdvyeagna.html

Go:   // 手写循环
来源：http://hz.hnqzz.top/gtqstorfvd.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.bjfxy.top/gtsoldetfo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.sufxvd.cn/gtuzipewxz.html

[D15] 去重
来源：http://hz.sysykeji.top/gtjssgxrwo.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.cdnleiting.top/gttldevucw.html

PHP:  array_unique($arr);
来源：http://hz.jianghu66.top/gtxznnudps.html

JS:   [...new Set(arr)]
来源：http://hz.nwbrower.top/gtlhdqkwkh.html

TS:   [...new Set(arr)]
来源：http://hz.ppjwa.cn/gtlbdwegqd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.zycfv.cn/gtmhhnedhx.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.ehwqpu.com/gtharsqnbt.html

Ruby: arr.uniq
来源：http://hz.yueranfly.top/gtfulvnykb.html

C#:   list.Distinct().ToList()
来源：http://hz.chenjidiqi.icu/gtwutbkesj.html

[D16] 求和与平均值
来源：http://hz.yj20258888.top/gttbfmpyht.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.aizwys.cn/gtlrcaoqff.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.hfpthk.cn/gtbjoygmhz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.c1oappe.top/gtpiovqnuh.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.hywenlv.cn/gtseypzztf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.zhoulong.xyz/gtvkvrlowz.html

Go:   // 手写循环累加
来源：http://hz.kuanghao11.cn/gtmlgsrtwy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhongyouzk.top/gtevpmyvar.html

C#:   list.Sum();  list.Average()
来源：http://hz.kuanghao11.cn/gtzuydgalb.html

[D17] 最大值与最小值
来源：http://hz.daria6918.cn/gtnakomskw.html

Py:   max(arr);  min(arr)
来源：http://hz.zycfv.cn/gtbgjqukhk.html

PHP:  max($arr);  min($arr);
来源：http://hz.nanxuanxn.top/gtwzeoyesp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yuanzhike.top/gtaayuorot.html

TS:   Math.max(...arr);
来源：http://hz.zycfv.cn/gtasnnonrr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zhongyouzk.top/gtnvwhbess.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.52xcode.cn/gtngbwlcmh.html

Ruby: arr.max;  arr.min
来源：http://hz.hammf.cn/gtoxtlnvph.html

C#:   list.Max();  list.Min()
来源：http://hz.jqgufenzy.top/gtvdnyozir.html

[D18] 扁平化嵌套数组
来源：http://hz.yongpay.top/gtxdcubhug.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.nanxinkj.top/gtzauqrqyz.html

PHP:  array_merge(...$nested);
来源：http://hz.xziqi.cn/gtfnxgzpvy.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yangfankeji.com/gtcrxdragk.html

TS:   nested.flat();
来源：http://hz.zhoulong.xyz/gtnlvcobvr.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.yangfankeji.com/gtvcdvrogm.html

Go:   // 手写双层循环
来源：http://hz.yuanzhike.top/gteabfnjzu.html

Ruby: nested.flatten
来源：http://hz.sysykeji.top/gtjarxfhaw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.zhijiandao.cn/gtbendtycf.html

[D19] 按字段分组
来源：http://hz.andypj.xyz/gtwraoseeo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.tianlin.xyz/gtbjjxqmke.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.ivvv.top/gtcjydhfes.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.guowangkeji.top/gtvpsvsqfp.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.cucudq.cn/gtxgqyfckh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.zhongyouzk.top/gtqycfgdge.html

Go:   // 手写 map[string][]T
来源：http://hz.xziqi.cn/gtzukynaey.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.xziqi.cn/gtfenxwnrr.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.vqdsnc.cn/gtgmciviif.html

[D20] 统计每个元素出现次数
来源：http://hz.jinyuanbaomall.cn/gtmitccfid.html

Py:   Counter(arr)
来源：http://hz.pengpengdd.cyou/gtpcfhcczo.html

PHP:  array_count_values($arr);
来源：http://hz.daria6918.cn/gttmkoempx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.fengsongda.top/gtqpdnyngu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ppjwa.cn/gtajmfllvm.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ehwqpu.com/gtlmmmovsq.html

Go:   // 手写 map[T]int
来源：http://hz.quarkkingdee.top/gttjqhxxjn.html

Ruby: arr.tally
来源：http://hz.gzhubu.top/gtrkvjzxks.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.ydzc1.top/gtriybsflq.html

[D21] 判断是否包含某元素
来源：http://hz.birdmap.top/gtbxldgnpb.html

Py:   x in arr
来源：http://hz.cucudq.cn/gtqpzllwsa.html

PHP:  in_array($x, $arr, true);
来源：http://hz.cucudq.cn/gtplwbfrie.html

JS:   arr.includes(x)
来源：http://hz.hysaishi.cn/gttwnyjlkc.html

TS:   arr.includes(x)
来源：http://hz.pycfn.com/gtyehkmwil.html

Java: list.contains(x)
来源：http://hz.daxiang520.top/gtuurdqtih.html

Go:   slices.Contains(arr, x)
来源：http://hz.cqqwz.cn/gtltdyvcgt.html

Ruby: arr.include?(x)
来源：http://hz.sweek.top/gteqwqkogi.html

C#:   list.Contains(x)
来源：http://hz.zhaomingkeji.xyz/gtajctssdv.html

[D22] 复制数组（避免共享引用）
来源：http://hz.tian-w.cn/gtuqcepifa.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.cucudq.cn/gtlmbwsbod.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yueranfly.top/gtbhybloak.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yonumen.top/gtppclqzmz.html

TS:   [...arr];
来源：http://hz.gaohongyu789.top/gtzwxoduii.html

Java: new ArrayList<>(list);
来源：http://hz.sufxvd.cn/gtmhabliay.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.shanyushiyangtech.top/gtwjgummfc.html

Ruby: arr.dup;  arr.clone
来源：http://hz.snrcjt.cn/gtiexjmszk.html

C#:   new List<int>(list);
来源：http://hz.yuanzhike.top/gtihtiilhl.html

[D23] reduce 累积计算
来源：http://hz.kuanghao11.cn/gtbfbapukd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.jinyuanbaomall.cn/gtnhgyidbw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.hfpthk.cn/gtqfxgofom.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.nwbrower.top/gtcoeuzdcu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinghuilouyu.cn/gtdjbvrtqv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jinqigufen.top/gtglttykop.html

Go:   // 手写循环
来源：http://hz.jianghu66.top/gtmrlqkglw.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.cucudq.cn/gtlbtxxqcq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.hammf.cn/gtrzlxgdtz.html

[D24] 字典 / Map 基本操作
来源：http://hz.yueranfly.top/gtelnpmoqs.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.xuanzx.com/gtwgfafkgm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.fzhhl.top/gtftnuahsq.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.316326.xyz/gtkrxvprpu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.nwbrower.top/gtmwmireyu.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jinghuilouyu.cn/gtoygmkhwz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.chenzaomai.com/gtuckjbbze.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.guowangkeji.top/gtwmmqkxle.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.cqqwz.cn/gtmnilvuui.html

[D25] Set 集合去重与交并差
来源：http://hz.ydzc1.top/gtcemlyacl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.zdqjudy.top/gtsgtmrumi.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.cashguo.top/gtvnrrfsmc.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.guowangkeji.top/gttlsqbaea.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.andypj.xyz/gtkamzbizr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.zhengqikj.top/gtjuoajdad.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.snrcjt.cn/gthtwughoo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.zhoulong.xyz/gtyzisgvkq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yuanzhike.top/gtutgscgoo.html

[D26] 数组转字符串
来源：http://hz.hfpthk.cn/gtjbhbxudr.html

Py:   ", ".join(map(str, arr))
来源：http://hz.jianghu66.top/gtvekzigva.html

PHP:  implode(", ", $arr);
来源：http://hz.gzhubu.top/gtdeqsnyns.html

JS:   arr.join(", ")
来源：http://hz.zhoulong.xyz/gtkndlyrdu.html

TS:   arr.join(", ")
来源：http://hz.tian-w.cn/gtwyzgwgko.html

Java: String.join(", ", list)
来源：http://hz.tianlin.xyz/gtxiguwkkc.html

Go:   strings.Join(strs, ", ")
来源：http://hz.guowangkeji.top/gtpgczexdw.html

Ruby: arr.join(", ")
来源：http://hz.bjfxy.top/gtkwylvdfa.html

C#:   string.Join(", ", list)
来源：http://hz.c1oappe.top/gthxxqiyce.html

================================================================================
来源：http://hz.shanyushiyangtech.top/gtkeunhkrj.html

E. 字符串处理
来源：http://hz.cheryme.top/gtqgqarhuz.html

================================================================================
来源：http://hz.dashuyun.cn/gtxhssghxm.html

[E01] 拼接字符串
来源：http://hz.jinqigufen.top/gtiyihxvzd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yj20258888.top/gtapomchnb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.chenzaomai.com/gtjpjwjwxp.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.guannengcc.top/gtpkwkvjgp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.fengsongda.top/gtyhptjeia.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.tian-w.cn/gtujfgtuhv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.cqqwz.cn/gtslmfzgcm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.sxryk.cn/gturjhojpd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.jinqigfzy.top/gtzrmotpyg.html

[E02] 重复字符串
来源：http://hz.guowangkeji.top/gtdmeiierz.html

Py:   "ab" * 3
来源：http://hz.fzhhl.top/gtrekpzjbp.html

PHP:  str_repeat("ab", 3);
来源：http://hz.vqdsnc.cn/gtefzvbevp.html

JS:   "ab".repeat(3)
来源：http://hz.zhoulong.xyz/gtwhppowhe.html

TS:   "ab".repeat(3)
来源：http://hz.xingfuxueyuan.xyz/gttctssijp.html

Java: "ab".repeat(3)
来源：http://hz.vqdsnc.cn/gtufqkqkqu.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.nanxuanxn.top/gtjknbnjlu.html

Ruby: "ab" * 3
来源：http://hz.xuetiantiany.cn/gtazuugoep.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.yvedp.cn/gtrrgtwuyq.html

[E03] 截取子串
来源：http://hz.fzhhl.top/gtduimyjdk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jinqigfzy.top/gtvjwylmbs.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.jyoumei.cn/gtzaxtsuir.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.gaohongyu789.top/gtqoavwwkk.html

TS:   s.slice(1, 4)
来源：http://hz.yvedp.cn/gtdsnpdbas.html

Java: s.substring(1, 4)
来源：http://hz.jinyuanbaomall.cn/gtmwogywqf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.snrcjt.cn/gthaxhzazl.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.jinghuilouyu.cn/gtlhiryiqq.html

C#:   s.Substring(1, 3)
来源：http://hz.havefunace.top/gtjganvthh.html

[E04] 查找子串位置
来源：http://hz.zhiwuduotai.top/gtbllahvqi.html

Py:   s.find("x");  s.index("x")
来源：http://hz.cdnleiting.top/gtchznaebg.html

PHP:  strpos($s, "x");
来源：http://hz.yongpay.top/gthathfjan.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.52xcode.cn/gttckmrriw.html

TS:   s.indexOf("x")
来源：http://hz.gzhubu.top/gtshdedvgy.html

Java: s.indexOf("x")
来源：http://hz.fengsongda.top/gtwnojqqtm.html

Go:   strings.Index(s, "x")
来源：http://hz.cqqwz.cn/gttszlhrgk.html

Ruby: s.index("x")
来源：http://hz.ywan-chungtsiang.top/gtbzwifibw.html

C#:   s.IndexOf("x")
来源：http://hz.ywan-chungtsiang.top/gthtlxqkna.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.jinqigfzy.top/gtdfqdlnkl.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yj20258.top/gtdwssvpxn.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.xylfe.cn/gtluioxzri.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.meibo888.top/gtisjilgam.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.shuidangran.top/gtzfnhizqu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yj20258888.top/gtdzeepsjp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.redwolf501.top/gtlidxmjnp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.xingfuxueyuan.xyz/gtyaxqylis.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.ivvv.top/gtirjzldpz.html

[E06] 替换子串
来源：http://hz.yonumen.top/gtrcxsgzlu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jiagoushi.top/gtngsapxzx.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.gogol.net.cn/gtjthuxsmj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.sysykeji.top/gtdlwlcsxi.html

TS:   s.replaceAll("a", "b")
来源：http://hz.cheryme.top/gtynedczcm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yongpay.top/gtpghbtkjo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.shuidangran.top/gtuknnngez.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.daria6918.cn/gtnvqtshxx.html

C#:   s.Replace("a", "b")
来源：http://hz.havefunace.top/gtgipbdwku.html

[E07] 按分隔符拆分
来源：http://hz.shanyushiyangkeji.top/gtxszbdgbm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yanxiufei.cn/gtmmaklmba.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.jinghuilouyu.cn/gtwbyzafum.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.bjfxy.top/gtgqebivsi.html

TS:   s.split(",")
来源：http://hz.tianlin.xyz/gtkuufcjwo.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.nanxuanxn.top/gtdecyzskp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.daria6918.cn/gtloepedow.html

Ruby: s.split(",");  s.split
来源：http://hz.meibo888.top/gturmwansu.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.andypj.xyz/gttkuygjkv.html

[E08] 数组按分隔符合并
来源：http://hz.nwbrower.top/gtjcehwemv.html

Py:   ",".join(items)
来源：http://hz.svipenyu.cn/gtqnqtsjmz.html

PHP:  implode(",", $items);
来源：http://hz.mhx1999.top/gtmuzvlfol.html

JS:   items.join(",")
来源：http://hz.cucudq.cn/gtcahhqxxz.html

TS:   items.join(",")
来源：http://hz.pycfn.com/gtafwfcswk.html

Java: String.join(",", items)
来源：http://hz.andypj.xyz/gtmsmfiuhb.html

Go:   strings.Join(items, ",")
来源：http://hz.chenlongwang.top/gtfmutcvuo.html

Ruby: items.join(",")
来源：http://hz.hnxiangtu.top/gtizmcterk.html

C#:   string.Join(",", items)
来源：http://hz.316326.xyz/gtlsjnviie.html

[E09] 去除所有空白字符
来源：http://hz.sysykeji.top/gtslowaeru.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zhijiandao.cn/gtsndeeniu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.redwolf501.top/gtqrnubvqc.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.ivvv.top/gtlpewirxp.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.fengsongda.top/gtdgmfashw.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.ywan-chungtsiang.top/gtqamhyorr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.cheryme.top/gtcbxsxudv.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.feifeiyinyue.top/gtfzlsmfmv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jinqigufen.top/gtjolbvxiu.html

[E10] 左侧补零 / 定长填充
来源：http://hz.hnxiangtu.top/gtdpgttmck.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.yj202588.top/gtpiccduhp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.bjfxy.top/gtlouqizdx.html

JS:   "7".padStart(3, "0")
来源：http://hz.cheryme.top/gtwtjkoela.html

TS:   "7".padStart(3, "0")
来源：http://hz.redwolf501.top/gtjqwszbtc.html

Java: String.format("%03d", 7)
来源：http://hz.quarkkingdee.top/gtjixbzazl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.chenzaomai.com/gtzegaotmu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yuanzhike.top/gtakqbhbli.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.nanxuanxn.top/gtqzdtrugx.html

[E11] 反转字符串
来源：http://hz.yj20258.top/gtemlncegt.html

Py:   s[::-1]
来源：http://hz.sufxvd.cn/gtxaifsurl.html

PHP:  strrev($s);
来源：http://hz.fengsongda.top/gtbnjxyonj.html

JS:   [...s].reverse().join("")
来源：http://hz.yj202588.top/gtkyjrneuh.html

TS:   [...s].reverse().join("")
来源：http://hz.fzhhl.top/gthodbdsyy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jinqigufen.top/gtcxoyzhqn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.316326.xyz/gtmgwbvovm.html

Ruby: s.reverse
来源：http://hz.guannengcc.top/gtgqfiodbx.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.hysaishi.cn/gtoehgirin.html

[E12] 统计某字符出现次数
来源：http://hz.jinqigufen.top/gtmhcvsumt.html

Py:   s.count("a")
来源：http://hz.cdnleiting.top/gtcbfsnkht.html


<!-- 参考信息 -->