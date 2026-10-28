代发 wailian999

TS:   arr.slice(1, 4);
来源：http://hz.yuxming.cn/gtwzjpqcpi.html

Java: list.subList(1, 4);
来源：http://hz.wangshuangyany.cn/gttaorddbe.html

Go:   arr[1:4]
来源：http://hz.cdnleiting.top/gtbarhojun.html

Ruby: arr[1, 3]
来源：http://hz.xuetiantiany.cn/gtwpahpbeh.html

C#:   list.GetRange(1, 3);
来源：http://hz.yuanzhike.top/gteovrfidf.html

[D08] 合并两个数组
来源：http://hz.chenjidiqi.icu/gtlzsojhqh.html

Py:   a + b;  a.extend(b)
来源：http://hz.zycfv.cn/gtdmvqyovn.html

PHP:  array_merge($a, $b);
来源：http://hz.vqdsnc.cn/gttfjwsjet.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.jianghu66.top/gteliemosh.html

TS:   [...a, ...b];
来源：http://hz.hfpthk.cn/gtvzfifgmd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.ehwqpu.com/gtfxiadeqj.html

Go:   append(a, b...)
来源：http://hz.nanxinkj.top/gtkixgbjho.html

Ruby: a + b;  a.concat(b)
来源：http://hz.hnqzz.top/gtxlsomlcq.html

C#:   a.Concat(b).ToList()
来源：http://hz.ppjwa.cn/gtnbqcwjsl.html

[D09] 排序（升序）
来源：http://hz.vqdsnc.cn/gtngvdpvpr.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.aibaodan.cn/gtedgkfegw.html

PHP:  sort($arr);
来源：http://hz.sysykeji.top/gtwssxmpfj.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.iojbl.cn/gtcpafwpdo.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.hysaishi.cn/gtibqgzjql.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.cheryme.top/gtnqvvecar.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.kuanghao11.cn/gtuzireuvz.html

Ruby: arr.sort
来源：http://hz.jinghuilouyu.cn/gtogpnoevk.html

C#:   list.Sort();
来源：http://hz.zhongyouzk.top/gthzgwsapm.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.mhx1999.top/gtaiupqnis.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yangfankeji.com/gtkxxijede.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.smart0.xyz/gtttmksvbm.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.haohaochexian.top/gtheuezdns.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yuxming.cn/gtrefbtigw.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.zhengqikj.top/gtkgkdmwhk.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.yuxming.cn/gtqvmhyarg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.fengsongda.top/gtyjlddndk.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.chenzaomai.com/gtkxoexcne.html

[D11] 反转数组
来源：http://hz.jianghu66.top/gtxsbghwbl.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.nanxinkj.top/gtodkulmhn.html

PHP:  array_reverse($arr);
来源：http://hz.yueranfly.top/gtjkvhpnum.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yj20258.top/gtavlvkgsu.html

TS:   [...arr].reverse();
来源：http://hz.svipenyu.cn/gtyzgyxibl.html

Java: Collections.reverse(list);
来源：http://hz.aizwys.cn/gtdusneqpf.html

Go:   slices.Reverse(arr)
来源：http://hz.chenlongwang.top/gtkoknltce.html

Ruby: arr.reverse
来源：http://hz.cqqwz.cn/gtkoaapmcr.html

C#:   list.Reverse();
来源：http://hz.shanyushiyangkeji.top/gtanstvhdd.html

[D12] 查找元素下标
来源：http://hz.cqqwz.cn/gtbtqmoxkh.html

Py:   arr.index(x);  x in arr
来源：http://hz.c1oappe.top/gtjeokikta.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.snrcjt.cn/gtnuehfljx.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.andypj.xyz/gtvmojeici.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.gogol.net.cn/gtelnzhizn.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.ydzc1.top/gtxgnugkxv.html

Go:   slices.Index(arr, x)
来源：http://hz.chenjidiqi.icu/gtqweurxtx.html

