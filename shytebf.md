代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.hesvh.cn/Article/details/gxbtdsmjt.sHtML

Go:   // 手写双层循环
来源：http://blog.fehbvm.com/Article/details/gzpnvjmmx.sHtML

Ruby: nested.flatten
来源：http://m.share.fehbvm.com/Article/details/gpqqxfvlj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fehbvm.com/Article/details/gmkjdyist.sHtML

[D19] 按字段分组
来源：http://3g.zdbjq.cn/Article/details/gjskiyvdb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.zdbjq.cn/Article/details/gsrdkxmgg.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gxffmxtxk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.zdbjq.cn/Article/details/ghyepuuct.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gdtsphrbw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.fehbvm.com/Article/details/gejxufjnl.sHtML

Go:   // 手写 map[string][]T
来源：http://wap.fehbvm.com/Article/details/gczxclmvm.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.hesvh.cn/Article/details/gbawfxuyi.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.hesvh.cn/Article/details/gahouedvr.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.zdbjq.cn/Article/details/gybzwohfo.sHtML

Py:   Counter(arr)
来源：http://www.blog.fehbvm.com/Article/details/gfifjhicr.sHtML

PHP:  array_count_values($arr);
来源：http://blog.zdbjq.cn/Article/details/gpvfzfpfu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/govvukpwo.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.hesvh.cn/Article/details/gbmdmigwz.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.zdbjq.cn/Article/details/glywwvcvl.sHtML

Go:   // 手写 map[T]int
来源：http://wap.hesvh.cn/Article/details/gqjskwdcr.sHtML

Ruby: arr.tally
来源：http://www.share.zdbjq.cn/Article/details/gektwwazo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.fehbvm.com/Article/details/gsqhclyvw.sHtML

[D21] 判断是否包含某元素
来源：http://blog.fehbvm.com/Article/details/gosjqgwna.sHtML

Py:   x in arr
来源：http://www.share.hesvh.cn/Article/details/gavdkabkj.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/gewernvjf.sHtML

JS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gkjiwigbt.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/gikximnua.sHtML

Java: list.contains(x)
来源：http://m.share.fehbvm.com/Article/details/gvjpyranw.sHtML

Go:   slices.Contains(arr, x)
来源：http://blog.hesvh.cn/Article/details/gfozmkdjo.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/gqaklpofi.sHtML

C#:   list.Contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gmlvcfirk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.zdbjq.cn/Article/details/gtpvskehs.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.hesvh.cn/Article/details/gubfrcche.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.hesvh.cn/Article/details/gafnklnmf.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://read.share.fehbvm.com/Article/details/gxgjghvnb.sHtML

TS:   [...arr];
来源：http://m.share.fehbvm.com/Article/details/gvhhdyozb.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fehbvm.com/Article/details/gysbvbsuz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gksxljjbc.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.share.hesvh.cn/Article/details/gzbzjfmvr.sHtML

C#:   new List<int>(list);
来源：http://m.share.fehbvm.com/Article/details/grxgzzxud.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.hesvh.cn/Article/details/gsokvsctc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/gwydeovjw.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fehbvm.com/Article/details/gotucqrez.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gxaczvzyu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gvapctbhm.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/gglqfcmsc.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gqzjljema.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.zdbjq.cn/Article/details/ghwuauxpf.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.hesvh.cn/Article/details/gvcgskzta.sHtML

[D24] 字典 / Map 基本操作
来源：http://baike.hesvh.cn/Article/details/gmvxrtgfp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gprwxmpmp.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/gtkdkisxl.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.hesvh.cn/Article/details/ghclgdnve.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.fehbvm.com/Article/details/ggsglmchl.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/ggvxwkako.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.zdbjq.cn/Article/details/gybrudifj.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.fehbvm.com/Article/details/grzpdlhgc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.hesvh.cn/Article/details/ggqyiodyg.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.hesvh.cn/Article/details/gcrgcmtcr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.zdbjq.cn/Article/details/gmtssjoyi.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.fehbvm.com/Article/details/ggefmjxbv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.zdbjq.cn/Article/details/gsbuqwiok.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.zdbjq.cn/Article/details/gcghmudin.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.share.hesvh.cn/Article/details/ghxlnvzsd.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.hesvh.cn/Article/details/gkzbjiuuz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://blog.zdbjq.cn/Article/details/gsnuhkous.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fehbvm.com/Article/details/gdtgdiogj.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/gdvpgmjzs.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.zdbjq.cn/Article/details/gwgpdyeym.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.hesvh.cn/Article/details/gnfpvzoaz.sHtML

