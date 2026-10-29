代发 wailian999

TS:   [...arr].reverse();
来源：http://mobile.zdbjq.cn/Article/details/gmytuaqpt.sHtML

Java: Collections.reverse(list);
来源：http://mobile.hesvh.cn/Article/details/ghjmmltph.sHtML

Go:   slices.Reverse(arr)
来源：http://wap.zdbjq.cn/Article/details/glxpeuksz.sHtML

Ruby: arr.reverse
来源：http://3g.fehbvm.com/Article/details/gptcyayab.sHtML

C#:   list.Reverse();
来源：http://www.m.share.hesvh.cn/Article/details/gqydgfado.sHtML

[D12] 查找元素下标
来源：http://wap.zdbjq.cn/Article/details/gorksoyeg.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.hesvh.cn/Article/details/gwvmbvkcc.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.share.fehbvm.com/Article/details/grigpxdqt.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://blog.zdbjq.cn/Article/details/gbwyxupuj.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.fehbvm.com/Article/details/guiqwdtxi.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.blog.fehbvm.com/Article/details/gtoxxoryp.sHtML

Go:   slices.Index(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gmmekjzob.sHtML

Ruby: arr.index(x)
来源：http://baike.hesvh.cn/Article/details/grfgcdxmr.sHtML

C#:   list.IndexOf(x);
来源：http://blog.fehbvm.com/Article/details/gmmjaeuns.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.blog.zdbjq.cn/Article/details/glykquzzx.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gfkaiyhhk.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://3g.fehbvm.com/Article/details/gpwdmtlsu.sHtML

JS:   arr.filter(x => x > 3)
来源：http://read.share.zdbjq.cn/Article/details/ghcamhfsy.sHtML

TS:   arr.filter(x => x > 3)
来源：http://blog.fehbvm.com/Article/details/gwyzkviex.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.share.fehbvm.com/Article/details/gzsrhfkua.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.fehbvm.com/Article/details/gvbbtcmda.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://wap.fehbvm.com/Article/details/ghrbcpbnd.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://www.share.zdbjq.cn/Article/details/gndwueyot.sHtML

[D14] 映射转换（每个元素变形）
来源：http://read.share.zdbjq.cn/Article/details/gneqhahlf.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.share.hesvh.cn/Article/details/gdnvuknwq.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.fehbvm.com/Article/details/goedwvdyx.sHtML

JS:   arr.map(x => x * 2)
来源：http://baike.zdbjq.cn/Article/details/gdmdhzkjv.sHtML

TS:   arr.map(x => x * 2)
来源：http://read.share.zdbjq.cn/Article/details/gjuaxbcmi.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.zdbjq.cn/Article/details/glorhtzms.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gylymegtb.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://wap.hesvh.cn/Article/details/gsshlrahb.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://mobile.fehbvm.com/Article/details/gizekhpoa.sHtML

[D15] 去重
来源：http://m.share.zdbjq.cn/Article/details/gkfjayhzp.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://read.share.fehbvm.com/Article/details/ghhezryqa.sHtML

PHP:  array_unique($arr);
来源：http://wap.fehbvm.com/Article/details/gywfbwjed.sHtML

JS:   [...new Set(arr)]
来源：http://blog.hesvh.cn/Article/details/gdvbtirui.sHtML

TS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gzlrmkdmm.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://baike.fehbvm.com/Article/details/gfwykqred.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.zdbjq.cn/Article/details/grvspikzu.sHtML

Ruby: arr.uniq
来源：http://read.share.hesvh.cn/Article/details/gkyjraupq.sHtML

C#:   list.Distinct().ToList()
来源：http://www.blog.fehbvm.com/Article/details/ggmmeliqx.sHtML

[D16] 求和与平均值
来源：http://mobile.zdbjq.cn/Article/details/gukqrmlev.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://wap.hesvh.cn/Article/details/guxphjrqi.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://m.share.zdbjq.cn/Article/details/geoaezwdw.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://read.share.zdbjq.cn/Article/details/grzixnxwp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gcdhbogmv.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://blog.zdbjq.cn/Article/details/glcukazwt.sHtML

Go:   // 手写循环累加
来源：http://mobile.fehbvm.com/Article/details/gtidbxmdz.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.fehbvm.com/Article/details/gujipqbuf.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.zdbjq.cn/Article/details/gduhorrpv.sHtML

[D17] 最大值与最小值
来源：http://3g.zdbjq.cn/Article/details/gtlkfpdqy.sHtML

Py:   max(arr);  min(arr)
来源：http://wap.hesvh.cn/Article/details/gdkoqzwgd.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gbkrfllwz.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/gsyifbrmp.sHtML

TS:   Math.max(...arr);
来源：http://www.share.zdbjq.cn/Article/details/ggsfxoroj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.zdbjq.cn/Article/details/guchvrmnm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.hesvh.cn/Article/details/gfqusweqo.sHtML

Ruby: arr.max;  arr.min
来源：http://wap.hesvh.cn/Article/details/goplqoupl.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.zdbjq.cn/Article/details/gptoxkvtb.sHtML

[D18] 扁平化嵌套数组
来源：http://www.share.fehbvm.com/Article/details/gqsaicxuz.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.m.share.zdbjq.cn/Article/details/gslcrtnag.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gfbfcyhxx.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.hesvh.cn/Article/details/gebtpyjal.sHtML

TS:   nested.flat();
来源：http://www.m.share.zdbjq.cn/Article/details/ggjawirte.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.fehbvm.com/Article/details/geyqsrcjx.sHtML

Go:   // 手写双层循环
来源：http://3g.fehbvm.com/Article/details/gppdlupoq.sHtML

Ruby: nested.flatten
来源：http://blog.hesvh.cn/Article/details/gluaqqhgr.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.hesvh.cn/Article/details/gxujlgore.sHtML

[D19] 按字段分组
来源：http://read.share.zdbjq.cn/Article/details/gmkitiajn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fehbvm.com/Article/details/gopbgsfcp.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.zdbjq.cn/Article/details/goesfwakv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.hesvh.cn/Article/details/gwjvqkqkz.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.fehbvm.com/Article/details/ghezcwiln.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/guilfkqvb.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.hesvh.cn/Article/details/gyrawotvp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.zdbjq.cn/Article/details/gjbahaeod.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fehbvm.com/Article/details/gepdcqiat.sHtML

[D20] 统计每个元素出现次数
来源：http://www.blog.hesvh.cn/Article/details/gximiuwix.sHtML

Py:   Counter(arr)
来源：http://www.share.fehbvm.com/Article/details/goqgnrexk.sHtML

PHP:  array_count_values($arr);
来源：http://baike.zdbjq.cn/Article/details/gjdwlzyjg.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/gdtkaqfqu.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gmvrnkbbh.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/gjjtnzupl.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.fehbvm.com/Article/details/gizcfuzwj.sHtML

Ruby: arr.tally
来源：http://wap.zdbjq.cn/Article/details/ghhanmqft.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.zdbjq.cn/Article/details/gptabfgiz.sHtML

[D21] 判断是否包含某元素
来源：http://blog.hesvh.cn/Article/details/gbzorminc.sHtML

Py:   x in arr
来源：http://read.share.zdbjq.cn/Article/details/gktfqnwfx.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/gbzdbmoxr.sHtML

JS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gzhedorhe.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gmjywxmaq.sHtML

Java: list.contains(x)
来源：http://www.share.hesvh.cn/Article/details/gmfyeqdml.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gcfcdihfd.sHtML

Ruby: arr.include?(x)
来源：http://3g.fehbvm.com/Article/details/gqhgrwtir.sHtML

C#:   list.Contains(x)
来源：http://blog.zdbjq.cn/Article/details/gqkrsnxyn.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/gmyrisnvv.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/genkmdxcm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://read.share.fehbvm.com/Article/details/gxaxontqp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://m.share.zdbjq.cn/Article/details/gaakjslxk.sHtML

TS:   [...arr];
来源：http://www.share.hesvh.cn/Article/details/gjvtwnqjm.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.zdbjq.cn/Article/details/ggehsirnq.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fehbvm.com/Article/details/gpzdaduji.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.fehbvm.com/Article/details/gwppfasnh.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/giwbuembg.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/giinbtuey.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fehbvm.com/Article/details/gvoqocqfa.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.fehbvm.com/Article/details/goojshwgn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gssprrgvw.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/ghatxplbq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.hesvh.cn/Article/details/gdkhnuizx.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gwxuhcasi.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fehbvm.com/Article/details/gjluukcwt.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.hesvh.cn/Article/details/grtjvqcet.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.hesvh.cn/Article/details/gehuxqfva.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.hesvh.cn/Article/details/ghqegmcxb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.zdbjq.cn/Article/details/gsxvaneib.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.share.hesvh.cn/Article/details/ggxqfjlzr.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.hesvh.cn/Article/details/ggphjqfkh.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fehbvm.com/Article/details/gjojukshc.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.zdbjq.cn/Article/details/guztrbpuc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.hesvh.cn/Article/details/gbaqmedzl.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/gewzrngjv.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/grsxyigim.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.hesvh.cn/Article/details/ggywwkayl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.hesvh.cn/Article/details/gmfsrgoqr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.hesvh.cn/Article/details/gdygsxejv.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.zdbjq.cn/Article/details/gdwjnaejq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.zdbjq.cn/Article/details/gewxxdipo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.hesvh.cn/Article/details/gxxjvqugo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fehbvm.com/Article/details/gqovdamhg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.zdbjq.cn/Article/details/gwwdchrwf.sHtML

[D26] 数组转字符串
来源：http://3g.zdbjq.cn/Article/details/gnsfideao.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.zdbjq.cn/Article/details/gqtskqfvb.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.hesvh.cn/Article/details/gewlzsubu.sHtML

JS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gpbdbaloj.sHtML

TS:   arr.join(", ")
来源：http://m.share.hesvh.cn/Article/details/gckdrygea.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gjukjtrpu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.zdbjq.cn/Article/details/ggljxhnca.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gpspwdluh.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.fehbvm.com/Article/details/gfhppodfe.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gnrkjijcv.sHtML

E. 字符串处理
来源：http://wap.hesvh.cn/Article/details/gvwhfkrcc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/golszrzmd.sHtML

[E01] 拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gaowifgbe.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fehbvm.com/Article/details/gzlltrohj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.zdbjq.cn/Article/details/gqrdwtljp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gfzghjnal.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gvxczkqgb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/gdsgltfiz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fehbvm.com/Article/details/gjqgkmwnn.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/gogqmmwim.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fehbvm.com/Article/details/gwbcditpq.sHtML

[E02] 重复字符串
来源：http://mobile.hesvh.cn/Article/details/gekmyoalw.sHtML

Py:   "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gjnyglsam.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.hesvh.cn/Article/details/gysncngii.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gtbbaxkny.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gtjekbnji.sHtML

Java: "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/glluaxioh.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/gvorccxla.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gomzqdptz.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fehbvm.com/Article/details/ggaqbfnbp.sHtML

[E03] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gvzyzqbay.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.zdbjq.cn/Article/details/gqnraicpt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gjvjzoxhz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gqyruvhbg.sHtML

TS:   s.slice(1, 4)
来源：http://blog.hesvh.cn/Article/details/godnavkma.sHtML

Java: s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gfybpgfvs.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.fehbvm.com/Article/details/gezcrijbh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.zdbjq.cn/Article/details/greosodzu.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.zdbjq.cn/Article/details/gwmhsdykf.sHtML

[E04] 查找子串位置
来源：http://3g.hesvh.cn/Article/details/gcprlvnsq.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/gmllnkhxt.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.zdbjq.cn/Article/details/grockfsty.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.zdbjq.cn/Article/details/glvpkvxaz.sHtML

TS:   s.indexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/glipuhyok.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gewurtsmp.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.zdbjq.cn/Article/details/gcaqgyeph.sHtML

Ruby: s.index("x")
来源：http://blog.fehbvm.com/Article/details/gwxztxotw.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.fehbvm.com/Article/details/gxulqqgdl.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fehbvm.com/Article/details/gzovuysun.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/ghmbirlhk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fehbvm.com/Article/details/gqxabdgan.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/gnisltrhb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.hesvh.cn/Article/details/gsbepcoxh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gaijkiito.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.fehbvm.com/Article/details/gtopudxmf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gkyltxawz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gpwclyicy.sHtML

[E06] 替换子串
来源：http://m.share.fehbvm.com/Article/details/gyjzuplgm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gqxiwyhyw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.hesvh.cn/Article/details/gcufvbaic.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gzrgydejq.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/glkhefjmo.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gbtjieoss.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.fehbvm.com/Article/details/gfwscuccx.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gtjnossxd.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.hesvh.cn/Article/details/gxpatvaux.sHtML

[E07] 按分隔符拆分
来源：http://mobile.hesvh.cn/Article/details/gmylczjum.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.zdbjq.cn/Article/details/gobwdvojv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.hesvh.cn/Article/details/gsxterucq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.zdbjq.cn/Article/details/guuhhewfl.sHtML

TS:   s.split(",")
来源：http://www.m.share.hesvh.cn/Article/details/gxciuczvo.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.zdbjq.cn/Article/details/gjfferuso.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.hesvh.cn/Article/details/gcigbtmhs.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.zdbjq.cn/Article/details/gcnylunae.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.hesvh.cn/Article/details/gksabpmvm.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fehbvm.com/Article/details/gslxnyqin.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/gorienltr.sHtML

PHP:  implode(",", $items);
来源：http://m.share.hesvh.cn/Article/details/gknijbmtv.sHtML

JS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gpljyjskg.sHtML

TS:   items.join(",")
来源：http://www.share.zdbjq.cn/Article/details/ghfglonqr.sHtML

Java: String.join(",", items)
来源：http://mobile.fehbvm.com/Article/details/ghrobjlrz.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.hesvh.cn/Article/details/gpnozpjwv.sHtML

Ruby: items.join(",")
来源：http://baike.hesvh.cn/Article/details/gpfcypzyk.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gcvkaticc.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/grzwrknzv.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.zdbjq.cn/Article/details/gqfqxgyrl.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fehbvm.com/Article/details/gyfjmbyzr.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.zdbjq.cn/Article/details/ggbojacqn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gucynrlfm.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.fehbvm.com/Article/details/gerblfdnk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.zdbjq.cn/Article/details/ghnlfvamy.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.hesvh.cn/Article/details/gfyysykvc.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gbzeemanf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.zdbjq.cn/Article/details/gagwstcbv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.hesvh.cn/Article/details/ggyynhpqs.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.zdbjq.cn/Article/details/gvvvxlvxp.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gdvnmbybl.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gdoojvlxj.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gaolhgroh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gjxeixhnu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/gddwxqzcx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.hesvh.cn/Article/details/giddvfwmi.sHtML

[E11] 反转字符串
来源：http://mobile.zdbjq.cn/Article/details/gcuzhezok.sHtML

Py:   s[::-1]
来源：http://3g.hesvh.cn/Article/details/ggeixnfwm.sHtML

PHP:  strrev($s);
来源：http://read.share.hesvh.cn/Article/details/gyioctrhc.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gskzuagyp.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gwpbbgdct.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/ghknhfovb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.zdbjq.cn/Article/details/gecshauqo.sHtML

Ruby: s.reverse
来源：http://www.share.zdbjq.cn/Article/details/giymgmvca.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.hesvh.cn/Article/details/gltgoygrl.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.zdbjq.cn/Article/details/gfhwavhck.sHtML

Py:   s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gjackjsto.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.fehbvm.com/Article/details/gfiwxvkxe.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gixwqtjrp.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gaezgwgit.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.fehbvm.com/Article/details/gxlrmmzfd.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/gwlxznkrz.sHtML

Ruby: s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gccbipxdl.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.zdbjq.cn/Article/details/gzzqwifyz.sHtML

[E13] 逐字符遍历
来源：http://mobile.fehbvm.com/Article/details/grrxuyjsj.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fehbvm.com/Article/details/gvktrtqtj.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.hesvh.cn/Article/details/ggzmwvwhg.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gswmvpvix.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gtkjcqrtp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.zdbjq.cn/Article/details/gjbygztce.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.zdbjq.cn/Article/details/gtrgrmrlu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.hesvh.cn/Article/details/gsvqshekd.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.hesvh.cn/Article/details/gwdbgemrg.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.zdbjq.cn/Article/details/grahhvvck.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.zdbjq.cn/Article/details/gesqwssnf.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.hesvh.cn/Article/details/gjfitluqn.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.zdbjq.cn/Article/details/gcpxjbdlp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/gduwwmkdc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.fehbvm.com/Article/details/gtrjqasgw.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fehbvm.com/Article/details/gzenqpfts.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fehbvm.com/Article/details/gwbmbmwxx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fehbvm.com/Article/details/guvaxgrgw.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/gfutfroym.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.fehbvm.com/Article/details/gpxjhkprr.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.zdbjq.cn/Article/details/gnrqqiauq.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fehbvm.com/Article/details/gguolxxhc.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fehbvm.com/Article/details/gbpgxzfqk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fehbvm.com/Article/details/gmfowlfkc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.hesvh.cn/Article/details/ghxekmela.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.hesvh.cn/Article/details/gjncamiwx.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.hesvh.cn/Article/details/ghuacnvvi.sHtML

[E16] 数字千分位
来源：http://blog.hesvh.cn/Article/details/gptkhgiwq.sHtML

Py:   f"{1234567:,}"
来源：http://wap.hesvh.cn/Article/details/gzkvzurke.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/gticzdwal.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gdksvdfbu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/gdwycpoxb.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.hesvh.cn/Article/details/gngtbculk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.zdbjq.cn/Article/details/gmnsybbij.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.fehbvm.com/Article/details/gjhxavopq.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fehbvm.com/Article/details/ggelbjepe.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/gxaernzas.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fehbvm.com/Article/details/gjbuqlbtu.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.zdbjq.cn/Article/details/geekqgmbo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.hesvh.cn/Article/details/grasndqju.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gikiyuqtr.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.hesvh.cn/Article/details/gbhbysmdq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/gvtzikoqd.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/glohwqjdp.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fehbvm.com/Article/details/gediekhps.sHtML

[E18] 模板占位符替换
来源：http://blog.fehbvm.com/Article/details/gmmphhhlx.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/gbdjrwmwp.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.hesvh.cn/Article/details/gzucauaxd.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/ggnxnzsyz.sHtML


<!-- 参考信息 -->