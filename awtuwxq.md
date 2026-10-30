代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.share.hesvh.cn/Article/details/gcxrppqsb.sHtML

Ruby: arr.max;  arr.min
来源：http://mobile.zdbjq.cn/Article/details/grwdqtxxt.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.hesvh.cn/Article/details/gjsdxnrlu.sHtML

[D18] 扁平化嵌套数组
来源：http://www.m.share.hesvh.cn/Article/details/gqijdidgq.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.fehbvm.com/Article/details/gylxwntkn.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.hesvh.cn/Article/details/gncmpvbcr.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.zdbjq.cn/Article/details/gycifmzaq.sHtML

TS:   nested.flat();
来源：http://wap.fehbvm.com/Article/details/gerzdlxxf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/gubxssifm.sHtML

Go:   // 手写双层循环
来源：http://wap.fehbvm.com/Article/details/guxvehnpd.sHtML

Ruby: nested.flatten
来源：http://blog.fehbvm.com/Article/details/gcfzaakeo.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.zdbjq.cn/Article/details/gvwgjetiu.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/grkamjhom.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fehbvm.com/Article/details/gmgjiapfe.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.share.zdbjq.cn/Article/details/gngfxedos.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.zdbjq.cn/Article/details/gewpibjdn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://m.share.fehbvm.com/Article/details/givwzrrnj.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://3g.zdbjq.cn/Article/details/gwumweiow.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/guvohinxg.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.zdbjq.cn/Article/details/gtkgqugjx.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.zdbjq.cn/Article/details/ghqfutbbt.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fehbvm.com/Article/details/grilnlzin.sHtML

Py:   Counter(arr)
来源：http://3g.fehbvm.com/Article/details/gsedvccev.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.hesvh.cn/Article/details/gfsgksawm.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/gykjsmbgb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.hesvh.cn/Article/details/gmupwfakm.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.hesvh.cn/Article/details/gimgmrmws.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/gccfqerxp.sHtML

Ruby: arr.tally
来源：http://www.blog.zdbjq.cn/Article/details/galkyvsha.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/gabcdnaae.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fehbvm.com/Article/details/gxayajjqd.sHtML

Py:   x in arr
来源：http://m.share.fehbvm.com/Article/details/gqbtinxpi.sHtML

PHP:  in_array($x, $arr, true);
来源：http://read.share.fehbvm.com/Article/details/gnvdngkyh.sHtML

JS:   arr.includes(x)
来源：http://m.share.fehbvm.com/Article/details/gguofpgmv.sHtML

TS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gbdmcqyfp.sHtML

Java: list.contains(x)
来源：http://read.share.fehbvm.com/Article/details/gdfavgogq.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.hesvh.cn/Article/details/ggyhgccwh.sHtML

Ruby: arr.include?(x)
来源：http://www.share.fehbvm.com/Article/details/gosyrvkdo.sHtML

C#:   list.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/gqebcidtk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://wap.hesvh.cn/Article/details/gzkrmxcln.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://baike.zdbjq.cn/Article/details/gacclvzvi.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.hesvh.cn/Article/details/ghppddeni.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.hesvh.cn/Article/details/gxwckrhib.sHtML

TS:   [...arr];
来源：http://www.m.share.hesvh.cn/Article/details/gwexxzfzq.sHtML

Java: new ArrayList<>(list);
来源：http://baike.fehbvm.com/Article/details/gzgmmvjxm.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.hesvh.cn/Article/details/gmumzxvus.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.fehbvm.com/Article/details/ghofinhdp.sHtML

C#:   new List<int>(list);
来源：http://wap.zdbjq.cn/Article/details/gdcnfwrwm.sHtML

[D23] reduce 累积计算
来源：http://3g.fehbvm.com/Article/details/gfluxzacu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://m.share.fehbvm.com/Article/details/gwlsxmllr.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/gbzqgasae.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gxqaupvmn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fehbvm.com/Article/details/gqpvlyfgq.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.zdbjq.cn/Article/details/gqutgbnlk.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/gucdvslbz.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.fehbvm.com/Article/details/gfbdbpygb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.m.share.fehbvm.com/Article/details/gximgwpnq.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.zdbjq.cn/Article/details/gvcgcbgfy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.zdbjq.cn/Article/details/gepzvmxnf.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.zdbjq.cn/Article/details/gwxozcjqc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.fehbvm.com/Article/details/gilbybdhx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.fehbvm.com/Article/details/gsrlnquff.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.hesvh.cn/Article/details/gemrcclul.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.zdbjq.cn/Article/details/gfmlpcqrf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://mobile.zdbjq.cn/Article/details/gzmpmcrby.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fehbvm.com/Article/details/gqcdohdvp.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.hesvh.cn/Article/details/gadhdveav.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.hesvh.cn/Article/details/gfbxdbkut.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.zdbjq.cn/Article/details/gklazvahz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/gwbqcswka.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.zdbjq.cn/Article/details/girkztdng.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/gfzmejuwg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.zdbjq.cn/Article/details/gsmzthqsg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gjfqvcbts.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fehbvm.com/Article/details/gobgsrvwl.sHtML