JS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gmhntrmcw.sHtML

TS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gqxzjmenn.sHtML

Java: String.join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/ghntysome.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.hesvh.cn/Article/details/gvvlldgld.sHtML

Ruby: arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gxrmdsznh.sHtML

C#:   string.Join(", ", list)
来源：http://blog.hesvh.cn/Article/details/gryxeenku.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghvekvfie.sHtML

E. 字符串处理
来源：http://www.share.zdbjq.cn/Article/details/gyxeayjrk.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gsochyuze.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gullmgtdp.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.hesvh.cn/Article/details/gtnhdhjcj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.fehbvm.com/Article/details/glywsbybk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.hesvh.cn/Article/details/grvsvfwbk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gpzquqtvd.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.zdbjq.cn/Article/details/grqqagzvx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.hesvh.cn/Article/details/gobahilgp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.zdbjq.cn/Article/details/gnybsyqzx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gwymlpuar.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/gnrqsimdq.sHtML

Py:   "ab" * 3
来源：http://blog.zdbjq.cn/Article/details/gsfccubni.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fehbvm.com/Article/details/ghdvvfsiu.sHtML

JS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gcfgapjtj.sHtML

TS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gdvrdobep.sHtML

Java: "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gcdgqxxux.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.zdbjq.cn/Article/details/gllzmfuri.sHtML

Ruby: "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gzsofkhvh.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fehbvm.com/Article/details/gapwjbosl.sHtML

[E03] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gewlpmdfr.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fehbvm.com/Article/details/gsacfumzs.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gvgwskhlm.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gkeiwlrvr.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/ggtxbpgna.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gibidlpzw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.hesvh.cn/Article/details/ghuqpyaqa.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.zdbjq.cn/Article/details/gnrmumyro.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.hesvh.cn/Article/details/giiiatcqs.sHtML

[E04] 查找子串位置
来源：http://wap.fehbvm.com/Article/details/gnrocgogg.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/ggwocmjjl.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.zdbjq.cn/Article/details/ggflmlhmd.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.zdbjq.cn/Article/details/gqtwjcvsc.sHtML

TS:   s.indexOf("x")
来源：http://m.share.hesvh.cn/Article/details/gwhqmqubk.sHtML

Java: s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gkdhllqtv.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.fehbvm.com/Article/details/gecuxaxju.sHtML

Ruby: s.index("x")
来源：http://www.blog.zdbjq.cn/Article/details/gbcvsxpnf.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fehbvm.com/Article/details/guhlbcwwf.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.hesvh.cn/Article/details/gmpyxjmcg.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.zdbjq.cn/Article/details/gladbuknm.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.m.share.zdbjq.cn/Article/details/gldlgeeyh.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/garkgrjer.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.hesvh.cn/Article/details/grqjspipg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gvtrwzmra.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.hesvh.cn/Article/details/ggnjrxlhz.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.hesvh.cn/Article/details/genfpxpar.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gmvznqyoo.sHtML

[E06] 替换子串
来源：http://www.blog.zdbjq.cn/Article/details/gqjpzpatn.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gxkvoutvu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.zdbjq.cn/Article/details/gtbwcdkgs.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gmdzzzxpg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.zdbjq.cn/Article/details/gdboyndmq.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gwhmxwztw.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.hesvh.cn/Article/details/gflrqmvsq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fehbvm.com/Article/details/gxqkmtapv.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.hesvh.cn/Article/details/gzbymwghg.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gastqlmmx.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fehbvm.com/Article/details/gaksalhtl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gbgqdgmcr.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.hesvh.cn/Article/details/gogyuxguq.sHtML

TS:   s.split(",")
来源：http://wap.fehbvm.com/Article/details/gqhqfrqpd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://mobile.hesvh.cn/Article/details/gsypfljrw.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.zdbjq.cn/Article/details/gmylcwrwp.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.fehbvm.com/Article/details/gmcjanxra.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fehbvm.com/Article/details/gvkevcwgd.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.zdbjq.cn/Article/details/galbgdpmn.sHtML

Py:   ",".join(items)
来源：http://m.share.zdbjq.cn/Article/details/ggsfdhzms.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.hesvh.cn/Article/details/gbelkmezj.sHtML

