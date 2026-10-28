代发 wailian999

TS:   arr.slice(1, 4);
来源：http://hz.jiagoushi.top/gtcregytay.html

Java: list.subList(1, 4);
来源：http://hz.fzhhl.top/gtsvjndzsx.html

Go:   arr[1:4]
来源：http://hz.ydzc1.top/gtfpipftiv.html

Ruby: arr[1, 3]
来源：http://hz.dashuyun.cn/gtftxpzjxj.html

C#:   list.GetRange(1, 3);
来源：http://hz.xziqi.cn/gtikplltnz.html

[D08] 合并两个数组
来源：http://hz.9152youxi.cn/gtqhaqoext.html

Py:   a + b;  a.extend(b)
来源：http://hz.hnqzz.top/gtanfajzrl.html

PHP:  array_merge($a, $b);
来源：http://hz.iojbl.cn/gtjrzgoioj.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.ppjwa.cn/gtzhfzhwuz.html

TS:   [...a, ...b];
来源：http://hz.zhongyouzk.top/gtfetbjebe.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.xylfe.cn/gtlfwqxiqr.html

Go:   append(a, b...)
来源：http://hz.gaohongyu789.top/gtpvpdeyzr.html

Ruby: a + b;  a.concat(b)
来源：http://hz.bjfxy.top/gtlcfxeano.html

C#:   a.Concat(b).ToList()
来源：http://hz.ybcxt.top/gtcavokvzj.html

[D09] 排序（升序）
来源：http://hz.birdmap.top/gtuxtcfsne.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.aibaodan.cn/gtfusohfrf.html

PHP:  sort($arr);
来源：http://hz.havefunace.top/gtbqfvymlx.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.sxryk.cn/gtwjgyulpr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.gzhubu.top/gtwujguwwo.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.yj202588.top/gtgmiojasl.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.ywan-chungtsiang.top/gttyvsastf.html

Ruby: arr.sort
来源：http://hz.dianchejie.cn/gtlqyanixo.html

C#:   list.Sort();
来源：http://hz.hongshengwenyu.top/gtkknfcvrv.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.sxryk.cn/gtgcemzbqv.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.9152youxi.cn/gtlpaemtxl.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.hongshengwenyu.top/gtoxcjrytr.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.jianghu66.top/gtephzvzpa.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.yj20258888.top/gtbcejhhbq.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.hongshengwenyu.top/gtduzvbpzc.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.jinghuilouyu.cn/gthkqhhyct.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.tian-w.cn/gtsjvdcvbj.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.sweek.top/gthaoreqst.html

[D11] 反转数组
来源：http://hz.quarkkingdee.top/gttkmtatgu.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.smart0.xyz/gtqmnsuobk.html

PHP:  array_reverse($arr);
来源：http://hz.andypj.xyz/gtqjtxjgpk.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.nanxuanxn.top/gthvciikgb.html

TS:   [...arr].reverse();
来源：http://hz.smart0.xyz/gtrvhuqjkf.html

Java: Collections.reverse(list);
来源：http://hz.jinghuilouyu.cn/gtovnzffww.html

Go:   slices.Reverse(arr)
来源：http://hz.hysaishi.cn/gtnczlefvl.html

Ruby: arr.reverse
来源：http://hz.zycfv.cn/gtscmcfimo.html

C#:   list.Reverse();
来源：http://hz.shuidangran.top/gtkhioklbu.html

[D12] 查找元素下标
来源：http://hz.jiagoushi.top/gtfjtxvvob.html

Py:   arr.index(x);  x in arr
来源：http://hz.tianlin.xyz/gtnkzmqzjf.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.cheryme.top/gtzobnjxfm.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.nanxinkj.top/gtjpsvbfsc.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.kuanghao11.cn/gtsacuhqns.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.zhoulong.xyz/gtltinmnas.html

Go:   slices.Index(arr, x)
来源：http://hz.nwbrower.top/gtcgowwzit.html

