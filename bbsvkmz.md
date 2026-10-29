代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://www.blog.zdbjq.cn/Article/details/gdzmmxgfy.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.zdbjq.cn/Article/details/gksadvbhl.sHtML

TS:   Math.max(...arr);
来源：http://wap.zdbjq.cn/Article/details/gdfwnlzbs.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://wap.hesvh.cn/Article/details/gmhyxzjse.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://baike.fehbvm.com/Article/details/glkyjvauo.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/glpprayac.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.zdbjq.cn/Article/details/gdzjiljeu.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fehbvm.com/Article/details/gapkwrhon.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.zdbjq.cn/Article/details/gkbrufozd.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.hesvh.cn/Article/details/gneipczhv.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.hesvh.cn/Article/details/goduwebiu.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/ggjzxmbnx.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fehbvm.com/Article/details/gscvqtdry.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fehbvm.com/Article/details/gzpdbtcoy.sHtML

Ruby: nested.flatten
来源：http://www.m.share.hesvh.cn/Article/details/gwfyrsxrn.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fehbvm.com/Article/details/ggaowaqwh.sHtML

[D19] 按字段分组
来源：http://baike.fehbvm.com/Article/details/gzjlmzcxb.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.blog.fehbvm.com/Article/details/gfzvwlgig.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.hesvh.cn/Article/details/gyyyuizun.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.zdbjq.cn/Article/details/gkmdtgihk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gvszztafz.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.hesvh.cn/Article/details/gjgdldnkf.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fehbvm.com/Article/details/grtozpdpa.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.hesvh.cn/Article/details/gmbklcpkb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://blog.fehbvm.com/Article/details/gwnikaepb.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.hesvh.cn/Article/details/gjgjfbjml.sHtML

Py:   Counter(arr)
来源：http://wap.fehbvm.com/Article/details/gsbopaauy.sHtML

PHP:  array_count_values($arr);
来源：http://wap.fehbvm.com/Article/details/gerfwbwhs.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fehbvm.com/Article/details/gflqibuge.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gjemavvqe.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fehbvm.com/Article/details/gyjevcdba.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.zdbjq.cn/Article/details/gajthplao.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/gmgcamkfo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/gweyhxmxb.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gqsuqvqwl.sHtML

Py:   x in arr
来源：http://3g.zdbjq.cn/Article/details/gstzsuygi.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.zdbjq.cn/Article/details/gfzzoshbc.sHtML

JS:   arr.includes(x)
来源：http://wap.zdbjq.cn/Article/details/gmbgutlvr.sHtML

TS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/glrizrcrj.sHtML

Java: list.contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gileguybe.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.hesvh.cn/Article/details/gjsxqbakh.sHtML

Ruby: arr.include?(x)
来源：http://read.share.hesvh.cn/Article/details/gletnksym.sHtML

C#:   list.Contains(x)
来源：http://m.share.zdbjq.cn/Article/details/gboltzehl.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/gipitocdd.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fehbvm.com/Article/details/gruqtmmgb.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fehbvm.com/Article/details/gabzpnikp.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://blog.hesvh.cn/Article/details/gpdhabieo.sHtML

TS:   [...arr];
来源：http://read.share.zdbjq.cn/Article/details/gohnljous.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.zdbjq.cn/Article/details/gihkfynoj.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fehbvm.com/Article/details/gesibmiye.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.fehbvm.com/Article/details/gpocayxvu.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/gbateetsp.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fehbvm.com/Article/details/ghzovcpcn.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.zdbjq.cn/Article/details/gxepgtobh.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fehbvm.com/Article/details/gsjyhneud.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.zdbjq.cn/Article/details/gecncztmm.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gnkzsetbk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://m.share.hesvh.cn/Article/details/gxhwcmhbo.sHtML

Go:   // 手写循环
来源：http://m.share.zdbjq.cn/Article/details/gjliupyda.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fehbvm.com/Article/details/gvujqevzw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/glikpgxao.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fehbvm.com/Article/details/gtuthkrkr.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.hesvh.cn/Article/details/gxbztbxyt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.hesvh.cn/Article/details/gqwsnlakm.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.hesvh.cn/Article/details/gublwxgyj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gzrsnabgz.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/gxsecvanf.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.zdbjq.cn/Article/details/griyvajtd.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fehbvm.com/Article/details/gjkvrkalf.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.fehbvm.com/Article/details/geyqdofyw.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.hesvh.cn/Article/details/gsnmalhrq.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.zdbjq.cn/Article/details/gingrphvi.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.zdbjq.cn/Article/details/gvjlhodwn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.hesvh.cn/Article/details/gyxygfdye.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fehbvm.com/Article/details/gcxdhriyf.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.fehbvm.com/Article/details/gimjfasom.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/ghurnxxhj.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.fehbvm.com/Article/details/ggoykriwl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/gbgvlzvyw.sHtML