JS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gritfmxlr.sHtML

TS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gnutcbqei.sHtML

Java: String.join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gglxfcybx.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.zdbjq.cn/Article/details/gcccbgmek.sHtML

Ruby: items.join(",")
来源：http://wap.fehbvm.com/Article/details/grwvwmvoj.sHtML

C#:   string.Join(",", items)
来源：http://wap.zdbjq.cn/Article/details/grpfroedg.sHtML

[E09] 去除所有空白字符
来源：http://baike.zdbjq.cn/Article/details/ghbcjzeux.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fehbvm.com/Article/details/gxjifybzx.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fehbvm.com/Article/details/gzivmcsia.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gxhurducq.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gsgirvttz.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.hesvh.cn/Article/details/gdccmvkdk.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fehbvm.com/Article/details/gshthzudo.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.zdbjq.cn/Article/details/gvpiferzi.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.hesvh.cn/Article/details/ggftdcdkl.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/gewybiymp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fehbvm.com/Article/details/gmkdztqwh.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.hesvh.cn/Article/details/grwsluibv.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gkccuzcxz.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gsjbrdmuz.sHtML

Java: String.format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gnuetaawb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/grdtyugck.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gghtklsdf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.hesvh.cn/Article/details/gkbjxacbi.sHtML

[E11] 反转字符串
来源：http://www.m.share.fehbvm.com/Article/details/grpvdkdxk.sHtML

Py:   s[::-1]
来源：http://mobile.zdbjq.cn/Article/details/grxztohsw.sHtML

PHP:  strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gkexxitzz.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gfpqpmwgq.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/gtuuvklla.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/gggkfgvkz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fehbvm.com/Article/details/gjimmcyil.sHtML

Ruby: s.reverse
来源：http://www.share.hesvh.cn/Article/details/gzcqisngg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.fehbvm.com/Article/details/gtywdchsr.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.zdbjq.cn/Article/details/gkbdyymtm.sHtML

Py:   s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gogicjrqg.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fehbvm.com/Article/details/gsgoixmci.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gicnnygub.sHtML

TS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gxzbrerdf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.zdbjq.cn/Article/details/gbgxtiodp.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.zdbjq.cn/Article/details/ghzwmqpcc.sHtML

Ruby: s.count("a")
来源：http://wap.hesvh.cn/Article/details/gduppgiph.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.fehbvm.com/Article/details/gxukskfhd.sHtML

[E13] 逐字符遍历
来源：http://wap.fehbvm.com/Article/details/gepuorzhx.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/geuzbaqxv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.hesvh.cn/Article/details/gxnmldnai.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.hesvh.cn/Article/details/gdrddohhw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/givbdfkar.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gqwjojxmj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.hesvh.cn/Article/details/gphkvexbl.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.hesvh.cn/Article/details/grmuodrby.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.zdbjq.cn/Article/details/gkvyprkaq.sHtML

[E14] URL 编码与 Base64
来源：http://3g.fehbvm.com/Article/details/gnwnyuunc.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.zdbjq.cn/Article/details/gebbyvemk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.hesvh.cn/Article/details/gdeuhhbrt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://baike.fehbvm.com/Article/details/gfeaeqcjv.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.zdbjq.cn/Article/details/guslodnwx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gmwolacqf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.fehbvm.com/Article/details/gveyvzuar.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.zdbjq.cn/Article/details/ghwzuddpl.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/gctwejcbn.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.fehbvm.com/Article/details/gnaekelua.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.hesvh.cn/Article/details/gtkhbqmwh.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.hesvh.cn/Article/details/gsmxbjras.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.zdbjq.cn/Article/details/gzqinpvww.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fehbvm.com/Article/details/gtasgaoip.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.hesvh.cn/Article/details/ggsjpwdkw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.zdbjq.cn/Article/details/gosognfaj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.zdbjq.cn/Article/details/gyasyhkqw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.fehbvm.com/Article/details/gjxoxtnix.sHtML

[E16] 数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gdffskkai.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fehbvm.com/Article/details/gaafbutnp.sHtML

PHP:  number_format(1234567);
来源：http://read.share.zdbjq.cn/Article/details/gcsovbprx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gxzglaqnq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/givexvslw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gprwenhdn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.zdbjq.cn/Article/details/gpkcihxgg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.fehbvm.com/Article/details/gwvutkvek.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.hesvh.cn/Article/details/gfxtasnme.sHtML