Ruby: arr.index(x)
来源：http://hz.yanxiufei.cn/gtodjtdecj.html

C#:   list.IndexOf(x);
来源：http://hz.nwbrower.top/gtvqrggyyy.html

[D13] 过滤（保留满足条件的）
来源：http://hz.redwolf501.top/gtogtntnwz.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.feifeiyinyue.top/gtxwefllbo.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.aibaodan.cn/gtytgradae.html

JS:   arr.filter(x => x > 3)
来源：http://hz.jianghu66.top/gtoxixrjsc.html

TS:   arr.filter(x => x > 3)
来源：http://hz.fzhhl.top/gtihkwyyve.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.aibaodan.cn/gttbovuaqk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.zycfv.cn/gtzguomgmm.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.ydjk.org.cn/gtflaxdrzc.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.ehwqpu.com/gtnyolliox.html

[D14] 映射转换（每个元素变形）
来源：http://hz.wangdashe.top/gtfpfdpkuc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.gzhubu.top/gtttbujsph.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.fzhhl.top/gtgxkknopu.html

JS:   arr.map(x => x * 2)
来源：http://hz.yueranfly.top/gtmgifypkc.html

TS:   arr.map(x => x * 2)
来源：http://hz.ehwqpu.com/gtxiqshwod.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.gogol.net.cn/gtbpxhbkdd.html

Go:   // 手写循环
来源：http://hz.ydzc1.top/gtbtylbhug.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.gzhubu.top/gtpgatrdhi.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.zdqjudy.top/gtlduwvroe.html

[D15] 去重
来源：http://hz.jqgfzy.top/gtmkknvnzy.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.quarkkingdee.top/gtiibbqsfw.html

PHP:  array_unique($arr);
来源：http://hz.jyoumei.cn/gtqyaxnwwx.html

JS:   [...new Set(arr)]
来源：http://hz.yuxming.cn/gttoribncw.html

TS:   [...new Set(arr)]
来源：http://hz.zhongyouzk.top/gtqgnlhnas.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.c1oappe.top/gtwcpjggnt.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.fzhhl.top/gtkpkwrybi.html

Ruby: arr.uniq
来源：http://hz.ybcxt.top/gtagelupkp.html

C#:   list.Distinct().ToList()
来源：http://hz.birdmap.top/gtlxgpkrgk.html

[D16] 求和与平均值
来源：http://hz.cheryme.top/gtriaoibil.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.zycfv.cn/gtspwctlse.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.zhixingplan.top/gtnyxeyzzk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jqgufenzy.top/gtrmrvyzue.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yonumen.top/gtjdlnazui.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.vqdsnc.cn/gtteqcbhsu.html

Go:   // 手写循环累加
来源：http://hz.dashuyun.cn/gtjiadnzsu.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.redwolf501.top/gtcskhvdxz.html

C#:   list.Sum();  list.Average()
来源：http://hz.jqgfzy.top/gtayfvbrlo.html

[D17] 最大值与最小值
来源：http://hz.cucudq.cn/gtahzzftdq.html

Py:   max(arr);  min(arr)
来源：http://hz.chenzaomai.com/gtswvflwmb.html

PHP:  max($arr);  min($arr);
来源：http://hz.hysaishi.cn/gtbksrsmcw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.hammf.cn/gtdabliypl.html

TS:   Math.max(...arr);
来源：http://hz.zhoulong.xyz/gtuthhlzfa.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.cashguo.top/gthkhqlppa.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.birdmap.top/gtbbqoyguo.html

Ruby: arr.max;  arr.min
来源：http://hz.wangshuangyany.cn/gtexjxjbsx.html

C#:   list.Max();  list.Min()
来源：http://hz.cheryme.top/gthktqdekz.html

[D18] 扁平化嵌套数组
来源：http://hz.yongpay.top/gtsyuwtppa.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.yj20258888.top/gtyxuklctb.html

