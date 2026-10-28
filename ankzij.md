代发 wailian999

C#:   list.GetRange(1, 3);
来源：http://hz.ehwqpu.com/gtxwwcjinf.html

[D08] 合并两个数组
来源：http://hz.meibo888.top/gtagndnmiw.html

Py:   a + b;  a.extend(b)
来源：http://hz.yvedp.cn/gtbrghzpwd.html

PHP:  array_merge($a, $b);
来源：http://hz.tanke756.top/gtvrtbsnga.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.aizwys.cn/gtzigbygka.html

TS:   [...a, ...b];
来源：http://hz.vqdsnc.cn/gtjmfpbnmd.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.aibaodan.cn/gtpxonflpd.html

Go:   append(a, b...)
来源：http://hz.shangyingyoupin.top/gtnwryyesu.html

Ruby: a + b;  a.concat(b)
来源：http://hz.shzxlz.cn/gtiuxtkcth.html

C#:   a.Concat(b).ToList()
来源：http://hz.316326.xyz/gttdsymsrf.html

[D09] 排序（升序）
来源：http://hz.gogol.net.cn/gtqderafij.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.sxryk.cn/gtgwpodxkn.html

PHP:  sort($arr);
来源：http://hz.hfpthk.cn/gtqvdsblbi.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.birdmap.top/gtdbxcfpgx.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.tianlin.xyz/gtgwjzkwvr.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.cheryme.top/gtunisvtuv.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.tianlin.xyz/gtfgpuwdms.html

Ruby: arr.sort
来源：http://hz.zhaomingkeji.xyz/gtjkqwpioj.html

C#:   list.Sort();
来源：http://hz.guowangkeji.top/gtebzfyjke.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.jyoumei.cn/gtezasrvys.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.dianchejie.cn/gtwytbaqfp.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.zycfv.cn/gtgwvpbkzw.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yj20258.top/gtkhvwezds.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.sxryk.cn/gtzfhpvkpp.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.feifeiyinyue.top/gtnboqzmzi.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.ydjk.org.cn/gtdwvqrjqg.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.chenjidiqi.icu/gtweqnlhyb.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.c1oappe.top/gtjttjxnli.html

[D11] 反转数组
来源：http://hz.zycfv.cn/gtqmyjlokm.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.jqgufenzy.top/gtcufgnzsc.html

PHP:  array_reverse($arr);
来源：http://hz.haohaochexian.top/gtptsjiuui.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.shangyingyoupin.top/gtgndlnvns.html

TS:   [...arr].reverse();
来源：http://hz.sweek.top/gthrwmkvbs.html

Java: Collections.reverse(list);
来源：http://hz.yvedp.cn/gtrbbghouk.html

Go:   slices.Reverse(arr)
来源：http://hz.yonumen.top/gteegqgduo.html

Ruby: arr.reverse
来源：http://hz.hammf.cn/gtsbzyrlre.html

C#:   list.Reverse();
来源：http://hz.daxiang520.top/gtngextyop.html

[D12] 查找元素下标
来源：http://hz.xylfe.cn/gtiaddecfa.html

Py:   arr.index(x);  x in arr
来源：http://hz.redwolf501.top/gttnkkmhes.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.ppjwa.cn/gtyicyazoi.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ybcxt.top/gtawhnmtjv.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.cqqwz.cn/gtfqpkszex.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.xziqi.cn/gtbztwuaue.html

Go:   slices.Index(arr, x)
来源：http://hz.xziqi.cn/gtwpesqfsr.html

Ruby: arr.index(x)
来源：http://hz.316326.xyz/gtfajljsqv.html

C#:   list.IndexOf(x);
来源：http://hz.yj202588.top/gtsifefhxu.html

[D13] 过滤（保留满足条件的）
来源：http://hz.daria6918.cn/gtcptfyqsl.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.zhengqikj.top/gtlvsgmmaa.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.nwbrower.top/gtziplpmle.html

