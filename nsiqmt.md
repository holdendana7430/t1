代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://hz.jinyuanbaomall.cn/gtalfnwydj.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jiagoushi.top/gtrddnkthh.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.andypj.xyz/gtvwpqjiht.html

[D06] 数组长度
来源：http://hz.sweek.top/gtsycrrvei.html

Py:   len(arr)
来源：http://hz.nanxuanxn.top/gtrqensgjh.html

PHP:  count($arr);
来源：http://hz.zhongyouzk.top/gtezzwpgjo.html

JS:   arr.length
来源：http://hz.zycfv.cn/gtnhhpuqpv.html

TS:   arr.length
来源：http://hz.yanxiufei.cn/gtmcfzkjbx.html

Java: list.size();
来源：http://hz.chenlongwang.top/gtdwlqwuak.html

Go:   len(arr)
来源：http://hz.gotoacloud.top/gtmiyrlwmc.html

Ruby: arr.length; arr.size
来源：http://hz.guowangkeji.top/gtfzuffxpf.html

C#:   list.Count;
来源：http://hz.cdnleiting.top/gtbnwtmhui.html

[D07] 切片 / 取子数组
来源：http://hz.gogol.net.cn/gtftyrusup.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.haohaochexian.top/gtrynyllri.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.yangfankeji.com/gtxwecmlzg.html

JS:   arr.slice(1, 4);
来源：http://hz.smart0.xyz/gtgqjbkiin.html

TS:   arr.slice(1, 4);
来源：http://hz.sysykeji.top/gtjgiaboth.html

Java: list.subList(1, 4);
来源：http://hz.ppjwa.cn/gtqocunkrx.html

Go:   arr[1:4]
来源：http://hz.feifeiyinyue.top/gtigcljvqz.html

Ruby: arr[1, 3]
来源：http://hz.cqqwz.cn/gtxljucxyb.html

C#:   list.GetRange(1, 3);
来源：http://hz.xylfe.cn/gtncuvhinz.html

[D08] 合并两个数组
来源：http://hz.wangshuangyany.cn/gtruveawmr.html

Py:   a + b;  a.extend(b)
来源：http://hz.hammf.cn/gtivufelyg.html

PHP:  array_merge($a, $b);
来源：http://hz.yuanzhike.top/gtjjmhbtij.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.gogol.net.cn/gtmqilfsuc.html

TS:   [...a, ...b];
来源：http://hz.yongpay.top/gttklxxtbo.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.tanke756.top/gthukdmmqo.html

Go:   append(a, b...)
来源：http://hz.jqgufenzy.top/gtzgbhlbhh.html

Ruby: a + b;  a.concat(b)
来源：http://hz.svipenyu.cn/gtsdofbeqj.html

C#:   a.Concat(b).ToList()
来源：http://hz.wangdashe.top/gtphfibjek.html

[D09] 排序（升序）
来源：http://hz.cucudq.cn/gtictqnvkr.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.jlsjyb.cn/gtydnqnggj.html

PHP:  sort($arr);
来源：http://hz.zhongyouzk.top/gtwuyrrmzg.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.dianchejie.cn/gtubdxcfcb.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.daxiang520.top/gtdxxmutsg.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.mhx1999.top/gteidipghq.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yanxiufei.cn/gtbfzllhio.html

Ruby: arr.sort
来源：http://hz.hnqzz.top/gtlcdlawoz.html

C#:   list.Sort();
来源：http://hz.iojbl.cn/gtyjfjublo.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.xziqi.cn/gtzoqmmqly.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yangfankeji.com/gtfglxigtv.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.svipenyu.cn/gtpejohpow.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ywan-chungtsiang.top/gtpkbfubtp.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.zhoulong.xyz/gtojxmmffe.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.pycfn.com/gtetypusqy.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.kuanghao11.cn/gtgcozjztb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.hywenlv.cn/gttfmqnegt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.guowangkeji.top/gtceyayhfe.html

