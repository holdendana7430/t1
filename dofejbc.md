代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://read.share.hesvh.cn/Article/details/gpzwhthwx.sHtML

Go:   // 手写循环
来源：http://wap.hesvh.cn/Article/details/gzdcbmywc.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://read.share.fehbvm.com/Article/details/ghdafllyo.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://wap.fehbvm.com/Article/details/gpenexnds.sHtML

[D15] 去重
来源：http://mobile.hesvh.cn/Article/details/gxbhcirjb.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://blog.zdbjq.cn/Article/details/gikbetcoy.sHtML

PHP:  array_unique($arr);
来源：http://blog.hesvh.cn/Article/details/gbalpvnmn.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.hesvh.cn/Article/details/gbvryzeoc.sHtML

TS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/gvbnihlrz.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://3g.fehbvm.com/Article/details/gxsewsmla.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://mobile.hesvh.cn/Article/details/gekzafzld.sHtML

Ruby: arr.uniq
来源：http://3g.fehbvm.com/Article/details/gyxvdmssc.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.zdbjq.cn/Article/details/grcucfjpw.sHtML

[D16] 求和与平均值
来源：http://mobile.hesvh.cn/Article/details/gagweoonh.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.blog.hesvh.cn/Article/details/ghicnhmfi.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://blog.fehbvm.com/Article/details/gvxiyuqax.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gczezkbcv.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gbykojfxr.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://m.share.fehbvm.com/Article/details/gjpblxfyc.sHtML

Go:   // 手写循环累加
来源：http://www.share.hesvh.cn/Article/details/gerxejcox.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.m.share.zdbjq.cn/Article/details/gefeqkuhv.sHtML

C#:   list.Sum();  list.Average()
来源：http://blog.hesvh.cn/Article/details/gadpsjgwh.sHtML

[D17] 最大值与最小值
来源：http://3g.hesvh.cn/Article/details/gcqxifrfn.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.zdbjq.cn/Article/details/gkcmibuwa.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fehbvm.com/Article/details/gqpfdxvzp.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.zdbjq.cn/Article/details/gwznnoltz.sHtML

TS:   Math.max(...arr);
来源：http://read.share.fehbvm.com/Article/details/gyjxnylqc.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://read.share.hesvh.cn/Article/details/gfxwcwzpm.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.zdbjq.cn/Article/details/gnksendpf.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.hesvh.cn/Article/details/gsqyccjbs.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.zdbjq.cn/Article/details/ghbjcfozu.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.zdbjq.cn/Article/details/ghqgvxjal.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.hesvh.cn/Article/details/gbtkcedzm.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/gwhfhhdiy.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://3g.fehbvm.com/Article/details/gtcfqkumh.sHtML

TS:   nested.flat();
来源：http://wap.fehbvm.com/Article/details/gdgkliped.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/ghlboqztw.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/gxqowrxeu.sHtML

Ruby: nested.flatten
来源：http://www.share.zdbjq.cn/Article/details/gohfdqvly.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.hesvh.cn/Article/details/gdapgujsz.sHtML

[D19] 按字段分组
来源：http://baike.zdbjq.cn/Article/details/glsyxflas.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.fehbvm.com/Article/details/gqpeklcju.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fehbvm.com/Article/details/ghxcpxtum.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/gsxlvnbni.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.fehbvm.com/Article/details/gzgcheyxf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.zdbjq.cn/Article/details/gqjiqkteh.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.hesvh.cn/Article/details/gvnznskxy.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.hesvh.cn/Article/details/gqqdpgjyg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/gtmgwrdye.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fehbvm.com/Article/details/gzkvqyajk.sHtML

Py:   Counter(arr)
来源：http://mobile.hesvh.cn/Article/details/gelrtutkv.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/geeeggefn.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/gfdsbjehr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/gnydjeybi.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://m.share.fehbvm.com/Article/details/gudxzabtp.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.fehbvm.com/Article/details/gaplupblj.sHtML

Ruby: arr.tally
来源：http://www.blog.hesvh.cn/Article/details/gcipuglgq.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.zdbjq.cn/Article/details/gmjcjqbhs.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/gkmiqtiyx.sHtML

Py:   x in arr
来源：http://read.share.hesvh.cn/Article/details/gnfcnljgh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.hesvh.cn/Article/details/gkxqvchgl.sHtML

JS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gbzlphdzw.sHtML