[D26] 数组转字符串
来源：http://baike.fehbvm.com/Article/details/gwgtpbvsg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gaiaulzkt.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.hesvh.cn/Article/details/gnwoxqevs.sHtML

JS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/ggrgbtobx.sHtML

TS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gbzaexlec.sHtML

Java: String.join(", ", list)
来源：http://www.share.fehbvm.com/Article/details/grtlghrzz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.fehbvm.com/Article/details/gtjaevvfr.sHtML

Ruby: arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gfemgqbwk.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gcleyugtp.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gubeyubex.sHtML

E. 字符串处理
来源：http://blog.fehbvm.com/Article/details/gtvpbqlyb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghmpkoxgh.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gttrjnvwa.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.hesvh.cn/Article/details/gvpjrptxw.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fehbvm.com/Article/details/gopmhccit.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/gztljtmml.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/guxjgnlex.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://mobile.hesvh.cn/Article/details/gdiktcizm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fehbvm.com/Article/details/gbngstubk.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.hesvh.cn/Article/details/gosvpnhei.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.hesvh.cn/Article/details/ghkxbmjxl.sHtML

[E02] 重复字符串
来源：http://www.m.share.hesvh.cn/Article/details/gxzattvfw.sHtML

Py:   "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gnxinruhj.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.fehbvm.com/Article/details/gbfzhmznr.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gphngbqpb.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.fehbvm.com/Article/details/gqmxdejqu.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.fehbvm.com/Article/details/gfldhytkc.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://3g.fehbvm.com/Article/details/glvvcyrbr.sHtML

Ruby: "ab" * 3
来源：http://mobile.zdbjq.cn/Article/details/gybfqlvxq.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.hesvh.cn/Article/details/gtsfzniam.sHtML

[E03] 截取子串
来源：http://blog.hesvh.cn/Article/details/ggbbezyix.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fehbvm.com/Article/details/gazumjfbx.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gieumdyhk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gqocjygye.sHtML

TS:   s.slice(1, 4)
来源：http://www.blog.hesvh.cn/Article/details/gelokpjzp.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gzgtuxbbj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.hesvh.cn/Article/details/gfyseoljk.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.hesvh.cn/Article/details/giqkefvjw.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.hesvh.cn/Article/details/gjzjgikjn.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/gwatpvcmr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://3g.hesvh.cn/Article/details/gzbhrzzyn.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fehbvm.com/Article/details/griskmarb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fehbvm.com/Article/details/gogmjpnow.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/glhgasxjn.sHtML

Java: s.indexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/grewvkbfx.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.hesvh.cn/Article/details/geuhmzvoq.sHtML

Ruby: s.index("x")
来源：http://wap.fehbvm.com/Article/details/gkblojtee.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gzrbqfjrn.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.zdbjq.cn/Article/details/glvwqsvhv.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.hesvh.cn/Article/details/geronbece.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.fehbvm.com/Article/details/gdftwdshz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fehbvm.com/Article/details/gquxiqsyy.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.fehbvm.com/Article/details/ggjxyigyh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gpwetsojw.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.fehbvm.com/Article/details/gvdzpjgaj.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fehbvm.com/Article/details/gaenkxggu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.hesvh.cn/Article/details/gflvyctsw.sHtML

[E06] 替换子串
来源：http://3g.fehbvm.com/Article/details/gazuwrokv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gwsisytqu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.hesvh.cn/Article/details/gtgbjoobz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gylbclrvs.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gppavceyt.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gcsyycjmt.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gyrgzgygg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.fehbvm.com/Article/details/gegbpylwd.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gbqlhqbpb.sHtML

[E07] 按分隔符拆分
来源：http://read.share.hesvh.cn/Article/details/gxtzvamfh.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.zdbjq.cn/Article/details/glpwxdjvt.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.hesvh.cn/Article/details/gyowsiuic.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.fehbvm.com/Article/details/guziuxxyu.sHtML