[D11] 反转数组
来源：http://hz.zycfv.cn/gtyaabrbxs.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.snrcjt.cn/gtopgycqkc.html

PHP:  array_reverse($arr);
来源：http://hz.yuanzhike.top/gtzzrvhrvr.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.gogol.net.cn/gtrfaudhua.html

TS:   [...arr].reverse();
来源：http://hz.xingfuxueyuan.xyz/gtgduxhwrv.html

Java: Collections.reverse(list);
来源：http://hz.yvedp.cn/gtackscuds.html

Go:   slices.Reverse(arr)
来源：http://hz.yuanzhike.top/gtayiabqao.html

Ruby: arr.reverse
来源：http://hz.gotoacloud.top/gtmtfewebx.html

C#:   list.Reverse();
来源：http://hz.guowangkeji.top/gtqggisucm.html

[D12] 查找元素下标
来源：http://hz.yueranfly.top/gtsggkxwti.html

Py:   arr.index(x);  x in arr
来源：http://hz.xuanzx.com/gtrlgkpkkg.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.fzhhl.top/gtmvbpkzuo.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.zhijiandao.cn/gtjffplmir.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ehwqpu.com/gtparkunkw.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.yj202588.top/gtjqbgdpcq.html

Go:   slices.Index(arr, x)
来源：http://hz.nwbrower.top/gtsijsecxd.html

Ruby: arr.index(x)
来源：http://hz.0kj1m.cn/gtkbnioguj.html

C#:   list.IndexOf(x);
来源：http://hz.jinqigufen.top/gtqeburscb.html

[D13] 过滤（保留满足条件的）
来源：http://hz.guowangkeji.top/gtbpjsldiz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.snrcjt.cn/gtpuwetvge.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.chenjidiqi.icu/gtolpzlmzp.html

JS:   arr.filter(x => x > 3)
来源：http://hz.fzhhl.top/gthxahegzt.html

TS:   arr.filter(x => x > 3)
来源：http://hz.jinqigfzy.top/gtgqlisnmj.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.ehwqpu.com/gtegkpqxgp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.jqgufenzy.top/gtuygmybmn.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.hnqzz.top/gtuwwpurfq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.zhaomingkeji.xyz/gtfmirapaf.html

[D14] 映射转换（每个元素变形）
来源：http://hz.yj20258.top/gtkxuokupj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.yj20258888.top/gtiwgatctn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.shzxlz.cn/gtjusdgjwq.html

JS:   arr.map(x => x * 2)
来源：http://hz.birdmap.top/gtneqnelzx.html

TS:   arr.map(x => x * 2)
来源：http://hz.xuanzx.com/gtjtjwknyd.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yonumen.top/gtnsmhcqgo.html

Go:   // 手写循环
来源：http://hz.hysaishi.cn/gtgelezwvq.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.52xcode.cn/gtprqughxe.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.svipenyu.cn/gtpkepkokj.html

[D15] 去重
来源：http://hz.gzhubu.top/gtfzfouhvq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yuanzhike.top/gtyymeiosp.html

PHP:  array_unique($arr);
来源：http://hz.bjfxy.top/gtjxshoxus.html

JS:   [...new Set(arr)]
来源：http://hz.gotoacloud.top/gtynocxpdj.html

TS:   [...new Set(arr)]
来源：http://hz.haohaochexian.top/gtetbpahlt.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.0kj1m.cn/gtatagpmdp.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yonumen.top/gtmckkxswk.html

Ruby: arr.uniq
来源：http://hz.316326.xyz/gtedtiqdtz.html

C#:   list.Distinct().ToList()
来源：http://hz.hnqzz.top/gtvmyeuulj.html

[D16] 求和与平均值
来源：http://hz.ydzc1.top/gtvklmdxjw.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.dashuyun.cn/gtglcnaqqc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.chenzaomai.com/gtwnuxzkjz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.bjfxy.top/gtvbvqfyos.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.nanxinkj.top/gtjtggxfgi.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.zycfv.cn/gtvvexxcnx.html

