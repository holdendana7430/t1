代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.zdbjq.cn/Article/details/gzpepttmm.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://baike.hesvh.cn/Article/details/gytyljtvq.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.m.share.fehbvm.com/Article/details/gfvoijwdl.sHtML

Go:   // 手写循环累加
来源：http://m.share.hesvh.cn/Article/details/gcjqqblxl.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://blog.zdbjq.cn/Article/details/gxcnakajt.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.zdbjq.cn/Article/details/gkbihpbkj.sHtML

[D17] 最大值与最小值
来源：http://www.share.zdbjq.cn/Article/details/gtmstlffb.sHtML

Py:   max(arr);  min(arr)
来源：http://m.share.zdbjq.cn/Article/details/gcyvfnine.sHtML

PHP:  max($arr);  min($arr);
来源：http://baike.fehbvm.com/Article/details/gvmtgcfxc.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.hesvh.cn/Article/details/glxsgejgz.sHtML

TS:   Math.max(...arr);
来源：http://3g.zdbjq.cn/Article/details/gwdzjzeoj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.fehbvm.com/Article/details/ggoldsxrx.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/grbbbzivf.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.zdbjq.cn/Article/details/grgdurjlt.sHtML

C#:   list.Max();  list.Min()
来源：http://www.blog.hesvh.cn/Article/details/gcjewhgmg.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.zdbjq.cn/Article/details/gntunrnal.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.fehbvm.com/Article/details/ghjvjtfkd.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/grsszpcso.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.zdbjq.cn/Article/details/gwczmjlhm.sHtML

TS:   nested.flat();
来源：http://www.m.share.zdbjq.cn/Article/details/gjnwdauao.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.share.fehbvm.com/Article/details/gojiakkau.sHtML

Go:   // 手写双层循环
来源：http://blog.hesvh.cn/Article/details/gqpqhttam.sHtML

Ruby: nested.flatten
来源：http://mobile.zdbjq.cn/Article/details/gxgarqrlf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fehbvm.com/Article/details/gjfikdsyq.sHtML

[D19] 按字段分组
来源：http://m.share.zdbjq.cn/Article/details/gusrheokq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.hesvh.cn/Article/details/ggertnokq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.zdbjq.cn/Article/details/gfkqskqrl.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/gyuewbevv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fehbvm.com/Article/details/gixxrbzxs.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.zdbjq.cn/Article/details/gnevofvfb.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.hesvh.cn/Article/details/gysvniult.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.fehbvm.com/Article/details/gnixpzyav.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.zdbjq.cn/Article/details/gporzgyat.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/gdhvwpmxz.sHtML

Py:   Counter(arr)
来源：http://wap.hesvh.cn/Article/details/gandqvtnk.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fehbvm.com/Article/details/gzyrgiafe.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.m.share.fehbvm.com/Article/details/gewafnbyr.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gdbmizyfk.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fehbvm.com/Article/details/gacundivv.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.hesvh.cn/Article/details/guykjshqg.sHtML

Ruby: arr.tally
来源：http://www.m.share.hesvh.cn/Article/details/gzwtqcvye.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.zdbjq.cn/Article/details/gpvwgxrlf.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fehbvm.com/Article/details/gkxjhwvam.sHtML

Py:   x in arr
来源：http://read.share.hesvh.cn/Article/details/gwshxrlra.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.zdbjq.cn/Article/details/gabaiqtup.sHtML

JS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gfkequtsa.sHtML

TS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/ghfythbgo.sHtML

Java: list.contains(x)
来源：http://read.share.hesvh.cn/Article/details/ggklqmzit.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gvllweink.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gpoajhvit.sHtML

C#:   list.Contains(x)
来源：http://mobile.hesvh.cn/Article/details/guuswnxmf.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/gjuyluonn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.hesvh.cn/Article/details/gzyxbsfcf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.fehbvm.com/Article/details/gzxbfaepj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.zdbjq.cn/Article/details/gryvpdsdb.sHtML

TS:   [...arr];
来源：http://read.share.zdbjq.cn/Article/details/gnaogigvy.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/gnoqdkpol.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gjxucdaxu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/giyyoswzi.sHtML