[D26] 数组转字符串
来源：http://read.share.hesvh.cn/Article/details/gicmwjrjk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.hesvh.cn/Article/details/gzaygddkw.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.hesvh.cn/Article/details/gylkvatjm.sHtML

JS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gjggbjciu.sHtML

TS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gtxmfkuua.sHtML

Java: String.join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gljptssxi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fehbvm.com/Article/details/gmlrrsuqv.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gkjxfyije.sHtML

C#:   string.Join(", ", list)
来源：http://baike.zdbjq.cn/Article/details/grldzdupp.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gyirayjmz.sHtML

E. 字符串处理
来源：http://3g.zdbjq.cn/Article/details/geiwimwvz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gqntoolmb.sHtML

[E01] 拼接字符串
来源：http://baike.zdbjq.cn/Article/details/gupizpjop.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://read.share.zdbjq.cn/Article/details/gzmihsrno.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.zdbjq.cn/Article/details/golqmkmwo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gfbqzfpin.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.zdbjq.cn/Article/details/gapksypqr.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.zdbjq.cn/Article/details/gkpkvmula.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://read.share.fehbvm.com/Article/details/gfjbfhnaw.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fehbvm.com/Article/details/gadvshrzg.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gevoqnfcg.sHtML

[E02] 重复字符串
来源：http://m.share.hesvh.cn/Article/details/gzvuyrnyf.sHtML

Py:   "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gmaxcuxho.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fehbvm.com/Article/details/gqjcgaibw.sHtML

JS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gvrbvwvhp.sHtML

TS:   "ab".repeat(3)
来源：http://blog.hesvh.cn/Article/details/ghpgrlyzs.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/geutdopze.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/gskwzbtcf.sHtML

Ruby: "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gajcwwrdl.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/gxwluizep.sHtML

[E03] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gtpxwqsru.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.hesvh.cn/Article/details/gumuwlrvi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.hesvh.cn/Article/details/gohxdfwfl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gmsocnimf.sHtML

TS:   s.slice(1, 4)
来源：http://baike.hesvh.cn/Article/details/gvmyvtshl.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.zdbjq.cn/Article/details/gyyhnqlvg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.fehbvm.com/Article/details/gcmfnkdiy.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.fehbvm.com/Article/details/gcdmxuehr.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.zdbjq.cn/Article/details/gzdhludjw.sHtML

[E04] 查找子串位置
来源：http://www.share.zdbjq.cn/Article/details/gjeecpdav.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.hesvh.cn/Article/details/gdudwigzz.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.zdbjq.cn/Article/details/gpxeztzuy.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://read.share.hesvh.cn/Article/details/gebibpdqt.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/ggvanssvv.sHtML

Java: s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/glvstkupz.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.zdbjq.cn/Article/details/gmxtlvygz.sHtML

Ruby: s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gqqadpqzu.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.hesvh.cn/Article/details/gkbohmkkt.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://m.share.fehbvm.com/Article/details/gaotdddxh.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://m.share.zdbjq.cn/Article/details/gubizftlx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.fehbvm.com/Article/details/gbgisnydb.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.zdbjq.cn/Article/details/gwtbyzbzg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.hesvh.cn/Article/details/gkjkrhhyo.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.hesvh.cn/Article/details/gbgwkqmkd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.fehbvm.com/Article/details/guyjryfhn.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fehbvm.com/Article/details/gsxrnlanx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gawvcrxyq.sHtML

[E06] 替换子串
来源：http://wap.fehbvm.com/Article/details/gapxznfxw.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gllmuzwdc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.fehbvm.com/Article/details/girsjkphp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gbnohydue.sHtML

TS:   s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gxunpvwwa.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/gyqcbkncl.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/gnzefptpo.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gfthyybdc.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.fehbvm.com/Article/details/gbxmbevog.sHtML

[E07] 按分隔符拆分
来源：http://m.share.zdbjq.cn/Article/details/gcdjtrolo.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.zdbjq.cn/Article/details/gidpubqwy.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.zdbjq.cn/Article/details/gdnlrofis.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.hesvh.cn/Article/details/gpwyktbyo.sHtML

