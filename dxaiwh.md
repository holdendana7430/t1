代发 wailian999

Go:   arr[0]; arr[0] = 9
来源：http://hz.haohaochexian.top/gtgnhvrvbl.html

Ruby: arr[0]; arr[-1]; arr[0] = 9
来源：http://hz.jlsjyb.cn/gtbelvljkb.html

C#:   list[0]; list[^1]; list[0] = 9;
来源：http://hz.gzhubu.top/gtuotxhbst.html

[D06] 数组长度
来源：http://hz.cucudq.cn/gtxegxumek.html

Py:   len(arr)
来源：http://hz.xziqi.cn/gtxtjpogmh.html

PHP:  count($arr);
来源：http://hz.ywan-chungtsiang.top/gtomekfkts.html

JS:   arr.length
来源：http://hz.kuanghao11.cn/gtpclfzykr.html

TS:   arr.length
来源：http://hz.chenzaomai.com/gtplxlyqgq.html

Java: list.size();
来源：http://hz.smart0.xyz/gtiqfksxyo.html

Go:   len(arr)
来源：http://hz.jinyuanbaomall.cn/gtgvxxkidk.html

Ruby: arr.length; arr.size
来源：http://hz.cqqwz.cn/gturgztirx.html

C#:   list.Count;
来源：http://hz.nwbrower.top/gtwtqzycoq.html

[D07] 切片 / 取子数组
来源：http://hz.birdmap.top/gtwcuhmxxj.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.yvedp.cn/gtxgcmzmbb.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.cashguo.top/gtppjfbrga.html

JS:   arr.slice(1, 4);
来源：http://hz.chenjidiqi.icu/gtvgxsuezn.html

TS:   arr.slice(1, 4);
来源：http://hz.aibaodan.cn/gthmttppgp.html

Java: list.subList(1, 4);
来源：http://hz.zdqjudy.top/gtnvtajyrd.html

Go:   arr[1:4]
来源：http://hz.yonumen.top/gtptvazaui.html

Ruby: arr[1, 3]
来源：http://hz.daxiang520.top/gtvdyilroo.html

C#:   list.GetRange(1, 3);
来源：http://hz.nwbrower.top/gtifcdojlh.html

[D08] 合并两个数组
来源：http://hz.jinghuilouyu.cn/gtqfrlzyco.html

Py:   a + b;  a.extend(b)
来源：http://hz.0kj1m.cn/gtbawzsswj.html

PHP:  array_merge($a, $b);
来源：http://hz.sxryk.cn/gtnhmvueum.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.vqdsnc.cn/gtrkmmggkw.html

TS:   [...a, ...b];
来源：http://hz.yongpay.top/gtqdibhlin.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.shanyushiyangkeji.top/gtspspyzde.html

Go:   append(a, b...)
来源：http://hz.shanyushiyangtech.top/gtylbvudlc.html

Ruby: a + b;  a.concat(b)
来源：http://hz.hfpthk.cn/gtszevsxri.html

C#:   a.Concat(b).ToList()
来源：http://hz.zhiwuduotai.top/gtqeytttek.html

[D09] 排序（升序）
来源：http://hz.quarkkingdee.top/gthahlqenl.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.zhongyouzk.top/gtpnmpbqlw.html

PHP:  sort($arr);
来源：http://hz.aibaodan.cn/gtlesxxnqh.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.zhijiandao.cn/gtjqboyulx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.cashguo.top/gtgiuazdob.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.tanke756.top/gtckwmyarh.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.guannengcc.top/gtcubknjyd.html

Ruby: arr.sort
来源：http://hz.tanke756.top/gtwaimwfvy.html

C#:   list.Sort();
来源：http://hz.yuanzhike.top/gtmealsone.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.hfpthk.cn/gtojxwpday.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yuanzhike.top/gteicupqas.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.yuxming.cn/gtmgcjknjq.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yanxiufei.cn/gtrpyizmpa.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.shuidangran.top/gtvnpiwira.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zycfv.cn/gtrkqxtzox.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.chenzaomai.com/gtmcwvfojp.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.cheryme.top/gtpmycuvcl.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.sweek.top/gthrolwbmu.html