C#:   new List<int>(list);
来源：http://mobile.zdbjq.cn/Article/details/geznaryoa.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/ghwecpazw.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.hesvh.cn/Article/details/gasvvlydp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.hesvh.cn/Article/details/gtdwpbarx.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gqyacsbwa.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gijqkokun.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fehbvm.com/Article/details/gpfxwxgka.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gmgxdvwxx.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.hesvh.cn/Article/details/gvvdpvydc.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.hesvh.cn/Article/details/grajxooua.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fehbvm.com/Article/details/ggvzpdbzw.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.zdbjq.cn/Article/details/gnlxmoubb.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.fehbvm.com/Article/details/gfyjwbpqq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.zdbjq.cn/Article/details/gdcinwcwy.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.fehbvm.com/Article/details/gxtlnlelx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.zdbjq.cn/Article/details/guyphqgia.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.zdbjq.cn/Article/details/gvoyfpxrh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.hesvh.cn/Article/details/gfvesbgos.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.zdbjq.cn/Article/details/gdmglyjgc.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fehbvm.com/Article/details/gdzbseauc.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.hesvh.cn/Article/details/gvqdfefqn.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.zdbjq.cn/Article/details/gafalorym.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fehbvm.com/Article/details/gnwrjqfoc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fehbvm.com/Article/details/gyceobkms.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://blog.fehbvm.com/Article/details/gszhiztpy.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.hesvh.cn/Article/details/ghxjzweqz.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://3g.hesvh.cn/Article/details/grnanwgbs.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.hesvh.cn/Article/details/gpoppliih.sHtML

[D26] 数组转字符串
来源：http://read.share.hesvh.cn/Article/details/gijrrslaj.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.m.share.hesvh.cn/Article/details/gxljhmkly.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gciczjvac.sHtML

JS:   arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gjocttnuk.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gvmwcgily.sHtML

Java: String.join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/ggjrmuaca.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.hesvh.cn/Article/details/gnuheyjzt.sHtML

Ruby: arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/gmrsmykfe.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.hesvh.cn/Article/details/gsajjgxmm.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ghrhnsszm.sHtML

E. 字符串处理
来源：http://www.m.share.fehbvm.com/Article/details/gwufucwbq.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gsojsqjvn.sHtML

[E01] 拼接字符串
来源：http://baike.hesvh.cn/Article/details/gfarkjute.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://mobile.fehbvm.com/Article/details/grsnwmehg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.zdbjq.cn/Article/details/glldesjmx.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.hesvh.cn/Article/details/gootwrewt.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/guvxmvspq.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.zdbjq.cn/Article/details/gbesmqchr.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fehbvm.com/Article/details/gyyeafdzs.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.hesvh.cn/Article/details/geliayfpp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gzsxkhndp.sHtML

[E02] 重复字符串
来源：http://read.share.zdbjq.cn/Article/details/gnkplizrs.sHtML

Py:   "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gltzujnad.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.hesvh.cn/Article/details/gkrbybigb.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gsmluyems.sHtML

TS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/ghodoyjer.sHtML

Java: "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/grfrlpvcs.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.hesvh.cn/Article/details/gtatzsgcj.sHtML

Ruby: "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gkcjcncrk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.hesvh.cn/Article/details/gcobznfbu.sHtML

[E03] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gmuopxhab.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.hesvh.cn/Article/details/glfmwgele.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gadzvwqsx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gopwlihbo.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gtpzvzzgr.sHtML

Java: s.substring(1, 4)
来源：http://m.share.fehbvm.com/Article/details/gtrxtvfcw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/gvpmptydz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.zdbjq.cn/Article/details/gxpfedubd.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fehbvm.com/Article/details/gogrhdnus.sHtML

[E04] 查找子串位置
来源：http://3g.zdbjq.cn/Article/details/ggvonghsw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gtmoviddx.sHtML

PHP:  strpos($s, "x");
来源：http://baike.hesvh.cn/Article/details/grhtzanin.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.hesvh.cn/Article/details/gfftavwuj.sHtML

TS:   s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/grvbbjezb.sHtML

Java: s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gfgjdgkbo.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.hesvh.cn/Article/details/gzqubjiic.sHtML

Ruby: s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gmfcphpga.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gexcdqcep.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.hesvh.cn/Article/details/grbnlkmoo.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.zdbjq.cn/Article/details/gwezpzjew.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.zdbjq.cn/Article/details/gjvyqkoqb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gfwwqbbhu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.zdbjq.cn/Article/details/gpzovchbk.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gbmrnfohy.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.hesvh.cn/Article/details/gzdxaeoqq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.fehbvm.com/Article/details/ghbjtwppo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fehbvm.com/Article/details/gpzvoozyf.sHtML