Go:   // 手写循环累加
来源：http://hz.jqgfzy.top/gtpsjadtwx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.jianghu66.top/gtjpgjccgf.html

C#:   list.Sum();  list.Average()
来源：http://hz.jqgfzy.top/gtimmlqnzw.html

[D17] 最大值与最小值
来源：http://hz.jianghu66.top/gthdktrlbz.html

Py:   max(arr);  min(arr)
来源：http://hz.meibo888.top/gtxqdowvye.html

PHP:  max($arr);  min($arr);
来源：http://hz.hfpthk.cn/gtarpsyvwk.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.tianlin.xyz/gteaogoksw.html

TS:   Math.max(...arr);
来源：http://hz.feifeiyinyue.top/gthdygesna.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.hysaishi.cn/gtgnlqdzaw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jlsjyb.cn/gtlgqopbgj.html

Ruby: arr.max;  arr.min
来源：http://hz.ehwqpu.com/gtkpwjnjos.html

C#:   list.Max();  list.Min()
来源：http://hz.jqgufenzy.top/gtqkrtvgkb.html

[D18] 扁平化嵌套数组
来源：http://hz.yueranfly.top/gtqjnrojhf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.cqqwz.cn/gtdnaplbaz.html

PHP:  array_merge(...$nested);
来源：http://hz.vqdsnc.cn/gtcagevbri.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.smart0.xyz/gtookcmbfi.html

TS:   nested.flat();
来源：http://hz.yangfankeji.com/gtncawqqcf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.kuanghao11.cn/gtsjhpjtbd.html

Go:   // 手写双层循环
来源：http://hz.iojbl.cn/gtxwocoxph.html

Ruby: nested.flatten
来源：http://hz.dashuyun.cn/gtztdeiptp.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.nanxinkj.top/gtrtibyufd.html

[D19] 按字段分组
来源：http://hz.jqgfzy.top/gtundshyxh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.hysaishi.cn/gtgzojkvsu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.guowangkeji.top/gtpifcqhia.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jinqigfzy.top/gtmdmgkllx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.c1oappe.top/gtobtkuewp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.smart0.xyz/gtcximpauk.html

Go:   // 手写 map[string][]T
来源：http://hz.shzxlz.cn/gtaffgpiaw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.gogol.net.cn/gtyxrenumw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.jinqigufen.top/gtbskygtlu.html

[D20] 统计每个元素出现次数
来源：http://hz.9152youxi.cn/gtpxkigten.html

Py:   Counter(arr)
来源：http://hz.wangshuangyany.cn/gtmawaxpoi.html

PHP:  array_count_values($arr);
来源：http://hz.sweek.top/gtuubpxvwq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.cashguo.top/gtzgafpukd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.0kj1m.cn/gtoaovjbfd.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.cucudq.cn/gtewdkakaf.html

Go:   // 手写 map[T]int
来源：http://hz.tian-w.cn/gtclbldxdp.html

Ruby: arr.tally
来源：http://hz.snrcjt.cn/gteybiepww.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.pycfn.com/gtgxnrzemc.html

[D21] 判断是否包含某元素
来源：http://hz.zhoulong.xyz/gtfhantpcn.html

Py:   x in arr
来源：http://hz.xylfe.cn/gttdyuyaml.html

PHP:  in_array($x, $arr, true);
来源：http://hz.zhongyouzk.top/gtonkcsokt.html

JS:   arr.includes(x)
来源：http://hz.hnxiangtu.top/gtxteidsep.html

TS:   arr.includes(x)
来源：http://hz.0kj1m.cn/gtyubdilgx.html

Java: list.contains(x)
来源：http://hz.zhaomingkeji.xyz/gtqpxylmtg.html

Go:   slices.Contains(arr, x)
来源：http://hz.zhixingplan.top/gtavhwaxnr.html

Ruby: arr.include?(x)
来源：http://hz.c1oappe.top/gtwtzypqtl.html

