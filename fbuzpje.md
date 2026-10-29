代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.hesvh.cn/Article/details/gmnfhimkg.sHtML

PHP:  array_merge(...$nested);
来源：http://blog.fehbvm.com/Article/details/ghkqtmsfo.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://baike.zdbjq.cn/Article/details/gsumzyfxe.sHtML

TS:   nested.flat();
来源：http://baike.zdbjq.cn/Article/details/giddgfveg.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.zdbjq.cn/Article/details/gfjyilpfj.sHtML

Go:   // 手写双层循环
来源：http://wap.hesvh.cn/Article/details/gpdiohwlr.sHtML

Ruby: nested.flatten
来源：http://mobile.hesvh.cn/Article/details/gcigrnalx.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.m.share.fehbvm.com/Article/details/gyxklpuvq.sHtML

[D19] 按字段分组
来源：http://www.m.share.hesvh.cn/Article/details/grvpquxkn.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fehbvm.com/Article/details/geifshpne.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://mobile.hesvh.cn/Article/details/guqciuvvq.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.zdbjq.cn/Article/details/gurheogeo.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gfsvqmwlf.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gouybqmkb.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.fehbvm.com/Article/details/gawytfdzi.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fehbvm.com/Article/details/glpkikmdh.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.zdbjq.cn/Article/details/gvtounolv.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/gnxckmgbp.sHtML

Py:   Counter(arr)
来源：http://m.share.hesvh.cn/Article/details/gojmhsorw.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.hesvh.cn/Article/details/gmyunlsnt.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gppdpcejc.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gitpufeyg.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.hesvh.cn/Article/details/gbprkqpck.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.hesvh.cn/Article/details/gtkiwpbam.sHtML

Ruby: arr.tally
来源：http://3g.hesvh.cn/Article/details/gdgmsovwd.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.zdbjq.cn/Article/details/gdapsxkba.sHtML

[D21] 判断是否包含某元素
来源：http://blog.zdbjq.cn/Article/details/gcvrsicjl.sHtML

Py:   x in arr
来源：http://www.share.fehbvm.com/Article/details/gbsyaxxjs.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.zdbjq.cn/Article/details/gfqsfkzpj.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gkzezidfk.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/griqgpkgx.sHtML

Java: list.contains(x)
来源：http://www.m.share.fehbvm.com/Article/details/glopvtbuz.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.zdbjq.cn/Article/details/gpnvsgbsh.sHtML

Ruby: arr.include?(x)
来源：http://read.share.zdbjq.cn/Article/details/gauvnbynz.sHtML

C#:   list.Contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/gzrvesocn.sHtML

[D22] 复制数组（避免共享引用）
来源：http://m.share.zdbjq.cn/Article/details/ggabtckma.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/gwjsdcxxr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.zdbjq.cn/Article/details/gjnfqowgw.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.hesvh.cn/Article/details/gxyjzezkt.sHtML

TS:   [...arr];
来源：http://www.blog.hesvh.cn/Article/details/gfcvuomdh.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.zdbjq.cn/Article/details/gymjllpyg.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/gcyyezwej.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/gafqwuanr.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/gomvujdvz.sHtML

[D23] reduce 累积计算
来源：http://www.blog.hesvh.cn/Article/details/gamfsmcrd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://wap.fehbvm.com/Article/details/gwjgxlrav.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.blog.fehbvm.com/Article/details/ggfzqsink.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gsfylunfv.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gftmpdavx.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.zdbjq.cn/Article/details/gfupgkzkb.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gcpmdscrj.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.m.share.fehbvm.com/Article/details/ghsmkpxmb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.zdbjq.cn/Article/details/gltfzaaqk.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.hesvh.cn/Article/details/gzjdvlpgy.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.zdbjq.cn/Article/details/gkjtpynng.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.blog.fehbvm.com/Article/details/gpazchxnn.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.zdbjq.cn/Article/details/gegkpsyie.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gkfsenbgx.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.zdbjq.cn/Article/details/ggibfhmiw.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/gicomhnwc.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.fehbvm.com/Article/details/gdifqazyc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.hesvh.cn/Article/details/gzlhgyzso.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.hesvh.cn/Article/details/gjihjpurk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.fehbvm.com/Article/details/gxohrjtko.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.hesvh.cn/Article/details/gdsaeampe.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.zdbjq.cn/Article/details/gzbjdikal.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fehbvm.com/Article/details/geldxovkq.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.zdbjq.cn/Article/details/gwdqyclei.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fehbvm.com/Article/details/gijyjxbji.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fehbvm.com/Article/details/gbcawzjex.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://blog.fehbvm.com/Article/details/gvtdgdxlf.sHtML