JS:   arr.filter(x => x > 3)
来源：http://hz.hysaishi.cn/gtcvxzmltk.html

TS:   arr.filter(x => x > 3)
来源：http://hz.snrcjt.cn/gtajfljeft.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.smart0.xyz/gteapaywie.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.pycfn.com/gthlobbsks.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.chenjidiqi.icu/gtadjuesei.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.shzxlz.cn/gtylczpjzj.html

[D14] 映射转换（每个元素变形）
来源：http://hz.jqgufenzy.top/gtrymvhfld.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.chenzaomai.com/gtsrxgrmgi.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.zhixingplan.top/gtmmixdnpu.html

JS:   arr.map(x => x * 2)
来源：http://hz.yueranfly.top/gtjhlosven.html

TS:   arr.map(x => x * 2)
来源：http://hz.chenzaomai.com/gtjnmoijgy.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.xziqi.cn/gtmrnybpqb.html

Go:   // 手写循环
来源：http://hz.guannengcc.top/gtmjjhsiun.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.52xcode.cn/gtqalqtetg.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.ywan-chungtsiang.top/gtuvwpxqpq.html

[D15] 去重
来源：http://hz.daria6918.cn/gtrolsbuao.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.snrcjt.cn/gtsilrjzur.html

PHP:  array_unique($arr);
来源：http://hz.yvedp.cn/gtverrsreq.html

JS:   [...new Set(arr)]
来源：http://hz.aizwys.cn/gtoztapbbe.html

TS:   [...new Set(arr)]
来源：http://hz.chenjidiqi.icu/gtpmpfmiun.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.snrcjt.cn/gtavebejbn.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.gaohongyu789.top/gtmczbdizg.html

Ruby: arr.uniq
来源：http://hz.hongshengwenyu.top/gtdgjlydkd.html

C#:   list.Distinct().ToList()
来源：http://hz.sweek.top/gtiheaytmy.html

[D16] 求和与平均值
来源：http://hz.smart0.xyz/gtcfkozncd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.dashuyun.cn/gthqcycpcw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.zhixingplan.top/gtkmszdkyn.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.shzxlz.cn/gtlfvaazib.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.sysykeji.top/gtuywsdjyd.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.ywan-chungtsiang.top/gteefinkzy.html

Go:   // 手写循环累加
来源：http://hz.yuanzhike.top/gtgdscnjbh.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.mhx1999.top/gtjjnxkdwa.html

C#:   list.Sum();  list.Average()
来源：http://hz.mhx1999.top/gtodfpxzyl.html

[D17] 最大值与最小值
来源：http://hz.smart0.xyz/gtayterjsy.html

Py:   max(arr);  min(arr)
来源：http://hz.jinghuilouyu.cn/gtmqobagxl.html

PHP:  max($arr);  min($arr);
来源：http://hz.hongshengwenyu.top/gtfzsitgys.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yangfankeji.com/gtdkpqwstj.html

TS:   Math.max(...arr);
来源：http://hz.shzxlz.cn/gthwdylgqk.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.zycfv.cn/gtjgcwsaue.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.guowangkeji.top/gtfapmpmpn.html

Ruby: arr.max;  arr.min
来源：http://hz.vqdsnc.cn/gtoffkgjrx.html

C#:   list.Max();  list.Min()
来源：http://hz.daria6918.cn/gtvbzylray.html

[D18] 扁平化嵌套数组
来源：http://hz.guowangkeji.top/gtwrcphiya.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.gzhubu.top/gtvskeyupw.html

PHP:  array_merge(...$nested);
来源：http://hz.chenzaomai.com/gtirrzmrdu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.hammf.cn/gttfnmzgje.html

TS:   nested.flat();
来源：http://hz.hnxiangtu.top/gtmsovoewm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.sxryk.cn/gtboduybgp.html