Ruby: arr.index(x)
来源：http://hz.nwbrower.top/gtbaqecmfh.html

C#:   list.IndexOf(x);
来源：http://hz.jyoumei.cn/gtewplnbvc.html

[D13] 过滤（保留满足条件的）
来源：http://hz.sysykeji.top/gtwpktoqzh.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.gogol.net.cn/gtnludtqoq.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.fzhhl.top/gtcpqithmg.html

JS:   arr.filter(x => x > 3)
来源：http://hz.dianchejie.cn/gtoalsijgj.html

TS:   arr.filter(x => x > 3)
来源：http://hz.nanxuanxn.top/gtwfqududm.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.dianchejie.cn/gtpnfbvfpm.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.mhx1999.top/gtgxnsqwkd.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.wangshuangyany.cn/gtfivckcaf.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.jinyuanbaomall.cn/gtlimorytn.html

[D14] 映射转换（每个元素变形）
来源：http://hz.zhoulong.xyz/gtrnclgnaz.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.ivvv.top/gtsysxjoyq.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.chenlongwang.top/gtrcptauom.html

JS:   arr.map(x => x * 2)
来源：http://hz.hysaishi.cn/gtgonbuldl.html

TS:   arr.map(x => x * 2)
来源：http://hz.ehwqpu.com/gtdonmiapc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.iojbl.cn/gtqjnghgeg.html

Go:   // 手写循环
来源：http://hz.nanxuanxn.top/gtidcryaop.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.daxiang520.top/gtjhoaqkxp.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.havefunace.top/gtphuolglw.html

[D15] 去重
来源：http://hz.jinghuilouyu.cn/gtmemrcjnm.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.fengsongda.top/gtiqbviaqt.html

PHP:  array_unique($arr);
来源：http://hz.xylfe.cn/gtzsmankhc.html

JS:   [...new Set(arr)]
来源：http://hz.wangdashe.top/gtqtscstyl.html

TS:   [...new Set(arr)]
来源：http://hz.ppjwa.cn/gtuxbridzd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.fzhhl.top/gtgxambfav.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.svipenyu.cn/gtqtqpxlaj.html

Ruby: arr.uniq
来源：http://hz.ybcxt.top/gttqgpsgwq.html

C#:   list.Distinct().ToList()
来源：http://hz.bjfxy.top/gtdjsbqmzd.html

[D16] 求和与平均值
来源：http://hz.zhengqikj.top/gtczjtpceo.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.chenjidiqi.icu/gtmkcevhzt.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.yj202588.top/gthxpgsdjy.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.yj20258.top/gtbemsqakw.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhijiandao.cn/gtivzclakf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.jinyuanbaomall.cn/gtlntpuafv.html

Go:   // 手写循环累加
来源：http://hz.gotoacloud.top/gtxipyfeye.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.nwbrower.top/gtirywxfgz.html

C#:   list.Sum();  list.Average()
来源：http://hz.tian-w.cn/gtlvblmwlo.html

[D17] 最大值与最小值
来源：http://hz.havefunace.top/gtbukmcjwk.html

Py:   max(arr);  min(arr)
来源：http://hz.gzhubu.top/gtyhbajyol.html

PHP:  max($arr);  min($arr);
来源：http://hz.smart0.xyz/gtgbltgnhf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.yongpay.top/gthfpzjsxb.html

TS:   Math.max(...arr);
来源：http://hz.pycfn.com/gtptkajvws.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.chenjidiqi.icu/gtgknfzztm.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.c1oappe.top/gtaadnlcxg.html

Ruby: arr.max;  arr.min
来源：http://hz.yj202588.top/gtpsafexoq.html

C#:   list.Max();  list.Min()
来源：http://hz.quarkkingdee.top/gtagfhyhpq.html

[D18] 扁平化嵌套数组
来源：http://hz.shanyushiyangtech.top/gtzgmusfgb.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.zhixingplan.top/gtyuigukzl.html