PHP:  array_merge(...$nested);
来源：http://hz.zdqjudy.top/gtfblhbpej.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.yj20258888.top/gtxmizypqu.html

TS:   nested.flat();
来源：http://hz.feifeiyinyue.top/gtabtmyffd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.feifeiyinyue.top/gtyiwbfeut.html

Go:   // 手写双层循环
来源：http://hz.feifeiyinyue.top/gtcbhlihbo.html

Ruby: nested.flatten
来源：http://hz.redwolf501.top/gtiboztzqe.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.316326.xyz/gtedmyypyn.html

[D19] 按字段分组
来源：http://hz.smart0.xyz/gtwhamwvjo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.nwbrower.top/gtwzyfiwoq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.iojbl.cn/gtpyfzfloz.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jinyuanbaomall.cn/gtqfkwnmub.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.zhixingplan.top/gtcufgbzkv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.ybcxt.top/gtrzcbcuat.html

Go:   // 手写 map[string][]T
来源：http://hz.shzxlz.cn/gtyrvadkuy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.cqqwz.cn/gtsghylbmu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zhiwuduotai.top/gtysyylciw.html

[D20] 统计每个元素出现次数
来源：http://hz.aibaodan.cn/gtwcytqlyn.html

Py:   Counter(arr)
来源：http://hz.fengsongda.top/gtvvrmfxnz.html

PHP:  array_count_values($arr);
来源：http://hz.xinyue.icu/gtaxnrpdim.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.xylfe.cn/gtfdysnola.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zdqjudy.top/gtaiyrxlpq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.ehwqpu.com/gtvytcopnl.html

Go:   // 手写 map[T]int
来源：http://hz.gotoacloud.top/gtsvoppqsr.html

Ruby: arr.tally
来源：http://hz.sxryk.cn/gtibsogsrg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.ivvv.top/gtjaprvgya.html

[D21] 判断是否包含某元素
来源：http://hz.fzhhl.top/gtzuqsdyjz.html

Py:   x in arr
来源：http://hz.yueranfly.top/gtuexmcgdo.html

PHP:  in_array($x, $arr, true);
来源：http://hz.daxiang520.top/gtsmliqihm.html

JS:   arr.includes(x)
来源：http://hz.52xcode.cn/gtsnmqomow.html

TS:   arr.includes(x)
来源：http://hz.zhaomingkeji.xyz/gtvfiaujax.html

Java: list.contains(x)
来源：http://hz.zhongyouzk.top/gtusehlgdr.html

Go:   slices.Contains(arr, x)
来源：http://hz.52xcode.cn/gtalmfrvlb.html

Ruby: arr.include?(x)
来源：http://hz.fzhhl.top/gtfnbgdtsx.html

C#:   list.Contains(x)
来源：http://hz.wangdashe.top/gtfkpuozin.html

[D22] 复制数组（避免共享引用）
来源：http://hz.ydzc1.top/gtzywkeydp.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.bjfxy.top/gtorkwrola.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.zhongyouzk.top/gtfphiwlyy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.chenlongwang.top/gtrusybuzq.html

TS:   [...arr];
来源：http://hz.jinyuanbaomall.cn/gtadipslpz.html

Java: new ArrayList<>(list);
来源：http://hz.gogol.net.cn/gtsosobunz.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.tian-w.cn/gtoufcecqi.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jiagoushi.top/gtwcftrryj.html

C#:   new List<int>(list);
来源：http://hz.yueranfly.top/gtnenamvun.html

[D23] reduce 累积计算
来源：http://hz.yvedp.cn/gtxbeaiysf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.tian-w.cn/gtcqqvrmwt.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.pycfn.com/gtdpetvrxp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.daxiang520.top/gtevgjcnfq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.shanyushiyangtech.top/gtjguyxyse.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.cdnleiting.top/gtitpfnrga.html

