代发 wailian999

Java: list.size();
来源：http://hz.yj20258.top/gtgnwmqite.html

Go:   len(arr)
来源：http://hz.xylfe.cn/gtrahvupsc.html

Ruby: arr.length; arr.size
来源：http://hz.jqgufenzy.top/gtrfmtgoqh.html

C#:   list.Count;
来源：http://hz.0kj1m.cn/gtpommpxiv.html

[D07] 切片 / 取子数组
来源：http://hz.xuanzx.com/gtknzcnpdn.html

Py:   arr[1:4]; arr[:3]; arr[::2]
来源：http://hz.nanxuanxn.top/gtadwguzkm.html

PHP:  array_slice($arr, 1, 3);
来源：http://hz.jlsjyb.cn/gtgxnnzios.html

JS:   arr.slice(1, 4);
来源：http://hz.meibo888.top/gtsvipecoq.html

TS:   arr.slice(1, 4);
来源：http://hz.cheryme.top/gtrtadbtjx.html

Java: list.subList(1, 4);
来源：http://hz.sufxvd.cn/gtxpoylpyj.html

Go:   arr[1:4]
来源：http://hz.ydzc1.top/gtptliewdx.html

Ruby: arr[1, 3]
来源：http://hz.hfpthk.cn/gtmfomsvmo.html

C#:   list.GetRange(1, 3);
来源：http://hz.mhx1999.top/gtohtfbfgw.html

[D08] 合并两个数组
来源：http://hz.snrcjt.cn/gtlcnxxgsy.html

Py:   a + b;  a.extend(b)
来源：http://hz.gaohongyu789.top/gtyjtnitji.html

PHP:  array_merge($a, $b);
来源：http://hz.yongpay.top/gtambfpfde.html

JS:   [...a, ...b];  a.concat(b);
来源：http://hz.cqqwz.cn/gtxqgkwxun.html

TS:   [...a, ...b];
来源：http://hz.0kj1m.cn/gtqbstlaqs.html

Java: Stream.concat(a.stream(), b.stream()).toList()
来源：http://hz.tian-w.cn/gtungbbszo.html

Go:   append(a, b...)
来源：http://hz.jinghuilouyu.cn/gtrflpbbdd.html

Ruby: a + b;  a.concat(b)
来源：http://hz.daxiang520.top/gtuqvzlwqb.html

C#:   a.Concat(b).ToList()
来源：http://hz.dianchejie.cn/gtfxwaaydj.html

[D09] 排序（升序）
来源：http://hz.shanyushiyangtech.top/gtmbeywyuj.html

Py:   sorted(arr);  arr.sort()
来源：http://hz.cdnleiting.top/gtbjyatwof.html

PHP:  sort($arr);
来源：http://hz.gotoacloud.top/gtjsamttgm.html

JS:   [...arr].sort((x, y) => x - y)     // 默认按字符串比较，数字必须给比较器
来源：http://hz.jianghu66.top/gtgyscovdr.html

TS:   [...arr].sort((x, y) => x - y);
来源：http://hz.haohaochexian.top/gtzsfyllaj.html

Java: Collections.sort(list);  list.sort(null);
来源：http://hz.ivvv.top/gtceuhgnai.html

Go:   sort.Ints(arr);  slices.Sort(arr)
来源：http://hz.yj202588.top/gtzukpipxo.html

Ruby: arr.sort
来源：http://hz.yangfankeji.com/gtngttxlxb.html

C#:   list.Sort();
来源：http://hz.xziqi.cn/gtsdxioxgk.html

[D10] 自定义排序（按字段 / 多条件）
来源：http://hz.xylfe.cn/gtgofkndqi.html

Py:   arr.sort(key=lambda x: x["age"]);  sorted(arr, key=len, reverse=True)
来源：http://hz.cheryme.top/gtaxtcmbxj.html