PHP:  array_merge(...$nested);
来源：http://hz.sweek.top/gtczrtydyo.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.jqgfzy.top/gtzcbglcvl.html

TS:   nested.flat();
来源：http://hz.ydjk.org.cn/gtgtloudqh.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.jiagoushi.top/gtwkxvwsxf.html

Go:   // 手写双层循环
来源：http://hz.ivvv.top/gtdpunfsad.html

Ruby: nested.flatten
来源：http://hz.shangyingyoupin.top/gtcdjrcbgh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.hammf.cn/gtkwetvwbe.html

[D19] 按字段分组
来源：http://hz.vqdsnc.cn/gtirapyauv.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.snrcjt.cn/gtaippzfas.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.nwbrower.top/gtaxzhbexk.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.iojbl.cn/gtmshrkxhc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.zycfv.cn/gtqcnjkhzn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.tanke756.top/gtsgqdddct.html

Go:   // 手写 map[string][]T
来源：http://hz.gzhubu.top/gtektwuejr.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.zhiwuduotai.top/gtfxohstoh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.smart0.xyz/gtajvobkww.html

[D20] 统计每个元素出现次数
来源：http://hz.316326.xyz/gtirfipnyk.html

Py:   Counter(arr)
来源：http://hz.xinyue.icu/gtafclpmyp.html

PHP:  array_count_values($arr);
来源：http://hz.shuidangran.top/gtmshsffjb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.ydjk.org.cn/gtngshzxoe.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.hongshengwenyu.top/gtjboyttpa.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.xziqi.cn/gtsgpwdrod.html

Go:   // 手写 map[T]int
来源：http://hz.xziqi.cn/gttxetwlpl.html

Ruby: arr.tally
来源：http://hz.meibo888.top/gtcejjsvqr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.316326.xyz/gtcqcuhygn.html

[D21] 判断是否包含某元素
来源：http://hz.ydzc1.top/gtovrnpmsq.html

Py:   x in arr
来源：http://hz.chenjidiqi.icu/gtbnffghge.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yueranfly.top/gtynpjtxga.html

JS:   arr.includes(x)
来源：http://hz.wangshuangyany.cn/gtemdhhhoi.html

TS:   arr.includes(x)
来源：http://hz.feifeiyinyue.top/gtadxypdjt.html

Java: list.contains(x)
来源：http://hz.zhixingplan.top/gtitceywpa.html

Go:   slices.Contains(arr, x)
来源：http://hz.ydzc1.top/gtjhrammus.html

Ruby: arr.include?(x)
来源：http://hz.cucudq.cn/gtlqtrevoc.html

C#:   list.Contains(x)
来源：http://hz.jqgufenzy.top/gtlvvlhjyk.html

[D22] 复制数组（避免共享引用）
来源：http://hz.dianchejie.cn/gtokmjpodn.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.guowangkeji.top/gtkxdhzkzx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.nanxuanxn.top/gtkcikkdaw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.meibo888.top/gtgldtaenw.html

TS:   [...arr];
来源：http://hz.hysaishi.cn/gtprpxsrqp.html

Java: new ArrayList<>(list);
来源：http://hz.tianlin.xyz/gtrvyqyrlt.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.andypj.xyz/gtflifbvtf.html

Ruby: arr.dup;  arr.clone
来源：http://hz.bjfxy.top/gtlemgvgoo.html

C#:   new List<int>(list);
来源：http://hz.meibo888.top/gtmvazagqo.html

[D23] reduce 累积计算
来源：http://hz.yonumen.top/gtqwfodyfc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.zhixingplan.top/gtntthmdys.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.aibaodan.cn/gtvgxcpaex.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.yongpay.top/gtgyuoiqaj.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.hfpthk.cn/gtxztburje.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.yonumen.top/gtfxydwdtc.html