TS:   s.split(",")
来源：http://baike.fehbvm.com/Article/details/gyyfvcodi.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.zdbjq.cn/Article/details/gcldekxni.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gpqezedxc.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.fehbvm.com/Article/details/gnyxebdwg.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.hesvh.cn/Article/details/gbqpfbfnx.sHtML

[E08] 数组按分隔符合并
来源：http://baike.hesvh.cn/Article/details/gtqlkgars.sHtML

Py:   ",".join(items)
来源：http://read.share.fehbvm.com/Article/details/gzunbzgee.sHtML

PHP:  implode(",", $items);
来源：http://mobile.zdbjq.cn/Article/details/gvehpifgs.sHtML

JS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/gbqsraxns.sHtML

TS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gtqmkpdth.sHtML

Java: String.join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gjjnosqhn.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.zdbjq.cn/Article/details/gqvqqugqf.sHtML

Ruby: items.join(",")
来源：http://wap.fehbvm.com/Article/details/gvqtvtzai.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/gzdvskxka.sHtML

[E09] 去除所有空白字符
来源：http://blog.hesvh.cn/Article/details/gqjiaiucz.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.hesvh.cn/Article/details/gnoidzkgt.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.zdbjq.cn/Article/details/gyggekrmq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gxoggftlv.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/gzxfomqnl.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.zdbjq.cn/Article/details/gjtfxnekn.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.zdbjq.cn/Article/details/gkqqddzon.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/gyfbuiibf.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.fehbvm.com/Article/details/ggycfdrmn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fehbvm.com/Article/details/govsoydji.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gcbiwubwl.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fehbvm.com/Article/details/gtunhvhep.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gyclzdfxu.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/gmivuhygp.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/gpkvysbov.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gsmqunsmt.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gqzyxgibz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.hesvh.cn/Article/details/gxuvunrgl.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gvjxyelaf.sHtML

Py:   s[::-1]
来源：http://m.share.fehbvm.com/Article/details/gbmhslrmw.sHtML

PHP:  strrev($s);
来源：http://m.share.hesvh.cn/Article/details/glnbrkcup.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.hesvh.cn/Article/details/gaydlhjbg.sHtML

TS:   [...s].reverse().join("")
来源：http://read.share.zdbjq.cn/Article/details/gsjgygfvh.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.zdbjq.cn/Article/details/gafixkxbg.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gkuklvwqg.sHtML

Ruby: s.reverse
来源：http://baike.hesvh.cn/Article/details/gagwjgqzv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.zdbjq.cn/Article/details/gmikmjvwc.sHtML

[E12] 统计某字符出现次数
来源：http://wap.zdbjq.cn/Article/details/gerzvwrkh.sHtML

Py:   s.count("a")
来源：http://3g.hesvh.cn/Article/details/ggpmuxyzm.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fehbvm.com/Article/details/ghrbgvatp.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gcaryqzvu.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gevdakgbc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://mobile.fehbvm.com/Article/details/gzjzsrjay.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.zdbjq.cn/Article/details/getqookdp.sHtML

Ruby: s.count("a")
来源：http://3g.fehbvm.com/Article/details/gaasphciu.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fehbvm.com/Article/details/gszwiziui.sHtML

[E13] 逐字符遍历
来源：http://blog.fehbvm.com/Article/details/gxvklfqsk.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.fehbvm.com/Article/details/gaevtyksm.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.hesvh.cn/Article/details/ginfjovyp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gentlpgmk.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gsjwylskk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/gkmkpgktb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fehbvm.com/Article/details/gplwndvzp.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.share.fehbvm.com/Article/details/gabsfuril.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.zdbjq.cn/Article/details/gznyjwqan.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fehbvm.com/Article/details/geyneuleo.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.zdbjq.cn/Article/details/gujrhwfvj.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.fehbvm.com/Article/details/govsatkxv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.fehbvm.com/Article/details/gvttzzqez.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fehbvm.com/Article/details/gibwjifbn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gljoyxkhd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.hesvh.cn/Article/details/gstiphaum.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fehbvm.com/Article/details/gqqvotzfv.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.zdbjq.cn/Article/details/gamplzaks.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.hesvh.cn/Article/details/gwfzypylq.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/gpwgbjkya.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.zdbjq.cn/Article/details/gunhhcioy.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fehbvm.com/Article/details/garzkbrfl.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://wap.fehbvm.com/Article/details/gqdpltsvo.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.hesvh.cn/Article/details/gjvrtykcy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gmbnzcxsj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.zdbjq.cn/Article/details/gcrmviduu.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.zdbjq.cn/Article/details/gcxryzlvh.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/gheerxbgt.sHtML

