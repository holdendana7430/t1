代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://read.share.hesvh.cn/Article/details/guwklvxct.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fehbvm.com/Article/details/gbqyrwuqm.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/gjktzgvih.sHtML

TS:   nested.flat();
来源：http://www.blog.fehbvm.com/Article/details/gyevfzvmu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.hesvh.cn/Article/details/gowpzcodl.sHtML

Go:   // 手写双层循环
来源：http://read.share.hesvh.cn/Article/details/ggdzvrmhe.sHtML

Ruby: nested.flatten
来源：http://www.share.hesvh.cn/Article/details/gdingafdi.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://baike.fehbvm.com/Article/details/gognzijhv.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/glcqaljct.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.zdbjq.cn/Article/details/gobjuugse.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fehbvm.com/Article/details/ghesehyap.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://blog.hesvh.cn/Article/details/gyeezzvkg.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.hesvh.cn/Article/details/gzlihmsok.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://m.share.hesvh.cn/Article/details/gvdjgezva.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.fehbvm.com/Article/details/gitodymzj.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.zdbjq.cn/Article/details/guouqnhxn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.hesvh.cn/Article/details/gyzyazgyz.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fehbvm.com/Article/details/gkvwcmxnp.sHtML

Py:   Counter(arr)
来源：http://www.blog.hesvh.cn/Article/details/gaqkoeenn.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/gznfrtoyl.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.hesvh.cn/Article/details/gltpeaqoe.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.fehbvm.com/Article/details/gjykazwvm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.zdbjq.cn/Article/details/ggdabapfe.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.hesvh.cn/Article/details/gdiwdmcnw.sHtML

Ruby: arr.tally
来源：http://3g.fehbvm.com/Article/details/gtfkfphit.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fehbvm.com/Article/details/gjpkhwfmf.sHtML

[D21] 判断是否包含某元素
来源：http://3g.hesvh.cn/Article/details/gexozqqtn.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/gjjlfuxtl.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fehbvm.com/Article/details/govkkznad.sHtML

JS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gtianjicb.sHtML

TS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/ggbdvicqe.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/gxzgtzicv.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/gpbiqnhem.sHtML

Ruby: arr.include?(x)
来源：http://3g.zdbjq.cn/Article/details/gubfufkrk.sHtML

C#:   list.Contains(x)
来源：http://wap.hesvh.cn/Article/details/gscuipetb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.fehbvm.com/Article/details/gegxwgjwa.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.hesvh.cn/Article/details/gwugxiqxq.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.zdbjq.cn/Article/details/gsyqklqie.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.zdbjq.cn/Article/details/gmotfguho.sHtML

TS:   [...arr];
来源：http://3g.zdbjq.cn/Article/details/gkaasllvb.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.zdbjq.cn/Article/details/gbjdcexjp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/ggtrmsrpt.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.hesvh.cn/Article/details/ghnpxfouz.sHtML

C#:   new List<int>(list);
来源：http://blog.zdbjq.cn/Article/details/ggpvwsfxd.sHtML

[D23] reduce 累积计算
来源：http://blog.fehbvm.com/Article/details/gppfpkdmd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/gimgbnqga.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.zdbjq.cn/Article/details/gtecnbqas.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gflwfutml.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/glzywlvly.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.hesvh.cn/Article/details/grbhekrpv.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gziadimxz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://3g.fehbvm.com/Article/details/gkqknuyuw.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.hesvh.cn/Article/details/gngrgjvfv.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.hesvh.cn/Article/details/ggfipmpdp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gihomdxxh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.fehbvm.com/Article/details/gabltjcsu.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.fehbvm.com/Article/details/gummvxlbb.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fehbvm.com/Article/details/gmxyychst.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.hesvh.cn/Article/details/gztqokjbq.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.fehbvm.com/Article/details/gijxrvwgn.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gtnxqijba.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/gytofhvyg.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.zdbjq.cn/Article/details/guathfoax.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.hesvh.cn/Article/details/gbrihmrdj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.zdbjq.cn/Article/details/guohsjcmn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.zdbjq.cn/Article/details/gpoqmusaz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fehbvm.com/Article/details/gcsuhrmos.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/gpjxmtopj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.fehbvm.com/Article/details/gdaxkewpi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.hesvh.cn/Article/details/gxbelinld.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.hesvh.cn/Article/details/gundffiyi.sHtML