[E06] 替换子串
来源：http://mobile.fehbvm.com/Article/details/gqyobdybh.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gsufhjoqs.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.zdbjq.cn/Article/details/gybljnhsm.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gjeuxvjkj.sHtML

TS:   s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gchmvvlyd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gorjjwywd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://3g.zdbjq.cn/Article/details/gduwkrjtl.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/goktelmgs.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gyjcvbove.sHtML

[E07] 按分隔符拆分
来源：http://wap.fehbvm.com/Article/details/gbgvaxyfv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.fehbvm.com/Article/details/gtemwhmgv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gtoauufzc.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/gartilcbj.sHtML

TS:   s.split(",")
来源：http://read.share.zdbjq.cn/Article/details/grtphrgut.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.zdbjq.cn/Article/details/gezkmewxc.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fehbvm.com/Article/details/ghtpwlyqn.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.zdbjq.cn/Article/details/gjivgfkbs.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fehbvm.com/Article/details/gaxswsyeb.sHtML

[E08] 数组按分隔符合并
来源：http://baike.hesvh.cn/Article/details/gdykraykt.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/ggeuyawoi.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.zdbjq.cn/Article/details/glckcbiwy.sHtML

JS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/guxsxncyh.sHtML

TS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gmufwizob.sHtML

Java: String.join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gtmdalwkv.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fehbvm.com/Article/details/gqlldksmb.sHtML

Ruby: items.join(",")
来源：http://3g.hesvh.cn/Article/details/gznlmolsv.sHtML

C#:   string.Join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gxffjvccz.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.zdbjq.cn/Article/details/gmyzdthlw.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.zdbjq.cn/Article/details/gzfrlgkvc.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.zdbjq.cn/Article/details/geyzhppue.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/ginliknfr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gbmluhbwy.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gkuiymozq.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.fehbvm.com/Article/details/giircnglp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.zdbjq.cn/Article/details/gsbruoqbd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gywnuszuv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.hesvh.cn/Article/details/gqudayxja.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gxluvimew.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.zdbjq.cn/Article/details/geptwargu.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gumjujszj.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gvaeyymrr.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/ghpuruptt.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gzkaoqkpp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gvvmzdqbx.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/gbupixelp.sHtML

[E11] 反转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gqbsuqxwo.sHtML

Py:   s[::-1]
来源：http://read.share.zdbjq.cn/Article/details/gopbanctx.sHtML

PHP:  strrev($s);
来源：http://3g.hesvh.cn/Article/details/gqakzsnhd.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.fehbvm.com/Article/details/gicpzupuk.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gvxbkmxlp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.zdbjq.cn/Article/details/geakuleaf.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.zdbjq.cn/Article/details/gpflihjhj.sHtML

Ruby: s.reverse
来源：http://wap.zdbjq.cn/Article/details/gzwkvdrnf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.hesvh.cn/Article/details/gzvyazlwf.sHtML

[E12] 统计某字符出现次数
来源：http://blog.fehbvm.com/Article/details/gmxpoodrg.sHtML

Py:   s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gmjkqwcxe.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.hesvh.cn/Article/details/gwcjfnfmg.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gmbisqzmf.sHtML

TS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/ggfmozelp.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.hesvh.cn/Article/details/gxwdyslkg.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.hesvh.cn/Article/details/gqvqfbbsb.sHtML

Ruby: s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gkzfvjvnc.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/guwesjbxe.sHtML

[E13] 逐字符遍历
来源：http://3g.zdbjq.cn/Article/details/gnehxdrfi.sHtML

Py:   for ch in s: print(ch)
来源：http://www.blog.hesvh.cn/Article/details/gpfaxvbjb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.hesvh.cn/Article/details/ghagakucp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/grlhvfvpc.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/geuvnyssw.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.fehbvm.com/Article/details/gbgyqmoqs.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fehbvm.com/Article/details/gmsmfwnqk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fehbvm.com/Article/details/gwjakfkat.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fehbvm.com/Article/details/glsnqnevn.sHtML