PHP:  usort($arr, fn($a, $b) => $a["age"] <=> $b["age"]);
来源：http://hz.bjfxy.top/gtpdtddlks.html

JS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.ybcxt.top/gtdozpllyi.html

TS:   arr.sort((a, b) => a.age - b.age)
来源：http://hz.pengpengdd.cyou/gtahajghns.html

Java: list.sort(Comparator.comparing(Person::age));
来源：http://hz.yangfankeji.com/gtzxdgangz.html

Go:   sort.Slice(items, func(i, j int) bool { return items[i].Age < items[j].Age })
来源：http://hz.shanyushiyangkeji.top/gtjewedlap.html

Ruby: arr.sort_by { |x| x[:age] }
来源：http://hz.yangfankeji.com/gtpitznmaw.html

C#:   list.Sort((a, b) => a.Age.CompareTo(b.Age));
来源：http://hz.guowangkeji.top/gtntokymit.html

[D11] 反转数组
来源：http://hz.yj20258888.top/gthtqefxny.html

Py:   arr[::-1];  arr.reverse()
来源：http://hz.yvedp.cn/gtktfwtsch.html

PHP:  array_reverse($arr);
来源：http://hz.dashuyun.cn/gtogrjqaum.html

JS:   [...arr].reverse();  arr.toReversed()
来源：http://hz.shanyushiyangkeji.top/gtwewsellw.html

TS:   [...arr].reverse();
来源：http://hz.andypj.xyz/gtyyyzpent.html

Java: Collections.reverse(list);
来源：http://hz.hnxiangtu.top/gtxhzxrpxt.html

Go:   slices.Reverse(arr)
来源：http://hz.gogol.net.cn/gtzngylejx.html

Ruby: arr.reverse
来源：http://hz.jyoumei.cn/gtnggdvrtb.html

C#:   list.Reverse();
来源：http://hz.daria6918.cn/gtxjoiiyar.html

[D12] 查找元素下标
来源：http://hz.shanyushiyangkeji.top/gtusktkfoe.html

Py:   arr.index(x);  x in arr
来源：http://hz.zhaomingkeji.xyz/gtumppvkca.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://hz.cashguo.top/gtldvwixsr.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.haohaochexian.top/gtxymyzaiu.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://hz.ydzc1.top/gtvbaerlya.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://hz.jianghu66.top/gtcolhlsdm.html

Go:   slices.Index(arr, x)
来源：http://hz.ehwqpu.com/gtqghhckuc.html

Ruby: arr.index(x)
来源：http://hz.tanke756.top/gtetnbztnh.html

C#:   list.IndexOf(x);
来源：http://hz.vqdsnc.cn/gtdcmdyeap.html

[D13] 过滤（保留满足条件的）
来源：http://hz.yueranfly.top/gtiozejckg.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://hz.hnxiangtu.top/gtmnqjxlxu.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://hz.jyoumei.cn/gticwdteby.html

JS:   arr.filter(x => x > 3)
来源：http://hz.pycfn.com/gtzoshyzcr.html

TS:   arr.filter(x => x > 3)
来源：http://hz.9152youxi.cn/gtfjpnpwfx.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://hz.aizwys.cn/gtztqbnrxe.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://hz.hfpthk.cn/gtmflvevrp.html

Ruby: arr.select { |x| x > 3 }
来源：http://hz.wangshuangyany.cn/gtwzotmesq.html

C#:   list.Where(x => x > 3).ToList()
来源：http://hz.quarkkingdee.top/gtpobkqybu.html

[D14] 映射转换（每个元素变形）
来源：http://hz.c1oappe.top/gtpdrdvwxq.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://hz.gzhubu.top/gtqothrrin.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://hz.yongpay.top/gtrsnullad.html

JS:   arr.map(x => x * 2)
来源：http://hz.nanxinkj.top/gtakvoxwlt.html

TS:   arr.map(x => x * 2)
来源：http://hz.xziqi.cn/gtvltkelol.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://hz.jqgfzy.top/gtyvgpzwoz.html