TS:   s.split(",")
来源：http://wap.zdbjq.cn/Article/details/ghugnnkqn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.zdbjq.cn/Article/details/gaglxticx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fehbvm.com/Article/details/gnppglgwj.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fehbvm.com/Article/details/gwytqmamb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.zdbjq.cn/Article/details/gjccyrapa.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.zdbjq.cn/Article/details/gkcfjsrrp.sHtML

Py:   ",".join(items)
来源：http://blog.hesvh.cn/Article/details/gxbghearc.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.zdbjq.cn/Article/details/gypwvoong.sHtML

JS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gmtoxjzbr.sHtML

TS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gsnwbvlee.sHtML

Java: String.join(",", items)
来源：http://wap.zdbjq.cn/Article/details/gjpvnjflv.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.zdbjq.cn/Article/details/grenosdqs.sHtML

Ruby: items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gosbpsmai.sHtML

C#:   string.Join(",", items)
来源：http://www.share.zdbjq.cn/Article/details/gaddupxqp.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fehbvm.com/Article/details/gqvbjfois.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.zdbjq.cn/Article/details/gtqmxgmpw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fehbvm.com/Article/details/gleotdlou.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gmrdnuifw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.zdbjq.cn/Article/details/gpdodkcnp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fehbvm.com/Article/details/gwhphmocd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.zdbjq.cn/Article/details/gkyxkprpv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.fehbvm.com/Article/details/gypxopddd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gaqlthjhb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.hesvh.cn/Article/details/gdnttcxcp.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gshqurnaw.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.zdbjq.cn/Article/details/gqjyxnscv.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gpjzuckwe.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.zdbjq.cn/Article/details/grschxbaa.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gwkvnwgkv.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gbcgyuhod.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gzgmiwyin.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fehbvm.com/Article/details/glmhunotd.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/gpefgtstc.sHtML

Py:   s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/ghxibeoan.sHtML

PHP:  strrev($s);
来源：http://m.share.hesvh.cn/Article/details/ggzswzyud.sHtML

JS:   [...s].reverse().join("")
来源：http://read.share.hesvh.cn/Article/details/gghzcoqnh.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gjjxproap.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fehbvm.com/Article/details/gveeufnjp.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gppdbtmlq.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/gzuuvmoxw.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gdwdhuhmq.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.hesvh.cn/Article/details/gbsdtvpxk.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gcdqncaek.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fehbvm.com/Article/details/gepzhtdjr.sHtML

JS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/ghimthwzl.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.hesvh.cn/Article/details/gzjlwxiin.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.zdbjq.cn/Article/details/gsrwwapgm.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.fehbvm.com/Article/details/ghbrvjidp.sHtML

Ruby: s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gveckvspe.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.hesvh.cn/Article/details/geedgecdt.sHtML

[E13] 逐字符遍历
来源：http://blog.zdbjq.cn/Article/details/gxqiouwaz.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fehbvm.com/Article/details/gdpaguyvi.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.zdbjq.cn/Article/details/gdvarcutn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gdtcltccv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gcecyjrfv.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gpqnfpxus.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.hesvh.cn/Article/details/gfhdutotg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.hesvh.cn/Article/details/gtftlzyfw.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.hesvh.cn/Article/details/gypnazlyt.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.zdbjq.cn/Article/details/gefwpirdv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.hesvh.cn/Article/details/geiqsuzds.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gnvyhximu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.fehbvm.com/Article/details/gdxvnknmc.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.zdbjq.cn/Article/details/gqdpxwlja.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gshxmutjn.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.hesvh.cn/Article/details/gjhxksthr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.zdbjq.cn/Article/details/gkeemueed.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.hesvh.cn/Article/details/gqditnrke.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.hesvh.cn/Article/details/grjpgxysu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.hesvh.cn/Article/details/govavkgrq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.hesvh.cn/Article/details/gfzwydsom.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fehbvm.com/Article/details/gitngpnto.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.fehbvm.com/Article/details/gmtitbpjf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fehbvm.com/Article/details/gsvntutkk.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gohwuimto.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.hesvh.cn/Article/details/gidtcqyqt.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.zdbjq.cn/Article/details/guvnmllds.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/getegkrxx.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fehbvm.com/Article/details/guamzhizm.sHtML