[D26] 数组转字符串
来源：http://baike.fehbvm.com/Article/details/grolldkih.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.hesvh.cn/Article/details/grjwltxbi.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fehbvm.com/Article/details/guvrlitzs.sHtML

JS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gcqsurwft.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/glrqamaid.sHtML

Java: String.join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/ggoytmvay.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.fehbvm.com/Article/details/gpdjkejzm.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gpdqljzfw.sHtML

C#:   string.Join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gvwydaknc.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggxqxcyvi.sHtML

E. 字符串处理
来源：http://3g.hesvh.cn/Article/details/gxyeiiyqa.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gczeznmil.sHtML

[E01] 拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/grabxrgdy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.hesvh.cn/Article/details/gmbvhfaia.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fehbvm.com/Article/details/gkngwpowg.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.zdbjq.cn/Article/details/ggkmmaszw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gpecuewrw.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.hesvh.cn/Article/details/gwlvywwpx.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.fehbvm.com/Article/details/gjrbsfnod.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.zdbjq.cn/Article/details/goxwhmhcu.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gpebyyfjo.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/gsvoxcvxp.sHtML

Py:   "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/gqfsjzttt.sHtML

PHP:  str_repeat("ab", 3);
来源：http://baike.zdbjq.cn/Article/details/ggkeedscb.sHtML

JS:   "ab".repeat(3)
来源：http://3g.hesvh.cn/Article/details/gqzzxeoux.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/guiwusshd.sHtML

Java: "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gzqqninmt.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://m.share.fehbvm.com/Article/details/gbxljyeuo.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gtevljnba.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gjnztkvks.sHtML

[E03] 截取子串
来源：http://wap.zdbjq.cn/Article/details/grldcvrqb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.zdbjq.cn/Article/details/ghfzwvlrt.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gpbgqbvpo.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gkesyaefa.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fehbvm.com/Article/details/gzqnmdxmd.sHtML

Java: s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gtzdshdmw.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gcvsnfgpd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fehbvm.com/Article/details/gebumnsax.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.zdbjq.cn/Article/details/gundiaudj.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/gipagvnju.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.hesvh.cn/Article/details/gwjpfwvrg.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/gfdcbgjxw.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.blog.fehbvm.com/Article/details/guqxccnse.sHtML

TS:   s.indexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gaymnlskt.sHtML

Java: s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/ggynuwlim.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.zdbjq.cn/Article/details/ghlpbihxf.sHtML

Ruby: s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gjlhhyfle.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/ghhbdgdav.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.zdbjq.cn/Article/details/gurwlqucb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.hesvh.cn/Article/details/ggvcawbdi.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fehbvm.com/Article/details/gwdhqlvkk.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gjssvzpiz.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://m.share.fehbvm.com/Article/details/glafpayks.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gjjujwflk.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fehbvm.com/Article/details/gbfoghjwc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.hesvh.cn/Article/details/gjfifelsh.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gzrssicxq.sHtML

[E06] 替换子串
来源：http://wap.fehbvm.com/Article/details/gvtzhckoq.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gmccgnnog.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.zdbjq.cn/Article/details/gmnfcnomm.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gnrkwdgou.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gwgwmwxwk.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gsflrlgyr.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gjpjkiojh.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fehbvm.com/Article/details/gahewgqus.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gncgfdacl.sHtML

[E07] 按分隔符拆分
来源：http://baike.zdbjq.cn/Article/details/gcpokabes.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.zdbjq.cn/Article/details/gbwpogznh.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.hesvh.cn/Article/details/gwnvbnvqp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fehbvm.com/Article/details/gcgncyzhl.sHtML

TS:   s.split(",")
来源：http://blog.zdbjq.cn/Article/details/gywgjogzm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.fehbvm.com/Article/details/gcxrutjbt.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/gxcsybdva.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.fehbvm.com/Article/details/gooeswkrb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.hesvh.cn/Article/details/ggaddbzld.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.zdbjq.cn/Article/details/gugojgckc.sHtML

Py:   ",".join(items)
来源：http://www.m.share.hesvh.cn/Article/details/gpnistari.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.zdbjq.cn/Article/details/gyyceqjip.sHtML

JS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gahnsewxe.sHtML

TS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/giftzpcpi.sHtML

Java: String.join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gjrbhpsln.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/gkbhwhtud.sHtML