Go:   // 手写循环
来源：http://hz.ydjk.org.cn/gttnfkovfe.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.jiagoushi.top/gtguxyrnpd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.shuidangran.top/gtdhdpuuqy.html

[D24] 字典 / Map 基本操作
来源：http://hz.shangyingyoupin.top/gtxvdfyafp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.meibo888.top/gtujgyygne.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.shzxlz.cn/gtgalsdfqp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.sxryk.cn/gtrjzhvwtc.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.yonumen.top/gtvrmbflvy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.zhixingplan.top/gtqyxqhnov.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.smart0.xyz/gtoslvqltm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zhaomingkeji.xyz/gtiaosgsky.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.zhaomingkeji.xyz/gtkxddvdxu.html

[D25] Set 集合去重与交并差
来源：http://hz.xziqi.cn/gtiwejjaet.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.iojbl.cn/gtmdyweehm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.nanxuanxn.top/gtncrihbnq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.cqqwz.cn/gtmomgtuwb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.chenlongwang.top/gtrfavbvfr.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.cheryme.top/gtkqamzgdu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.nanxuanxn.top/gtlzmnzcbu.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.ybcxt.top/gtnfivxxyu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.zdqjudy.top/gtybeehvzl.html

[D26] 数组转字符串
来源：http://hz.zhengqikj.top/gtsixxtexq.html

Py:   ", ".join(map(str, arr))
来源：http://hz.pycfn.com/gtgchqcglu.html

PHP:  implode(", ", $arr);
来源：http://hz.zhengqikj.top/gtrjwcdjcr.html

JS:   arr.join(", ")
来源：http://hz.pengpengdd.cyou/gtpvbabllc.html

TS:   arr.join(", ")
来源：http://hz.hywenlv.cn/gtvaihzvyb.html

Java: String.join(", ", list)
来源：http://hz.sysykeji.top/gtdaeqlher.html

Go:   strings.Join(strs, ", ")
来源：http://hz.xuanzx.com/gtygmqncoo.html

Ruby: arr.join(", ")
来源：http://hz.hysaishi.cn/gtqdgixaey.html

C#:   string.Join(", ", list)
来源：http://hz.tanke756.top/gtvbtcbeqr.html

================================================================================
来源：http://hz.yangfankeji.com/gtuycuyzqx.html

E. 字符串处理
来源：http://hz.havefunace.top/gtrflusrlq.html

================================================================================
来源：http://hz.yj202588.top/gtzhvdgsof.html

[E01] 拼接字符串
来源：http://hz.wangdashe.top/gteihtzeub.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.yj202588.top/gtsvzlkvga.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.feifeiyinyue.top/gtraigoxhd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.bjfxy.top/gtjwcjnegv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.cucudq.cn/gtueamwqen.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.pengpengdd.cyou/gtumtvnphl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.shanyushiyangtech.top/gtvwbjrhin.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.bjfxy.top/gtycbafojo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.andypj.xyz/gtmpymbqic.html

[E02] 重复字符串
来源：http://hz.hongshengwenyu.top/gtosuryeqa.html

Py:   "ab" * 3
来源：http://hz.mhx1999.top/gtupqvxzsa.html

PHP:  str_repeat("ab", 3);
来源：http://hz.zdqjudy.top/gtwqxpiiqw.html

JS:   "ab".repeat(3)
来源：http://hz.wangshuangyany.cn/gtzdcwkqqe.html

TS:   "ab".repeat(3)
来源：http://hz.pengpengdd.cyou/gttjvonjyu.html

Java: "ab".repeat(3)
来源：http://hz.xuetiantiany.cn/gtsozvuuvr.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.smart0.xyz/gtflizlubl.html

Ruby: "ab" * 3
来源：http://hz.jyoumei.cn/gthnfkaddr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.feifeiyinyue.top/gtygthbmqo.html