Go:   // 手写双层循环
来源：http://hz.pengpengdd.cyou/gtquysrbfc.html

Ruby: nested.flatten
来源：http://hz.guannengcc.top/gtxbmiixpf.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.xziqi.cn/gtjugjstod.html

[D19] 按字段分组
来源：http://hz.yongpay.top/gtmfkzyzai.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.sysykeji.top/gtsopvkocc.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.pycfn.com/gtecxubxdh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.ehwqpu.com/gtibxcwbzz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.hammf.cn/gtgxffjrkp.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.kuanghao11.cn/gthjxnmxyy.html

Go:   // 手写 map[string][]T
来源：http://hz.fengsongda.top/gtccvftlge.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.gaohongyu789.top/gtnbnqeems.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.haohaochexian.top/gtniucafqw.html

[D20] 统计每个元素出现次数
来源：http://hz.iojbl.cn/gtsklzkquq.html

Py:   Counter(arr)
来源：http://hz.cucudq.cn/gtlrztrwyw.html

PHP:  array_count_values($arr);
来源：http://hz.wangshuangyany.cn/gtrltfdmgt.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.svipenyu.cn/gtfntzuawc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hongshengwenyu.top/gtphuxvioj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.xziqi.cn/gtyggabuza.html

Go:   // 手写 map[T]int
来源：http://hz.sysykeji.top/gtdjojfpog.html

Ruby: arr.tally
来源：http://hz.fengsongda.top/gtmvrhdzxb.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.yvedp.cn/gthlrtnmnz.html

[D21] 判断是否包含某元素
来源：http://hz.pycfn.com/gtxlywfkjc.html

Py:   x in arr
来源：http://hz.hongshengwenyu.top/gtbsxpgnqf.html

PHP:  in_array($x, $arr, true);
来源：http://hz.ybcxt.top/gtnpbohlzz.html

JS:   arr.includes(x)
来源：http://hz.guannengcc.top/gtgxtusxnn.html

TS:   arr.includes(x)
来源：http://hz.quarkkingdee.top/gttyjtyezs.html

Java: list.contains(x)
来源：http://hz.daria6918.cn/gtfaexqmhe.html

Go:   slices.Contains(arr, x)
来源：http://hz.cucudq.cn/gtdhlrsvaw.html

Ruby: arr.include?(x)
来源：http://hz.chenjidiqi.icu/gtxpbhqbip.html

C#:   list.Contains(x)
来源：http://hz.hywenlv.cn/gtgzhkjtzg.html

[D22] 复制数组（避免共享引用）
来源：http://hz.ywan-chungtsiang.top/gtychpixhq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.hysaishi.cn/gtdsnugilp.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.ivvv.top/gtdhcypkoq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.c1oappe.top/gtmmgrphln.html

TS:   [...arr];
来源：http://hz.jiagoushi.top/gtjmazmpgf.html

Java: new ArrayList<>(list);
来源：http://hz.tian-w.cn/gtfbgujofe.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.hfpthk.cn/gtvudwzvpw.html

Ruby: arr.dup;  arr.clone
来源：http://hz.yj202588.top/gtdvglmqws.html

C#:   new List<int>(list);
来源：http://hz.ivvv.top/gtyplppnay.html

[D23] reduce 累积计算
来源：http://hz.yueranfly.top/gtcxolwtux.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.birdmap.top/gtnscnmirk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.gotoacloud.top/gtopxlrupd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.ybcxt.top/gtkjcscakx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.c1oappe.top/gtpmaodvrz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.52xcode.cn/gtlulkzdwt.html

Go:   // 手写循环
来源：http://hz.zhongyouzk.top/gtfxexdtgv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.tianlin.xyz/gtywwliwvq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.gzhubu.top/gtlarwgvcn.html