C#:   list.Contains(x)
来源：http://hz.c1oappe.top/gtgqswbcnk.html

[D22] 复制数组（避免共享引用）
来源：http://hz.tianlin.xyz/gtobyrwfjz.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.guowangkeji.top/gtxcyebbbd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.tianlin.xyz/gtosodnevd.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.gaohongyu789.top/gtuyggigsd.html

TS:   [...arr];
来源：http://hz.yuanzhike.top/gteuwjitst.html

Java: new ArrayList<>(list);
来源：http://hz.birdmap.top/gtumjuurbc.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jinghuilouyu.cn/gtxocqgord.html

Ruby: arr.dup;  arr.clone
来源：http://hz.nanxuanxn.top/gttzjzkans.html

C#:   new List<int>(list);
来源：http://hz.aibaodan.cn/gtvxwbsduc.html

[D23] reduce 累积计算
来源：http://hz.shuidangran.top/gtgyqpcffi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yangfankeji.com/gtshztfonr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.gzhubu.top/gtuufzndpv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.sufxvd.cn/gtbzvebuga.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.sweek.top/gtxgohtjbp.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.gotoacloud.top/gtvrrifvik.html

Go:   // 手写循环
来源：http://hz.zhengqikj.top/gtslapetzp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.zhengqikj.top/gtafpizpui.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.shanyushiyangkeji.top/gtviduzgwi.html

[D24] 字典 / Map 基本操作
来源：http://hz.chenlongwang.top/gtuxtqnnjj.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.meibo888.top/gthkkgenfb.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.yueranfly.top/gtunlccaxl.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.jinghuilouyu.cn/gtiiyezoze.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.vqdsnc.cn/gtqdwxxrzz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.ppjwa.cn/gtkdlajbtk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.jlsjyb.cn/gtadgospvn.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.nwbrower.top/gtwvffcrjg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.chenjidiqi.icu/gthsmfihml.html

[D25] Set 集合去重与交并差
来源：http://hz.xingfuxueyuan.xyz/gtohznoocl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.jqgfzy.top/gtrcfgpssu.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jqgufenzy.top/gtddhskzmw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.zhengqikj.top/gteirqeuux.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.gaohongyu789.top/gtazcptabs.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.daria6918.cn/gtcsafeeha.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.316326.xyz/gtsaoepfnz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.hysaishi.cn/gtobljoafb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.hfpthk.cn/gtfioqwmzr.html

[D26] 数组转字符串
来源：http://hz.birdmap.top/gtlkteggng.html

Py:   ", ".join(map(str, arr))
来源：http://hz.tianlin.xyz/gtdumhrbgf.html

PHP:  implode(", ", $arr);
来源：http://hz.gzhubu.top/gtsnjqczku.html

JS:   arr.join(", ")
来源：http://hz.ydzc1.top/gtrydvovge.html

TS:   arr.join(", ")
来源：http://hz.dianchejie.cn/gtlfwwefir.html

Java: String.join(", ", list)
来源：http://hz.daria6918.cn/gtvibcpywf.html

Go:   strings.Join(strs, ", ")
来源：http://hz.zhixingplan.top/gttlnijvku.html

Ruby: arr.join(", ")
来源：http://hz.52xcode.cn/gtbbznljuq.html

C#:   string.Join(", ", list)
来源：http://hz.havefunace.top/gtgtoqaylr.html

================================================================================
来源：http://hz.daxiang520.top/gtcwhrmapc.html

E. 字符串处理
来源：http://hz.pengpengdd.cyou/gtahgjtdmm.html

================================================================================
来源：http://hz.zhongyouzk.top/gtdnxxsbgh.html

[E01] 拼接字符串
来源：http://hz.jqgufenzy.top/gtrkppbuxu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.sufxvd.cn/gtnettqclb.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.jinyuanbaomall.cn/gtwxaplacr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.cashguo.top/gtyticabzf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.cheryme.top/gtjhtztwma.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.kuanghao11.cn/gtpfsdcbhc.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.gogol.net.cn/gtjzzdxgkq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.pycfn.com/gtspnfizsl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.xziqi.cn/gtwpohoopd.html

