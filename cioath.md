代发 wailian999

Ruby: a + b;  a.concat(b)
来源：http://hz.guowangkeji.top/gtwcetkmhs.html

C#:   a.Concat(b).ToList()
来源：http://hz.jinqigufen.top/gtnixpapnc.html

[D09] 排序（升序）
来源：http://hz.iojbl.cn/gtncxabpzi.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.pycfn.com/gtohppnwlq.html

PHP:  sort($arr);
来源：http://hz.zhengqikj.top/gthcukyrgl.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.mhx1999.top/gtedmemuyj.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.jinqigfzy.top/gtmugeapeh.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.svipenyu.cn/gtnwygwfuu.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.birdmap.top/gtumpricyl.html

Ruby: arr.sort
来源：http://hz.yuanzhike.top/gtkogscdoi.html

C#:   list.Sort();
来源：http://hz.gzhubu.top/gtmgenjlou.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.redwolf501.top/gthkrtyaaq.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.feifeiyinyue.top/gtxpgkhquk.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.gogol.net.cn/gtzhydmgtw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.xziqi.cn/gtjnoqjnza.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jinghuilouyu.cn/gtrqocukow.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.jinqigufen.top/gtjkpiqyir.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.kuanghao11.cn/gtqpnduabe.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yongpay.top/gttchhxeca.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.jinghuilouyu.cn/gtlvmeworv.html

[D11] 反转数组
来源：http://hz.xziqi.cn/gtohhsgksm.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.jinyuanbaomall.cn/gthgzcyafi.html

PHP:  array_reverse($arr);
来源：http://hz.xuetiantiany.cn/gtxxgunoea.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.ybcxt.top/gtfhevhvcg.html

TS:   [...arr].reverse();
来源：http://hz.zhoulong.xyz/gtnzxhitxo.html

Java: Collections.reverse(list);
来源：http://hz.yangfankeji.com/gtsaeomdqy.html

Go:   slices.Reverse(arr)
来源：http://hz.zhiwuduotai.top/gtrvkntfua.html

Ruby: arr.reverse
来源：http://hz.fzhhl.top/gtdmfgqewv.html

C#:   list.Reverse();
来源：http://hz.mhx1999.top/gtlxvhqtwz.html

[D12] 查找元素下标
来源：http://hz.cucudq.cn/gtbzbagisb.html

Py:   arr.index(x);  x in arr
来源：http://hz.xuetiantiany.cn/gtmivbcbfz.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.jqgfzy.top/gtxvuduaht.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.shanyushiyangtech.top/gtotrkgqxm.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.sysykeji.top/gtulmffirh.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.hnqzz.top/gtsddxyzgm.html

Go:   slices.Index(arr, x)
来源：http://hz.jianghu66.top/gtecmbkbgt.html

Ruby: arr.index(x)
来源：http://hz.jiagoushi.top/gtnvaxsuko.html

C#:   list.IndexOf(x);
来源：http://hz.fzhhl.top/gtwuxbyefu.html

[D13] 过滤（保留满足条件的）
来源：http://hz.9152youxi.cn/gtayrcyxyw.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.tian-w.cn/gtjuzqhfzz.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.cheryme.top/gtmgnttusf.html

JS:   arr.filter(x => x > 3)
来源：http://hz.shzxlz.cn/gthlfsddwm.html

TS:   arr.filter(x => x > 3)
来源：http://hz.sxryk.cn/gtismcvjyd.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.zycfv.cn/gtlqffmvfa.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.xuanzx.com/gtrnchufwy.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.ydjk.org.cn/gtuwmolkqw.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.cheryme.top/gtucjvfogr.html

[D14] 映射转换（每个元素变形）
来源：http://hz.cheryme.top/gtdrvdcnoh.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.shuidangran.top/gtsexvahea.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.shangyingyoupin.top/gtoyamzscj.html

JS:   arr.map(x => x * 2)
来源：http://hz.zhongyouzk.top/gtlgkwwqyf.html

TS:   arr.map(x => x * 2)
来源：http://hz.yangfankeji.com/gtxduigyax.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.yueranfly.top/gtgmgzyscx.html

Go:   // 手写循环
来源：http://hz.jlsjyb.cn/gttwrobnms.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.gzhubu.top/gtmqzwywdr.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.yj202588.top/gtntpbnxlb.html

[D15] 去重
来源：http://hz.yanxiufei.cn/gtdwvhthes.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.nwbrower.top/gtxiqvxdiq.html

PHP:  array_unique($arr);
来源：http://hz.zhiwuduotai.top/gtenorghzw.html