TS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gefjvaamx.sHtML

Java: list.contains(x)
来源：http://baike.fehbvm.com/Article/details/glqixzyxs.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/ghfrybbvs.sHtML

Ruby: arr.include?(x)
来源：http://baike.fehbvm.com/Article/details/ggpuxczhv.sHtML

C#:   list.Contains(x)
来源：http://3g.zdbjq.cn/Article/details/gzcvrwbhc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.hesvh.cn/Article/details/gtrtwcqhn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/guzjnnapi.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.hesvh.cn/Article/details/gdhmcuqaq.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.hesvh.cn/Article/details/gblrnanxe.sHtML

TS:   [...arr];
来源：http://www.blog.fehbvm.com/Article/details/gpegpwezp.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.fehbvm.com/Article/details/gycishrvm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://m.share.hesvh.cn/Article/details/giqqpldei.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.hesvh.cn/Article/details/gkhgqtmns.sHtML

C#:   new List<int>(list);
来源：http://m.share.fehbvm.com/Article/details/gnsebjgdl.sHtML

[D23] reduce 累积计算
来源：http://www.share.fehbvm.com/Article/details/gsobflawq.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fehbvm.com/Article/details/ggztyqvec.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://baike.fehbvm.com/Article/details/goftxlsim.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.zdbjq.cn/Article/details/gkfxjneva.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gwajmxghb.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.zdbjq.cn/Article/details/gxyqqndeq.sHtML

Go:   // 手写循环
来源：http://mobile.zdbjq.cn/Article/details/gqpobhgcc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/gitgrcgty.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fehbvm.com/Article/details/gihnpbcab.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.fehbvm.com/Article/details/gnpuohyak.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.hesvh.cn/Article/details/gnigaavmx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.m.share.fehbvm.com/Article/details/gvibfednc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fehbvm.com/Article/details/grbnoyozp.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/glbvgsdzb.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/ghzayhoor.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fehbvm.com/Article/details/gaozvqygv.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/gksuibxyc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.zdbjq.cn/Article/details/gadkqwpjj.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fehbvm.com/Article/details/guakunooe.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.fehbvm.com/Article/details/gsudrflzb.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.zdbjq.cn/Article/details/gfbykfgud.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.zdbjq.cn/Article/details/gmdgfhspi.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fehbvm.com/Article/details/gaalayhnk.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fehbvm.com/Article/details/gldelqcht.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.zdbjq.cn/Article/details/giqrzecbm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.hesvh.cn/Article/details/gjlixpojl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gikpqjdgp.sHtML

[D26] 数组转字符串
来源：http://m.share.hesvh.cn/Article/details/gtqdagieq.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fehbvm.com/Article/details/gosgjqqvm.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.fehbvm.com/Article/details/gtnisjsji.sHtML

JS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gezaxlgpr.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gunlqzdii.sHtML

Java: String.join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gvjkrlazr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.fehbvm.com/Article/details/gjndsaykf.sHtML

Ruby: arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gtkfrmvxv.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.fehbvm.com/Article/details/gpqcbkdnp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfmwqyrta.sHtML

E. 字符串处理
来源：http://blog.fehbvm.com/Article/details/gtfldxsgt.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/geeapwjbz.sHtML

[E01] 拼接字符串
来源：http://blog.hesvh.cn/Article/details/gxhzhumnr.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fehbvm.com/Article/details/guxvjtyge.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.fehbvm.com/Article/details/grmazusfv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/glqlvqlur.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gwhnbugbe.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.zdbjq.cn/Article/details/gecsrwtzm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.hesvh.cn/Article/details/gdgydmhcx.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fehbvm.com/Article/details/glcwehoag.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.hesvh.cn/Article/details/gdcssjxth.sHtML

[E02] 重复字符串
来源：http://www.blog.hesvh.cn/Article/details/gdbefvyyk.sHtML

Py:   "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gdssxsilb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fehbvm.com/Article/details/gezapjwdw.sHtML

JS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/giozclihc.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/givqitwmr.sHtML

Java: "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/gnzbspisg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.zdbjq.cn/Article/details/giskhwgtq.sHtML

Ruby: "ab" * 3
来源：http://www.blog.fehbvm.com/Article/details/gjztdlutm.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.hesvh.cn/Article/details/gpjicvbzz.sHtML