Go:   // 手写循环
来源：http://hz.havefunace.top/gtjexjnxke.html

Ruby: arr.map { |x| x * 2 }
来源：http://hz.xziqi.cn/gtpvvndaes.html

C#:   list.Select(x => x * 2).ToList()
来源：http://hz.ivvv.top/gtqxesvcwe.html

[D15] 去重
来源：http://hz.haohaochexian.top/gtvlvqbmto.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://hz.hysaishi.cn/gtfyinxjrr.html

PHP:  array_unique($arr);
来源：http://hz.yvedp.cn/gtldjgmqza.html

JS:   [...new Set(arr)]
来源：http://hz.jinghuilouyu.cn/gtxgfcobla.html

TS:   [...new Set(arr)]
来源：http://hz.nwbrower.top/gtgnwpuojy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://hz.52xcode.cn/gtixwyzemk.html

Go:   // 用 map[T]struct{} 手写
来源：http://hz.zhengqikj.top/gtpsjfvftx.html

Ruby: arr.uniq
来源：http://hz.chenlongwang.top/gtxgbyrbbg.html

C#:   list.Distinct().ToList()
来源：http://hz.jianghu66.top/gtzarcyswh.html

[D16] 求和与平均值
来源：http://hz.c1oappe.top/gtfdwqgazj.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://hz.jinqigufen.top/gtzwidiumf.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://hz.cucudq.cn/gtgswnfxxw.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.zhiwuduotai.top/gttimblmzk.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://hz.ydjk.org.cn/gtmyehgnvq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://hz.chenjidiqi.icu/gtfgqgeafy.html

Go:   // 手写循环累加
来源：http://hz.yuanzhike.top/gtbqzymqtn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://hz.chenjidiqi.icu/gtmwoevyso.html

C#:   list.Sum();  list.Average()
来源：http://hz.hfpthk.cn/gtysozxeyc.html

[D17] 最大值与最小值
来源：http://hz.cheryme.top/gtdzgqpnhx.html

Py:   max(arr);  min(arr)
来源：http://hz.hnxiangtu.top/gtvuhfrewc.html

PHP:  max($arr);  min($arr);
来源：http://hz.316326.xyz/gtzmpbwblf.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://hz.quarkkingdee.top/gthiuonkwv.html

TS:   Math.max(...arr);
来源：http://hz.cqqwz.cn/gtrzmayjpx.html

Java: Collections.max(list);  Collections.min(list);
来源：http://hz.jinqigufen.top/gthxdllzbf.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://hz.52xcode.cn/gtbimualpo.html

Ruby: arr.max;  arr.min
来源：http://hz.daria6918.cn/gtujiwfsso.html

C#:   list.Max();  list.Min()
来源：http://hz.ywan-chungtsiang.top/gtcyyjsshx.html

[D18] 扁平化嵌套数组
来源：http://hz.cashguo.top/gtlupdhnfl.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://hz.gaohongyu789.top/gtbttvgkxa.html

PHP:  array_merge(...$nested);
来源：http://hz.gaohongyu789.top/gtquteszpb.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://hz.jinqigfzy.top/gtiebygoho.html

TS:   nested.flat();
来源：http://hz.vqdsnc.cn/gtkchukccj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://hz.dashuyun.cn/gtzzifxrvj.html

Go:   // 手写双层循环
来源：http://hz.xuetiantiany.cn/gtrwymocxe.html

Ruby: nested.flatten
来源：http://hz.quarkkingdee.top/gtujjbnbhy.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://hz.hongshengwenyu.top/gtjxvrcfxp.html

[D19] 按字段分组
来源：http://hz.hammf.cn/gtaugclvwd.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://hz.zhiwuduotai.top/gtwodeeawr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://hz.jiagoushi.top/gtklhajsid.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://hz.tian-w.cn/gtrzejbdah.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://hz.sweek.top/gtfgsfwnhm.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://hz.ywan-chungtsiang.top/gtusigzhtg.html

