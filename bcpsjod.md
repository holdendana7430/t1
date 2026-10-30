代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gkycfyude.sHtML

Go:   // 手写双层循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhymzyzc.sHtML

Ruby: nested.flatten
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkwhlhql.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjaqkjbz.sHtML

[D19] 按字段分组
来源：http://baike.fanxiaobao.xyz/Article/details/gkcpdvpip.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdznwhoi.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvlsoiob.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.share.fanxiaobao.xyz/Article/details/ghvrthtic.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.fanxiaobao.xyz/Article/details/gvjsqbmvd.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://read.share.fanxiaobao.xyz/Article/details/gijvpvjqu.sHtML

Go:   // 手写 map[string][]T
来源：http://www.share.fanxiaobao.xyz/Article/details/gepnsncva.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://read.share.fanxiaobao.xyz/Article/details/gbujobliw.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.fanxiaobao.xyz/Article/details/gpbdrzfnl.sHtML

[D20] 统计每个元素出现次数
来源：http://3g.fanxiaobao.xyz/Article/details/ghboqyltj.sHtML

Py:   Counter(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxugtddv.sHtML

PHP:  array_count_values($arr);
来源：http://mobile.fanxiaobao.xyz/Article/details/gdaajjada.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fanxiaobao.xyz/Article/details/garwyrtut.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.fanxiaobao.xyz/Article/details/gpgvodbku.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvuovimii.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fanxiaobao.xyz/Article/details/gpewdrizy.sHtML

Ruby: arr.tally
来源：http://read.share.fanxiaobao.xyz/Article/details/gjaperrxr.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://blog.fanxiaobao.xyz/Article/details/gxoaktkal.sHtML

[D21] 判断是否包含某元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gorgaezgg.sHtML

Py:   x in arr
来源：http://3g.fanxiaobao.xyz/Article/details/grrxfulxc.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fanxiaobao.xyz/Article/details/ghsglxtkt.sHtML

JS:   arr.includes(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gigduxvsk.sHtML

TS:   arr.includes(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjqsplnv.sHtML

Java: list.contains(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxycobeui.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glftmyjwh.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsojoojok.sHtML

C#:   list.Contains(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gutuhutmh.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.fanxiaobao.xyz/Article/details/gcqumvzmp.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fanxiaobao.xyz/Article/details/glgttyfea.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwdrhhsz.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.fanxiaobao.xyz/Article/details/gszbhsqiq.sHtML

TS:   [...arr];
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyudpkxx.sHtML

Java: new ArrayList<>(list);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjeuadhr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://3g.fanxiaobao.xyz/Article/details/gkfjnqyeh.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmtxyphay.sHtML

C#:   new List<int>(list);
来源：http://3g.fanxiaobao.xyz/Article/details/gloexdhbm.sHtML

[D23] reduce 累积计算
来源：http://wap.fanxiaobao.xyz/Article/details/gwvoilopc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.fanxiaobao.xyz/Article/details/geuniluio.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcdvtadf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/gptthhzbo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjgteqwpy.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.fanxiaobao.xyz/Article/details/glpyekrum.sHtML

Go:   // 手写循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxuxeqov.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fanxiaobao.xyz/Article/details/guntkuebv.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fanxiaobao.xyz/Article/details/gkenxjsny.sHtML

[D24] 字典 / Map 基本操作
来源：http://wap.fanxiaobao.xyz/Article/details/gmsrfvftt.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.fanxiaobao.xyz/Article/details/grlctswaz.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://wap.fanxiaobao.xyz/Article/details/gfwjxszpn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxbcdxkf.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gxuedihnq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://3g.fanxiaobao.xyz/Article/details/gcvuoujny.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fanxiaobao.xyz/Article/details/gidseguew.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrpkxssr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.fanxiaobao.xyz/Article/details/gjyjrloyp.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fanxiaobao.xyz/Article/details/grcmnvsrx.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzlkggpqj.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.fanxiaobao.xyz/Article/details/gothbjlqz.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqndvjfw.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fanxiaobao.xyz/Article/details/gzivasoak.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzvnmzvl.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvuvcjwhm.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fanxiaobao.xyz/Article/details/gthfzuqfx.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwfqrnhc.sHtML

[D26] 数组转字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdnqittk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://3g.fanxiaobao.xyz/Article/details/gmihpfzmh.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gnfkqhwmh.sHtML

JS:   arr.join(", ")
来源：http://mobile.fanxiaobao.xyz/Article/details/gnzvxcwyk.sHtML

TS:   arr.join(", ")
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxfxphdh.sHtML

Java: String.join(", ", list)
来源：http://mobile.fanxiaobao.xyz/Article/details/gehmrwkru.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.fanxiaobao.xyz/Article/details/gmgnykgrf.sHtML

Ruby: arr.join(", ")
来源：http://wap.fanxiaobao.xyz/Article/details/gcwccskjq.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fanxiaobao.xyz/Article/details/ghyhqzkdw.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcxmuvig.sHtML

E. 字符串处理
来源：http://m.share.fanxiaobao.xyz/Article/details/geizrnzxv.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyhbuvfr.sHtML

[E01] 拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gcqntyete.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.fanxiaobao.xyz/Article/details/gjabxpyja.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdeceuzml.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fanxiaobao.xyz/Article/details/gtlgogtdj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaaupvbhi.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqjcitym.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fanxiaobao.xyz/Article/details/grvivdeeg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fanxiaobao.xyz/Article/details/gxxfjdhqz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.fanxiaobao.xyz/Article/details/gucyqugjg.sHtML

[E02] 重复字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gnhkleaza.sHtML

Py:   "ab" * 3
来源：http://www.share.fanxiaobao.xyz/Article/details/gxizvmwjo.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gqxecktnp.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzovlmwr.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhfdkfup.sHtML

Java: "ab".repeat(3)
来源：http://baike.fanxiaobao.xyz/Article/details/girujskle.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fanxiaobao.xyz/Article/details/gvcqhbimu.sHtML

Ruby: "ab" * 3
来源：http://read.share.fanxiaobao.xyz/Article/details/gjoajgkoa.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.fanxiaobao.xyz/Article/details/gghfelpba.sHtML

[E03] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/givngiioh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdmdzbcc.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.fanxiaobao.xyz/Article/details/gfspsjzyc.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadbrduyi.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.fanxiaobao.xyz/Article/details/geqibhhpr.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcyeymfmg.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlcaqjeh.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvkxhvnt.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.fanxiaobao.xyz/Article/details/gblagzeol.sHtML

[E04] 查找子串位置
来源：http://m.share.fanxiaobao.xyz/Article/details/gfsygfulj.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjahethtt.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqibkzajc.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.fanxiaobao.xyz/Article/details/ghwifatbx.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndmagfta.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsxudjbt.sHtML

Go:   strings.Index(s, "x")
来源：http://blog.fanxiaobao.xyz/Article/details/ggtfitlns.sHtML

Ruby: s.index("x")
来源：http://read.share.fanxiaobao.xyz/Article/details/gkiiyawiy.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fanxiaobao.xyz/Article/details/gtkfudief.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.fanxiaobao.xyz/Article/details/gdzaowrcy.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpralxun.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fanxiaobao.xyz/Article/details/gypjiigiz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fanxiaobao.xyz/Article/details/gditqgxhv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fanxiaobao.xyz/Article/details/gunhoeqal.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fanxiaobao.xyz/Article/details/gyrudqaou.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpolmlxpp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.fanxiaobao.xyz/Article/details/gcfmigbzo.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fanxiaobao.xyz/Article/details/gpmwlxljr.sHtML

[E06] 替换子串
来源：http://read.share.fanxiaobao.xyz/Article/details/ggoklgvje.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gewryaokx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkuncedz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpkeldra.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fanxiaobao.xyz/Article/details/gziojxsaf.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gblmpzzao.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gxcdnqsgc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fanxiaobao.xyz/Article/details/gkxbenuoj.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjvielbb.sHtML

[E07] 按分隔符拆分
来源：http://www.share.fanxiaobao.xyz/Article/details/gotlqvjae.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjwjssqt.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gktajmzry.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fanxiaobao.xyz/Article/details/gntjcqwpd.sHtML

TS:   s.split(",")
来源：http://3g.fanxiaobao.xyz/Article/details/guywubzil.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fanxiaobao.xyz/Article/details/garnfpppy.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gqrkcgkrr.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fanxiaobao.xyz/Article/details/gewbbiwas.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fanxiaobao.xyz/Article/details/gvovadsgx.sHtML

[E08] 数组按分隔符合并
来源：http://wap.fanxiaobao.xyz/Article/details/gruussvxk.sHtML

Py:   ",".join(items)
来源：http://wap.fanxiaobao.xyz/Article/details/gakyjmbdo.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fanxiaobao.xyz/Article/details/gseatepqp.sHtML

JS:   items.join(",")
来源：http://mobile.fanxiaobao.xyz/Article/details/gzioiskfq.sHtML

TS:   items.join(",")
来源：http://www.share.fanxiaobao.xyz/Article/details/gynvqzzvm.sHtML

Java: String.join(",", items)
来源：http://wap.fanxiaobao.xyz/Article/details/gqbckonxf.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpkwnadcz.sHtML

Ruby: items.join(",")
来源：http://blog.fanxiaobao.xyz/Article/details/garpkcisw.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjzjmuhe.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgwblkea.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkutymqli.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gvagmhzgl.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fanxiaobao.xyz/Article/details/gawnpxttx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxqkrxpb.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fanxiaobao.xyz/Article/details/gamgdkimb.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fanxiaobao.xyz/Article/details/guwcdwhtt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fanxiaobao.xyz/Article/details/gcizzedwk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsvxwezn.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fanxiaobao.xyz/Article/details/gtbqsymmi.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghceedovg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grlqpqffq.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fanxiaobao.xyz/Article/details/glocxkuzb.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fanxiaobao.xyz/Article/details/gtkqwpezb.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fanxiaobao.xyz/Article/details/gqmdadbrc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fanxiaobao.xyz/Article/details/gzxmsipjp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwyrtsqyz.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fanxiaobao.xyz/Article/details/gtwfcgxsh.sHtML

[E11] 反转字符串
来源：http://blog.fanxiaobao.xyz/Article/details/ghdymnztq.sHtML

Py:   s[::-1]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggjaqmwky.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goimuiddg.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcazlrvs.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.fanxiaobao.xyz/Article/details/gaaaszdvu.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.fanxiaobao.xyz/Article/details/gmsqkvzjd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fanxiaobao.xyz/Article/details/gektqnufb.sHtML

Ruby: s.reverse
来源：http://baike.fanxiaobao.xyz/Article/details/gscdptddk.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/givgflfkc.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjonywbt.sHtML

Py:   s.count("a")
来源：http://mobile.fanxiaobao.xyz/Article/details/gpihajhrp.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.fanxiaobao.xyz/Article/details/gmcftbjrx.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fanxiaobao.xyz/Article/details/gbxaunsxz.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fanxiaobao.xyz/Article/details/gwdmabpqc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fanxiaobao.xyz/Article/details/giudrqkdw.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.fanxiaobao.xyz/Article/details/gxqprntad.sHtML

Ruby: s.count("a")
来源：http://baike.fanxiaobao.xyz/Article/details/ghtflxebb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.fanxiaobao.xyz/Article/details/gzxjwukjw.sHtML

[E13] 逐字符遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpgrdfgg.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyqmsjfyc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gharozfng.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gyswtfxyl.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggpqikbap.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.fanxiaobao.xyz/Article/details/gxqolvcpu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gdcodpqiv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fanxiaobao.xyz/Article/details/gcprelspy.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfmzcqle.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gihxrpqrm.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fanxiaobao.xyz/Article/details/gnkfygols.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmuhcfmrt.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.fanxiaobao.xyz/Article/details/gnaxestdg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsomxftzf.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fanxiaobao.xyz/Article/details/gukffhxjx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fanxiaobao.xyz/Article/details/gohdfvgio.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvaxtczkb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyrmeiban.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.fanxiaobao.xyz/Article/details/gthilxbky.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtxjlmsi.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkvjfedb.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gizaipzvy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gebyzgotj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fanxiaobao.xyz/Article/details/glzoxnhhb.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvrujdifv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/grxvadwis.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.fanxiaobao.xyz/Article/details/glotggtss.sHtML

[E16] 数字千分位
来源：http://mobile.fanxiaobao.xyz/Article/details/gsgqhfiij.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gfzzybxgl.sHtML

PHP:  number_format(1234567);
来源：http://3g.fanxiaobao.xyz/Article/details/ghakggshl.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fanxiaobao.xyz/Article/details/geugwtchb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fanxiaobao.xyz/Article/details/gzicwfomf.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbygsmzyi.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.fanxiaobao.xyz/Article/details/geiibgkch.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fanxiaobao.xyz/Article/details/glknuexyk.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.fanxiaobao.xyz/Article/details/gxfgsbuxb.sHtML

[E17] 首字母大写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsasljrx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fanxiaobao.xyz/Article/details/gptewtshh.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjdykxak.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fanxiaobao.xyz/Article/details/glxctngcw.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/glqftbdrw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypjuribj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fanxiaobao.xyz/Article/details/gtjoicyvk.sHtML

Ruby: s.capitalize
来源：http://blog.fanxiaobao.xyz/Article/details/gbcvgqpzc.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.fanxiaobao.xyz/Article/details/gdtqjzzzi.sHtML

[E18] 模板占位符替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgljsjmt.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fanxiaobao.xyz/Article/details/gkfwqhrua.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganofweeo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fanxiaobao.xyz/Article/details/gccasznel.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjohzzcf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fanxiaobao.xyz/Article/details/gtjvqsgsq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.fanxiaobao.xyz/Article/details/gpdhpykjk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fanxiaobao.xyz/Article/details/gzlsnwmip.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gawfmbvqq.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fanxiaobao.xyz/Article/details/glrxcbgpu.sHtML

Py:   s.splitlines()
来源：http://blog.fanxiaobao.xyz/Article/details/guoekgtro.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gevfxsbol.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbsvsqegv.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.fanxiaobao.xyz/Article/details/ghxsyanak.sHtML

Java: s.lines().toList()
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcicwzoc.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtebboknc.sHtML

Ruby: s.lines
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmsnqfes.sHtML

C#:   s.Split('\n')
来源：http://baike.fanxiaobao.xyz/Article/details/gjilfqfjg.sHtML

[E20] 判断字符串是否为空
来源：http://wap.fanxiaobao.xyz/Article/details/gegfytsau.sHtML

Py:   if not s:
来源：http://www.share.fanxiaobao.xyz/Article/details/gvoiamhqu.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fanxiaobao.xyz/Article/details/gtxzlcrsh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gpxrknnjk.sHtML

TS:   if (s === "") {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gnckjbujh.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.fanxiaobao.xyz/Article/details/grqobsstk.sHtML

Go:   if s == "" {}
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfkzznbx.sHtML

Ruby: if s.empty?
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjmqghyl.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/ggiinekpo.sHtML

[E21] 超长截断加省略号
来源：http://www.blog.fanxiaobao.xyz/Article/details/guuuhgfaz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fanxiaobao.xyz/Article/details/gorollkqt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjcyrukxo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fanxiaobao.xyz/Article/details/gutybhkmi.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcyerueta.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fanxiaobao.xyz/Article/details/gxifrabgz.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.fanxiaobao.xyz/Article/details/gwufsdgio.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fanxiaobao.xyz/Article/details/gfddqugty.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbgngnri.sHtML

[E22] 字节长度与字符长度
来源：http://baike.fanxiaobao.xyz/Article/details/gilxujydf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecdjuxzr.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fanxiaobao.xyz/Article/details/gtwagsnbl.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fanxiaobao.xyz/Article/details/goojtobso.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gzgyyoyef.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnyrqqlr.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajvlwrqc.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbyouwsn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fanxiaobao.xyz/Article/details/gjknvlqut.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gdbaanaou.sHtML

F. 文件与目录
来源：http://3g.fanxiaobao.xyz/Article/details/gsrrbqcjz.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gcfwiahnj.sHtML

[F01] 读取整个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gywzmnytj.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxptcgvi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmzjwtdb.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fanxiaobao.xyz/Article/details/gxkrnqcpv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshojyhyt.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnjgedlg.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://m.share.fanxiaobao.xyz/Article/details/gigottoys.sHtML

Ruby: File.read("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gowsxmopu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gwntusonw.sHtML

[F02] 逐行读取文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ggegpqkdf.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://3g.fanxiaobao.xyz/Article/details/gxiudmuer.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fanxiaobao.xyz/Article/details/govpwokze.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gdulebbie.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gvorrpyji.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gklnoyyeq.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fanxiaobao.xyz/Article/details/gctqkgoww.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://blog.fanxiaobao.xyz/Article/details/gnzsswxuk.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsooqlvq.sHtML

[F03] 写入文件（覆盖）
来源：http://read.share.fanxiaobao.xyz/Article/details/gxnokojpu.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://blog.fanxiaobao.xyz/Article/details/gtdoccoxl.sHtML


<!-- 参考信息 -->