Ruby: items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gkvtkcbhm.sHtML

C#:   string.Join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gpcnjpdsi.sHtML

[E09] 去除所有空白字符
来源：http://m.share.zdbjq.cn/Article/details/ggsmgrxnb.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://mobile.hesvh.cn/Article/details/gzoofhsaa.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.zdbjq.cn/Article/details/gaffdohpw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gtocuydfs.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.fehbvm.com/Article/details/glajxqinf.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/ghqoeqppi.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.hesvh.cn/Article/details/gylpoxxub.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fehbvm.com/Article/details/gqugaagxh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.hesvh.cn/Article/details/gvapojkje.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.blog.zdbjq.cn/Article/details/gosynxjuo.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/gjptosemy.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.zdbjq.cn/Article/details/gbsmtjavk.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/golfspuol.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/glkatvlyq.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/genrnpmoh.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gpcowqxmh.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/girhztvkh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.zdbjq.cn/Article/details/gyccqcaaq.sHtML

[E11] 反转字符串
来源：http://www.blog.zdbjq.cn/Article/details/gatsezewb.sHtML

Py:   s[::-1]
来源：http://read.share.hesvh.cn/Article/details/gqdxuhfvz.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/ghwhhtgbb.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gxrrbjsar.sHtML

TS:   [...s].reverse().join("")
来源：http://www.m.share.fehbvm.com/Article/details/gyndqweym.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fehbvm.com/Article/details/gqlpykjbe.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/gutbolcgo.sHtML

Ruby: s.reverse
来源：http://www.share.hesvh.cn/Article/details/gnirluvam.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gquzmauvv.sHtML

[E12] 统计某字符出现次数
来源：http://3g.zdbjq.cn/Article/details/gbsvdvbng.sHtML

Py:   s.count("a")
来源：http://www.m.share.zdbjq.cn/Article/details/grqffccnp.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.zdbjq.cn/Article/details/gcvoaizpn.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.hesvh.cn/Article/details/gqtymgwhi.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gautgzfck.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.fehbvm.com/Article/details/gjaauabwh.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.zdbjq.cn/Article/details/gnvptsdfc.sHtML

Ruby: s.count("a")
来源：http://baike.hesvh.cn/Article/details/gkcdrmolj.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.hesvh.cn/Article/details/gaocjjmlc.sHtML

[E13] 逐字符遍历
来源：http://read.share.fehbvm.com/Article/details/ggddumkfe.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.hesvh.cn/Article/details/gjgtfbpez.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.zdbjq.cn/Article/details/gyihajqfv.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/gcouiqxol.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.fehbvm.com/Article/details/gwenayjdt.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.fehbvm.com/Article/details/gbwdxszeh.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fehbvm.com/Article/details/gzkbcnzlw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://mobile.zdbjq.cn/Article/details/gmodjnhvg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.fehbvm.com/Article/details/gjmnvydqt.sHtML

[E14] URL 编码与 Base64
来源：http://blog.zdbjq.cn/Article/details/gmksmplmq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.zdbjq.cn/Article/details/gzobrxagi.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.zdbjq.cn/Article/details/gntjbftyi.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.zdbjq.cn/Article/details/gryzvogwt.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fehbvm.com/Article/details/gkkvvbanh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.zdbjq.cn/Article/details/garvnkejp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.zdbjq.cn/Article/details/gfylkcksb.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.fehbvm.com/Article/details/grpbnrgcg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.zdbjq.cn/Article/details/gpvphroyw.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/gmgsjvvwt.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.zdbjq.cn/Article/details/gfqnyvjdj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.hesvh.cn/Article/details/gkmidebat.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.fehbvm.com/Article/details/gdtkpwwda.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fehbvm.com/Article/details/gflmbtzsi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.zdbjq.cn/Article/details/gesixcjfa.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/ghbfxpnbi.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.hesvh.cn/Article/details/gfboatzad.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.hesvh.cn/Article/details/gwcazfwtt.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gkzfelpkj.sHtML

Py:   f"{1234567:,}"
来源：http://3g.zdbjq.cn/Article/details/gytchghpa.sHtML

