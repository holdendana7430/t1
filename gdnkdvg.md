代发 wailian999

C#:   list.Reverse();
来源：http://www.share.zdbjq.cn/Article/details/gusxxkmqt.sHtML

[D12] 查找元素下标
来源：http://www.blog.hesvh.cn/Article/details/gjayldyli.sHtML

Py:   arr.index(x);  x in arr
来源：http://baike.hesvh.cn/Article/details/glvtvcgyf.sHtML

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://read.share.fehbvm.com/Article/details/grjhkdgsk.sHtML

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://m.share.fehbvm.com/Article/details/ggwsohzxb.sHtML

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.share.zdbjq.cn/Article/details/gijjbwnlq.sHtML

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://m.share.fehbvm.com/Article/details/gydymmptl.sHtML

Go:   slices.Index(arr, x)
来源：http://wap.hesvh.cn/Article/details/gdbiebqgm.sHtML

Ruby: arr.index(x)
来源：http://wap.fehbvm.com/Article/details/gieqmusvq.sHtML

C#:   list.IndexOf(x);
来源：http://3g.zdbjq.cn/Article/details/gxxfnjjpg.sHtML

[D13] 过滤（保留满足条件的）
来源：http://www.m.share.zdbjq.cn/Article/details/gzssgzpjd.sHtML

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://baike.hesvh.cn/Article/details/gaedzlqfx.sHtML

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://read.share.hesvh.cn/Article/details/gskqscrvn.sHtML

JS:   arr.filter(x => x > 3)
来源：http://3g.zdbjq.cn/Article/details/ghferutvg.sHtML

TS:   arr.filter(x => x > 3)
来源：http://wap.fehbvm.com/Article/details/gwwaaqlua.sHtML

Java: list.stream().filter(x -> x > 3).toList()
来源：http://read.share.zdbjq.cn/Article/details/gzrzdguvu.sHtML

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://m.share.zdbjq.cn/Article/details/gkcfwqpva.sHtML

Ruby: arr.select { |x| x > 3 }
来源：http://m.share.zdbjq.cn/Article/details/gipqqtgpm.sHtML

C#:   list.Where(x => x > 3).ToList()
来源：http://blog.hesvh.cn/Article/details/gflbyjucy.sHtML

[D14] 映射转换（每个元素变形）
来源：http://www.blog.zdbjq.cn/Article/details/ggtblxfog.sHtML

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.m.share.fehbvm.com/Article/details/gyrxymbwf.sHtML

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://m.share.hesvh.cn/Article/details/gydmmivym.sHtML

JS:   arr.map(x => x * 2)
来源：http://www.share.fehbvm.com/Article/details/gusmoyita.sHtML

TS:   arr.map(x => x * 2)
来源：http://www.blog.fehbvm.com/Article/details/gyqvyjpul.sHtML

Java: list.stream().map(x -> x * 2).toList()
来源：http://blog.zdbjq.cn/Article/details/goyjbxzcv.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/gxrekomzq.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gxwxxvsre.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://blog.hesvh.cn/Article/details/gslbbsarr.sHtML

[D15] 去重
来源：http://www.share.hesvh.cn/Article/details/gdfxzqyev.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://3g.hesvh.cn/Article/details/gjmnecznh.sHtML

PHP:  array_unique($arr);
来源：http://www.share.fehbvm.com/Article/details/grpbgajwb.sHtML

JS:   [...new Set(arr)]
来源：http://baike.zdbjq.cn/Article/details/gxhxgjymr.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.fehbvm.com/Article/details/gzpiesdjz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://wap.hesvh.cn/Article/details/gxhgtokyn.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://www.blog.fehbvm.com/Article/details/gxkbcsrus.sHtML

Ruby: arr.uniq
来源：http://3g.fehbvm.com/Article/details/gfgwdwjbg.sHtML

C#:   list.Distinct().ToList()
来源：http://wap.fehbvm.com/Article/details/gnajmapkx.sHtML

[D16] 求和与平均值
来源：http://www.m.share.hesvh.cn/Article/details/gzgpamtgs.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://blog.hesvh.cn/Article/details/ghhaadypu.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://baike.hesvh.cn/Article/details/gclvrpwlu.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.fehbvm.com/Article/details/gtkzerdcs.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gpsmdasho.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.share.hesvh.cn/Article/details/gittmpjky.sHtML

Go:   // 手写循环累加
来源：http://blog.fehbvm.com/Article/details/gzakqvrts.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.fehbvm.com/Article/details/gocohfmxp.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.zdbjq.cn/Article/details/gvoawyrff.sHtML

[D17] 最大值与最小值
来源：http://wap.fehbvm.com/Article/details/gytfmcatw.sHtML

