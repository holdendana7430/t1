代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://hz.yj20258.top/gtnzbjmodc.html

[D08] 合并两个数组
来源：http://hz.nwbrower.top/gtdxzhuwvi.html

Py:   a + b;  a.extend(b)
来源：http://hz.jlsjyb.cn/gtnvbltpvy.html

PHP:  array_merge($a, $b);
来源：http://hz.jinyuanbaomall.cn/gtgrpuqdos.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.yj20258888.top/gtnncpfgma.html

TS:   [...a, ...b];
来源：http://hz.pengpengdd.cyou/gtcasivnuk.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.9152youxi.cn/gtubqkcbxe.html

Go:   append(a, b...)
来源：http://hz.zycfv.cn/gtxgelrnzt.html

Ruby: a + b;  a.concat(b)
来源：http://hz.shuidangran.top/gtzwzbgvao.html

C#:   a.Concat(b).ToList()
来源：http://hz.andypj.xyz/gthfatszel.html

[D09] 排序（升序）
来源：http://hz.ydzc1.top/gtveebifdk.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.shzxlz.cn/gtqwtmdfgq.html

PHP:  sort($arr);
来源：http://hz.jlsjyb.cn/gtkaidqguv.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.cashguo.top/gtctuhmfpg.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.sweek.top/gtdmestftj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.fzhhl.top/gtjldocjkr.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.fengsongda.top/gtjaevoust.html

Ruby: arr.sort
来源：http://hz.yongpay.top/gtxgzuubci.html

C#:   list.Sort();
来源：http://hz.shangyingyoupin.top/gtlyabtvdv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.dashuyun.cn/gtrmgmbfcf.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.yongpay.top/gtdygmamwj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.jqgufenzy.top/gtfshnaird.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yangfankeji.com/gtvtrjxwrq.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ydzc1.top/gtirmmruwz.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.hongshengwenyu.top/gtidubmsyt.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.dianchejie.cn/gtxewyaoqb.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.dianchejie.cn/gtuwioqxxt.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.zhixingplan.top/gtzmnwyutc.html

[D11] 反转数组
来源：http://hz.bjfxy.top/gtelcczvfp.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.tanke756.top/gtghnglrrm.html

PHP:  array_reverse($arr);
来源：http://hz.ivvv.top/gtnzbjjijc.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.yanxiufei.cn/gtxstiomoh.html

TS:   [...arr].reverse();
来源：http://hz.jiagoushi.top/gtngtymxfz.html

Java: Collections.reverse(list);
来源：http://hz.shanyushiyangkeji.top/gtfetdvviw.html

Go:   slices.Reverse(arr)
来源：http://hz.jianghu66.top/gtwdfxmqyl.html

Ruby: arr.reverse
来源：http://hz.daxiang520.top/gtimsjifkh.html

C#:   list.Reverse();
来源：http://hz.mhx1999.top/gtpuxlpfbl.html

[D12] 查找元素下标
来源：http://hz.shzxlz.cn/gtqwfsmqnu.html

Py:   arr.index(x);  x in arr
来源：http://hz.ybcxt.top/gtlrjgazpc.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.hnqzz.top/gtgloyknwn.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.aizwys.cn/gtqyhaedws.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.gotoacloud.top/gtnxbuooyc.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.ywan-chungtsiang.top/gtkfjhfaqq.html

Go:   slices.Index(arr, x)
来源：http://hz.sweek.top/gtzvhnwnso.html

Ruby: arr.index(x)
来源：http://hz.9152youxi.cn/gtgufqzgxv.html

C#:   list.IndexOf(x);
来源：http://hz.aibaodan.cn/gtmbgrifna.html

[D13] 过滤（保留满足条件的）
来源：http://hz.0kj1m.cn/gtfyaxkarf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.cashguo.top/gtuhvbgwdl.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.xuetiantiany.cn/gthhuhkgtp.html

JS:   arr.filter(x => x > 3)
来源：http://hz.zhengqikj.top/gtqjdfqeaj.html

TS:   arr.filter(x => x > 3)
来源：http://hz.xuetiantiany.cn/gtmjrygsnf.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.ywan-chungtsiang.top/gtgcezcdoo.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.xziqi.cn/gtycuukyzr.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.xuanzx.com/gtdljbsvub.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.ywan-chungtsiang.top/gtwhnxyswt.html

[D14] 映射转换（每个元素变形）
来源：http://hz.haohaochexian.top/gtzobfvewx.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.mhx1999.top/gtdniyhwgq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.sweek.top/gtoqauaiwj.html

JS:   arr.map(x => x * 2)
来源：http://hz.andypj.xyz/gtnuymybnq.html