PHP:  number_format(1234567);
来源：http://www.share.zdbjq.cn/Article/details/gijwyxney.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.fehbvm.com/Article/details/ggzxnvfde.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gmkuttkig.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.hesvh.cn/Article/details/gnkbxyajb.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.hesvh.cn/Article/details/guoommjda.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.zdbjq.cn/Article/details/gdllzmbqd.sHtML

C#:   1234567.ToString("N0")
来源：http://www.share.fehbvm.com/Article/details/gfbipnkwd.sHtML

[E17] 首字母大写
来源：http://blog.zdbjq.cn/Article/details/gamnvmtph.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fehbvm.com/Article/details/gkoxzwcau.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.zdbjq.cn/Article/details/gneaumcco.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gelkrcsce.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gaclixybk.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.fehbvm.com/Article/details/gxartbcjz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fehbvm.com/Article/details/gzgkssrjv.sHtML

Ruby: s.capitalize
来源：http://www.share.fehbvm.com/Article/details/gssynfstr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.zdbjq.cn/Article/details/grwfpdkoo.sHtML

[E18] 模板占位符替换
来源：http://read.share.hesvh.cn/Article/details/glifxerax.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.fehbvm.com/Article/details/gbcmizvjq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.zdbjq.cn/Article/details/gempfcwpj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gcfxvsgrt.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gkgipumij.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gzttgczqo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gbltgytln.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fehbvm.com/Article/details/ghyjhlbgx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.zdbjq.cn/Article/details/gjhotkfjy.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.fehbvm.com/Article/details/gijfirhmy.sHtML

Py:   s.splitlines()
来源：http://read.share.fehbvm.com/Article/details/gpasfrqzx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://wap.fehbvm.com/Article/details/gmrubtkso.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gcpfbsudj.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.zdbjq.cn/Article/details/goeattwpt.sHtML

Java: s.lines().toList()
来源：http://wap.hesvh.cn/Article/details/gkahipeze.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/gvxufqxlp.sHtML

Ruby: s.lines
来源：http://www.blog.hesvh.cn/Article/details/gsqlrdswb.sHtML

C#:   s.Split('\n')
来源：http://baike.hesvh.cn/Article/details/glakqbzlr.sHtML

[E20] 判断字符串是否为空
来源：http://blog.zdbjq.cn/Article/details/gsthsvkzk.sHtML

Py:   if not s:
来源：http://m.share.zdbjq.cn/Article/details/gogqyuetv.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.fehbvm.com/Article/details/gnsykvzdd.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.zdbjq.cn/Article/details/gxjktspeb.sHtML

TS:   if (s === "") {}
来源：http://blog.hesvh.cn/Article/details/gsqpspggh.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gvzlzzvck.sHtML

Go:   if s == "" {}
来源：http://wap.fehbvm.com/Article/details/ghqqgqyds.sHtML

Ruby: if s.empty?
来源：http://wap.zdbjq.cn/Article/details/gxzjjiang.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gbavhctkx.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.zdbjq.cn/Article/details/gpzeykzwx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://m.share.fehbvm.com/Article/details/gqokghkli.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gsvjqbboq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gaofuoepp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/golclbsjj.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gpueqbugs.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.fehbvm.com/Article/details/gtwzczcgc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gbnoqaqyo.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gnzqrqadi.sHtML

[E22] 字节长度与字符长度
来源：http://blog.zdbjq.cn/Article/details/gbcknuett.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gqxtfqnpg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gcbtwgdve.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/glvsmlobi.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gjnqinrwi.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.fehbvm.com/Article/details/gpghhxdfa.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fehbvm.com/Article/details/ghzmlykbt.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.fehbvm.com/Article/details/gjgoefykr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.zdbjq.cn/Article/details/ggpxxaehq.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gasevwcws.sHtML

F. 文件与目录
来源：http://wap.hesvh.cn/Article/details/goxvfkgtq.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ghokgwdfq.sHtML

[F01] 读取整个文件
来源：http://wap.fehbvm.com/Article/details/gyymhpiza.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.hesvh.cn/Article/details/gsacbggvu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gumfhlwnv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fehbvm.com/Article/details/gckbldpaw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.fehbvm.com/Article/details/gvwgqeric.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gjrpqcnto.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.zdbjq.cn/Article/details/gtnjokrjp.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gomtvruko.sHtML


<!-- 参考信息 -->