[E02] 重复字符串
来源：http://hz.fzhhl.top/gtuwnouksh.html

Py:   "ab" * 3
来源：http://hz.feifeiyinyue.top/gtpwlaqtff.html

PHP:  str_repeat("ab", 3);
来源：http://hz.pycfn.com/gtnnjetmsk.html

JS:   "ab".repeat(3)
来源：http://hz.hnxiangtu.top/gtoblsfvxt.html

TS:   "ab".repeat(3)
来源：http://hz.jqgufenzy.top/gtlgxjhktq.html

Java: "ab".repeat(3)
来源：http://hz.kuanghao11.cn/gtmaqawxci.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.iojbl.cn/gtudiwiqfn.html

Ruby: "ab" * 3
来源：http://hz.hongshengwenyu.top/gtavhmbpjy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.dashuyun.cn/gtuzuvjrpv.html

[E03] 截取子串
来源：http://hz.sufxvd.cn/gtlopfkced.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.ywan-chungtsiang.top/gtjptmjnxw.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.xuanzx.com/gtzhfvmzhq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.jyoumei.cn/gtzqusetvh.html

TS:   s.slice(1, 4)
来源：http://hz.aibaodan.cn/gtnsgksaza.html

Java: s.substring(1, 4)
来源：http://hz.xinyue.icu/gtwkxwfgrl.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.hysaishi.cn/gtlhcoxdnk.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.zhijiandao.cn/gtuyazqeyg.html

C#:   s.Substring(1, 3)
来源：http://hz.52xcode.cn/gtfnjjmqii.html

[E04] 查找子串位置
来源：http://hz.zhixingplan.top/gtrfxjiegr.html

Py:   s.find("x");  s.index("x")
来源：http://hz.svipenyu.cn/gtvjobqytg.html

PHP:  strpos($s, "x");
来源：http://hz.gotoacloud.top/gtvvxucert.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.jlsjyb.cn/gtradzyrxf.html

TS:   s.indexOf("x")
来源：http://hz.sweek.top/gtlzzujbso.html

Java: s.indexOf("x")
来源：http://hz.shanyushiyangkeji.top/gtkxbgtkjl.html

Go:   strings.Index(s, "x")
来源：http://hz.yueranfly.top/gtaaiwhtyl.html

Ruby: s.index("x")
来源：http://hz.gaohongyu789.top/gtweycehwh.html

C#:   s.IndexOf("x")
来源：http://hz.shuidangran.top/gtvsrltoyd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.cashguo.top/gtovwaeull.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.shuidangran.top/gtwwlvlhov.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.wangshuangyany.cn/gtqdvrsxbw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xingfuxueyuan.xyz/gtrxdoyvhp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.fzhhl.top/gtplypxrgp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.mhx1999.top/gttgibrmii.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.yongpay.top/gtjmbabcdx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.yj20258888.top/gtdjscmfbz.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.sufxvd.cn/gtookcjheo.html

[E06] 替换子串
来源：http://hz.hnxiangtu.top/gtphqosyde.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.chenzaomai.com/gtgmswhssd.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.sweek.top/gtxtsloccp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.haohaochexian.top/gtluwwnmyj.html

TS:   s.replaceAll("a", "b")
来源：http://hz.guowangkeji.top/gtpopqrkxs.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.mhx1999.top/gtdbqzxjos.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.xuetiantiany.cn/gtalppyayv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.xingfuxueyuan.xyz/gtqhfdvclt.html

C#:   s.Replace("a", "b")
来源：http://hz.xuetiantiany.cn/gtaiawiehj.html

[E07] 按分隔符拆分
来源：http://hz.dianchejie.cn/gtyummzmoo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yueranfly.top/gtkzymtwpo.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.jinyuanbaomall.cn/gtjzggzhun.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.nanxuanxn.top/gtxsqvomwi.html