[D26] 数组转字符串
来源：http://baike.hesvh.cn/Article/details/goyuzyyhr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.hesvh.cn/Article/details/gtqoyrcmk.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gpqraxzhn.sHtML

JS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/gksqupxxc.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gcwiskacq.sHtML

Java: String.join(", ", list)
来源：http://blog.zdbjq.cn/Article/details/ggxalkalu.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.zdbjq.cn/Article/details/ghjjgktrf.sHtML

Ruby: arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gznbltnkx.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gwmqbpcub.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gseetwfom.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/gbbivnhiw.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gejxawfjy.sHtML

[E01] 拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/ghfnarriz.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/gubuqcuib.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.hesvh.cn/Article/details/gzhjqautb.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.zdbjq.cn/Article/details/gofivlamo.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gccrhnpzi.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.zdbjq.cn/Article/details/grxoqegin.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fehbvm.com/Article/details/gvkxcqppu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://m.share.fehbvm.com/Article/details/gswaoxvoo.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gpgbtglaw.sHtML

[E02] 重复字符串
来源：http://www.m.share.zdbjq.cn/Article/details/ggcskvmkp.sHtML

Py:   "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gnborjspu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.zdbjq.cn/Article/details/gtnfuvlvd.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gweydecub.sHtML

TS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/grmybahnr.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/gdisclkgu.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.zdbjq.cn/Article/details/gkgbgbcia.sHtML

Ruby: "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/glijrsvgr.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/gvekjnsdq.sHtML

[E03] 截取子串
来源：http://www.share.hesvh.cn/Article/details/ghycbxjln.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.zdbjq.cn/Article/details/grbfhnjzi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gwljsdjfz.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gpfbbvozh.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gmmpzmmgh.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/glysmkalm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.hesvh.cn/Article/details/gdtnsyqvq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.hesvh.cn/Article/details/gpheykeqy.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.hesvh.cn/Article/details/gtnakdgan.sHtML

[E04] 查找子串位置
来源：http://m.share.hesvh.cn/Article/details/gkipdcyhl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gknmlhwgx.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.hesvh.cn/Article/details/gwufsoujp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fehbvm.com/Article/details/gvhbsvdvb.sHtML

TS:   s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/grwtferxc.sHtML

Java: s.indexOf("x")
来源：http://3g.fehbvm.com/Article/details/gehuxarhb.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.hesvh.cn/Article/details/gwowcjeyl.sHtML

Ruby: s.index("x")
来源：http://wap.fehbvm.com/Article/details/grwsrqiev.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fehbvm.com/Article/details/godenywnv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://read.share.hesvh.cn/Article/details/gvqdfxyne.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.zdbjq.cn/Article/details/gqstpilnd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/glarwlpta.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gmuqvafpw.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fehbvm.com/Article/details/glalyjnvs.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/gjicngcyl.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://mobile.hesvh.cn/Article/details/glcsgbvmu.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.hesvh.cn/Article/details/gppfmxuii.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gyvuykqhg.sHtML

[E06] 替换子串
来源：http://wap.hesvh.cn/Article/details/glogdddjg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gcpedyjzu.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/gsosdgfam.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gqszlxewo.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gjxzsycvc.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/guutxdeab.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gdekupsir.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.hesvh.cn/Article/details/glbdebfcg.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gukiwwwpx.sHtML

[E07] 按分隔符拆分
来源：http://mobile.zdbjq.cn/Article/details/gfcsjyujm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fehbvm.com/Article/details/gzozuhobq.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gymnatbfv.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.fehbvm.com/Article/details/gjretselj.sHtML

TS:   s.split(",")
来源：http://blog.fehbvm.com/Article/details/grkwjtigs.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.zdbjq.cn/Article/details/gweosewxa.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.zdbjq.cn/Article/details/grahieymq.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.hesvh.cn/Article/details/glhollqxe.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.zdbjq.cn/Article/details/gjxgremms.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.zdbjq.cn/Article/details/gyuqekbho.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/gbffxpoiw.sHtML