TS:   arr.map(x => x * 2)
来源：http://hz.cashguo.top/gtgmpznmbl.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.shanyushiyangtech.top/gtsfwtqabe.html

Go:   // 手写循环
来源：http://hz.daria6918.cn/gtkflvnzds.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.wangdashe.top/gtttrbjjvs.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.cqqwz.cn/gtbbzjzlyf.html

[D15] 去重
来源：http://hz.shuidangran.top/gtuqxibnjc.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.yueranfly.top/gtcpvpgile.html

PHP:  array_unique($arr);
来源：http://hz.zhijiandao.cn/gtuzpaunaa.html

JS:   [...new Set(arr)]
来源：http://hz.jqgufenzy.top/gtjlwcanjt.html

TS:   [...new Set(arr)]
来源：http://hz.shanyushiyangtech.top/gtgtnnahqu.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.jiagoushi.top/gtxgnhciip.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.yonumen.top/gtfejijkha.html

Ruby: arr.uniq
来源：http://hz.yvedp.cn/gtnnvvwlkr.html

C#:   list.Distinct().ToList()
来源：http://hz.0kj1m.cn/gtaiudqlqg.html

[D16] 求和与平均值
来源：http://hz.cdnleiting.top/gtnvfduogi.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.havefunace.top/gtavmigrnd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.dashuyun.cn/gtpkqwzvyk.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zycfv.cn/gtgrqbjrwu.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.jqgufenzy.top/gtfklinbon.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.ywan-chungtsiang.top/gtxhcoyjld.html

Go:   // 手写循环累加
来源：http://hz.shuidangran.top/gtctghyxji.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.zhixingplan.top/gtcrkbejts.html

C#:   list.Sum();  list.Average()
来源：http://hz.tian-w.cn/gtwxzzxasi.html

[D17] 最大值与最小值
来源：http://hz.hfpthk.cn/gtllnfvtcn.html

Py:   max(arr);  min(arr)
来源：http://hz.hongshengwenyu.top/gtbpzekmqv.html

PHP:  max($arr);  min($arr);
来源：http://hz.svipenyu.cn/gtdhxdbvai.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.9152youxi.cn/gtdijkqcuy.html

TS:   Math.max(...arr);
来源：http://hz.yangfankeji.com/gtwcldzder.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.shuidangran.top/gtisqefapi.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.wangdashe.top/gtudssxaed.html

Ruby: arr.max;  arr.min
来源：http://hz.chenzaomai.com/gtuqkchnng.html

C#:   list.Max();  list.Min()
来源：http://hz.hysaishi.cn/gterowfilh.html

[D18] 扁平化嵌套数组
来源：http://hz.zhoulong.xyz/gtvdwvnlso.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.hywenlv.cn/gtccklbgos.html

PHP:  array_merge(...$nested);
来源：http://hz.jinqigfzy.top/gtwxjxjcmp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.cqqwz.cn/gtzfwtyqeu.html

TS:   nested.flat();
来源：http://hz.yueranfly.top/gtbtrjebzq.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.cashguo.top/gtlhrjinid.html

Go:   // 手写双层循环
来源：http://hz.smart0.xyz/gttdtdmtra.html

Ruby: nested.flatten
来源：http://hz.yuxming.cn/gtegpimghz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.ydjk.org.cn/gtvuhrrnqi.html

[D19] 按字段分组
来源：http://hz.zhijiandao.cn/gtvnqlpylw.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.hnxiangtu.top/gtlzaitpvi.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.redwolf501.top/gtbfekkazi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.jqgufenzy.top/gtqtrkcwdd.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.sxryk.cn/gttayxaevx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.xziqi.cn/gtazdhcblf.html

Go:   // 手写 map[string][]T
来源：http://hz.havefunace.top/gtthuhzkty.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.kuanghao11.cn/gtwaqtsill.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.shangyingyoupin.top/gtdnmjnfzo.html

[D20] 统计每个元素出现次数
来源：http://hz.andypj.xyz/gtexyoxocx.html

Py:   Counter(arr)
来源：http://hz.yj20258888.top/gtpmribffm.html

PHP:  array_count_values($arr);
来源：http://hz.iojbl.cn/gttxdmszse.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.gotoacloud.top/gtjoaoniwl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.zhaomingkeji.xyz/gtpxzcedpa.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.fzhhl.top/gtgxyyybar.html

Go:   // 手写 map[T]int
来源：http://hz.bjfxy.top/gtnymkcugc.html

Ruby: arr.tally
来源：http://hz.zycfv.cn/gtaguqlcxm.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.xuetiantiany.cn/gtbxallbxy.html