Py:   max(arr);  min(arr)
来源：http://blog.fehbvm.com/Article/details/goxcpnpri.sHtML

PHP:  max($arr);  min($arr);
来源：http://3g.hesvh.cn/Article/details/gkwlvttfr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.fehbvm.com/Article/details/gssrihcnt.sHtML

TS:   Math.max(...arr);
来源：http://baike.hesvh.cn/Article/details/gjlgmpdun.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.hesvh.cn/Article/details/gmkinbdrm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/goblbhgpp.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.fehbvm.com/Article/details/ghybtdnwc.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.hesvh.cn/Article/details/gclawcupv.sHtML

[D18] 扁平化嵌套数组
来源：http://www.blog.fehbvm.com/Article/details/gxxccdvln.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://baike.hesvh.cn/Article/details/gbonslkpf.sHtML

PHP:  array_merge(...$nested);
来源：http://baike.hesvh.cn/Article/details/gmsijqrod.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://wap.hesvh.cn/Article/details/gfcpqzpgr.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/gkdfnodff.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.zdbjq.cn/Article/details/gznjcxynj.sHtML

Go:   // 手写双层循环
来源：http://wap.zdbjq.cn/Article/details/gqqzgggku.sHtML

Ruby: nested.flatten
来源：http://www.blog.zdbjq.cn/Article/details/galzyyopx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.hesvh.cn/Article/details/gzmbumemw.sHtML

[D19] 按字段分组
来源：http://m.share.zdbjq.cn/Article/details/gcslrrhmb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.hesvh.cn/Article/details/ggjwxmjdf.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.zdbjq.cn/Article/details/gkonvwame.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/getzhgaed.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.zdbjq.cn/Article/details/gpuuocxvv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/gkfepfffp.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.zdbjq.cn/Article/details/gtbzcyltp.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.fehbvm.com/Article/details/glmgcrtyy.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://wap.fehbvm.com/Article/details/glpzvsssf.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/gueczljir.sHtML

Py:   Counter(arr)
来源：http://m.share.hesvh.cn/Article/details/gmcxcdzzu.sHtML

PHP:  array_count_values($arr);
来源：http://3g.zdbjq.cn/Article/details/gcheelyvu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.zdbjq.cn/Article/details/gzsoqjlaw.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gcxqvssty.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.hesvh.cn/Article/details/getskywwu.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.hesvh.cn/Article/details/gblirasqf.sHtML

Ruby: arr.tally
来源：http://www.m.share.fehbvm.com/Article/details/gzqghlfkg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.hesvh.cn/Article/details/gsaopltib.sHtML

[D21] 判断是否包含某元素
来源：http://wap.zdbjq.cn/Article/details/gdqoxjcua.sHtML

Py:   x in arr
来源：http://www.m.share.fehbvm.com/Article/details/gczcqbtqo.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.zdbjq.cn/Article/details/gwzbougzz.sHtML

JS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gjppuglzv.sHtML

TS:   arr.includes(x)
来源：http://read.share.fehbvm.com/Article/details/ganepfsdt.sHtML

Java: list.contains(x)
来源：http://3g.zdbjq.cn/Article/details/gtxqhwqsc.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.hesvh.cn/Article/details/gsbfpenzn.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/grhsysvcb.sHtML

C#:   list.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/ghoprdqjy.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fehbvm.com/Article/details/guztfkgoo.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fehbvm.com/Article/details/gmikzswox.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.hesvh.cn/Article/details/ghzmijuqp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.zdbjq.cn/Article/details/gjqphdkul.sHtML

TS:   [...arr];
来源：http://mobile.hesvh.cn/Article/details/gitczjfkt.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.zdbjq.cn/Article/details/ggmbtuakb.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://mobile.zdbjq.cn/Article/details/gsrymepvr.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fehbvm.com/Article/details/gtckzgrpu.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.fehbvm.com/Article/details/guniokruw.sHtML

[D23] reduce 累积计算
来源：http://baike.zdbjq.cn/Article/details/gaeftyrbt.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.zdbjq.cn/Article/details/glaesvspg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.zdbjq.cn/Article/details/gbcduzenp.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gqrmumkwi.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gauqgirnx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.fehbvm.com/Article/details/gwvrfqzrx.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gcnbdtsdd.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fehbvm.com/Article/details/gocvdbfen.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fehbvm.com/Article/details/ggbrojwem.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.hesvh.cn/Article/details/gqvqmzomm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.hesvh.cn/Article/details/gipopxnsn.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.hesvh.cn/Article/details/gondhzwrr.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.hesvh.cn/Article/details/gzywjovwv.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gppjkfnko.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/gvwzvhrcy.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.zdbjq.cn/Article/details/gyzenopwg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fehbvm.com/Article/details/gelithuay.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.hesvh.cn/Article/details/gyzvdflsi.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.fehbvm.com/Article/details/gsykjnpjf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fehbvm.com/Article/details/gngvzsxrd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.hesvh.cn/Article/details/gczubvzhs.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.hesvh.cn/Article/details/gdhmsdvdz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.hesvh.cn/Article/details/gsgqvewsp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gdtdbvlfb.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.fehbvm.com/Article/details/ggnwuqhrs.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.fehbvm.com/Article/details/ggoyaaipn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gsijvyscg.sHtML