[D11] 反转数组
来源：http://hz.chenjidiqi.icu/gtrjtvgikx.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.birdmap.top/gtshwxwwld.html

PHP:  array_reverse($arr);
来源：http://hz.jqgufenzy.top/gthetcjhmb.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.c1oappe.top/gtwluwbxkf.html

TS:   [...arr].reverse();
来源：http://hz.xingfuxueyuan.xyz/gtekfqtglp.html

Java: Collections.reverse(list);
来源：http://hz.nwbrower.top/gtqaqzqqwv.html

Go:   slices.Reverse(arr)
来源：http://hz.yanxiufei.cn/gttjzrqyzg.html

Ruby: arr.reverse
来源：http://hz.chenjidiqi.icu/gtxlmzwnld.html

C#:   list.Reverse();
来源：http://hz.sufxvd.cn/gtthexrntb.html

[D12] 查找元素下标
来源：http://hz.bjfxy.top/gthykxjcpu.html

Py:   arr.index(x);  x in arr
来源：http://hz.ydzc1.top/gtawzrqyxc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.ywan-chungtsiang.top/gtvnmamoid.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.yangfankeji.com/gtgwrsobfd.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.9152youxi.cn/gtedwbkdzf.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.shuidangran.top/gtfsiwceai.html

Go:   slices.Index(arr, x)
来源：http://hz.shangyingyoupin.top/gtjzgklukh.html

Ruby: arr.index(x)
来源：http://hz.tanke756.top/gtwoyxercb.html

C#:   list.IndexOf(x);
来源：http://hz.gaohongyu789.top/gtdyikzxun.html

[D13] 过滤（保留满足条件的）
来源：http://hz.yvedp.cn/gtjasueolk.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zhengqikj.top/gtiklfhyox.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.gaohongyu789.top/gtuamnopwz.html

JS:   arr.filter(x => x > 3)
来源：http://hz.yvedp.cn/gtnxrqhugt.html

TS:   arr.filter(x => x > 3)
来源：http://hz.tanke756.top/gtjvyqfrby.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.pengpengdd.cyou/gtszaubnli.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.sysykeji.top/gtvvcbovwg.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.pycfn.com/gtelptpccv.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.ehwqpu.com/gtepbumiki.html

[D14] 映射转换（每个元素变形）
来源：http://hz.hnxiangtu.top/gtrkjigmot.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.52xcode.cn/gtjakbxlnk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.zhaomingkeji.xyz/gticrcgaps.html

JS:   arr.map(x => x * 2)
来源：http://hz.tanke756.top/gtxortbgnl.html

TS:   arr.map(x => x * 2)
来源：http://hz.havefunace.top/gttytrxvzk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.xziqi.cn/gteitmvmcf.html

Go:   // 手写循环
来源：http://hz.jqgufenzy.top/gtsmeylihr.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.ydzc1.top/gtpwraxfxp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.kuanghao11.cn/gtolkixtnd.html

[D15] 去重
来源：http://hz.0kj1m.cn/gtpoqmhpex.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.zhixingplan.top/gtzxmhwuin.html

PHP:  array_unique($arr);
来源：http://hz.pengpengdd.cyou/gtgcgrdtqm.html

JS:   [...new Set(arr)]
来源：http://hz.yanxiufei.cn/gtagbwowvv.html

TS:   [...new Set(arr)]
来源：http://hz.yvedp.cn/gtiobtyatp.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.aibaodan.cn/gtstbgykjq.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zycfv.cn/gtdsxlqbzo.html

Ruby: arr.uniq
来源：http://hz.yj20258888.top/gtjeckqdyh.html

C#:   list.Distinct().ToList()
来源：http://hz.xinyue.icu/gtbdliipwj.html