Go:   // 手写 map[string][]T
来源：http://hz.zhijiandao.cn/gtxindvfpe.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://hz.c1oappe.top/gtgnjltkml.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://hz.zhongyouzk.top/gtrjsujshp.html

[D20] 统计每个元素出现次数
来源：http://hz.zdqjudy.top/gtaigagzru.html

Py:   Counter(arr)
来源：http://hz.wangdashe.top/gtqtoqpzhf.html

PHP:  array_count_values($arr);
来源：http://hz.dianchejie.cn/gtnkkzitrb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.yvedp.cn/gtlxmjhuqg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://hz.9152youxi.cn/gttggcayua.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://hz.yonumen.top/gtquskjios.html

Go:   // 手写 map[T]int
来源：http://hz.xinyue.icu/gtjzeipmzp.html

Ruby: arr.tally
来源：http://hz.dianchejie.cn/gtzchjfatj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://hz.feifeiyinyue.top/gtmsrbczvf.html

[D21] 判断是否包含某元素
来源：http://hz.havefunace.top/gtuzkhiapj.html

Py:   x in arr
来源：http://hz.yonumen.top/gtzgkojqzn.html

PHP:  in_array($x, $arr, true);
来源：http://hz.yj20258888.top/gtkyxskyai.html

JS:   arr.includes(x)
来源：http://hz.dashuyun.cn/gtrdaxpcxk.html

TS:   arr.includes(x)
来源：http://hz.hammf.cn/gtcobzptqx.html

Java: list.contains(x)
来源：http://hz.c1oappe.top/gtiemznpvz.html

Go:   slices.Contains(arr, x)
来源：http://hz.zhaomingkeji.xyz/gtklzxcvwx.html

Ruby: arr.include?(x)
来源：http://hz.redwolf501.top/gtrlpsvzdd.html

C#:   list.Contains(x)
来源：http://hz.vqdsnc.cn/gtleqtjszw.html

[D22] 复制数组（避免共享引用）
来源：http://hz.jianghu66.top/gtelsboaud.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://hz.zhengqikj.top/gtatyorqxd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://hz.yj202588.top/gtbwfdzlvj.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://hz.ivvv.top/gtwmlpgtmz.html

TS:   [...arr];
来源：http://hz.xuetiantiany.cn/gtxwopiryt.html

Java: new ArrayList<>(list);
来源：http://hz.shuidangran.top/gtwpvsrrdq.html

Go:   copied := append([]int(nil), arr...)
来源：http://hz.daxiang520.top/gtlgexfrmj.html

Ruby: arr.dup;  arr.clone
来源：http://hz.jqgufenzy.top/gtojncfphx.html

C#:   new List<int>(list);
来源：http://hz.hnxiangtu.top/gtbpredkkh.html

[D23] reduce 累积计算
来源：http://hz.guannengcc.top/gtzgtafuhl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://hz.ehwqpu.com/gtfahcnpmn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://hz.hywenlv.cn/gthvgflfeh.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.wangshuangyany.cn/gtjmaztbxz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://hz.smart0.xyz/gttorfgxxe.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://hz.jiagoushi.top/gtjzgokgcv.html

Go:   // 手写循环
来源：http://hz.xingfuxueyuan.xyz/gtpcqvqtam.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://hz.ehwqpu.com/gtfkzqzhqb.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://hz.quarkkingdee.top/gtyhsjokwr.html

[D24] 字典 / Map 基本操作
来源：http://hz.fengsongda.top/gtkdjfmiec.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://hz.0kj1m.cn/gthefevoni.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://hz.haohaochexian.top/gtqtjovuaa.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://hz.mhx1999.top/gtjxgyqhfl.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://hz.nwbrower.top/gtuolvvqqn.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://hz.cdnleiting.top/gtoopurmwr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://hz.zhijiandao.cn/gtwigomqww.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://hz.zhongyouzk.top/gtuiocukia.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://hz.yueranfly.top/gtvogscpgb.html