Go:   // 手写循环
来源：http://hz.mhx1999.top/gtwpcncszs.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.hfpthk.cn/gtdfltxcud.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.chenlongwang.top/gtgmmgvbpr.html

[D24] 字典 / Map 基本操作
来源：http://hz.jlsjyb.cn/gtrtecsdos.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.fzhhl.top/gtrokkxzip.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.iojbl.cn/gtpqsweswu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.xingfuxueyuan.xyz/gtdkbhsvgm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.hnqzz.top/gtzvnrbnmc.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.fengsongda.top/gtvjenlsvy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ywan-chungtsiang.top/gtaltamnwb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.quarkkingdee.top/gtjcobvday.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.tanke756.top/gtgputrgkd.html

[D25] Set 集合去重与交并差
来源：http://hz.meibo888.top/gtpblqhjkv.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.hongshengwenyu.top/gtaobpfnua.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.xingfuxueyuan.xyz/gtokdttcwy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.fzhhl.top/gtveeqyafx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.0kj1m.cn/gtaffpybzg.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.aibaodan.cn/gtzurvpmpm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.cheryme.top/gtrcjhgdql.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.havefunace.top/gtrsooypzh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.ydzc1.top/gtjpmynqjo.html

[D26] 数组转字符串
来源：http://hz.gaohongyu789.top/gtxeotuvbp.html

Py:   ", ".join(map(str, arr))
来源：http://hz.aizwys.cn/gtpyxtpwnm.html

PHP:  implode(", ", $arr);
来源：http://hz.52xcode.cn/gtlysrovjp.html

JS:   arr.join(", ")
来源：http://hz.nanxuanxn.top/gtjlbkcvsb.html

TS:   arr.join(", ")
来源：http://hz.ydjk.org.cn/gtakmnysfm.html

Java: String.join(", ", list)
来源：http://hz.feifeiyinyue.top/gtziqlkxig.html

Go:   strings.Join(strs, ", ")
来源：http://hz.ppjwa.cn/gtvbjsttkg.html

Ruby: arr.join(", ")
来源：http://hz.ppjwa.cn/gtfbaitddo.html

C#:   string.Join(", ", list)
来源：http://hz.nanxuanxn.top/gttdwjhyfm.html

================================================================================
来源：http://hz.shanyushiyangkeji.top/gttqnzkbbg.html

E. 字符串处理
来源：http://hz.chenjidiqi.icu/gtncwhdbku.html

================================================================================
来源：http://hz.aibaodan.cn/gtfjcsqqqq.html

[E01] 拼接字符串
来源：http://hz.hnqzz.top/gtyiigeudy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.dianchejie.cn/gtluprzxxg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.svipenyu.cn/gtwkevjfhj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.daria6918.cn/gtzsdlasrg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.shangyingyoupin.top/gtdrprtpuz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.ivvv.top/gtyijjliwg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.aizwys.cn/gtsouzecao.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.fengsongda.top/gtmozoxofu.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.wangshuangyany.cn/gtlkgwdktz.html

[E02] 重复字符串
来源：http://hz.shangyingyoupin.top/gtyewxfhbk.html

Py:   "ab" * 3
来源：http://hz.yongpay.top/gtwnusxqvy.html

PHP:  str_repeat("ab", 3);
来源：http://hz.pycfn.com/gthhtbnlfq.html

JS:   "ab".repeat(3)
来源：http://hz.redwolf501.top/gttutbxsiy.html

TS:   "ab".repeat(3)
来源：http://hz.shangyingyoupin.top/gtdnsdwhmk.html

Java: "ab".repeat(3)
来源：http://hz.ydjk.org.cn/gtfwecemhe.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.yj202588.top/gtydfymunk.html

Ruby: "ab" * 3
来源：http://hz.sxryk.cn/gtovpagfvi.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.snrcjt.cn/gtmjbshvcn.html

[E03] 截取子串
来源：http://hz.zycfv.cn/gtsbwbofas.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.pycfn.com/gtihqdhept.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.yvedp.cn/gttnwbjneg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.gzhubu.top/gtftzxthjn.html