[D16] 求和与平均值
来源：http://hz.yj202588.top/gtbdldzhkm.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.yj202588.top/gtjehnpirh.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.jinyuanbaomall.cn/gtkklwjrvn.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.kuanghao11.cn/gtgezdwias.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yonumen.top/gtkrouzusb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.andypj.xyz/gthbrofxrj.html

Go:   // 手写循环累加
来源：http://hz.shangyingyoupin.top/gtjueyqsuc.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhongyouzk.top/gtzpwvoxdq.html

C#:   list.Sum();  list.Average()
来源：http://hz.nanxuanxn.top/gtytyhknid.html

[D17] 最大值与最小值
来源：http://hz.yongpay.top/gtcpsthzzk.html

Py:   max(arr);  min(arr)
来源：http://hz.snrcjt.cn/gtvryvoboh.html

PHP:  max($arr);  min($arr);
来源：http://hz.jianghu66.top/gthixmgfhy.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yuanzhike.top/gtiniovumt.html

TS:   Math.max(...arr);
来源：http://hz.gaohongyu789.top/gtyiobysne.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.daria6918.cn/gtidogjwxa.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.jqgufenzy.top/gtmyppubsh.html

Ruby: arr.max;  arr.min
来源：http://hz.zhoulong.xyz/gtzjucxovo.html

C#:   list.Max();  list.Min()
来源：http://hz.nwbrower.top/gtrcjoiuyy.html

[D18] 扁平化嵌套数组
来源：http://hz.snrcjt.cn/gtekhomfwt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.cqqwz.cn/gtfewirxus.html

PHP:  array_merge(...$nested);
来源：http://hz.hysaishi.cn/gtuqghzbbs.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.ydzc1.top/gtyumcibrz.html

TS:   nested.flat();
来源：http://hz.vqdsnc.cn/gtoopylzhk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.jyoumei.cn/gthqeodpbu.html

Go:   // 手写双层循环
来源：http://hz.svipenyu.cn/gtxikqjtug.html

Ruby: nested.flatten
来源：http://hz.nanxuanxn.top/gtatbvblcu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.jinqigufen.top/gtfnktppxf.html

[D19] 按字段分组
来源：http://hz.cdnleiting.top/gtwouifbvf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.zhiwuduotai.top/gtlvkviczy.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.cucudq.cn/gtjdsiwoie.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.shanyushiyangkeji.top/gtvjaurnnd.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.nwbrower.top/gtuaqrjyco.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.9152youxi.cn/gtnsxuenxb.html

Go:   // 手写 map[string][]T
来源：http://hz.dashuyun.cn/gtjyetecln.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.nwbrower.top/gtanphsksa.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.yj202588.top/gtxyctutfi.html

[D20] 统计每个元素出现次数
来源：http://hz.chenjidiqi.icu/gtvvrsycsm.html

Py:   Counter(arr)
来源：http://hz.yj20258.top/gtpqrkasmy.html

PHP:  array_count_values($arr);
来源：http://hz.vqdsnc.cn/gtpdpfuymo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.jqgufenzy.top/gtojiclvgp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.vqdsnc.cn/gttrpytjpe.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.dianchejie.cn/gtdkammrzm.html

Go:   // 手写 map[T]int
来源：http://hz.birdmap.top/gtiqqhrbco.html

Ruby: arr.tally
来源：http://hz.xinyue.icu/gtxpgewogx.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.gzhubu.top/gtlddihlqf.html

[D21] 判断是否包含某元素
来源：http://hz.feifeiyinyue.top/gteaqmmeyy.html

Py:   x in arr
来源：http://hz.hammf.cn/gtnzcsdwwb.html

PHP:  in_array($x, $arr, true);
来源：http://hz.hysaishi.cn/gtwsbwwwdg.html

JS:   arr.includes(x)
来源：http://hz.aibaodan.cn/gtzqxfduqh.html

TS:   arr.includes(x)
来源：http://hz.birdmap.top/gtxfrpiybb.html

Java: list.contains(x)
来源：http://hz.xuetiantiany.cn/gtdwnhwpee.html