[D25] Set 集合去重与交并差
来源：http://hz.smart0.xyz/gtpeuxykau.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://hz.316326.xyz/gtwbhqhyqg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://hz.c1oappe.top/gtzrmaxbwz.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://hz.snrcjt.cn/gtktkfeohm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://hz.iojbl.cn/gtzrexytum.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://hz.feifeiyinyue.top/gtylcrwxcz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://hz.vqdsnc.cn/gtjhfzozew.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://hz.jlsjyb.cn/gtclzoptyb.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://hz.yangfankeji.com/gtukjnujar.html

[D26] 数组转字符串
来源：http://hz.jyoumei.cn/gtvlgzzocn.html

Py:   ", ".join(map(str, arr))
来源：http://hz.chenzaomai.com/gtggjsukah.html

PHP:  implode(", ", $arr);
来源：http://hz.fengsongda.top/gtklrkvzzg.html

JS:   arr.join(", ")
来源：http://hz.kuanghao11.cn/gtxelcvrmv.html

TS:   arr.join(", ")
来源：http://hz.ehwqpu.com/gtmtsuvlmm.html

Java: String.join(", ", list)
来源：http://hz.dashuyun.cn/gtwkjjfcxt.html

Go:   strings.Join(strs, ", ")
来源：http://hz.havefunace.top/gtzntioguq.html

Ruby: arr.join(", ")
来源：http://hz.fengsongda.top/gtcfjpmzte.html

C#:   string.Join(", ", list)
来源：http://hz.xingfuxueyuan.xyz/gtdrmoieed.html

================================================================================
来源：http://hz.gogol.net.cn/gtwqhdtuku.html

E. 字符串处理
来源：http://hz.sufxvd.cn/gtgygarzvr.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtlwvgnceh.html

[E01] 拼接字符串
来源：http://hz.shanyushiyangkeji.top/gtstzqblxj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://hz.xinyue.icu/gtuleckhmz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://hz.birdmap.top/gtesgrmrdn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.fengsongda.top/gtxprwcdol.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://hz.jlsjyb.cn/gtkjnqjszg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://hz.kuanghao11.cn/gtxvovqywk.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://hz.jlsjyb.cn/gtwnhkkadd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://hz.jqgfzy.top/gtqcnftflj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://hz.gogol.net.cn/gtgudxyxwh.html

[E02] 重复字符串
来源：http://hz.ppjwa.cn/gtwuinhpjj.html

Py:   "ab" * 3
来源：http://hz.sufxvd.cn/gtaviwpmbb.html

PHP:  str_repeat("ab", 3);
来源：http://hz.jinqigufen.top/gtnogwnnxc.html

JS:   "ab".repeat(3)
来源：http://hz.gaohongyu789.top/gthiudifof.html

TS:   "ab".repeat(3)
来源：http://hz.0kj1m.cn/gtkvffcvla.html

Java: "ab".repeat(3)
来源：http://hz.ydjk.org.cn/gtdzgnzfjm.html

Go:   strings.Repeat("ab", 3)
来源：http://hz.jiagoushi.top/gtftqovfgk.html

Ruby: "ab" * 3
来源：http://hz.redwolf501.top/gtfzboyttu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://hz.jinghuilouyu.cn/gtevhfnjfe.html

[E03] 截取子串
来源：http://hz.mhx1999.top/gtafxvmqpg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://hz.tianlin.xyz/gtsrfdcyhv.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://hz.hywenlv.cn/gtriwpenby.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://hz.cdnleiting.top/gtzycdpfom.html

TS:   s.slice(1, 4)
来源：http://hz.ybcxt.top/gtbvvloeqw.html