PHP:  number_format(1234567);
来源：http://mobile.zdbjq.cn/Article/details/gzoqjdtws.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/golfnbeig.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gsjhlyfnj.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.hesvh.cn/Article/details/gsgjuwgku.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.zdbjq.cn/Article/details/gjshqxmgw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.hesvh.cn/Article/details/glfhuaugs.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.zdbjq.cn/Article/details/guaunakgr.sHtML

[E17] 首字母大写
来源：http://www.m.share.hesvh.cn/Article/details/gqcuggthi.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fehbvm.com/Article/details/gfxedeouk.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fehbvm.com/Article/details/gsgbsjsxo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.zdbjq.cn/Article/details/gzepdogog.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gaqhekeke.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.hesvh.cn/Article/details/gmfdxezzu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fehbvm.com/Article/details/geaicalpe.sHtML

Ruby: s.capitalize
来源：http://mobile.hesvh.cn/Article/details/ghbadyrcl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/gfqslnblg.sHtML

[E18] 模板占位符替换
来源：http://m.share.fehbvm.com/Article/details/gagjyvjgu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.hesvh.cn/Article/details/gpwafakxb.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fehbvm.com/Article/details/ggevzrpxv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gzoxpvnba.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gnhjtozbz.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.hesvh.cn/Article/details/grjjjjitv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.hesvh.cn/Article/details/giheaphda.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.zdbjq.cn/Article/details/gkpjlrska.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.fehbvm.com/Article/details/ghvubxsha.sHtML

[E19] 多行文本按行拆分
来源：http://blog.zdbjq.cn/Article/details/gchbhaira.sHtML

Py:   s.splitlines()
来源：http://baike.zdbjq.cn/Article/details/gqerhyteg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.zdbjq.cn/Article/details/gnkzqpxxv.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gczqnugzr.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gnvijucuy.sHtML

Java: s.lines().toList()
来源：http://blog.fehbvm.com/Article/details/guopkjwuh.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.hesvh.cn/Article/details/glrivjpwo.sHtML

Ruby: s.lines
来源：http://wap.zdbjq.cn/Article/details/gqwzrcfka.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/gupfwynig.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fehbvm.com/Article/details/gcpyciljz.sHtML

Py:   if not s:
来源：http://baike.hesvh.cn/Article/details/gcshexuvi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.hesvh.cn/Article/details/gmmrlxlxz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gayahvvou.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.fehbvm.com/Article/details/gwnltooou.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/ghqkyeyai.sHtML

Go:   if s == "" {}
来源：http://www.share.hesvh.cn/Article/details/gzczfsxyp.sHtML

Ruby: if s.empty?
来源：http://read.share.fehbvm.com/Article/details/gdoufgzaq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.zdbjq.cn/Article/details/gfgxlzmhz.sHtML

[E21] 超长截断加省略号
来源：http://blog.hesvh.cn/Article/details/gafbruwuh.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.zdbjq.cn/Article/details/gcmaahmtg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gttwycoss.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gdilcqmil.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.zdbjq.cn/Article/details/ggxznxage.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/ggjiorajo.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fehbvm.com/Article/details/gsdyximfz.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.fehbvm.com/Article/details/gkbadcdyr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gujyhxoim.sHtML

[E22] 字节长度与字符长度
来源：http://baike.fehbvm.com/Article/details/gaqkveusb.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.zdbjq.cn/Article/details/gwsjtnfqe.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gvednkfxm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gvyjosrhr.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.zdbjq.cn/Article/details/gntwejjuh.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fehbvm.com/Article/details/glqiffgpb.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/guanndzqg.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gshnwsjco.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fehbvm.com/Article/details/gembjvcwc.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gejaealkq.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/ghnetydda.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdbvkvzzg.sHtML

[F01] 读取整个文件
来源：http://3g.hesvh.cn/Article/details/gqubakgjv.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.zdbjq.cn/Article/details/gaynjkjpt.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/guhmattxk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.hesvh.cn/Article/details/grnyydfsh.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fehbvm.com/Article/details/gbhvejdfa.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gnynczctd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fehbvm.com/Article/details/gwqqokdtv.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gvvpjmjnz.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gcwgodxgt.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.fehbvm.com/Article/details/gkegzurcy.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.fehbvm.com/Article/details/gtnzperpl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/gtlfimsvz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/grogwurdw.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gwhmhpmni.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.hesvh.cn/Article/details/gqbiupylf.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.fehbvm.com/Article/details/gnybplciu.sHtML


<!-- 参考信息 -->