TS:   s.slice(1, 4)
来源：http://hz.xuetiantiany.cn/gtavofbrns.html

Java: s.substring(1, 4)
来源：http://hz.zhongyouzk.top/gtuirtpqto.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.pycfn.com/gtblbxfozh.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.yueranfly.top/gtkajnsrou.html

C#:   s.Substring(1, 3)
来源：http://hz.zhijiandao.cn/gtcxfcrfca.html

[E04] 查找子串位置
来源：http://hz.gzhubu.top/gtxohfzlar.html

Py:   s.find("x");  s.index("x")
来源：http://hz.chenlongwang.top/gtkvwfkhgr.html

PHP:  strpos($s, "x");
来源：http://hz.birdmap.top/gtxndghbjb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.wangshuangyany.cn/gtmukmykis.html

TS:   s.indexOf("x")
来源：http://hz.andypj.xyz/gtahypgnim.html

Java: s.indexOf("x")
来源：http://hz.jiagoushi.top/gthmccnbej.html

Go:   strings.Index(s, "x")
来源：http://hz.fengsongda.top/gtzjebgymm.html

Ruby: s.index("x")
来源：http://hz.kuanghao11.cn/gtonwagkkj.html

C#:   s.IndexOf("x")
来源：http://hz.cashguo.top/gthtwmqtvq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.tian-w.cn/gttbrrsuax.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.yueranfly.top/gtuoyowgrh.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.xylfe.cn/gtvdwzybib.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hywenlv.cn/gtrsbdloaf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zhongyouzk.top/gtdjtbgrzv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.fzhhl.top/gtmtgzypuf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.mhx1999.top/gteymwbkzi.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.chenlongwang.top/gtsdlmralo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.guowangkeji.top/gtvdnekgea.html

[E06] 替换子串
来源：http://hz.ywan-chungtsiang.top/gthcfhwhje.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.zdqjudy.top/gtkesemacn.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.bjfxy.top/gtjxdzqayn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yvedp.cn/gtjmjekgjw.html

TS:   s.replaceAll("a", "b")
来源：http://hz.meibo888.top/gtcefdmgao.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.svipenyu.cn/gtdfxutdch.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.zhengqikj.top/gtfhhatoho.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.aizwys.cn/gtlrzalfxd.html

C#:   s.Replace("a", "b")
来源：http://hz.ydzc1.top/gtlerijexh.html

[E07] 按分隔符拆分
来源：http://hz.jinyuanbaomall.cn/gthjzhmkib.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.xziqi.cn/gtarpnuzvw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.ydjk.org.cn/gtnmxgpeku.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.smart0.xyz/gtzmkmzcxb.html

TS:   s.split(",")
来源：http://hz.gzhubu.top/gtygwewkop.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.yanxiufei.cn/gtmitsrmqp.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.svipenyu.cn/gtusepynrh.html

Ruby: s.split(",");  s.split
来源：http://hz.jlsjyb.cn/gtctgxsldt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.dashuyun.cn/gttoqwtvkw.html

[E08] 数组按分隔符合并
来源：http://hz.yongpay.top/gtivjsfhfr.html

Py:   ",".join(items)
来源：http://hz.sweek.top/gtwrkpebhw.html

PHP:  implode(",", $items);
来源：http://hz.0kj1m.cn/gtssejkchj.html

JS:   items.join(",")
来源：http://hz.9152youxi.cn/gtylnnsufg.html

TS:   items.join(",")
来源：http://hz.yonumen.top/gtfmbadatr.html

Java: String.join(",", items)
来源：http://hz.zhijiandao.cn/gtbxmirhil.html

Go:   strings.Join(items, ",")
来源：http://hz.jinyuanbaomall.cn/gtwajpwxki.html

Ruby: items.join(",")
来源：http://hz.yj20258.top/gtjfjpwzla.html