[E03] 截取子串
来源：http://hz.tian-w.cn/gtvtfnaipi.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.sysykeji.top/gtxksvykeu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.hnqzz.top/gtzaytwmhc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.yvedp.cn/gtoskoapgc.html

TS:   s.slice(1, 4)
来源：http://hz.pengpengdd.cyou/gtbinwkren.html

Java: s.substring(1, 4)
来源：http://hz.xuetiantiany.cn/gtbagjloii.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.c1oappe.top/gtfxafrasz.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.hammf.cn/gtzciahhvw.html

C#:   s.Substring(1, 3)
来源：http://hz.sxryk.cn/gtkzlaykah.html

[E04] 查找子串位置
来源：http://hz.zhiwuduotai.top/gtsvsjrcty.html

Py:   s.find("x");  s.index("x")
来源：http://hz.jinqigfzy.top/gtuamntify.html

PHP:  strpos($s, "x");
来源：http://hz.meibo888.top/gtxobzwubu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.xinyue.icu/gtgecpogjn.html

TS:   s.indexOf("x")
来源：http://hz.guowangkeji.top/gtkwmfucas.html

Java: s.indexOf("x")
来源：http://hz.gaohongyu789.top/gtpvyttmbz.html

Go:   strings.Index(s, "x")
来源：http://hz.cheryme.top/gtvbyfqfrl.html

Ruby: s.index("x")
来源：http://hz.cqqwz.cn/gtqttmjnno.html

C#:   s.IndexOf("x")
来源：http://hz.vqdsnc.cn/gtryhucxyp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.gogol.net.cn/gtnrqjeihx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.zhongyouzk.top/gtfazmegtt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.guannengcc.top/gtdmeziteq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.cqqwz.cn/gtswycqicx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.zdqjudy.top/gtppwtpnqc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.jqgufenzy.top/gtsowxsstj.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.birdmap.top/gtzkkdtvmg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.xuanzx.com/gtqcrtaocp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.feifeiyinyue.top/gtekkpxume.html

[E06] 替换子串
来源：http://hz.zhengqikj.top/gteyqxtmmb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.zhoulong.xyz/gtgwljextq.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.dashuyun.cn/gtvmgpmnzh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.haohaochexian.top/gtgslikvig.html

TS:   s.replaceAll("a", "b")
来源：http://hz.yj20258888.top/gtxanwyzpr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.redwolf501.top/gttfvmkfow.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.tianlin.xyz/gtyazphcsq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.xuanzx.com/gtznpoqtck.html

C#:   s.Replace("a", "b")
来源：http://hz.fengsongda.top/gtmguydqzf.html

[E07] 按分隔符拆分
来源：http://hz.pycfn.com/gtyqtyizkq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.yvedp.cn/gtqrzgixki.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.hysaishi.cn/gtughdccaf.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.meibo888.top/gtybmmovhy.html

TS:   s.split(",")
来源：http://hz.pengpengdd.cyou/gtgwexremh.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.mhx1999.top/gtvellpjwo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.tanke756.top/gtnrdxdyjl.html

Ruby: s.split(",");  s.split
来源：http://hz.zycfv.cn/gtsfuxmmww.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.chenlongwang.top/gtrznxbrbm.html

[E08] 数组按分隔符合并
来源：http://hz.zdqjudy.top/gtydasnelj.html

Py:   ",".join(items)
来源：http://hz.hammf.cn/gthkubkpmp.html

PHP:  implode(",", $items);
来源：http://hz.cashguo.top/gtpoylemkd.html

JS:   items.join(",")
来源：http://hz.ivvv.top/gtvdxhpkvz.html

TS:   items.join(",")
来源：http://hz.dashuyun.cn/gtfzyavccd.html

Java: String.join(",", items)
来源：http://hz.hnxiangtu.top/gtowpfmgft.html

Go:   strings.Join(items, ",")
来源：http://hz.smart0.xyz/gtevnzxkbg.html