[E14] URL 编码与 Base64
来源：http://blog.fehbvm.com/Article/details/gdbwcuksq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fehbvm.com/Article/details/gfynjbhfj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.fehbvm.com/Article/details/gdrrlqlvf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.hesvh.cn/Article/details/ghluzhqqt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fehbvm.com/Article/details/giotuefzx.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.zdbjq.cn/Article/details/geshkhuoq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fehbvm.com/Article/details/gzibkciug.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/gfnxfzjfd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.hesvh.cn/Article/details/gkqlqjufr.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fehbvm.com/Article/details/gzjpnhshc.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/gtqvrnysm.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.fehbvm.com/Article/details/gtdhbpbjb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.hesvh.cn/Article/details/gbedkerae.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/gdiagxjpu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fehbvm.com/Article/details/gwghbccgh.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.hesvh.cn/Article/details/gawiwhwwq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.zdbjq.cn/Article/details/gulrkxpkg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.hesvh.cn/Article/details/gafrxdnmw.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gyeksdxbc.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.zdbjq.cn/Article/details/galjtytrn.sHtML

PHP:  number_format(1234567);
来源：http://blog.fehbvm.com/Article/details/gdenadkbs.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/ggdxmdrfs.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gavnximqy.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.fehbvm.com/Article/details/ghgomxutm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fehbvm.com/Article/details/gdugqisbv.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fehbvm.com/Article/details/gtqudoqsj.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fehbvm.com/Article/details/gkwfagfpx.sHtML

[E17] 首字母大写
来源：http://wap.fehbvm.com/Article/details/gctbbgtff.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.zdbjq.cn/Article/details/gfvplbwia.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.hesvh.cn/Article/details/ggvyyzbfe.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/genbagdsk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gksjvtpgm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.hesvh.cn/Article/details/gsvbsukfq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.hesvh.cn/Article/details/gqjbeevrn.sHtML

Ruby: s.capitalize
来源：http://www.blog.fehbvm.com/Article/details/ggpamurtf.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.zdbjq.cn/Article/details/ghgivbcqv.sHtML

[E18] 模板占位符替换
来源：http://wap.hesvh.cn/Article/details/gfvwuwovo.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.hesvh.cn/Article/details/gaqmcpoix.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.zdbjq.cn/Article/details/gxtmzhydk.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gqcqaztoa.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gjosjrxan.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gvjtavlea.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.zdbjq.cn/Article/details/gzalbdwoa.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.hesvh.cn/Article/details/gbixlaccu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.hesvh.cn/Article/details/gzbdcpttf.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.zdbjq.cn/Article/details/grtsjdwrm.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/garirnxyu.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.hesvh.cn/Article/details/gadywzypr.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gxgvyzhqd.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/gqsdjwgct.sHtML

Java: s.lines().toList()
来源：http://mobile.hesvh.cn/Article/details/gymnnkitp.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.hesvh.cn/Article/details/gilzteiki.sHtML

Ruby: s.lines
来源：http://wap.hesvh.cn/Article/details/gjmqxwkdx.sHtML

C#:   s.Split('\n')
来源：http://www.blog.hesvh.cn/Article/details/gfzqjkloy.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.hesvh.cn/Article/details/gvmomeisw.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gfnshywxa.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.hesvh.cn/Article/details/gctcherhx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fehbvm.com/Article/details/gzmbqaihs.sHtML

TS:   if (s === "") {}
来源：http://wap.zdbjq.cn/Article/details/goyyskpki.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gwfszcnwg.sHtML

Go:   if s == "" {}
来源：http://blog.zdbjq.cn/Article/details/gkdhrgwna.sHtML

Ruby: if s.empty?
来源：http://wap.fehbvm.com/Article/details/gwuxkyset.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.zdbjq.cn/Article/details/gtnusjrut.sHtML

[E21] 超长截断加省略号
来源：http://read.share.hesvh.cn/Article/details/gijsyzrnt.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fehbvm.com/Article/details/gswhekrtt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gvcizhnit.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gteggljhr.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gwefiekir.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gxbossclw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.zdbjq.cn/Article/details/gqaafoygw.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/getwgupjq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gkbezhqpl.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.hesvh.cn/Article/details/gooobjvsv.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.hesvh.cn/Article/details/gozsopkwr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.zdbjq.cn/Article/details/ghmtxqhsy.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/gqpewaort.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gznkgtjlf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fehbvm.com/Article/details/gmqnsarde.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.zdbjq.cn/Article/details/gjwwxyhwi.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/glpefkhxc.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.zdbjq.cn/Article/details/ggfonfqlw.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpjtbuded.sHtML

F. 文件与目录
来源：http://www.share.zdbjq.cn/Article/details/gcaoazfqh.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvcdexcpi.sHtML


<!-- 参考信息 -->