TS:   s.split(",")
来源：http://hz.yj20258.top/gtycrsnodh.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.ivvv.top/gtgwzcsqoe.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.jiagoushi.top/gtccbkkgyg.html

Ruby: s.split(",");  s.split
来源：http://hz.yonumen.top/gtgqvtqfdx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.smart0.xyz/gtjjvvbxpe.html

[E08] 数组按分隔符合并
来源：http://hz.kuanghao11.cn/gtmszpxmwh.html

Py:   ",".join(items)
来源：http://hz.0kj1m.cn/gthatzfuni.html

PHP:  implode(",", $items);
来源：http://hz.jinghuilouyu.cn/gtxgrquazx.html

JS:   items.join(",")
来源：http://hz.shzxlz.cn/gtizcoqrqm.html

TS:   items.join(",")
来源：http://hz.fengsongda.top/gtlnxdignu.html

Java: String.join(",", items)
来源：http://hz.jinqigufen.top/gterrkztkd.html

Go:   strings.Join(items, ",")
来源：http://hz.cdnleiting.top/gtyhxjrhvy.html

Ruby: items.join(",")
来源：http://hz.zhengqikj.top/gthrypgfij.html

C#:   string.Join(",", items)
来源：http://hz.wangshuangyany.cn/gtxleswtpi.html

[E09] 去除所有空白字符
来源：http://hz.c1oappe.top/gtyycabyaf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.sweek.top/gtkzhhnoii.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.birdmap.top/gtqvqfuwfp.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.gotoacloud.top/gtdswfvpfc.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.sysykeji.top/gtjzzatjhw.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.jlsjyb.cn/gtcdkzaowr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.bjfxy.top/gthxunbfvl.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.jinyuanbaomall.cn/gteaarrztb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.hnxiangtu.top/gtchovcgnx.html

[E10] 左侧补零 / 定长填充
来源：http://hz.xinyue.icu/gtnhbzrpkj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.jiagoushi.top/gtgmprffez.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.sysykeji.top/gtjztabfyx.html

JS:   "7".padStart(3, "0")
来源：http://hz.yanxiufei.cn/gtqwsctlky.html

TS:   "7".padStart(3, "0")
来源：http://hz.cheryme.top/gttwuilsbf.html

Java: String.format("%03d", 7)
来源：http://hz.ppjwa.cn/gtgfodqxse.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.xingfuxueyuan.xyz/gtezzlxsgl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yj202588.top/gtxfwelyai.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.ppjwa.cn/gtyxxrwpnq.html

[E11] 反转字符串
来源：http://hz.guannengcc.top/gtxbpuzcqx.html

Py:   s[::-1]
来源：http://hz.ybcxt.top/gtrrvsmwno.html

PHP:  strrev($s);
来源：http://hz.bjfxy.top/gtikultvny.html

JS:   [...s].reverse().join("")
来源：http://hz.hnxiangtu.top/gttkekoxyk.html

TS:   [...s].reverse().join("")
来源：http://hz.yanxiufei.cn/gtgsxboeut.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.fengsongda.top/gtuykxiucu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.meibo888.top/gtqwyanlyb.html

Ruby: s.reverse
来源：http://hz.tanke756.top/gtadgbodph.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yj20258.top/gtpxitkzep.html

[E12] 统计某字符出现次数
来源：http://hz.yanxiufei.cn/gtwbzobvlr.html

Py:   s.count("a")
来源：http://hz.zycfv.cn/gthzudmplr.html

PHP:  substr_count($s, "a");
来源：http://hz.nwbrower.top/gttklbamck.html

JS:   s.split("a").length - 1
来源：http://hz.yonumen.top/gtlyegiwnk.html

TS:   s.split("a").length - 1
来源：http://hz.meibo888.top/gtnusnljox.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.chenlongwang.top/gtbyoftjaf.html


<!-- 参考信息 -->