Go:   slices.Contains(arr, x)
来源：http://hz.yuxming.cn/gtpvnutefr.html

Ruby: arr.include?(x)
来源：http://hz.yueranfly.top/gtywpgitmy.html

C#:   list.Contains(x)
来源：http://hz.havefunace.top/gtcmxzduan.html

[D22] 复制数组（避免共享引用）
来源：http://hz.aibaodan.cn/gtwmduxqoo.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.yueranfly.top/gtclbnmtjv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.daxiang520.top/gtcolxngxg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.yuanzhike.top/gtksexmwou.html

TS:   [...arr];
来源：http://hz.hammf.cn/gtemmeioja.html

Java: new ArrayList<>(list);
来源：http://hz.jqgfzy.top/gtulttjryq.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jqgfzy.top/gtbzlukcsk.html

Ruby: arr.dup;  arr.clone
来源：http://hz.nanxuanxn.top/gtjmqxebto.html

C#:   new List<int>(list);
来源：http://hz.xziqi.cn/gtqasiuhun.html

[D23] reduce 累积计算
来源：http://hz.haohaochexian.top/gtamzgrsso.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.yvedp.cn/gtxkiaaszh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.chenzaomai.com/gthiblayeu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.bjfxy.top/gtipndfthe.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.xylfe.cn/gtdalevoxz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.ydzc1.top/gtudqiephd.html

Go:   // 手写循环
来源：http://hz.yj20258888.top/gtolqudses.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.chenlongwang.top/gtbhdpbryu.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.ywan-chungtsiang.top/gtknxflwbv.html

[D24] 字典 / Map 基本操作
来源：http://hz.ybcxt.top/gtetxrubgm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.xinyue.icu/gtpkbltmcw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.xuetiantiany.cn/gtddjkmqqp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.chenzaomai.com/gtmoujupxu.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.aizwys.cn/gttzshqwpz.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.hnqzz.top/gtmievcapq.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.snrcjt.cn/gtyfbqwkrw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.chenzaomai.com/gtghmhschh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.nwbrower.top/gtkixdzule.html

[D25] Set 集合去重与交并差
来源：http://hz.zhijiandao.cn/gtzeganrcm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.ydjk.org.cn/gttosetcqc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jqgufenzy.top/gtihkrfxyp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.ywan-chungtsiang.top/gtbnxoxoml.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.jyoumei.cn/gtxjckclvk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.yvedp.cn/gtgbkmctfq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yongpay.top/gtqaalspyx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.mhx1999.top/gtyzlsuktx.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.hywenlv.cn/gtqwccokuh.html

[D26] 数组转字符串
来源：http://hz.quarkkingdee.top/gtqwduujni.html

Py:   ", ".join(map(str, arr))
来源：http://hz.quarkkingdee.top/gtpnszfukl.html

PHP:  implode(", ", $arr);
来源：http://hz.chenzaomai.com/gtmlvhdewn.html

JS:   arr.join(", ")
来源：http://hz.gotoacloud.top/gtvuwthtgz.html

TS:   arr.join(", ")
来源：http://hz.svipenyu.cn/gtktsooedd.html

Java: String.join(", ", list)
来源：http://hz.havefunace.top/gteuenrxzq.html

Go:   strings.Join(strs, ", ")
来源：http://hz.yj202588.top/gttammsbmn.html

Ruby: arr.join(", ")
来源：http://hz.ppjwa.cn/gthswpktzs.html

C#:   string.Join(", ", list)
来源：http://hz.jlsjyb.cn/gtduxieasa.html

================================================================================
来源：http://hz.hysaishi.cn/gtgnggligf.html

E. 字符串处理
来源：http://hz.feifeiyinyue.top/gtvnocizqy.html

================================================================================
来源：http://hz.daria6918.cn/gtmtnnxodx.html