PHP:  implode(",", $items);
来源：http://blog.fehbvm.com/Article/details/gmiygjyfc.sHtML

JS:   items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gpgmftdkr.sHtML

TS:   items.join(",")
来源：http://m.share.hesvh.cn/Article/details/gkxhpmocb.sHtML

Java: String.join(",", items)
来源：http://blog.hesvh.cn/Article/details/gqdtpauwj.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fehbvm.com/Article/details/gwjrpbngt.sHtML

Ruby: items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gpdqnjnrw.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.hesvh.cn/Article/details/gthcwiims.sHtML

[E09] 去除所有空白字符
来源：http://baike.zdbjq.cn/Article/details/ghadugxdd.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.zdbjq.cn/Article/details/gmgwrqppy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.hesvh.cn/Article/details/ggfkkcppa.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gjotwucgx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gyvosrtjv.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://baike.fehbvm.com/Article/details/gmmydlfsz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/gjjzlxoop.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fehbvm.com/Article/details/gewnwyugj.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/ggvynqrlz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.fehbvm.com/Article/details/glmcwuawi.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/ggdyxiunk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.zdbjq.cn/Article/details/gdmdehkwy.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gvvvcaasx.sHtML

TS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/ghbctbnbq.sHtML

Java: String.format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gbmprvscd.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gcnwqgszc.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/ghimygzwy.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fehbvm.com/Article/details/gasakdlbf.sHtML

[E11] 反转字符串
来源：http://read.share.fehbvm.com/Article/details/grzielhtm.sHtML

Py:   s[::-1]
来源：http://www.blog.hesvh.cn/Article/details/gvxqasbfk.sHtML

PHP:  strrev($s);
来源：http://baike.fehbvm.com/Article/details/guajssyyu.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gjohdohxf.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gngfzkdoe.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.hesvh.cn/Article/details/gnqnkiaus.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.hesvh.cn/Article/details/gdrojxfkd.sHtML

Ruby: s.reverse
来源：http://3g.zdbjq.cn/Article/details/gafqtzzbd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.hesvh.cn/Article/details/gmlajqxpq.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.hesvh.cn/Article/details/gaoqbtqqb.sHtML

Py:   s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gtesmvkwp.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fehbvm.com/Article/details/gizygfwxw.sHtML

JS:   s.split("a").length - 1
来源：http://wap.zdbjq.cn/Article/details/ggcpsozpj.sHtML

TS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gofcixhkb.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.zdbjq.cn/Article/details/glnrcpein.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.hesvh.cn/Article/details/gwqqtsizj.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gbgabfnig.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.zdbjq.cn/Article/details/glurgtboh.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/gmdrtmlea.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fehbvm.com/Article/details/ggfqheqzh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.hesvh.cn/Article/details/gxgpqvpse.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gusyfpiel.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/ghdmaltwc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gkycixmap.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.hesvh.cn/Article/details/gvkbxoaol.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://baike.hesvh.cn/Article/details/gngkqttde.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.hesvh.cn/Article/details/gwiblvfsw.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fehbvm.com/Article/details/guzcyjrnr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.hesvh.cn/Article/details/gorskhzbn.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gzgrzaysh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.zdbjq.cn/Article/details/glrmmzehn.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.hesvh.cn/Article/details/ghpxcrksv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.hesvh.cn/Article/details/gktwmslaz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.zdbjq.cn/Article/details/gbrrxktwf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.zdbjq.cn/Article/details/gfwbvprqd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gnboyigbr.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fehbvm.com/Article/details/gstdxliqi.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.hesvh.cn/Article/details/gokmrsqxc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.hesvh.cn/Article/details/gyfjlwmfw.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.zdbjq.cn/Article/details/gyvsqwacl.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.zdbjq.cn/Article/details/gtrslkjgf.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fehbvm.com/Article/details/ghkvmbgcq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.fehbvm.com/Article/details/goowziepk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fehbvm.com/Article/details/gqknoxkzi.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.hesvh.cn/Article/details/gldevtvgp.sHtML