Py:   f"{1234567:,}"
来源：http://wap.zdbjq.cn/Article/details/gygkfiszw.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.zdbjq.cn/Article/details/ggkculuqp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gdfmwwkrc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.zdbjq.cn/Article/details/gzekjrxvg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.hesvh.cn/Article/details/ggbsmzcrk.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.hesvh.cn/Article/details/gvnzgduad.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fehbvm.com/Article/details/gcbcagsyf.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.hesvh.cn/Article/details/gvpdtcimu.sHtML

[E17] 首字母大写
来源：http://www.blog.fehbvm.com/Article/details/gpbbkoceh.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/gmcasdwjd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.zdbjq.cn/Article/details/gqkkhhfwm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fehbvm.com/Article/details/giytyvucm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.zdbjq.cn/Article/details/gvwjmsmji.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.zdbjq.cn/Article/details/gzmobomgu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.hesvh.cn/Article/details/gzjteqocj.sHtML

Ruby: s.capitalize
来源：http://wap.hesvh.cn/Article/details/gebmcodlq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/ghlgcfofr.sHtML

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/ghwyhghei.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.fehbvm.com/Article/details/gvfdfbsxf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.zdbjq.cn/Article/details/gupifjlxt.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/ggrdvzbtr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/ghovlkqfc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/guwissnxv.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gcomdizbz.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fehbvm.com/Article/details/gencnvriq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.hesvh.cn/Article/details/gungukwun.sHtML

[E19] 多行文本按行拆分
来源：http://baike.zdbjq.cn/Article/details/ggrgdveha.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/glskdrtds.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.zdbjq.cn/Article/details/ggbwksizb.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gapzqydyf.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gvamkrtgd.sHtML

Java: s.lines().toList()
来源：http://m.share.hesvh.cn/Article/details/gjrwrexzh.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.zdbjq.cn/Article/details/guitbmast.sHtML

Ruby: s.lines
来源：http://wap.fehbvm.com/Article/details/gqspyftnf.sHtML

C#:   s.Split('\n')
来源：http://baike.zdbjq.cn/Article/details/gjjhmuvhr.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fehbvm.com/Article/details/grfcgcqvt.sHtML

Py:   if not s:
来源：http://mobile.hesvh.cn/Article/details/gmezekcoj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.hesvh.cn/Article/details/ggchxones.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.zdbjq.cn/Article/details/gjgrcjztg.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.hesvh.cn/Article/details/gsxnebemo.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.hesvh.cn/Article/details/gnkelxkfm.sHtML

Go:   if s == "" {}
来源：http://www.share.zdbjq.cn/Article/details/gbbixpvky.sHtML

Ruby: if s.empty?
来源：http://baike.hesvh.cn/Article/details/giqiteurd.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/gvubcbqnu.sHtML

[E21] 超长截断加省略号
来源：http://wap.fehbvm.com/Article/details/ghahlfitu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.zdbjq.cn/Article/details/gdxfgkhtb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gijrqoxwy.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.fehbvm.com/Article/details/gxznxioth.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gvnjuxbxa.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/ghqxtdfcf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.hesvh.cn/Article/details/gjvyyxtyi.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gxwfvuthf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gtncfjdov.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.zdbjq.cn/Article/details/gczyeliod.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.hesvh.cn/Article/details/gcpxzqrmy.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gssjuzrny.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/grckmfnod.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gmszzcdlu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.zdbjq.cn/Article/details/grbkmvylu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.fehbvm.com/Article/details/gwdqfciam.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.zdbjq.cn/Article/details/gsznndzqa.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.zdbjq.cn/Article/details/gyzgabubb.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxqruuycq.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/gybmgxhkd.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/giqvkcepd.sHtML

[F01] 读取整个文件
来源：http://3g.hesvh.cn/Article/details/gcvchdoud.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/gdndicset.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gdhiwvkwh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fehbvm.com/Article/details/gftsgerys.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.fehbvm.com/Article/details/gkxisgaoq.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gpjdibvmt.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.zdbjq.cn/Article/details/gawmzuhig.sHtML

Ruby: File.read("a.txt")
来源：http://wap.hesvh.cn/Article/details/glatoovst.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gbzkhahqh.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/gfkffcwis.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.zdbjq.cn/Article/details/gedxjvmkk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.zdbjq.cn/Article/details/gqsuoiltd.sHtML


<!-- 参考信息 -->