Java: s.substring(1, 4)
来源：http://hz.zdqjudy.top/gtskbhrksv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://hz.ehwqpu.com/gtzxebxmrg.html

Ruby: s[1, 3];  s[1..3]
来源：http://hz.xuetiantiany.cn/gtqfhsgpqj.html

C#:   s.Substring(1, 3)
来源：http://hz.xinyue.icu/gttxwghask.html

[E04] 查找子串位置
来源：http://hz.tianlin.xyz/gtfpjucckp.html

Py:   s.find("x");  s.index("x")
来源：http://hz.haohaochexian.top/gtznsheqge.html

PHP:  strpos($s, "x");
来源：http://hz.aibaodan.cn/gtygxpaquy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://hz.yj202588.top/gtogreuopy.html

TS:   s.indexOf("x")
来源：http://hz.xziqi.cn/gtjmsrhnlp.html

Java: s.indexOf("x")
来源：http://hz.xingfuxueyuan.xyz/gtsgckwohq.html

Go:   strings.Index(s, "x")
来源：http://hz.ybcxt.top/gtbbroguvh.html

Ruby: s.index("x")
来源：http://hz.jyoumei.cn/gtmqqxanbp.html

C#:   s.IndexOf("x")
来源：http://hz.xziqi.cn/gtdhnlgwvr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://hz.shzxlz.cn/gtemcdebcm.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://hz.9152youxi.cn/gttwdguvfo.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://hz.redwolf501.top/gtzyzabguj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.chenjidiqi.icu/gtxaioeket.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://hz.ehwqpu.com/gtriaakcye.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://hz.yj20258888.top/gtsdybebed.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://hz.yuxming.cn/gtdtxguebz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://hz.jinyuanbaomall.cn/gthdpygkub.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://hz.jqgufenzy.top/gtyhsxnbsv.html

[E06] 替换子串
来源：http://hz.aibaodan.cn/gthuchdxvs.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://hz.chenlongwang.top/gtcpbjfjsx.html

PHP:  str_replace("a", "b", $s);
来源：http://hz.nwbrower.top/gtlyrpazkl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.tanke756.top/gtgcmcskzp.html

TS:   s.replaceAll("a", "b")
来源：http://hz.tianlin.xyz/gtlzcnodam.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://hz.hysaishi.cn/gtwhlfhnon.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://hz.tian-w.cn/gtrxjqvsjr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://hz.cheryme.top/gtdryrttek.html

C#:   s.Replace("a", "b")
来源：http://hz.ydzc1.top/gtplafryzv.html

[E07] 按分隔符拆分
来源：http://hz.guannengcc.top/gtncfikvhh.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://hz.zhoulong.xyz/gtpcmqtqyp.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://hz.guowangkeji.top/gthyiloyrs.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://hz.9152youxi.cn/gtvxtgzdqy.html

TS:   s.split(",")
来源：http://hz.shangyingyoupin.top/gtknlccomf.html

Java: s.split(",");  s.split("\\s+")
来源：http://hz.yvedp.cn/gtvwtwnjpv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://hz.chenjidiqi.icu/gtvctlupuc.html

Ruby: s.split(",");  s.split
来源：http://hz.yj20258.top/gtijnfbhnb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://hz.smart0.xyz/gthxbbkdku.html

[E08] 数组按分隔符合并
来源：http://hz.dianchejie.cn/gtkkjjgrvy.html

Py:   ",".join(items)
来源：http://hz.jinqigfzy.top/gtofqsysnd.html

PHP:  implode(",", $items);
来源：http://hz.meibo888.top/gtvayqztha.html

JS:   items.join(",")
来源：http://hz.yj20258888.top/gtapztrytb.html

TS:   items.join(",")
来源：http://hz.yj20258.top/gtuytfzyxd.html

Java: String.join(",", items)
来源：http://hz.chenzaomai.com/gtyhaonfcr.html

Go:   strings.Join(items, ",")
来源：http://hz.chenzaomai.com/gtzziasnab.html