[E01] 拼接字符串
来源：http://hz.jiagoushi.top/gtrxvgsfoc.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.kuanghao11.cn/gtjrocjxfp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.zhongyouzk.top/gtyrfcwazd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xinyue.icu/gtcrpzwdbk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.tanke756.top/gtkaasgtvn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.jiagoushi.top/gtvvydcoac.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.cqqwz.cn/gtdyxiskrn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.zhijiandao.cn/gtlppuqldx.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.wangshuangyany.cn/gtckpncqqv.html

[E02] 重复字符串
来源：http://hz.yuanzhike.top/gtpefdlhdf.html

Py:   "ab" * 3
来源：http://hz.aizwys.cn/gtzmckqrik.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jyoumei.cn/gtmiwkxsow.html

JS:   "ab".repeat(3)
来源：http://hz.hfpthk.cn/gtgexfqrce.html

TS:   "ab".repeat(3)
来源：http://hz.dianchejie.cn/gtzoyxoifg.html

Java: "ab".repeat(3)
来源：http://hz.svipenyu.cn/gtntqnlqxl.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zhongyouzk.top/gtlwdzzlim.html

Ruby: "ab" * 3
来源：http://hz.xuanzx.com/gtjklmjkqd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.xziqi.cn/gtwubmjvxg.html

[E03] 截取子串
来源：http://hz.cqqwz.cn/gtsddfznlf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.xinyue.icu/gtyjchtggv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.wangshuangyany.cn/gtxrltkhek.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.gogol.net.cn/gtcrovvwbp.html

TS:   s.slice(1, 4)
来源：http://hz.ybcxt.top/gtqgznyjrz.html

Java: s.substring(1, 4)
来源：http://hz.zhixingplan.top/gtqswgnkpn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.xingfuxueyuan.xyz/gtrtiumrre.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.svipenyu.cn/gtafjiefbc.html

C#:   s.Substring(1, 3)
来源：http://hz.daxiang520.top/gtcddwtyyd.html

[E04] 查找子串位置
来源：http://hz.svipenyu.cn/gtiyflqojv.html

Py:   s.find("x");  s.index("x")
来源：http://hz.hfpthk.cn/gtckaqbjzg.html

PHP:  strpos($s, "x");
来源：http://hz.zycfv.cn/gthgjxcopq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.wangdashe.top/gtxrweqciu.html

TS:   s.indexOf("x")
来源：http://hz.dashuyun.cn/gtveofezbx.html

Java: s.indexOf("x")
来源：http://hz.ivvv.top/gtygutuykk.html

Go:   strings.Index(s, "x")
来源：http://hz.shzxlz.cn/gtzupsndhc.html

Ruby: s.index("x")
来源：http://hz.jianghu66.top/gtkzyefftc.html

C#:   s.IndexOf("x")
来源：http://hz.xuetiantiany.cn/gtsdhyxssp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.ppjwa.cn/gtshmfyvzv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.nanxuanxn.top/gtpnrvceqg.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.andypj.xyz/gttwokvqyc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.guowangkeji.top/gtokroxsxv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.sxryk.cn/gtzaoedvir.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.xinyue.icu/gtoicvyped.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.shanyushiyangkeji.top/gtddwppguk.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.aibaodan.cn/gtfjimoyrl.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.yj20258.top/gthptdlyca.html

[E06] 替换子串
来源：http://hz.jianghu66.top/gtzjigdbdk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.pengpengdd.cyou/gtqckgoyro.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.zhongyouzk.top/gtwourtmmd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yueranfly.top/gtopsimawd.html

TS:   s.replaceAll("a", "b")
来源：http://hz.svipenyu.cn/gtespumsxf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.aizwys.cn/gtdthqclyh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.aibaodan.cn/gtcjkeemdf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.jinqigfzy.top/gtottldbfg.html

C#:   s.Replace("a", "b")
来源：http://hz.jqgfzy.top/gthshsaiyc.html

[E07] 按分隔符拆分
来源：http://hz.yj20258.top/gtuksfzsks.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.daria6918.cn/gtrazzumdy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.nanxuanxn.top/gtgfulamxv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.zhongyouzk.top/gthhbszppb.html