[D24] 字典 / Map 基本操作
来源：http://hz.hammf.cn/gtbxfaqzyw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.pengpengdd.cyou/gtuvmpoltq.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.jiagoushi.top/gtzsvurbud.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.xingfuxueyuan.xyz/gtvoiebtbl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.chenjidiqi.icu/gtabsauepk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.nanxinkj.top/gtpppeqtul.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.hywenlv.cn/gtgiexaapf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.iojbl.cn/gtggwljoaw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.chenjidiqi.icu/gtqjxcupzn.html

[D25] Set 集合去重与交并差
来源：http://hz.jqgufenzy.top/gtfwpilrgo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.fengsongda.top/gtqggrille.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.hnxiangtu.top/gtbfiqlrrw.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.yuanzhike.top/gtjmvkneru.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.9152youxi.cn/gtnnpufxmh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.shanyushiyangtech.top/gthoaqdzse.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.feifeiyinyue.top/gtufdcfxgg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.yangfankeji.com/gtwempkcyw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.hammf.cn/gtqqepmgwc.html

[D26] 数组转字符串
来源：http://hz.hammf.cn/gtsxsoeexo.html

Py:   ", ".join(map(str, arr))
来源：http://hz.ehwqpu.com/gtejvuitcz.html

PHP:  implode(", ", $arr);
来源：http://hz.tian-w.cn/gtylyoquim.html

JS:   arr.join(", ")
来源：http://hz.cashguo.top/gtpkfiafbn.html

TS:   arr.join(", ")
来源：http://hz.yj20258.top/gtrmbnywsk.html

Java: String.join(", ", list)
来源：http://hz.jlsjyb.cn/gtfdirjeed.html

Go:   strings.Join(strs, ", ")
来源：http://hz.havefunace.top/gticvwaypf.html

Ruby: arr.join(", ")
来源：http://hz.shanyushiyangtech.top/gtyantbbsr.html

C#:   string.Join(", ", list)
来源：http://hz.chenlongwang.top/gtnaahuzvk.html

================================================================================
来源：http://hz.bjfxy.top/gtnjxhaatk.html

E. 字符串处理
来源：http://hz.shanyushiyangkeji.top/gtxumkadvf.html

================================================================================
来源：http://hz.zhixingplan.top/gtomrujrjj.html

[E01] 拼接字符串
来源：http://hz.52xcode.cn/gtvddjxldx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.dianchejie.cn/gtvrqnlati.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.kuanghao11.cn/gtdzwxlcus.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.bjfxy.top/gtzbifpcot.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.smart0.xyz/gtzmdmqatg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.sweek.top/gtxmdjdbcw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.nwbrower.top/gtvlzlfejl.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.shanyushiyangkeji.top/gtwnbskbtl.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.ivvv.top/gtvbwockwf.html

[E02] 重复字符串
来源：http://hz.hnxiangtu.top/gtscxjxcpw.html

Py:   "ab" * 3
来源：http://hz.nwbrower.top/gtpwersyxc.html

PHP:  str_repeat("ab", 3);
来源：http://hz.haohaochexian.top/gtwumhtzsz.html

JS:   "ab".repeat(3)
来源：http://hz.jinyuanbaomall.cn/gtlrieirzf.html

TS:   "ab".repeat(3)
来源：http://hz.xuetiantiany.cn/gtkyiltxlk.html

Java: "ab".repeat(3)
来源：http://hz.shzxlz.cn/gtgbvopmnx.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.birdmap.top/gtlvybahzs.html

Ruby: "ab" * 3
来源：http://hz.svipenyu.cn/gtxtwwwtac.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.gotoacloud.top/gtgqsijaoq.html

[E03] 截取子串
来源：http://hz.shzxlz.cn/gtnjbkuztm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.aibaodan.cn/gtibskzjrr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.zdqjudy.top/gtowkieidn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.gotoacloud.top/gtafhrwepu.html

TS:   s.slice(1, 4)
来源：http://hz.hongshengwenyu.top/gtxabnqlmw.html