Ruby: items.join(",")
来源：http://hz.dashuyun.cn/gtrbgvypco.html

C#:   string.Join(",", items)
来源：http://hz.fzhhl.top/gtqdsfnolv.html

[E09] 去除所有空白字符
来源：http://hz.haohaochexian.top/gtacdldeao.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.jinqigfzy.top/gterbpwpxt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.ehwqpu.com/gtxooeqfmo.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.xinyue.icu/gtlpotguwz.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.chenjidiqi.icu/gtdpxugjwz.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.cashguo.top/gtdigyjxwv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.dashuyun.cn/gtepdaaddu.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.ehwqpu.com/gtwlaocmaw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.sxryk.cn/gtumhmnydt.html

[E10] 左侧补零 / 定长填充
来源：http://hz.cashguo.top/gtbtqgmbmp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.cqqwz.cn/gtwlxbhdkx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.fengsongda.top/gtuivondqv.html

JS:   "7".padStart(3, "0")
来源：http://hz.yuxming.cn/gtkfwrikyj.html

TS:   "7".padStart(3, "0")
来源：http://hz.andypj.xyz/gtpcwkbmkd.html

Java: String.format("%03d", 7)
来源：http://hz.yanxiufei.cn/gtbrtgulym.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.yanxiufei.cn/gtdajpwdds.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.yangfankeji.com/gtabccwleu.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.cashguo.top/gtcvwhygeb.html

[E11] 反转字符串
来源：http://hz.hfpthk.cn/gtkctuaoql.html

Py:   s[::-1]
来源：http://hz.ybcxt.top/gtbkgmccwp.html

PHP:  strrev($s);
来源：http://hz.pycfn.com/gtwzbwmmqu.html

JS:   [...s].reverse().join("")
来源：http://hz.smart0.xyz/gtxlwjouth.html

TS:   [...s].reverse().join("")
来源：http://hz.shangyingyoupin.top/gtlvcbwegg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.sxryk.cn/gtrxjthtza.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.gzhubu.top/gtxtkgkhbk.html

Ruby: s.reverse
来源：http://hz.wangdashe.top/gtfraszouk.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.chenzaomai.com/gtkdljzpgs.html

[E12] 统计某字符出现次数
来源：http://hz.pengpengdd.cyou/gtxpecozxq.html

Py:   s.count("a")
来源：http://hz.gogol.net.cn/gtgeqkveuu.html

PHP:  substr_count($s, "a");
来源：http://hz.jyoumei.cn/gtlqxohacs.html

JS:   s.split("a").length - 1
来源：http://hz.pycfn.com/gthxrghzlm.html

TS:   s.split("a").length - 1
来源：http://hz.meibo888.top/gtcacyrnaw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.kuanghao11.cn/gtmqgvcobm.html

Go:   strings.Count(s, "a")
来源：http://hz.svipenyu.cn/gtwjgnsbku.html

Ruby: s.count("a")
来源：http://hz.gotoacloud.top/gtovrdvsxs.html

C#:   s.Count(c => c == 'a')
来源：http://hz.zycfv.cn/gttthatosz.html

[E13] 逐字符遍历
来源：http://hz.xylfe.cn/gtrulzsyux.html

Py:   for ch in s: print(ch)
来源：http://hz.xziqi.cn/gtxfxklowp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.quarkkingdee.top/gtoeuyabph.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jqgufenzy.top/gttxufgfts.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.chenjidiqi.icu/gtchtxhunb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.hfpthk.cn/gtffumevzn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.quarkkingdee.top/gtvspqxjyn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.guowangkeji.top/gtrtsulfed.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.ydjk.org.cn/gtgtgcoucd.html

[E14] URL 编码与 Base64
来源：http://hz.zycfv.cn/gtcgceqgwd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.chenlongwang.top/gtdmuazglb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.hongshengwenyu.top/gtgtxrzujw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.sweek.top/gtiaxlxrkr.html


<!-- 参考信息 -->