TS:   s.split(",")
来源：http://hz.havefunace.top/gtmrgrwtvm.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.chenzaomai.com/gtxritgfxd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.zhiwuduotai.top/gttyobgfmb.html

Ruby: s.split(",");  s.split
来源：http://hz.daria6918.cn/gtnotqdqwq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.haohaochexian.top/gtqeapcbeq.html

[E08] 数组按分隔符合并
来源：http://hz.gaohongyu789.top/gtclltqigv.html

Py:   ",".join(items)
来源：http://hz.cucudq.cn/gtuqnqvyge.html

PHP:  implode(",", $items);
来源：http://hz.zdqjudy.top/gtzzbmkliv.html

JS:   items.join(",")
来源：http://hz.snrcjt.cn/gtnrcmscea.html

TS:   items.join(",")
来源：http://hz.daria6918.cn/gtqswzymcq.html

Java: String.join(",", items)
来源：http://hz.hnxiangtu.top/gtgffalnky.html

Go:   strings.Join(items, ",")
来源：http://hz.dianchejie.cn/gtofvqpwvt.html

Ruby: items.join(",")
来源：http://hz.xuetiantiany.cn/gtmofnhtsf.html

C#:   string.Join(",", items)
来源：http://hz.vqdsnc.cn/gtugfmehir.html

[E09] 去除所有空白字符
来源：http://hz.shzxlz.cn/gtmcpxqgwu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.316326.xyz/gtvwjwyiem.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.chenjidiqi.icu/gtgepwiqen.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.chenjidiqi.icu/gttwnpphoi.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.cheryme.top/gtvdomtbyh.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.gotoacloud.top/gtbqeafwdp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.nanxuanxn.top/gtstmknueb.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.dashuyun.cn/gtkfujpecj.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.guowangkeji.top/gtpanxwvtw.html

[E10] 左侧补零 / 定长填充
来源：http://hz.yj202588.top/gtkjbrbomh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.fzhhl.top/gtqxjigpjd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.shanyushiyangtech.top/gtogvpbiui.html

JS:   "7".padStart(3, "0")
来源：http://hz.hongshengwenyu.top/gtewguvdto.html

TS:   "7".padStart(3, "0")
来源：http://hz.ybcxt.top/gtqpsivrvo.html

Java: String.format("%03d", 7)
来源：http://hz.havefunace.top/gthshwaqhv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.c1oappe.top/gtyspyevpp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.snrcjt.cn/gtmwqjoghr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.shangyingyoupin.top/gtytrfblwr.html

[E11] 反转字符串
来源：http://hz.iojbl.cn/gtklyfuxne.html

Py:   s[::-1]
来源：http://hz.nanxinkj.top/gtctfeebkb.html

PHP:  strrev($s);
来源：http://hz.birdmap.top/gtinrrfbut.html

JS:   [...s].reverse().join("")
来源：http://hz.redwolf501.top/gtralwhkmd.html

TS:   [...s].reverse().join("")
来源：http://hz.gzhubu.top/gtmvatxtbd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.jinyuanbaomall.cn/gtxicozatf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.shuidangran.top/gtostmodim.html

Ruby: s.reverse
来源：http://hz.zhixingplan.top/gtxwqasyhh.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.chenjidiqi.icu/gthbgxkzlu.html

[E12] 统计某字符出现次数
来源：http://hz.nanxuanxn.top/gtvumaunng.html

Py:   s.count("a")
来源：http://hz.yanxiufei.cn/gtmrflgfkv.html

PHP:  substr_count($s, "a");
来源：http://hz.guowangkeji.top/gtxngyxnve.html

JS:   s.split("a").length - 1
来源：http://hz.haohaochexian.top/gtywzkmlav.html

TS:   s.split("a").length - 1
来源：http://hz.shuidangran.top/gtbfqtxkqm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.tanke756.top/gtzyfkeeye.html


<!-- 参考信息 -->