JS:   [...new Set(arr)]
来源：http://hz.gogol.net.cn/gtzhrqmnud.html

TS:   [...new Set(arr)]
来源：http://hz.jqgufenzy.top/gtbmoospdy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.ydjk.org.cn/gtcnccbrwi.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.52xcode.cn/gtcllnrxbx.html

Ruby: arr.uniq
来源：http://hz.52xcode.cn/gtsxbbvlab.html

C#:   list.Distinct().ToList()
来源：http://hz.hammf.cn/gtgzlandxz.html

[D16] 求和与平均值
来源：http://hz.feifeiyinyue.top/gthadwpxle.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.zdqjudy.top/gtnkjbqgaz.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.pycfn.com/gtjlwvlkeu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.wangshuangyany.cn/gtrlicqdsj.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhoulong.xyz/gtrvfdwvgt.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.pycfn.com/gtxnqrxtci.html

Go:   // 手写循环累加
来源：http://hz.tianlin.xyz/gtpdnxfflp.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.havefunace.top/gtrzvqengf.html

C#:   list.Sum();  list.Average()
来源：http://hz.shuidangran.top/gtgoebuyny.html

[D17] 最大值与最小值
来源：http://hz.smart0.xyz/gttctqdrfw.html

Py:   max(arr);  min(arr)
来源：http://hz.dianchejie.cn/gtzvscgory.html

PHP:  max($arr);  min($arr);
来源：http://hz.redwolf501.top/gtptkvnbsl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.daxiang520.top/gtvvxpmivt.html

TS:   Math.max(...arr);
来源：http://hz.wangdashe.top/gtqomuyhtq.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.havefunace.top/gtdyzhvtcz.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.xinyue.icu/gtgndslbxz.html

Ruby: arr.max;  arr.min
来源：http://hz.ivvv.top/gtkessrhyi.html

C#:   list.Max();  list.Min()
来源：http://hz.hongshengwenyu.top/gttnzvierj.html

[D18] 扁平化嵌套数组
来源：http://hz.dashuyun.cn/gtplnquunn.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.daria6918.cn/gthtkcwcnc.html

PHP:  array_merge(...$nested);
来源：http://hz.yj202588.top/gtjcohuzab.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.c1oappe.top/gtfdxasayk.html

TS:   nested.flat();
来源：http://hz.aibaodan.cn/gtfjjwiode.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.jinqigfzy.top/gtzinqfuol.html

Go:   // 手写双层循环
来源：http://hz.hysaishi.cn/gtbxikivmy.html

Ruby: nested.flatten
来源：http://hz.meibo888.top/gtaldjdzda.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.shanyushiyangkeji.top/gttxfbodaz.html

[D19] 按字段分组
来源：http://hz.sweek.top/gtcvzypiqt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.wangdashe.top/gtnpfxrxiq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.zhixingplan.top/gtzsvpjrjj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.sysykeji.top/gtylbmttvh.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.fengsongda.top/gtyjcwgzkd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.xziqi.cn/gtbxmgmdok.html

Go:   // 手写 map[string][]T
来源：http://hz.yuanzhike.top/gthutvqzyp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.cheryme.top/gtppovutwo.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.chenzaomai.com/gtxxgjiabn.html

[D20] 统计每个元素出现次数
来源：http://hz.jqgufenzy.top/gthjtwtlgz.html

Py:   Counter(arr)
来源：http://hz.fzhhl.top/gthsjrujsj.html

PHP:  array_count_values($arr);
来源：http://hz.snrcjt.cn/gtizhlszmz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hammf.cn/gttereiqfi.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.shanyushiyangkeji.top/gtorgghtfz.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.zhixingplan.top/gtbndtphjf.html

Go:   // 手写 map[T]int
来源：http://hz.ywan-chungtsiang.top/gtrkygnbcg.html

Ruby: arr.tally
来源：http://hz.xinyue.icu/gtrjfjzrma.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.jqgfzy.top/gtbooyisot.html

[D21] 判断是否包含某元素
来源：http://hz.zhoulong.xyz/gtnwnsbatv.html

Py:   x in arr
来源：http://hz.meibo888.top/gtmecnbqdl.html

PHP:  in_array($x, $arr, true);
来源：http://hz.mhx1999.top/gtyzmgidsx.html

JS:   arr.includes(x)
来源：http://hz.zdqjudy.top/gtqzdkftpt.html

TS:   arr.includes(x)
来源：http://hz.kuanghao11.cn/gtyakitwec.html

Java: list.contains(x)
来源：http://hz.ehwqpu.com/gtrcehfinx.html

