代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://m.share.fehbvm.com/Article/details/gidahfdxk.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/gpozuvtqm.sHtML

Ruby: arr.map { |x| x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gbiqlgzef.sHtML

C#:   list.Select(x => x * 2).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gxbzbyfkt.sHtML

[D15] 去重
来源：http://m.share.hesvh.cn/Article/details/gtkagbytg.sHtML

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.share.hesvh.cn/Article/details/gldebhfhe.sHtML

PHP:  array_unique($arr);
来源：http://m.share.zdbjq.cn/Article/details/guiojqdno.sHtML

JS:   [...new Set(arr)]
来源：http://read.share.zdbjq.cn/Article/details/grkpacfnw.sHtML

TS:   [...new Set(arr)]
来源：http://3g.zdbjq.cn/Article/details/ggxqpsnkn.sHtML

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://mobile.zdbjq.cn/Article/details/gutzeytas.sHtML

Go:   // 用 map[T]struct{} 手写
来源：http://baike.hesvh.cn/Article/details/gfhhwdzfy.sHtML

Ruby: arr.uniq
来源：http://www.share.hesvh.cn/Article/details/gnzaqmhzu.sHtML

C#:   list.Distinct().ToList()
来源：http://m.share.zdbjq.cn/Article/details/ggavkwgwp.sHtML

[D16] 求和与平均值
来源：http://www.m.share.zdbjq.cn/Article/details/gtzwnizae.sHtML

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gxeuykxix.sHtML

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://wap.hesvh.cn/Article/details/gzevntvlo.sHtML

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.share.hesvh.cn/Article/details/gzxkuuzyk.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://m.share.hesvh.cn/Article/details/ggpmmqnmc.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://mobile.hesvh.cn/Article/details/gomprrqih.sHtML

Go:   // 手写循环累加
来源：http://www.blog.zdbjq.cn/Article/details/grwnudpcg.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.fehbvm.com/Article/details/gdxllteco.sHtML

C#:   list.Sum();  list.Average()
来源：http://3g.zdbjq.cn/Article/details/ghlrklnvs.sHtML

[D17] 最大值与最小值
来源：http://mobile.hesvh.cn/Article/details/gcyvmehhh.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fehbvm.com/Article/details/gdudnbplt.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/guuterwqe.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://3g.zdbjq.cn/Article/details/gplxvuqyx.sHtML

TS:   Math.max(...arr);
来源：http://www.blog.hesvh.cn/Article/details/gcxdzqmfu.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://m.share.zdbjq.cn/Article/details/grqdsiiau.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.hesvh.cn/Article/details/gtkijigrs.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.zdbjq.cn/Article/details/gosokwhhl.sHtML

C#:   list.Max();  list.Min()
来源：http://www.share.hesvh.cn/Article/details/gkirypdvl.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/ginkeuhlf.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.zdbjq.cn/Article/details/gafaxworw.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.zdbjq.cn/Article/details/gvedpqxzp.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.fehbvm.com/Article/details/gqsaxiipe.sHtML

TS:   nested.flat();
来源：http://baike.hesvh.cn/Article/details/gnrdtglne.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://mobile.zdbjq.cn/Article/details/givbzkfcb.sHtML

Go:   // 手写双层循环
来源：http://www.share.zdbjq.cn/Article/details/gtujuilhr.sHtML

Ruby: nested.flatten
来源：http://read.share.fehbvm.com/Article/details/gwdpgqvbo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.hesvh.cn/Article/details/gaaxpqebl.sHtML

[D19] 按字段分组
来源：http://wap.fehbvm.com/Article/details/gbizfwvwp.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.hesvh.cn/Article/details/gfvkipbeh.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://baike.fehbvm.com/Article/details/gakdfrrgp.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.zdbjq.cn/Article/details/gsswqgelv.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.hesvh.cn/Article/details/gdwhuyrzz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gqczwylhk.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fehbvm.com/Article/details/gobxbfctt.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.hesvh.cn/Article/details/gtnggydzu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.zdbjq.cn/Article/details/gdqjahmqa.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.hesvh.cn/Article/details/gtaclvrzl.sHtML

Py:   Counter(arr)
来源：http://mobile.hesvh.cn/Article/details/gpuutlpse.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fehbvm.com/Article/details/guuunnpde.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gbelreyxn.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.zdbjq.cn/Article/details/gzntpzgbb.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.fehbvm.com/Article/details/gcsvtiooo.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.hesvh.cn/Article/details/givkqstfl.sHtML

Ruby: arr.tally
来源：http://www.share.hesvh.cn/Article/details/gpvomxvlo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.hesvh.cn/Article/details/gjqcximyq.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.hesvh.cn/Article/details/gxbqpzbhq.sHtML

Py:   x in arr
来源：http://m.share.fehbvm.com/Article/details/gasepurkh.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/gejsyibbh.sHtML

JS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gvzdujnlf.sHtML

TS:   arr.includes(x)
来源：http://3g.zdbjq.cn/Article/details/gxsmnhoin.sHtML

Java: list.contains(x)
来源：http://wap.hesvh.cn/Article/details/gamyakjkd.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.fehbvm.com/Article/details/gjwmkltqu.sHtML

Ruby: arr.include?(x)
来源：http://blog.zdbjq.cn/Article/details/gdcplzmgg.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/ghcetbblc.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.fehbvm.com/Article/details/gcsgouyve.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.fehbvm.com/Article/details/gybmrceli.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/gfzcnzdew.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.hesvh.cn/Article/details/gosppwdnn.sHtML

TS:   [...arr];
来源：http://www.share.fehbvm.com/Article/details/gjgunmywj.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.zdbjq.cn/Article/details/gdyzghjey.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.zdbjq.cn/Article/details/gvktfyywu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://read.share.hesvh.cn/Article/details/gusycoqxx.sHtML

C#:   new List<int>(list);
来源：http://m.share.zdbjq.cn/Article/details/gqtekhocw.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fehbvm.com/Article/details/givejiwpb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.share.zdbjq.cn/Article/details/glgajhnsf.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/gryddxfzh.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gbeierbdm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.fehbvm.com/Article/details/gpbvjntwl.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.hesvh.cn/Article/details/grvkvgnaw.sHtML

Go:   // 手写循环
来源：http://3g.fehbvm.com/Article/details/gdecgolqc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.fehbvm.com/Article/details/gtiebqtxm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://3g.fehbvm.com/Article/details/gkwycvhhe.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.hesvh.cn/Article/details/glihmuwff.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.fehbvm.com/Article/details/gxmmhoooz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fehbvm.com/Article/details/gaztlzxak.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fehbvm.com/Article/details/gsisjgjfm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/geyyertyy.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/gnuenygia.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.hesvh.cn/Article/details/gdmhzrpiq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.hesvh.cn/Article/details/ghqlqcduv.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.zdbjq.cn/Article/details/gdrgwymva.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.hesvh.cn/Article/details/ghrawcoqy.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fehbvm.com/Article/details/ggjabzjid.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fehbvm.com/Article/details/gvtiofwiy.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.fehbvm.com/Article/details/gghgxgyhc.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fehbvm.com/Article/details/gymnoluub.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gesyxjfwn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/gppiqnzud.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.hesvh.cn/Article/details/grolqytdf.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gmerokidv.sHtML

[D26] 数组转字符串
来源：http://baike.fehbvm.com/Article/details/gztmdohpk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://blog.fehbvm.com/Article/details/gplekhcli.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gaesqmcux.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gmdvuytkr.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gzsnxgyns.sHtML

Java: String.join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gbstjszkj.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/ggiogsaqr.sHtML

Ruby: arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gkyflsvtk.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/glysjeqlg.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gmcodziqj.sHtML

E. 字符串处理
来源：http://read.share.zdbjq.cn/Article/details/gaztyslvq.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gycgaiqxq.sHtML

[E01] 拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gaqlbymtg.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fehbvm.com/Article/details/gyldtcdmb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/gcezxzhmp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/ggbgvirnj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gvvysgrqy.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.hesvh.cn/Article/details/gwfwqdneh.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.hesvh.cn/Article/details/gsolrgkde.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.zdbjq.cn/Article/details/gxhawyttn.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gmtjsibvv.sHtML

[E02] 重复字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gyqpgqhnx.sHtML

Py:   "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gvhiyzwey.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.hesvh.cn/Article/details/gbgsffduc.sHtML

JS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gsoptgnwl.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gnigmnhne.sHtML

Java: "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gwkgxjdka.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.fehbvm.com/Article/details/geeojiztw.sHtML

Ruby: "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gvxgxqfaa.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.hesvh.cn/Article/details/gfqmoegmk.sHtML

[E03] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gicdaquzw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.zdbjq.cn/Article/details/ggmwjyrbb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gmgiqivlr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gbozlbnmy.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gjfrymkpn.sHtML

Java: s.substring(1, 4)
来源：http://wap.hesvh.cn/Article/details/gkcccfvdg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://baike.hesvh.cn/Article/details/gmjrsufhh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/goyzahpla.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/guhlwpegs.sHtML

[E04] 查找子串位置
来源：http://3g.hesvh.cn/Article/details/gvfwysmai.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.fehbvm.com/Article/details/gyfgzdbwj.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fehbvm.com/Article/details/gtkexpxxi.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.fehbvm.com/Article/details/gejhelrja.sHtML

TS:   s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gjhfygrxl.sHtML

Java: s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gzefwlben.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.fehbvm.com/Article/details/gbjyrmsjh.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gkyhakxhx.sHtML

C#:   s.IndexOf("x")
来源：http://3g.hesvh.cn/Article/details/gxmcthxgi.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.fehbvm.com/Article/details/gdutqbpbf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.zdbjq.cn/Article/details/gtwmyhfet.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.fehbvm.com/Article/details/gfxobmiye.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gbedamjsy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.zdbjq.cn/Article/details/ghlmjlqks.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gtudomvar.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.hesvh.cn/Article/details/gkaxhsemf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.hesvh.cn/Article/details/gihenjlgf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fehbvm.com/Article/details/gmbvxupns.sHtML

[E06] 替换子串
来源：http://3g.fehbvm.com/Article/details/gyshwxkev.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://mobile.fehbvm.com/Article/details/gbjvitpet.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://blog.zdbjq.cn/Article/details/giucfdins.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gewxvctrl.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gdjwvsmig.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gcszljuaq.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.hesvh.cn/Article/details/gmoppeqdg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gxajenhbn.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.hesvh.cn/Article/details/gswogmute.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.zdbjq.cn/Article/details/gdgxrybnm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.hesvh.cn/Article/details/grmbjrkte.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.hesvh.cn/Article/details/gauzyvyix.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.zdbjq.cn/Article/details/gdkwlzuft.sHtML

TS:   s.split(",")
来源：http://www.m.share.hesvh.cn/Article/details/gfobmjpmp.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.fehbvm.com/Article/details/grrzpvmaf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fehbvm.com/Article/details/gfdylbkia.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.fehbvm.com/Article/details/gxxbhvjxm.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.zdbjq.cn/Article/details/gzrklqcfp.sHtML

[E08] 数组按分隔符合并
来源：http://blog.hesvh.cn/Article/details/galnzhrrl.sHtML

Py:   ",".join(items)
来源：http://3g.zdbjq.cn/Article/details/gaplncxjn.sHtML

PHP:  implode(",", $items);
来源：http://3g.zdbjq.cn/Article/details/gddbxuutl.sHtML

JS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gbyeudcek.sHtML

TS:   items.join(",")
来源：http://3g.zdbjq.cn/Article/details/gzuftdqvj.sHtML

Java: String.join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gwcaawbwc.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fehbvm.com/Article/details/gblrvzhbp.sHtML

Ruby: items.join(",")
来源：http://3g.fehbvm.com/Article/details/gwspovozy.sHtML

C#:   string.Join(",", items)
来源：http://baike.fehbvm.com/Article/details/gdtwknwma.sHtML

[E09] 去除所有空白字符
来源：http://blog.zdbjq.cn/Article/details/gpxixzxgg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.zdbjq.cn/Article/details/gfzxcwphr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.hesvh.cn/Article/details/gileyxpyc.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/gdqhfmmen.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gsbdevcnk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gjmcdbkee.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fehbvm.com/Article/details/gaesdrakp.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.zdbjq.cn/Article/details/gwsyulamk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.hesvh.cn/Article/details/gattlssvc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.fehbvm.com/Article/details/gwciuuqnd.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gzwbqexvg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://wap.hesvh.cn/Article/details/gwpoqoebh.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gehuzwoxf.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gmusnbpxv.sHtML

Java: String.format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gyobthsuq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gdinuvkej.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gdndwwate.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.zdbjq.cn/Article/details/ggpwflvkl.sHtML

[E11] 反转字符串
来源：http://blog.hesvh.cn/Article/details/gurrkovxz.sHtML

Py:   s[::-1]
来源：http://baike.fehbvm.com/Article/details/gatbeocwn.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/gkztioyjm.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gqzpyecbe.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gdmangwhq.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.zdbjq.cn/Article/details/gowuqpocu.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gqekqkxzv.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gixsognvz.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gzmuyoukt.sHtML

[E12] 统计某字符出现次数
来源：http://3g.hesvh.cn/Article/details/ggiwjpmtq.sHtML

Py:   s.count("a")
来源：http://wap.zdbjq.cn/Article/details/ggnvqsuaw.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.hesvh.cn/Article/details/gexiutkne.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gqvxkjvcl.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/ggtpkdsvf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.zdbjq.cn/Article/details/grnluvfdg.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fehbvm.com/Article/details/ggupayvyq.sHtML

Ruby: s.count("a")
来源：http://3g.hesvh.cn/Article/details/gplxzsdry.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.zdbjq.cn/Article/details/ggnrcxetq.sHtML

[E13] 逐字符遍历
来源：http://baike.hesvh.cn/Article/details/gfdzaftwy.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.fehbvm.com/Article/details/gqibumgqn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.fehbvm.com/Article/details/gvcyunjle.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fehbvm.com/Article/details/gsteabqbx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gpbuycmsl.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fehbvm.com/Article/details/gsydilgfx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.hesvh.cn/Article/details/gtbupztyh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fehbvm.com/Article/details/geyoxvtmx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/gaoyypnsx.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.hesvh.cn/Article/details/gbyzzyphs.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.hesvh.cn/Article/details/gdfpooedk.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.share.fehbvm.com/Article/details/gagqmdiui.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.fehbvm.com/Article/details/gmgqocztg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fehbvm.com/Article/details/gocqtuyjv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.hesvh.cn/Article/details/gntfxisht.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.zdbjq.cn/Article/details/gbdchsjuo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fehbvm.com/Article/details/gftwvytoh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fehbvm.com/Article/details/gzxxqkazb.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.hesvh.cn/Article/details/gsyszhtvw.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fehbvm.com/Article/details/gqfipfxis.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.zdbjq.cn/Article/details/gvmbydrzo.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.hesvh.cn/Article/details/gnlonqygw.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.fehbvm.com/Article/details/gkophcksk.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.hesvh.cn/Article/details/gkcewiiai.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.fehbvm.com/Article/details/ghbnmxwxg.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.zdbjq.cn/Article/details/ggjkdaqsh.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.fehbvm.com/Article/details/gwhzbsces.sHtML

[E16] 数字千分位
来源：http://3g.zdbjq.cn/Article/details/gsmzcjvry.sHtML

Py:   f"{1234567:,}"
来源：http://baike.hesvh.cn/Article/details/gxuccahoe.sHtML

PHP:  number_format(1234567);
来源：http://www.share.hesvh.cn/Article/details/gutyufpsw.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gifxhaikr.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/ginerrwbj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.fehbvm.com/Article/details/gecroicjk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.hesvh.cn/Article/details/gdutznkai.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.zdbjq.cn/Article/details/gcwlmujeo.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/gfsbprvsc.sHtML

[E17] 首字母大写
来源：http://www.blog.hesvh.cn/Article/details/gwdqxqovd.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fehbvm.com/Article/details/gkjlrxuup.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.zdbjq.cn/Article/details/gwxzeczcf.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/guirhblnb.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/girejqstf.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/gfmesmyvb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.hesvh.cn/Article/details/gysakktdz.sHtML

Ruby: s.capitalize
来源：http://blog.zdbjq.cn/Article/details/gubvpqfur.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.zdbjq.cn/Article/details/gxrlwqyif.sHtML

[E18] 模板占位符替换
来源：http://baike.zdbjq.cn/Article/details/gvdpfkwcb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.zdbjq.cn/Article/details/gqghcuzpg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/gcoxaison.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/ghmzztosw.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gpikxiany.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gxpfaewui.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gkzkvgjxi.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.hesvh.cn/Article/details/gbhojvmhp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/gylykoefj.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fehbvm.com/Article/details/gyhbnyqzm.sHtML

Py:   s.splitlines()
来源：http://baike.zdbjq.cn/Article/details/gllqdjpcn.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fehbvm.com/Article/details/gwkkwfwjr.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gsnrlqtvz.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/ghadjqbkz.sHtML

Java: s.lines().toList()
来源：http://baike.zdbjq.cn/Article/details/gxqnewzmy.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.hesvh.cn/Article/details/gfsgrkoyw.sHtML

Ruby: s.lines
来源：http://mobile.fehbvm.com/Article/details/grefddulx.sHtML

C#:   s.Split('\n')
来源：http://read.share.fehbvm.com/Article/details/glnjwegyi.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.hesvh.cn/Article/details/gbrdjtzfw.sHtML

Py:   if not s:
来源：http://read.share.fehbvm.com/Article/details/ggebpwrwa.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.hesvh.cn/Article/details/geaawpolm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.zdbjq.cn/Article/details/gtquvzoar.sHtML

TS:   if (s === "") {}
来源：http://3g.fehbvm.com/Article/details/gstdnimqk.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fehbvm.com/Article/details/gcwxacucf.sHtML

Go:   if s == "" {}
来源：http://wap.hesvh.cn/Article/details/gydehsluq.sHtML

Ruby: if s.empty?
来源：http://3g.hesvh.cn/Article/details/giyuypvlp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.hesvh.cn/Article/details/gdzaekcwu.sHtML

[E21] 超长截断加省略号
来源：http://www.share.hesvh.cn/Article/details/ggzvjewtk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fehbvm.com/Article/details/gnquixgvt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.hesvh.cn/Article/details/gxpuqlsai.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gtovdhlvq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gzmkowcsl.sHtML


<!-- 参考信息 -->