Java: s.substring(1, 4)
来源：http://hz.ydzc1.top/gtbnzchlvm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.ivvv.top/gtlmhcznhc.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.9152youxi.cn/gtanxiyrdl.html

C#:   s.Substring(1, 3)
来源：http://hz.jlsjyb.cn/gtnyiwxfxe.html

[E04] 查找子串位置
来源：http://hz.daxiang520.top/gtiejjxegn.html

Py:   s.find("x");  s.index("x")
来源：http://hz.gotoacloud.top/gtozmfbyre.html

PHP:  strpos($s, "x");
来源：http://hz.zhijiandao.cn/gtmnghydox.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.zhongyouzk.top/gtazzjmqxx.html

TS:   s.indexOf("x")
来源：http://hz.316326.xyz/gtllycrvto.html

Java: s.indexOf("x")
来源：http://hz.iojbl.cn/gtiwpvwivx.html

Go:   strings.Index(s, "x")
来源：http://hz.tianlin.xyz/gtnahxumgr.html

Ruby: s.index("x")
来源：http://hz.sxryk.cn/gttiqyzbth.html

C#:   s.IndexOf("x")
来源：http://hz.sysykeji.top/gtraqtkcic.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.guannengcc.top/gtkmcgqrli.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.redwolf501.top/gthwthtaip.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.chenlongwang.top/gtadlnrpzg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.feifeiyinyue.top/gtjqimcvra.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.gogol.net.cn/gtlnquvaei.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yvedp.cn/gtcclmhfdf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.ehwqpu.com/gtzdgvgzjl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.sxryk.cn/gtxkdtkdqi.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.fzhhl.top/gtbwmwlffc.html

[E06] 替换子串
来源：http://hz.shzxlz.cn/gtgddhlzrz.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.yj20258888.top/gtjtlsnztk.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.gogol.net.cn/gtvahdyhsd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.yj20258888.top/gtawvkcawg.html

TS:   s.replaceAll("a", "b")
来源：http://hz.guannengcc.top/gthzqniqom.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.quarkkingdee.top/gtmmwxweni.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.svipenyu.cn/gtvcvuigwe.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.xuanzx.com/gtnifcjycu.html

C#:   s.Replace("a", "b")
来源：http://hz.guowangkeji.top/gtdpnxxxel.html

[E07] 按分隔符拆分
来源：http://hz.shangyingyoupin.top/gtthbnbvjr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.pycfn.com/gtvdzyffpo.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.yuxming.cn/gtiyhfdvig.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.jqgufenzy.top/gtwkfouwti.html

TS:   s.split(",")
来源：http://hz.sxryk.cn/gtoaivvboz.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.ywan-chungtsiang.top/gtrgtlfexf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.gotoacloud.top/gtdiyawctf.html

Ruby: s.split(",");  s.split
来源：http://hz.hnxiangtu.top/gtezrcakig.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.cucudq.cn/gttaqtbsne.html

[E08] 数组按分隔符合并
来源：http://hz.jinghuilouyu.cn/gtmwzjtraw.html

Py:   ",".join(items)
来源：http://hz.tianlin.xyz/gtglwbkhvy.html

PHP:  implode(",", $items);
来源：http://hz.yj202588.top/gtwoaiephk.html

JS:   items.join(",")
来源：http://hz.zhijiandao.cn/gtdppuqlrd.html

TS:   items.join(",")
来源：http://hz.iojbl.cn/gtmrxvdqot.html

Java: String.join(",", items)
来源：http://hz.hnxiangtu.top/gtcpvmfroo.html

Go:   strings.Join(items, ",")
来源：http://hz.hnxiangtu.top/gtcsoikyyb.html

Ruby: items.join(",")
来源：http://hz.sysykeji.top/gtjuowmjlc.html

C#:   string.Join(",", items)
来源：http://hz.zdqjudy.top/gtevijwref.html