Go:   slices.Contains(arr, x)
来源：http://hz.jyoumei.cn/gtokrciijg.html

Ruby: arr.include?(x)
来源：http://hz.nanxinkj.top/gtlqqfnqhx.html

C#:   list.Contains(x)
来源：http://hz.havefunace.top/gtcglalkdv.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jlsjyb.cn/gtmbjdodak.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.jinghuilouyu.cn/gtresfcmmd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.gotoacloud.top/gtkbfkpxve.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.jqgfzy.top/gtuclwrmcs.html

TS:   [...arr];
来源：http://hz.hysaishi.cn/gtvtrwzjhu.html

Java: new ArrayList<>(list);
来源：http://hz.zhongyouzk.top/gtbqcoxrpi.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.feifeiyinyue.top/gtacpdfxqm.html

Ruby: arr.dup;  arr.clone
来源：http://hz.hongshengwenyu.top/gtywfmatif.html

C#:   new List<int>(list);
来源：http://hz.cdnleiting.top/gtpsokvmrp.html

[D23] reduce 累积计算
来源：http://hz.hongshengwenyu.top/gthezghzvu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.zhijiandao.cn/gtdbcmqycx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.iojbl.cn/gtapbuxkvn.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hysaishi.cn/gtvowubdrf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinqigfzy.top/gtdhjadskn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.shzxlz.cn/gtftybndhl.html

Go:   // 手写循环
来源：http://hz.jinqigufen.top/gttcenxicf.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.316326.xyz/gtyofrfuko.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.ehwqpu.com/gthucuzngt.html

[D24] 字典 / Map 基本操作
来源：http://hz.jlsjyb.cn/gtqgefqgns.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.9152youxi.cn/gtpsnftcnn.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.sysykeji.top/gtbgffziuc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.tianlin.xyz/gtcmlttbgt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.sysykeji.top/gtiszjekbp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.jqgfzy.top/gtgbwnancd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.fengsongda.top/gtvgmplcmi.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.jlsjyb.cn/gtsefygngm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zycfv.cn/gttbxcmhra.html

[D25] Set 集合去重与交并差
来源：http://hz.mhx1999.top/gtfxdunanj.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.0kj1m.cn/gtrqwuhhhj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.jinqigfzy.top/gtkaolecoq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.aibaodan.cn/gtrpigkxlx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.wangshuangyany.cn/gtkqtjhxgc.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.hysaishi.cn/gtlucamyip.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.snrcjt.cn/gtdnzzcbvb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.kuanghao11.cn/gtgjpsaiur.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.tianlin.xyz/gthruyzupv.html

[D26] 数组转字符串
来源：http://hz.jinqigfzy.top/gtramqxyqw.html

Py:   ", ".join(map(str, arr))
来源：http://hz.shanyushiyangkeji.top/gtykhxuaeb.html

PHP:  implode(", ", $arr);
来源：http://hz.cheryme.top/gtmvpbzevs.html

JS:   arr.join(", ")
来源：http://hz.svipenyu.cn/gtloolceby.html

TS:   arr.join(", ")
来源：http://hz.cqqwz.cn/gtlkdgvjcu.html

Java: String.join(", ", list)
来源：http://hz.sysykeji.top/gtirgrjrcr.html

Go:   strings.Join(strs, ", ")
来源：http://hz.feifeiyinyue.top/gtmfrkdjuv.html

Ruby: arr.join(", ")
来源：http://hz.yueranfly.top/gtqfediufz.html

C#:   string.Join(", ", list)
来源：http://hz.nanxinkj.top/gtqivqzqgz.html

================================================================================
来源：http://hz.chenzaomai.com/gtzozgdzhl.html

E. 字符串处理
来源：http://hz.bjfxy.top/gtruqqqhnr.html

================================================================================
来源：http://hz.yanxiufei.cn/gtpmswnekj.html

[E01] 拼接字符串
来源：http://hz.nwbrower.top/gtkpwomfrf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.quarkkingdee.top/gtiwsmglpd.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.shangyingyoupin.top/gtwjtqtwae.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.ivvv.top/gtcgwlnezs.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.gzhubu.top/gtomzdjrlp.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.yuanzhike.top/gtksgmtfta.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.hongshengwenyu.top/gtiezkckct.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.tanke756.top/gtwufodkkg.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.ywan-chungtsiang.top/gteeudtrxd.html

[E02] 重复字符串
来源：http://hz.zhoulong.xyz/gtxhnxcezc.html

Py:   "ab" * 3
来源：http://hz.zhoulong.xyz/gtzzawowfd.html