[D21] 判断是否包含某元素
来源：http://hz.ywan-chungtsiang.top/gtwctxkjau.html

Py:   x in arr
来源：http://hz.smart0.xyz/gtrhvqzpgc.html

PHP:  in_array($x, $arr, true);
来源：http://hz.daxiang520.top/gtfsvjqhjk.html

JS:   arr.includes(x)
来源：http://hz.kuanghao11.cn/gtodzgkcjp.html

TS:   arr.includes(x)
来源：http://hz.yueranfly.top/gtwbjoqwxi.html

Java: list.contains(x)
来源：http://hz.guannengcc.top/gtbtluvsbb.html

Go:   slices.Contains(arr, x)
来源：http://hz.ppjwa.cn/gttxhleyih.html

Ruby: arr.include?(x)
来源：http://hz.zhongyouzk.top/gtkimqyrzm.html

C#:   list.Contains(x)
来源：http://hz.vqdsnc.cn/gtfysugzps.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jiagoushi.top/gtykxcjyve.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.gogol.net.cn/gthjroafet.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.chenjidiqi.icu/gtytvlhjct.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.sysykeji.top/gtlrqhrbpb.html

TS:   [...arr];
来源：http://hz.svipenyu.cn/gtipnndegn.html

Java: new ArrayList<>(list);
来源：http://hz.xuetiantiany.cn/gtyqzafkcn.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.jinghuilouyu.cn/gteotmwpjk.html

Ruby: arr.dup;  arr.clone
来源：http://hz.aizwys.cn/gtxsifqvji.html

C#:   new List<int>(list);
来源：http://hz.shzxlz.cn/gtfrygqrxm.html

[D23] reduce 累积计算
来源：http://hz.zycfv.cn/gtrepryawn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.wangdashe.top/gtmbcxszoh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.yueranfly.top/gtsvuaxfhu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.jinqigufen.top/gtvvowdrfe.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.daria6918.cn/gtydbvyzql.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.9152youxi.cn/gtazirdaix.html

Go:   // 手写循环
来源：http://hz.hysaishi.cn/gtmvtnchfc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.hysaishi.cn/gtdjwaejix.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.iojbl.cn/gtqjpijssk.html

[D24] 字典 / Map 基本操作
来源：http://hz.hammf.cn/gttrkjtnec.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.nwbrower.top/gtrafydkkh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.xuanzx.com/gtnjfgqixd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.pengpengdd.cyou/gtyihknrta.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.ybcxt.top/gtrxbvmrjk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.vqdsnc.cn/gtcsgaqqnn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.ehwqpu.com/gtfgfgvbxc.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.nanxinkj.top/gtezeardnc.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.gogol.net.cn/gtfwaegxkc.html

[D25] Set 集合去重与交并差
来源：http://hz.meibo888.top/gtigeooivd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.shangyingyoupin.top/gtehfjruct.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.xylfe.cn/gtiyqlures.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yj202588.top/gthsaxwiic.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.sxryk.cn/gtuqeeweed.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.cashguo.top/gtqfqnzncl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.yvedp.cn/gtnkksndwx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.dianchejie.cn/gtjpuqcgko.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.tanke756.top/gtkqllmbtd.html

[D26] 数组转字符串
来源：http://hz.nwbrower.top/gthnweqske.html

Py:   ", ".join(map(str, arr))
来源：http://hz.pycfn.com/gtugazpwzg.html

PHP:  implode(", ", $arr);
来源：http://hz.hammf.cn/gtmtpahrfr.html

JS:   arr.join(", ")
来源：http://hz.hammf.cn/gtalfxsnru.html

TS:   arr.join(", ")
来源：http://hz.xylfe.cn/gtijgrzoiu.html

Java: String.join(", ", list)
来源：http://hz.zdqjudy.top/gtpwraeorx.html

Go:   strings.Join(strs, ", ")
来源：http://hz.zhaomingkeji.xyz/gtrolgrdwk.html

Ruby: arr.join(", ")
来源：http://hz.gogol.net.cn/gtljouukra.html

C#:   string.Join(", ", list)
来源：http://hz.hnxiangtu.top/gtxfwxcscj.html

================================================================================
来源：http://hz.havefunace.top/gtqjxonyfh.html

E. 字符串处理
来源：http://hz.9152youxi.cn/gtlpjkdkfe.html

================================================================================
来源：http://hz.cashguo.top/gtslxyrhxu.html