[E09] 去除所有空白字符
来源：http://hz.chenzaomai.com/gtfguzowpo.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.pengpengdd.cyou/gtmrysansk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.yj202588.top/gtwjtmfqrr.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.fengsongda.top/gtavzzuwqs.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.52xcode.cn/gtjvrtyfnb.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.havefunace.top/gtmnxqhnhh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.yangfankeji.com/gtvnqabyis.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.chenjidiqi.icu/gtpgwmolvt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yonumen.top/gtkednopch.html

[E10] 左侧补零 / 定长填充
来源：http://hz.gaohongyu789.top/gtnmbvkjuv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.dashuyun.cn/gtxaxgzudr.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.jinghuilouyu.cn/gtyxtmghyg.html

JS:   "7".padStart(3, "0")
来源：http://hz.ivvv.top/gtiqbgpgwd.html

TS:   "7".padStart(3, "0")
来源：http://hz.sxryk.cn/gtwotmqtqx.html

Java: String.format("%03d", 7)
来源：http://hz.dianchejie.cn/gtmpxhhvke.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yangfankeji.com/gtqljbtqil.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yuanzhike.top/gttbjonqjm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.xylfe.cn/gtycbyvvaq.html

[E11] 反转字符串
来源：http://hz.jlsjyb.cn/gtayzrpavx.html

Py:   s[::-1]
来源：http://hz.ivvv.top/gtocpvbfay.html

PHP:  strrev($s);
来源：http://hz.yangfankeji.com/gtdyyzkoiq.html

JS:   [...s].reverse().join("")
来源：http://hz.nanxinkj.top/gtobzbndzb.html

TS:   [...s].reverse().join("")
来源：http://hz.aibaodan.cn/gtmrmvcvsq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.dashuyun.cn/gtbrbaarqt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.xylfe.cn/gthrpuxoch.html

Ruby: s.reverse
来源：http://hz.yj20258.top/gtbrwhigzd.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.dashuyun.cn/gtuzclmtfa.html

[E12] 统计某字符出现次数
来源：http://hz.hywenlv.cn/gtfwljmyly.html

Py:   s.count("a")
来源：http://hz.zycfv.cn/gtohflenfd.html

PHP:  substr_count($s, "a");
来源：http://hz.yangfankeji.com/gtcteysttp.html

JS:   s.split("a").length - 1
来源：http://hz.0kj1m.cn/gtdpnpaqym.html

TS:   s.split("a").length - 1
来源：http://hz.jinyuanbaomall.cn/gtodduqirp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.svipenyu.cn/gtejotqudd.html

Go:   strings.Count(s, "a")
来源：http://hz.jinyuanbaomall.cn/gtbtqklyvl.html

Ruby: s.count("a")
来源：http://hz.zhengqikj.top/gtdstbgahr.html

C#:   s.Count(c => c == 'a')
来源：http://hz.cheryme.top/gtqeuubpho.html

[E13] 逐字符遍历
来源：http://hz.cashguo.top/gtmcxaofng.html

Py:   for ch in s: print(ch)
来源：http://hz.nanxuanxn.top/gtzgdbpsjw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.xziqi.cn/gtqnrrgoap.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shangyingyoupin.top/gtmrjiibsq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yvedp.cn/gtlwdzhazt.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.cucudq.cn/gtowuwhfjx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.xinyue.icu/gtrebaobrv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.gaohongyu789.top/gtmnoozdkq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.wangshuangyany.cn/gtdygiogbc.html

[E14] URL 编码与 Base64
来源：http://hz.redwolf501.top/gtoqixsizz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.guannengcc.top/gtvugqfynr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.sysykeji.top/gttzuqshkf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.guowangkeji.top/gtccwxoabt.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.zhixingplan.top/gtietpnxov.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.hywenlv.cn/gtxsfmypta.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yuanzhike.top/gtdoxguujt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.316326.xyz/gtzbdzwakr.html


<!-- 参考信息 -->