PHP:  str_repeat("ab", 3);
来源：http://hz.birdmap.top/gtewdhiuau.html

JS:   "ab".repeat(3)
来源：http://hz.yj202588.top/gtcmntqkpv.html

TS:   "ab".repeat(3)
来源：http://hz.smart0.xyz/gtqxsqrkud.html

Java: "ab".repeat(3)
来源：http://hz.mhx1999.top/gtqbjwkjso.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.nanxuanxn.top/gtipdlkfge.html

Ruby: "ab" * 3
来源：http://hz.jinghuilouyu.cn/gtwhribtne.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.iojbl.cn/gtlalhrjrq.html

[E03] 截取子串
来源：http://hz.kuanghao11.cn/gthjahwysf.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.jqgufenzy.top/gtszkxinxs.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.birdmap.top/gtcvcutwbc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.cashguo.top/gtngobftjo.html

TS:   s.slice(1, 4)
来源：http://hz.yongpay.top/gtpybtvhwx.html

Java: s.substring(1, 4)
来源：http://hz.svipenyu.cn/gtazdipquw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.zhijiandao.cn/gtmvjoijas.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.sufxvd.cn/gtwenjtwvl.html

C#:   s.Substring(1, 3)
来源：http://hz.jinghuilouyu.cn/gtnostgvpt.html

[E04] 查找子串位置
来源：http://hz.mhx1999.top/gtazqtlcxn.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jiagoushi.top/gtazjoswme.html

PHP:  strpos($s, "x");
来源：http://hz.meibo888.top/gtomynyfyc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yuxming.cn/gtdpzwyijp.html

TS:   s.indexOf("x")
来源：http://hz.ivvv.top/gtzzpgvqpg.html

Java: s.indexOf("x")
来源：http://hz.yueranfly.top/gtjjsdqyzf.html

Go:   strings.Index(s, "x")
来源：http://hz.0kj1m.cn/gtyztbvixm.html

Ruby: s.index("x")
来源：http://hz.yongpay.top/gtistgejiw.html

C#:   s.IndexOf("x")
来源：http://hz.hywenlv.cn/gtzmqpbxta.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.dianchejie.cn/gtxiivmfaq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.shanyushiyangkeji.top/gtqgllyjrc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.zhengqikj.top/gtodjqfpxm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.nanxuanxn.top/gtnxbrcvus.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.yueranfly.top/gtyqqnwapj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.pycfn.com/gtigngzwco.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.zhoulong.xyz/gtccmshbtx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.fzhhl.top/gtgmqzsqth.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.svipenyu.cn/gtzjkwwoiu.html

[E06] 替换子串
来源：http://hz.c1oappe.top/gtlwhbsupd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.shangyingyoupin.top/gtldcusljl.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.cucudq.cn/gtjuikrxyi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.iojbl.cn/gtadtccudm.html

TS:   s.replaceAll("a", "b")
来源：http://hz.snrcjt.cn/gtbtizwnnu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.gzhubu.top/gtwbelrngd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.aizwys.cn/gtvomjniet.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.shangyingyoupin.top/gtmmhgbpum.html

C#:   s.Replace("a", "b")
来源：http://hz.jqgufenzy.top/gtgwxhjpzd.html

[E07] 按分隔符拆分
来源：http://hz.quarkkingdee.top/gthjvosnba.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.guannengcc.top/gttfkcsapm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.cucudq.cn/gtmphycsmr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.haohaochexian.top/gtldbhgcrg.html

TS:   s.split(",")
来源：http://hz.ydzc1.top/gtvvfaindg.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.yanxiufei.cn/gtmwrefyos.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.mhx1999.top/gtwnqsxfze.html

Ruby: s.split(",");  s.split
来源：http://hz.shanyushiyangtech.top/gtndptlrqv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.vqdsnc.cn/gtjysoahqf.html

[E08] 数组按分隔符合并
来源：http://hz.yvedp.cn/gtwvipntsf.html

Py:   ",".join(items)
来源：http://hz.aibaodan.cn/gtuacmslxz.html

PHP:  implode(",", $items);
来源：http://hz.hywenlv.cn/gtqkpiypav.html

JS:   items.join(",")
来源：http://hz.nanxinkj.top/gtoqvzsgnr.html

TS:   items.join(",")
来源：http://hz.aibaodan.cn/gtvtzvsunj.html

Java: String.join(",", items)
来源：http://hz.cqqwz.cn/gticwolyes.html

Go:   strings.Join(items, ",")
来源：http://hz.sysykeji.top/gtdyufvjxx.html