[E01] 拼接字符串
来源：http://hz.hongshengwenyu.top/gtehepqfxe.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.cdnleiting.top/gtmwwlhrri.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.chenjidiqi.icu/gtwrjugpoo.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jqgfzy.top/gtmimyueky.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.xziqi.cn/gtabvlirrr.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.9152youxi.cn/gtjsifjgsw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.zhijiandao.cn/gtoplmovrk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.sxryk.cn/gtveiexbyc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.chenjidiqi.icu/gtylsxgaku.html

[E02] 重复字符串
来源：http://hz.dashuyun.cn/gtrzcyofsa.html

Py:   "ab" * 3
来源：http://hz.bjfxy.top/gtxhemtgxd.html

PHP:  str_repeat("ab", 3);
来源：http://hz.hfpthk.cn/gtdqcxkvex.html

JS:   "ab".repeat(3)
来源：http://hz.sufxvd.cn/gtgncunivq.html

TS:   "ab".repeat(3)
来源：http://hz.ydjk.org.cn/gtksfrkoia.html

Java: "ab".repeat(3)
来源：http://hz.316326.xyz/gtkcolksbb.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.zdqjudy.top/gttxqwtbgx.html

Ruby: "ab" * 3
来源：http://hz.smart0.xyz/gtkuhxekhp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.xinyue.icu/gtxnyquyuz.html

[E03] 截取子串
来源：http://hz.jinqigfzy.top/gtyxqflkod.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.xziqi.cn/gtkzjrhqnz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.quarkkingdee.top/gtecaxxzui.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.zhoulong.xyz/gtbwpaxjrk.html

TS:   s.slice(1, 4)
来源：http://hz.52xcode.cn/gtbwcfilzb.html

Java: s.substring(1, 4)
来源：http://hz.feifeiyinyue.top/gtpmjjufxk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.hongshengwenyu.top/gtkaksrckw.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.fzhhl.top/gteulsginx.html

C#:   s.Substring(1, 3)
来源：http://hz.dianchejie.cn/gtwnsdueux.html

[E04] 查找子串位置
来源：http://hz.316326.xyz/gtxgfibpph.html

Py:   s.find("x");  s.index("x")
来源：http://hz.fzhhl.top/gtkmhpzdvz.html

PHP:  strpos($s, "x");
来源：http://hz.wangshuangyany.cn/gtikjgkdwr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zhoulong.xyz/gtonqaoaya.html

TS:   s.indexOf("x")
来源：http://hz.zhongyouzk.top/gtouepeuti.html

Java: s.indexOf("x")
来源：http://hz.zhoulong.xyz/gtwpiqcgjq.html

Go:   strings.Index(s, "x")
来源：http://hz.birdmap.top/gtuokrxffe.html

Ruby: s.index("x")
来源：http://hz.tianlin.xyz/gtsookdgsf.html

C#:   s.IndexOf("x")
来源：http://hz.9152youxi.cn/gtpditchze.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.yvedp.cn/gtdyikbtqs.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.feifeiyinyue.top/gtafmhimsp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.jinqigfzy.top/gtpyckyptn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.svipenyu.cn/gtdlgxrqfz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.ppjwa.cn/gtbbuwjxhe.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.hongshengwenyu.top/gtitlyrqeo.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.svipenyu.cn/gtkerkczdx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.meibo888.top/gtzitvpgul.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.xinyue.icu/gtcxkzbcmn.html

[E06] 替换子串
来源：http://hz.mhx1999.top/gtpgvjreti.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.jiagoushi.top/gtpiarebkm.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.mhx1999.top/gtgohzpweh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hnxiangtu.top/gtabkzcthm.html

TS:   s.replaceAll("a", "b")
来源：http://hz.jqgfzy.top/gtveajuxlq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.gzhubu.top/gtkrcjjnfr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.snrcjt.cn/gtghhffmwg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.jqgfzy.top/gtlsqenruy.html

C#:   s.Replace("a", "b")
来源：http://hz.0kj1m.cn/gtppzluqli.html

[E07] 按分隔符拆分
来源：http://hz.ivvv.top/gtzubmagtr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.ppjwa.cn/gtmbizmirs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yuxming.cn/gtzgfwsscd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.dashuyun.cn/gtqysxublt.html

TS:   s.split(",")
来源：http://hz.nwbrower.top/gtzwsxaatr.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.fengsongda.top/gtgooathoe.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.iojbl.cn/gtwcjiwwmq.html

Ruby: s.split(",");  s.split
来源：http://hz.sysykeji.top/gtgvxcnrrb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.zycfv.cn/gtxvgzzmly.html

[E08] 数组按分隔符合并
来源：http://hz.316326.xyz/gtuybjizpn.html

Py:   ",".join(items)
来源：http://hz.daria6918.cn/gttvdwppji.html