Ruby: items.join(",")
来源：http://hz.shanyushiyangtech.top/gtgughvldj.html

C#:   string.Join(",", items)
来源：http://hz.tianlin.xyz/gtorbpzfud.html

[E09] 去除所有空白字符
来源：http://hz.jinqigfzy.top/gtqilqvbub.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://hz.tianlin.xyz/gtxgcynznd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://hz.9152youxi.cn/gtjrfmeucj.html

JS:   s.replace(/\s+/g, "")
来源：http://hz.jlsjyb.cn/gtcyplldxh.html

TS:   s.replace(/\s+/g, "")
来源：http://hz.xziqi.cn/gtrnupoogb.html

Java: s.replaceAll("\\s+", "")
来源：http://hz.yangfankeji.com/gtrcxeifad.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://hz.kuanghao11.cn/gtriebaspf.html

Ruby: s.gsub(/\s+/, "")
来源：http://hz.hfpthk.cn/gtjzkxiecf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://hz.yangfankeji.com/gtpkikpiqa.html

[E10] 左侧补零 / 定长填充
来源：http://hz.jinqigfzy.top/gtnmseezry.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://hz.snrcjt.cn/gtnxkqinmq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://hz.gotoacloud.top/gthuhufyrt.html

JS:   "7".padStart(3, "0")
来源：http://hz.hysaishi.cn/gtwxcushfm.html

TS:   "7".padStart(3, "0")
来源：http://hz.gaohongyu789.top/gtnrohwnnq.html

Java: String.format("%03d", 7)
来源：http://hz.wangdashe.top/gtixkpjxfn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://hz.ybcxt.top/gtcgnovxmn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://hz.xingfuxueyuan.xyz/gtlcbgsipw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.shangyingyoupin.top/gtifgygljn.html

[E11] 反转字符串
来源：http://hz.yueranfly.top/gtvzlhgxzb.html

Py:   s[::-1]
来源：http://hz.tanke756.top/gtabeecxuu.html

PHP:  strrev($s);
来源：http://hz.chenzaomai.com/gtjbcsauqb.html

JS:   [...s].reverse().join("")
来源：http://hz.zhaomingkeji.xyz/gtgjbuiqsx.html

TS:   [...s].reverse().join("")
来源：http://hz.cucudq.cn/gtvviomilj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.wangdashe.top/gtycqnemdl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.hnxiangtu.top/gtoebdjswn.html

Ruby: s.reverse
来源：http://hz.ydzc1.top/gtktnmbcxw.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.jinqigufen.top/gtnefnglzn.html

[E12] 统计某字符出现次数
来源：http://hz.shuidangran.top/gtvzihacxi.html

Py:   s.count("a")
来源：http://hz.redwolf501.top/gtndvqokel.html

PHP:  substr_count($s, "a");
来源：http://hz.sufxvd.cn/gtbumaajda.html

JS:   s.split("a").length - 1
来源：http://hz.hfpthk.cn/gtdoewsevi.html

TS:   s.split("a").length - 1
来源：http://hz.hongshengwenyu.top/gtgctcmrjb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.chenzaomai.com/gtfzapaetq.html

Go:   strings.Count(s, "a")
来源：http://hz.shzxlz.cn/gtejdwvjni.html

Ruby: s.count("a")
来源：http://hz.mhx1999.top/gtpndhtmwr.html

C#:   s.Count(c => c == 'a')
来源：http://hz.redwolf501.top/gtzisusoxb.html

[E13] 逐字符遍历
来源：http://hz.hnxiangtu.top/gtaqhzseyv.html

Py:   for ch in s: print(ch)
来源：http://hz.jiagoushi.top/gthgtbnxla.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zhijiandao.cn/gtnoutefle.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jinqigfzy.top/gtwdsiprel.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.vqdsnc.cn/gtlhhjonab.html


<!-- 参考信息 -->