Ruby: items.join(",")
来源：http://hz.zhengqikj.top/gtntxbhdbj.html

C#:   string.Join(",", items)
来源：http://hz.fzhhl.top/gtxstxlhkp.html

[E09] 去除所有空白字符
来源：http://hz.fzhhl.top/gtagirsdvm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.zdqjudy.top/gtzivubwsk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.52xcode.cn/gtnxbcnojs.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.haohaochexian.top/gtqrfvqqlq.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.shanyushiyangkeji.top/gtevhyoyxb.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.cucudq.cn/gtylrunnjk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.9152youxi.cn/gtzqcahflu.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.shanyushiyangkeji.top/gtlkrqijiy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.jiagoushi.top/gtahvcmpsw.html

[E10] 左侧补零 / 定长填充
来源：http://hz.havefunace.top/gtmuzqifhw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.hongshengwenyu.top/gtxkvsenhl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yj20258888.top/gtzvsakyxm.html

JS:   "7".padStart(3, "0")
来源：http://hz.bjfxy.top/gtefvbibib.html

TS:   "7".padStart(3, "0")
来源：http://hz.52xcode.cn/gtvfivedzv.html

Java: String.format("%03d", 7)
来源：http://hz.jqgufenzy.top/gtwqpdnein.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.ydjk.org.cn/gtypcazjrm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.zhongyouzk.top/gtigxegaex.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.hongshengwenyu.top/gtjlldrznp.html

[E11] 反转字符串
来源：http://hz.mhx1999.top/gtqtmfhkwc.html

Py:   s[::-1]
来源：http://hz.jiagoushi.top/gtxasjnljy.html

PHP:  strrev($s);
来源：http://hz.vqdsnc.cn/gttymohyeq.html

JS:   [...s].reverse().join("")
来源：http://hz.zhengqikj.top/gtofcwqjye.html

TS:   [...s].reverse().join("")
来源：http://hz.bjfxy.top/gtyehsuxup.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.bjfxy.top/gtzfklpzip.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.yj20258.top/gtfmkgwcpt.html

Ruby: s.reverse
来源：http://hz.xuetiantiany.cn/gtavjtnfjh.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.shanyushiyangkeji.top/gtfthidrdn.html

[E12] 统计某字符出现次数
来源：http://hz.kuanghao11.cn/gtcddfnnet.html

Py:   s.count("a")
来源：http://hz.jlsjyb.cn/gtlvizyqjy.html

PHP:  substr_count($s, "a");
来源：http://hz.gzhubu.top/gtfureyvhm.html

JS:   s.split("a").length - 1
来源：http://hz.yvedp.cn/gtramjfktb.html

TS:   s.split("a").length - 1
来源：http://hz.pycfn.com/gtcriyphrt.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.sysykeji.top/gtqpdcgypt.html

Go:   strings.Count(s, "a")
来源：http://hz.ivvv.top/gtfbzggvae.html

Ruby: s.count("a")
来源：http://hz.shanyushiyangtech.top/gtljxthbwd.html

C#:   s.Count(c => c == 'a')
来源：http://hz.yangfankeji.com/gtxescxbct.html

[E13] 逐字符遍历
来源：http://hz.yangfankeji.com/gteivbuzno.html

Py:   for ch in s: print(ch)
来源：http://hz.nwbrower.top/gtojtwppog.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.tian-w.cn/gtnhaupzir.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.snrcjt.cn/gtqlnykrcz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.nanxuanxn.top/gtcggxklsj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.316326.xyz/gtwmipqjhg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.ywan-chungtsiang.top/gtwqpjrghw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.mhx1999.top/gtwmqoqcdl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yj20258888.top/gtlszgluhp.html

[E14] URL 编码与 Base64
来源：http://hz.sweek.top/gtgkuqvheq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yonumen.top/gtellptcpt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.zycfv.cn/gtylyslsed.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yuxming.cn/gtxwoztxqy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.ybcxt.top/gteiujhggg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.havefunace.top/gtwnrmvjip.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.pengpengdd.cyou/gtzlwhfiar.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.ybcxt.top/gtkxswigid.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.gotoacloud.top/gtdcipyusd.html

[E15] HTML 转义 / 反转义
来源：http://hz.sufxvd.cn/gtnseugqad.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.wangshuangyany.cn/gtjjoblacz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.sufxvd.cn/gtcjdcrqaw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.316326.xyz/gtcifsujwp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yvedp.cn/gtmzwsdfjk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.gotoacloud.top/gtedsycuzg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.cucudq.cn/gtebxixxar.html


<!-- 参考信息 -->