[D26] 数组转字符串
来源：http://www.blog.hesvh.cn/Article/details/gvpushctd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.zdbjq.cn/Article/details/gyxmjzbrt.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/guzncbnud.sHtML

JS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gvdmajqps.sHtML

TS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gcalqczgn.sHtML

Java: String.join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gynsmbuvs.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/gfthfsxys.sHtML

Ruby: arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gjbbbsdmp.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gxijvtbdv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ggzvwkjci.sHtML

E. 字符串处理
来源：http://mobile.hesvh.cn/Article/details/gxgelllpv.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gocfyykvz.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gzuwrtuqr.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.hesvh.cn/Article/details/gydtnnunu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/gkznnjkgc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gyeczwyez.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/gqzghgelu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.zdbjq.cn/Article/details/gkvojiofh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.zdbjq.cn/Article/details/gentemjxd.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.zdbjq.cn/Article/details/gkgwjufgu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gtcqxmojw.sHtML

[E02] 重复字符串
来源：http://www.m.share.hesvh.cn/Article/details/gjdxlkrhe.sHtML

Py:   "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/gcgilrnow.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.zdbjq.cn/Article/details/gcisxwblq.sHtML

JS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/glwtblhkg.sHtML

TS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/gmocyolhh.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gssbgevqc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.hesvh.cn/Article/details/gyotxvjit.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gbxkswonr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://blog.hesvh.cn/Article/details/gscwxdpeb.sHtML

[E03] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gzvofdzsg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.zdbjq.cn/Article/details/gpauazuff.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gdmvdblqm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gwqsgnetl.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gundwvzkt.sHtML

Java: s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gyzgqbghj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.hesvh.cn/Article/details/gpamfuudz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/gnxsrwjyy.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fehbvm.com/Article/details/ghnmrnmyz.sHtML

[E04] 查找子串位置
来源：http://wap.hesvh.cn/Article/details/gdjwvczub.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/gglzlmxlf.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.hesvh.cn/Article/details/geedgdeyv.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.zdbjq.cn/Article/details/gfgdfnnmo.sHtML

TS:   s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/ggpdwwmjb.sHtML

Java: s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gqwrfzuaj.sHtML

Go:   strings.Index(s, "x")
来源：http://m.share.hesvh.cn/Article/details/giwpzscth.sHtML

Ruby: s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gcojhihgo.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gdrcnkdlb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.zdbjq.cn/Article/details/gvjordxax.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.hesvh.cn/Article/details/gicizarok.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fehbvm.com/Article/details/glccjrojg.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.hesvh.cn/Article/details/gnsuzisjf.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.zdbjq.cn/Article/details/gspmesoju.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.zdbjq.cn/Article/details/gdqkpvqjz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.fehbvm.com/Article/details/gncadcxfi.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.hesvh.cn/Article/details/gqjjocrqy.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fehbvm.com/Article/details/gvqswycva.sHtML

[E06] 替换子串
来源：http://www.share.zdbjq.cn/Article/details/gdwpnahho.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gwhbcdonw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fehbvm.com/Article/details/gchazhvzd.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/guvptokkg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gyhkfuvnf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gdrwnhbmb.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gcbhznqhy.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gyebgoowi.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.hesvh.cn/Article/details/gownfxcxt.sHtML

[E07] 按分隔符拆分
来源：http://blog.zdbjq.cn/Article/details/gkmbokbgv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://read.share.hesvh.cn/Article/details/gyeuhsjyw.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gmzguzjon.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.zdbjq.cn/Article/details/gwnvekmsu.sHtML

TS:   s.split(",")
来源：http://www.blog.hesvh.cn/Article/details/ghryivkfz.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.zdbjq.cn/Article/details/ghaipisbl.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fehbvm.com/Article/details/gvcsmhicj.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.zdbjq.cn/Article/details/gabbemwzt.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/gxrrytjhu.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.hesvh.cn/Article/details/gamxvnbfa.sHtML

Py:   ",".join(items)
来源：http://baike.fehbvm.com/Article/details/gwwzqemce.sHtML

PHP:  implode(",", $items);
来源：http://wap.zdbjq.cn/Article/details/gvazxrpuo.sHtML

JS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gwjfxrbrn.sHtML

TS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gctkumask.sHtML