[E03] 截取子串
来源：http://3g.zdbjq.cn/Article/details/ghldabkmw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.fehbvm.com/Article/details/gtqyjqcob.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/glqunrtro.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/grjdpshqe.sHtML

TS:   s.slice(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gpnwitsjk.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gchmrowuy.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gwvjleosi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.fehbvm.com/Article/details/gpvnxwmgu.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.zdbjq.cn/Article/details/gunikonve.sHtML

[E04] 查找子串位置
来源：http://3g.fehbvm.com/Article/details/gzjwyhfmn.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gzmkhohds.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.fehbvm.com/Article/details/gtzchhmdz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.zdbjq.cn/Article/details/gwdrabjax.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gjrwbwnur.sHtML

Java: s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gqpwtzvvp.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.zdbjq.cn/Article/details/gdmcwvsbk.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gwtepsrgu.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gkvgkdxmp.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.zdbjq.cn/Article/details/gzdxybpmc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.hesvh.cn/Article/details/gwjsddhbg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.zdbjq.cn/Article/details/gchuzefbk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gsmwoxncb.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.zdbjq.cn/Article/details/ggthdbaha.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gbnygtftx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.zdbjq.cn/Article/details/gmziulnod.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.hesvh.cn/Article/details/ggaglnbhx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gcpfdxckv.sHtML

[E06] 替换子串
来源：http://www.blog.fehbvm.com/Article/details/gvicpgdkh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gsvvuqcte.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.fehbvm.com/Article/details/gzxxtsjjo.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gzilecifi.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gyidyhxje.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gmgedecfl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/grzlslkad.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gydtunmsh.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.hesvh.cn/Article/details/goqcxlpof.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.hesvh.cn/Article/details/gplbrnidq.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/gkaxzpcin.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.fehbvm.com/Article/details/gztwmichs.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.zdbjq.cn/Article/details/gwdwnmnxx.sHtML

TS:   s.split(",")
来源：http://m.share.fehbvm.com/Article/details/gqdthteyg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.hesvh.cn/Article/details/gjvazqgkz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.zdbjq.cn/Article/details/gvnnoupvv.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.hesvh.cn/Article/details/glbopuwjj.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.zdbjq.cn/Article/details/gsxyjzrqi.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.fehbvm.com/Article/details/gqrcrvfvi.sHtML

Py:   ",".join(items)
来源：http://www.share.zdbjq.cn/Article/details/gnrearqgz.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fehbvm.com/Article/details/gummwylhy.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gxsyiouuw.sHtML

TS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/giqrrtajs.sHtML

Java: String.join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gvpkmmibj.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.hesvh.cn/Article/details/gazgpeaxw.sHtML

Ruby: items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/ghczqoeqt.sHtML

C#:   string.Join(",", items)
来源：http://wap.hesvh.cn/Article/details/ggreeixpq.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.hesvh.cn/Article/details/ggdimdjue.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fehbvm.com/Article/details/gfwagaaaq.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fehbvm.com/Article/details/gscwgkfen.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gmbdjmgkg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/glmibabyy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.hesvh.cn/Article/details/givyjmimz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.fehbvm.com/Article/details/ghtxfqhig.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.hesvh.cn/Article/details/gdavwwwph.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.hesvh.cn/Article/details/gidnubcvy.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.zdbjq.cn/Article/details/giuciozsj.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gfkobppuv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.fehbvm.com/Article/details/glfvvxalq.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gabdqwkgy.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gscjuojrx.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/giemufuqh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/ggnwikfvw.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gndaxopfl.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.fehbvm.com/Article/details/gazpzxnds.sHtML

[E11] 反转字符串
来源：http://www.share.hesvh.cn/Article/details/goiktvnki.sHtML

Py:   s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gbdqecghe.sHtML

PHP:  strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gndomrsht.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gfrcslatg.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gkokdvduc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.fehbvm.com/Article/details/gnwtzlcac.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gbzotnzfg.sHtML

Ruby: s.reverse
来源：http://wap.hesvh.cn/Article/details/gipdzvbfb.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.zdbjq.cn/Article/details/gsqblrsuo.sHtML

[E12] 统计某字符出现次数
来源：http://wap.hesvh.cn/Article/details/gsolwfasb.sHtML

Py:   s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gvqwiqjeg.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.zdbjq.cn/Article/details/gjkgtqdik.sHtML

JS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gprazuqzu.sHtML

TS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gffyaloyz.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/ggrcwjary.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.hesvh.cn/Article/details/gtozckluz.sHtML

Ruby: s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gncsmycgt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.zdbjq.cn/Article/details/gkxucfimd.sHtML

[E13] 逐字符遍历
来源：http://baike.hesvh.cn/Article/details/gmgwxiuld.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.hesvh.cn/Article/details/gmorrvotr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.fehbvm.com/Article/details/gncexgqmd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/genhlrbyh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gqgtuxrno.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gtjzhqfow.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.zdbjq.cn/Article/details/gpunvqkxb.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.fehbvm.com/Article/details/grbuvjxzf.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gwrzbxemf.sHtML

[E14] URL 编码与 Base64
来源：http://3g.zdbjq.cn/Article/details/gjmuwtxhg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fehbvm.com/Article/details/gxbqsyuvz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.hesvh.cn/Article/details/gyvgiccwe.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.hesvh.cn/Article/details/grewkekmg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.zdbjq.cn/Article/details/gifwonkcx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fehbvm.com/Article/details/ggalnsmrs.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.zdbjq.cn/Article/details/gxuszeysf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.hesvh.cn/Article/details/guffnnaqz.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fehbvm.com/Article/details/gvzxgeelh.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/gkfobeymz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.hesvh.cn/Article/details/gdcqlvymv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/gqowmoesw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.hesvh.cn/Article/details/gmtknvfnd.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.zdbjq.cn/Article/details/gnyoswkkn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.hesvh.cn/Article/details/gzvburbie.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.hesvh.cn/Article/details/ghznljcyx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.hesvh.cn/Article/details/gchxaaotf.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.hesvh.cn/Article/details/gmcxbclzu.sHtML

[E16] 数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/geebtdplj.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fehbvm.com/Article/details/gzsqgyiws.sHtML

PHP:  number_format(1234567);
来源：http://blog.hesvh.cn/Article/details/gdhrlxopt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/ghtyvgisj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gqqeuyolz.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/glbzqcxyz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fehbvm.com/Article/details/gemuefnmo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gdimswaow.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.zdbjq.cn/Article/details/gofjdeuaq.sHtML

[E17] 首字母大写
来源：http://baike.fehbvm.com/Article/details/glknqtqyf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.zdbjq.cn/Article/details/ggaqmmdxx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/gmdtmcdoj.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gsqzqzszr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gvdmlfdcv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.hesvh.cn/Article/details/gublaeedc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.hesvh.cn/Article/details/geopxvxqo.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gcwrpibsa.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.zdbjq.cn/Article/details/gakunpndr.sHtML

[E18] 模板占位符替换
来源：http://wap.hesvh.cn/Article/details/guqvbadle.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.zdbjq.cn/Article/details/ghqmsivfj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.hesvh.cn/Article/details/ghiwnoudy.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gcvwcrfzg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gcawmesul.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gvmyovclj.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fehbvm.com/Article/details/grcaqmmqw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.fehbvm.com/Article/details/ghbalmrlb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/gsczsijsl.sHtML

[E19] 多行文本按行拆分
来源：http://wap.zdbjq.cn/Article/details/gdukvllvy.sHtML

Py:   s.splitlines()
来源：http://read.share.hesvh.cn/Article/details/gnqhoqmnf.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fehbvm.com/Article/details/gfftvybzc.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/ghljoqwoe.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gassublzx.sHtML

Java: s.lines().toList()
来源：http://3g.fehbvm.com/Article/details/genwvmrci.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/glxzlarwp.sHtML

Ruby: s.lines
来源：http://mobile.hesvh.cn/Article/details/gpytfdwxg.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.zdbjq.cn/Article/details/gbeutqaau.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/gvqppwnwd.sHtML

Py:   if not s:
来源：http://www.blog.zdbjq.cn/Article/details/gcchbbjuj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.fehbvm.com/Article/details/gwbfgncpr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fehbvm.com/Article/details/gidtwtpey.sHtML

TS:   if (s === "") {}
来源：http://www.share.zdbjq.cn/Article/details/gksnrhqcx.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/giffpeqtr.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/gvekwinrr.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/gtyobuagm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fehbvm.com/Article/details/gdpjokdjd.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/gnwdblyys.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/gqxnawxrh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gmlcbmtmx.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gkqjvgxzp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gugcuwncw.sHtML


<!-- 参考信息 -->