[E17] 首字母大写
来源：http://www.blog.zdbjq.cn/Article/details/gleifyycz.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.hesvh.cn/Article/details/glwdnsjpg.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fehbvm.com/Article/details/ggoaybnle.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gfirbvlif.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gxtonxmjf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.zdbjq.cn/Article/details/gcrnxvlxg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.fehbvm.com/Article/details/ghlfaovpn.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gupgykqxs.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fehbvm.com/Article/details/gyigktwii.sHtML

[E18] 模板占位符替换
来源：http://www.blog.hesvh.cn/Article/details/gekatkgce.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.hesvh.cn/Article/details/gssuwerpc.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fehbvm.com/Article/details/gqhbiqhww.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gjpxlhumx.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gpexbnzht.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/goydqhqxd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gvgaanyiy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.hesvh.cn/Article/details/gdrrkivlt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.zdbjq.cn/Article/details/gtnyakiej.sHtML

[E19] 多行文本按行拆分
来源：http://3g.hesvh.cn/Article/details/gwsgetnmy.sHtML

Py:   s.splitlines()
来源：http://baike.hesvh.cn/Article/details/glcbwnhie.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.hesvh.cn/Article/details/gqfhzucve.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gnsvlohxv.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gtqazirze.sHtML

Java: s.lines().toList()
来源：http://read.share.zdbjq.cn/Article/details/grionktcv.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.hesvh.cn/Article/details/glfgyyfvx.sHtML

Ruby: s.lines
来源：http://mobile.hesvh.cn/Article/details/gwqxxeuqr.sHtML

C#:   s.Split('\n')
来源：http://3g.hesvh.cn/Article/details/gngvawsqj.sHtML

[E20] 判断字符串是否为空
来源：http://mobile.fehbvm.com/Article/details/gexneqffl.sHtML

Py:   if not s:
来源：http://read.share.hesvh.cn/Article/details/gubtfqfpu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.zdbjq.cn/Article/details/goykgdgor.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.hesvh.cn/Article/details/gakxodify.sHtML

TS:   if (s === "") {}
来源：http://m.share.fehbvm.com/Article/details/gitytlryg.sHtML

Java: if (s.isEmpty()) {}
来源：http://baike.zdbjq.cn/Article/details/gzdjboydi.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/gxakhdteb.sHtML

Ruby: if s.empty?
来源：http://wap.hesvh.cn/Article/details/gyvngtvqt.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.fehbvm.com/Article/details/grjkabsce.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.hesvh.cn/Article/details/gycfxdkoq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.fehbvm.com/Article/details/gwbphugnm.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gjqrydkit.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gqehrrqus.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gkgcrlugz.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gyrgydlda.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fehbvm.com/Article/details/guwjpzmtj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gesepedpy.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gwnksyzqv.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fehbvm.com/Article/details/gwimjhpcn.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fehbvm.com/Article/details/gulzwfldb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/greefdamf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gilwbpfgt.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fehbvm.com/Article/details/gkkqddqdw.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fehbvm.com/Article/details/gjabfgdir.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.zdbjq.cn/Article/details/gzxzihwrp.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.hesvh.cn/Article/details/gwkhwqfmt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/gdbxcysnc.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gqpyhdljq.sHtML

F. 文件与目录
来源：http://3g.fehbvm.com/Article/details/gzbutjtlh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/grkqegzyq.sHtML

[F01] 读取整个文件
来源：http://blog.fehbvm.com/Article/details/gxcubbehv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.hesvh.cn/Article/details/gawafldzv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gqsoepjbh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/gqvapwpha.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.hesvh.cn/Article/details/gzafkenir.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/grblhxrpt.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fehbvm.com/Article/details/gwiyhdlnp.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gulygergb.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/guglgecrm.sHtML

[F02] 逐行读取文件
来源：http://www.share.hesvh.cn/Article/details/gwayggtro.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.zdbjq.cn/Article/details/gwkvdghdh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.hesvh.cn/Article/details/geihlizwk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/grcgtvwua.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.fehbvm.com/Article/details/gxmjzxxmo.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gbufzqzze.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.zdbjq.cn/Article/details/gkjgytwbo.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/gidwebvqv.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://3g.zdbjq.cn/Article/details/gxirqvebg.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.zdbjq.cn/Article/details/gkhiqlryg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.zdbjq.cn/Article/details/ghptlzxfm.sHtML


<!-- 参考信息 -->