C#:   string.Join(",", items)
来源：http://hz.c1oappe.top/gtrnzvcmup.html

[E09] 去除所有空白字符
来源：http://hz.hnxiangtu.top/gtbzhufhmx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jlsjyb.cn/gtfxzkvzdr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.shanyushiyangkeji.top/gtzsulgjlr.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jinqigufen.top/gtqarldymo.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.hongshengwenyu.top/gtsgmcinyc.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.kuanghao11.cn/gtjdriursc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.ydzc1.top/gtpphjhshs.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.nanxinkj.top/gthgydfwql.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yvedp.cn/gtbkiywiad.html

[E10] 左侧补零 / 定长填充
来源：http://hz.316326.xyz/gthpfkooqn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.hywenlv.cn/gtbpdznbdq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.redwolf501.top/gtjuzvfkpo.html

JS:   "7".padStart(3, "0")
来源：http://hz.dashuyun.cn/gtpnicxlng.html

TS:   "7".padStart(3, "0")
来源：http://hz.ywan-chungtsiang.top/gtsyyzivjn.html

Java: String.format("%03d", 7)
来源：http://hz.havefunace.top/gtabjsbepf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.xuetiantiany.cn/gthkijslze.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.shangyingyoupin.top/gtuomzwqeu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.hnxiangtu.top/gttewtqeuf.html

[E11] 反转字符串
来源：http://hz.zhaomingkeji.xyz/gtllswfrer.html

Py:   s[::-1]
来源：http://hz.feifeiyinyue.top/gtmrheaowf.html

PHP:  strrev($s);
来源：http://hz.xingfuxueyuan.xyz/gtzbtkqswn.html

JS:   [...s].reverse().join("")
来源：http://hz.jqgfzy.top/gtmzkfzotb.html

TS:   [...s].reverse().join("")
来源：http://hz.yj20258.top/gtymewolmt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.meibo888.top/gtzljfffiz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.ybcxt.top/gtpzdtdorg.html

Ruby: s.reverse
来源：http://hz.redwolf501.top/gtqiuzfcwi.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.fzhhl.top/gtknkttigl.html

[E12] 统计某字符出现次数
来源：http://hz.jlsjyb.cn/gtxdkuzueq.html

Py:   s.count("a")
来源：http://hz.c1oappe.top/gtzigaahyc.html

PHP:  substr_count($s, "a");
来源：http://hz.zhongyouzk.top/gtitxchmtj.html

JS:   s.split("a").length - 1
来源：http://hz.zycfv.cn/gthzirunno.html

TS:   s.split("a").length - 1
来源：http://hz.gotoacloud.top/gtdwhfblvi.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.ivvv.top/gtpmyemgdx.html

Go:   strings.Count(s, "a")
来源：http://hz.yvedp.cn/gtohbxcdzi.html

Ruby: s.count("a")
来源：http://hz.shanyushiyangkeji.top/gtqepenpcc.html

C#:   s.Count(c => c == 'a')
来源：http://hz.nwbrower.top/gtjwltamcg.html

[E13] 逐字符遍历
来源：http://hz.dashuyun.cn/gtpllxlnuw.html

Py:   for ch in s: print(ch)
来源：http://hz.yueranfly.top/gtgwgiravf.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.cdnleiting.top/gtqyuiiqmr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.nanxuanxn.top/gtgqizglwy.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yangfankeji.com/gtelyqiphl.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.xziqi.cn/gtppwmidhj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.sufxvd.cn/gtxpagucoh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.52xcode.cn/gtpbrkbtjd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.nanxinkj.top/gtjzbgdbzj.html

[E14] URL 编码与 Base64
来源：http://hz.svipenyu.cn/gtakccmczb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.chenlongwang.top/gtrcjhvnuy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yonumen.top/gtdxlpxzek.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.bjfxy.top/gtugvehyfl.html


<!-- 参考信息 -->