[E16] 数字千分位
来源：http://mobile.fehbvm.com/Article/details/gaaqvfimu.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/ghaoihasz.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/gjpqvwllf.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/gcwqldcar.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gcultatro.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gifbdivkn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.zdbjq.cn/Article/details/gmbscbfjo.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.fehbvm.com/Article/details/gcefqtrdr.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fehbvm.com/Article/details/gwiqgwtec.sHtML

[E17] 首字母大写
来源：http://m.share.fehbvm.com/Article/details/giswzxrvu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/gllzytnof.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.hesvh.cn/Article/details/gjzdmcfng.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.hesvh.cn/Article/details/gsbdqjtfc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/ghobabspd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.zdbjq.cn/Article/details/gugsvefau.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/gzicjqbzu.sHtML

Ruby: s.capitalize
来源：http://3g.fehbvm.com/Article/details/gzvnxrnrk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.fehbvm.com/Article/details/gibvmrlgw.sHtML

[E18] 模板占位符替换
来源：http://www.share.fehbvm.com/Article/details/girnxbnob.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.hesvh.cn/Article/details/gwjcuedjl.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.hesvh.cn/Article/details/gmcnbpdjs.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gsfenlums.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gvjfhafka.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/ginrhozvo.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gntjtcynb.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.zdbjq.cn/Article/details/gktndpwgi.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gkrqgnaob.sHtML

[E19] 多行文本按行拆分
来源：http://3g.hesvh.cn/Article/details/gyqhqmmje.sHtML

Py:   s.splitlines()
来源：http://www.share.fehbvm.com/Article/details/gxreaurfx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gkzeioeei.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/grnqonrhx.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.hesvh.cn/Article/details/gnlpmiyeu.sHtML

Java: s.lines().toList()
来源：http://www.share.hesvh.cn/Article/details/gwsuejyhj.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/grafgvsvm.sHtML

Ruby: s.lines
来源：http://www.m.share.zdbjq.cn/Article/details/ghykngzss.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/gsdehlpfx.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fehbvm.com/Article/details/gqxuptbvn.sHtML

Py:   if not s:
来源：http://www.m.share.fehbvm.com/Article/details/glszxczmk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fehbvm.com/Article/details/gplcizjnr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.hesvh.cn/Article/details/gaucfuals.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.hesvh.cn/Article/details/gahttvtvy.sHtML

Java: if (s.isEmpty()) {}
来源：http://blog.hesvh.cn/Article/details/gtskbmlpn.sHtML

Go:   if s == "" {}
来源：http://read.share.zdbjq.cn/Article/details/gutvflbvm.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/gysbawbmb.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fehbvm.com/Article/details/gkvujnjyu.sHtML

[E21] 超长截断加省略号
来源：http://mobile.zdbjq.cn/Article/details/gywzessmk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.hesvh.cn/Article/details/goiulyism.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gbjbupyxr.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/ghjshsjif.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gyjwtlunb.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gywizdhhy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/gajewqeev.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gvxksvswa.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gihodenij.sHtML

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/gkpeinove.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fehbvm.com/Article/details/gjrczemai.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gounwbqig.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gsdbqixzc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gzjhuetdz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/gybyzzkat.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.hesvh.cn/Article/details/ggffigili.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.zdbjq.cn/Article/details/galxyload.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/grrobciuw.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/grmuzkwjo.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/gedykjfjy.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjifhgivk.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fehbvm.com/Article/details/gqmoaclmh.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fehbvm.com/Article/details/gmbbjivol.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gmqfwsqgp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fehbvm.com/Article/details/gfgeurttv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.fehbvm.com/Article/details/gevtykwav.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://wap.zdbjq.cn/Article/details/gyjsgevyo.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.hesvh.cn/Article/details/gbzyegtzj.sHtML

Ruby: File.read("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gljsvsnie.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.hesvh.cn/Article/details/gtycblvmx.sHtML

[F02] 逐行读取文件
来源：http://baike.zdbjq.cn/Article/details/gmnxkmxko.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fehbvm.com/Article/details/gzgyffaix.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.zdbjq.cn/Article/details/gcdwlhzdo.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/ghaojsiii.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/ghzketosq.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gdylylgyk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://read.share.fehbvm.com/Article/details/gljmckbvb.sHtML


<!-- 参考信息 -->