PHP:  implode(",", $items);
来源：http://hz.daria6918.cn/gtdlkcggrz.html

JS:   items.join(",")
来源：http://hz.redwolf501.top/gtjxqtggwr.html

TS:   items.join(",")
来源：http://hz.aizwys.cn/gtgoqkounf.html

Java: String.join(",", items)
来源：http://hz.hammf.cn/gttufgqmnv.html

Go:   strings.Join(items, ",")
来源：http://hz.shanyushiyangtech.top/gtboggjosg.html

Ruby: items.join(",")
来源：http://hz.xylfe.cn/gtvrgycbnr.html

C#:   string.Join(",", items)
来源：http://hz.guowangkeji.top/gtjmjxtynu.html

[E09] 去除所有空白字符
来源：http://hz.chenzaomai.com/gtflszxrcq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.fzhhl.top/gtgjzuedfp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.zdqjudy.top/gthgcfokuo.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jinqigfzy.top/gtvpbmriua.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.fzhhl.top/gtdpytkcto.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.fengsongda.top/gtmpjljebn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.meibo888.top/gtkbcbxale.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.xziqi.cn/gthnodxxft.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.zhixingplan.top/gtncaivota.html

[E10] 左侧补零 / 定长填充
来源：http://hz.xinyue.icu/gtgmswspxw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.wangshuangyany.cn/gtsuwvvxyj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.yonumen.top/gtosonxqvj.html

JS:   "7".padStart(3, "0")
来源：http://hz.snrcjt.cn/gtmlalfenl.html

TS:   "7".padStart(3, "0")
来源：http://hz.gzhubu.top/gtwfqdjjcz.html

Java: String.format("%03d", 7)
来源：http://hz.wangshuangyany.cn/gtagujlgjt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.svipenyu.cn/gtyawughqn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.chenlongwang.top/gtilkokzow.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.snrcjt.cn/gtuwdddzrt.html

[E11] 反转字符串
来源：http://hz.zhijiandao.cn/gtxggjditu.html

Py:   s[::-1]
来源：http://hz.jinghuilouyu.cn/gtdjchahqt.html

PHP:  strrev($s);
来源：http://hz.jinqigufen.top/gtotfsmyti.html

JS:   [...s].reverse().join("")
来源：http://hz.jyoumei.cn/gtmlwmdmeh.html

TS:   [...s].reverse().join("")
来源：http://hz.zhengqikj.top/gtkjlmdmwa.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.ehwqpu.com/gtnzkywglw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zhengqikj.top/gtxrszwwir.html

Ruby: s.reverse
来源：http://hz.yonumen.top/gtjzeyozon.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.tianlin.xyz/gtpqwkslii.html

[E12] 统计某字符出现次数
来源：http://hz.xuetiantiany.cn/gtlcatnpzj.html

Py:   s.count("a")
来源：http://hz.xylfe.cn/gtzjnoxzxd.html

PHP:  substr_count($s, "a");
来源：http://hz.zhaomingkeji.xyz/gthuehurkq.html

JS:   s.split("a").length - 1
来源：http://hz.yonumen.top/gthsiliwwa.html

TS:   s.split("a").length - 1
来源：http://hz.chenjidiqi.icu/gttscljyox.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.zhengqikj.top/gtaejduwre.html

Go:   strings.Count(s, "a")
来源：http://hz.hfpthk.cn/gtlupouakg.html

Ruby: s.count("a")
来源：http://hz.gotoacloud.top/gtwfbwgssb.html

C#:   s.Count(c => c == 'a')
来源：http://hz.tanke756.top/gtrluicvil.html

[E13] 逐字符遍历
来源：http://hz.shuidangran.top/gtfvrrgpwf.html

Py:   for ch in s: print(ch)
来源：http://hz.gaohongyu789.top/gtohkmdrkr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.sweek.top/gtimxxvgbt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.ydzc1.top/gtmywshtyu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.wangshuangyany.cn/gtuamipwjn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.gzhubu.top/gtypwbgwqa.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.redwolf501.top/gtyizefkcq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.shuidangran.top/gtuasjpiwr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jinqigfzy.top/gthtnjafrb.html

[E14] URL 编码与 Base64
来源：http://hz.52xcode.cn/gtqgxmahav.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.fzhhl.top/gtibfwmpxg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.guannengcc.top/gtlpusjmlp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.snrcjt.cn/gtjrgifevp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.316326.xyz/gtusmvscbm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.snrcjt.cn/gtrnalpyey.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.cashguo.top/gthjdlpcaj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jianghu66.top/gtyjnjkrdf.html


<!-- 参考信息 -->