Java: String.join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gmgcekfds.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.zdbjq.cn/Article/details/gkwmwnrob.sHtML

Ruby: items.join(",")
来源：http://baike.hesvh.cn/Article/details/gjrmjzmvt.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gclsrwsir.sHtML

[E09] 去除所有空白字符
来源：http://blog.fehbvm.com/Article/details/gsojhwugt.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.hesvh.cn/Article/details/gmtekvpim.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/gxlauinqj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gpcvdjbha.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gvoctrxgo.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/gpledbysp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fehbvm.com/Article/details/gaitaqepm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.zdbjq.cn/Article/details/gkkijoyci.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.share.fehbvm.com/Article/details/gbpzhjldb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.zdbjq.cn/Article/details/gkpooksib.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gnwufxkjv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/glrykrjdy.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gzwhxmnul.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gnootxnfk.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/grrpxzfph.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gqoquhbms.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gccyarzvl.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.hesvh.cn/Article/details/gbavfmttm.sHtML

[E11] 反转字符串
来源：http://read.share.zdbjq.cn/Article/details/grpthgkit.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/gxulytieg.sHtML

PHP:  strrev($s);
来源：http://wap.zdbjq.cn/Article/details/gvxgxrwrq.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gohmgxxuc.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gcejwjmrd.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/gwveiwbvn.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fehbvm.com/Article/details/gzrsbmttu.sHtML

Ruby: s.reverse
来源：http://baike.fehbvm.com/Article/details/gyfuworsu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/ghjxzpxzi.sHtML

[E12] 统计某字符出现次数
来源：http://blog.zdbjq.cn/Article/details/gxtermjwq.sHtML

Py:   s.count("a")
来源：http://blog.fehbvm.com/Article/details/gbbreawqg.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.fehbvm.com/Article/details/gghwwuhfl.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gsjkpfird.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/grbshinlc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.zdbjq.cn/Article/details/gzwdisqva.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fehbvm.com/Article/details/gphuorypw.sHtML

Ruby: s.count("a")
来源：http://www.blog.hesvh.cn/Article/details/grvyeojfl.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.zdbjq.cn/Article/details/gxjoaazbz.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/gfcwrvgon.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/gzltekxcu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.hesvh.cn/Article/details/guuimisqp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gpyvygebx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gmajdzbus.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.hesvh.cn/Article/details/gekknqviw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.zdbjq.cn/Article/details/gagkqaojr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fehbvm.com/Article/details/gonekpgfa.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fehbvm.com/Article/details/gdrpoyzln.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fehbvm.com/Article/details/gvsxlseko.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/gsugqoorh.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/gnozpgeba.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/gycbijdsz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.zdbjq.cn/Article/details/gzdzownsw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.hesvh.cn/Article/details/glvkzcdti.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fehbvm.com/Article/details/gbefakrpa.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.hesvh.cn/Article/details/gypoyzeog.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/geursdumf.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.hesvh.cn/Article/details/gumvfoigb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/gkdjlfits.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fehbvm.com/Article/details/gehbricmp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.zdbjq.cn/Article/details/gvnsdoban.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fehbvm.com/Article/details/gqulicncq.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.zdbjq.cn/Article/details/gynzafazj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fehbvm.com/Article/details/gmqbamsll.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.m.share.fehbvm.com/Article/details/gntksxskr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fehbvm.com/Article/details/gengjihvv.sHtML

[E16] 数字千分位
来源：http://baike.zdbjq.cn/Article/details/gdermhsud.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fehbvm.com/Article/details/gsbhccpae.sHtML

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/grjrstlql.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gmasygldw.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.zdbjq.cn/Article/details/glzrppnkn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gptvjprir.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.hesvh.cn/Article/details/gtbiphwjq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.zdbjq.cn/Article/details/gjkdnjxfm.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.fehbvm.com/Article/details/gqnxhhoch.sHtML

[E17] 首字母大写
来源：http://m.share.hesvh.cn/Article/details/gvnfsqsdi.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.zdbjq.cn/Article/details/gefyotkfd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fehbvm.com/Article/details/gevodyfaz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gocyztodh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gbwpnvdad.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.hesvh.cn/Article/details/gcotymbqf.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/gugjwsiew.sHtML

Ruby: s.capitalize
来源：http://www.share.zdbjq.cn/Article/details/garrunesk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.hesvh.cn/Article/details/gvfzurpbh.sHtML

[E18] 模板占位符替换
来源：http://m.share.hesvh.cn/Article/details/gpezypgkv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/gqculsnka.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.zdbjq.cn/Article/details/gsevkfhbu.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.hesvh.cn/Article/details/gpvqdltlr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gjtqymfxn.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gboqkxfbo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/ggivfcwld.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/gbqaywbdr.sHtML


<!-- 参考信息 -->