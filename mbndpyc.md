代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://wap.fanxiaobao.xyz/Article/details/gffupjjeh.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.fanxiaobao.xyz/Article/details/gcxtwnbko.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemhcnjst.sHtML

TS:   nested.flat();
来源：http://3g.fanxiaobao.xyz/Article/details/gwnbiootj.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://baike.fanxiaobao.xyz/Article/details/gdytegaxb.sHtML

Go:   // 手写双层循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gjezndihq.sHtML

Ruby: nested.flatten
来源：http://m.share.fanxiaobao.xyz/Article/details/gdqjvsykk.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fanxiaobao.xyz/Article/details/gqzneisac.sHtML

[D19] 按字段分组
来源：http://read.share.fanxiaobao.xyz/Article/details/gvffbzayk.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsyxlran.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmdlpmpil.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://3g.fanxiaobao.xyz/Article/details/gdbszqwft.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.fanxiaobao.xyz/Article/details/gokvixbgm.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyqpshefn.sHtML

Go:   // 手写 map[string][]T
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnvfjrtu.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvkqshywk.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://read.share.fanxiaobao.xyz/Article/details/gchcsfnxg.sHtML

[D20] 统计每个元素出现次数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjxxpnhbl.sHtML

Py:   Counter(arr)
来源：http://blog.fanxiaobao.xyz/Article/details/gcejottzt.sHtML

PHP:  array_count_values($arr);
来源：http://3g.fanxiaobao.xyz/Article/details/gilyywoid.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fanxiaobao.xyz/Article/details/gadnfqqsy.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fanxiaobao.xyz/Article/details/ghtqvnrti.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.fanxiaobao.xyz/Article/details/gcugemvxa.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fanxiaobao.xyz/Article/details/gtdgctgcr.sHtML

Ruby: arr.tally
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgjecxre.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://wap.fanxiaobao.xyz/Article/details/gnfflhnby.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.fanxiaobao.xyz/Article/details/grrylfjad.sHtML

Py:   x in arr
来源：http://baike.fanxiaobao.xyz/Article/details/gudztixiw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fanxiaobao.xyz/Article/details/gblmeezqd.sHtML

JS:   arr.includes(x)
来源：http://blog.fanxiaobao.xyz/Article/details/gskvjkryq.sHtML

TS:   arr.includes(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdiisluk.sHtML

Java: list.contains(x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gjstfhakn.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.fanxiaobao.xyz/Article/details/gobemzfgf.sHtML

Ruby: arr.include?(x)
来源：http://wap.fanxiaobao.xyz/Article/details/gippnzdii.sHtML

C#:   list.Contains(x)
来源：http://mobile.fanxiaobao.xyz/Article/details/gerojidyx.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.fanxiaobao.xyz/Article/details/gjyowvxsl.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.fanxiaobao.xyz/Article/details/ghdisgnch.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fanxiaobao.xyz/Article/details/gqenxxhiv.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://wap.fanxiaobao.xyz/Article/details/gqswkobuz.sHtML

TS:   [...arr];
来源：http://baike.fanxiaobao.xyz/Article/details/glnbjcuqm.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fanxiaobao.xyz/Article/details/ganvpndbp.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsaevcyl.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfmzdxrle.sHtML

C#:   new List<int>(list);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqpjsurc.sHtML

[D23] reduce 累积计算
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnjpxfkg.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.fanxiaobao.xyz/Article/details/gbarowblq.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.fanxiaobao.xyz/Article/details/gziswyvpw.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhjnddjz.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxnvecfam.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.fanxiaobao.xyz/Article/details/gvajwlxes.sHtML

Go:   // 手写循环
来源：http://m.share.fanxiaobao.xyz/Article/details/ggwkjweiy.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.fanxiaobao.xyz/Article/details/gozbmubxb.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbwfpjfl.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gslokqzez.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fanxiaobao.xyz/Article/details/gdgjqpixt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvuqllhep.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdxtvbim.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gfighffak.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gifpcjzbr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.fanxiaobao.xyz/Article/details/gixvkljvo.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fanxiaobao.xyz/Article/details/gpwbwtbfb.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fanxiaobao.xyz/Article/details/genvddaqm.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxufcwwki.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrfsrcvl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxiorkxep.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbgtjygx.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvhyqgzd.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/goinbiniw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.fanxiaobao.xyz/Article/details/gtpubsuwl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.fanxiaobao.xyz/Article/details/gvfcpvqvs.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwodkqtkm.sHtML

[D26] 数组转字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gwxujesgb.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghpgoxfex.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvrqsrrs.sHtML

JS:   arr.join(", ")
来源：http://read.share.fanxiaobao.xyz/Article/details/glwvzwvdv.sHtML

TS:   arr.join(", ")
来源：http://wap.fanxiaobao.xyz/Article/details/gqdfgbvkl.sHtML

Java: String.join(", ", list)
来源：http://wap.fanxiaobao.xyz/Article/details/gdnirjivx.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fanxiaobao.xyz/Article/details/grpirxqrd.sHtML

Ruby: arr.join(", ")
来源：http://wap.fanxiaobao.xyz/Article/details/gtojnzbbj.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggblgbczv.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gueakhfuf.sHtML

E. 字符串处理
来源：http://wap.fanxiaobao.xyz/Article/details/gjqxgtbzd.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gakxdrqsm.sHtML

[E01] 拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfslcxtv.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmhifdxy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.fanxiaobao.xyz/Article/details/grpdtkrkp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmspivwqj.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpoxevpxk.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjolfduib.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fanxiaobao.xyz/Article/details/gbohibjzp.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.fanxiaobao.xyz/Article/details/gkrdshvdp.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvezuuip.sHtML

[E02] 重复字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzkwvdeu.sHtML

Py:   "ab" * 3
来源：http://m.share.fanxiaobao.xyz/Article/details/glqnydwgv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnypjlwz.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fanxiaobao.xyz/Article/details/gzpowgrax.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gedvsvwco.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkxglawj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.fanxiaobao.xyz/Article/details/gxxfbcjxa.sHtML

Ruby: "ab" * 3
来源：http://3g.fanxiaobao.xyz/Article/details/gznceovto.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpexldjg.sHtML

[E03] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gugyvqrbg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fanxiaobao.xyz/Article/details/gmyfhxcnq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixwtdudr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gknetaelz.sHtML

TS:   s.slice(1, 4)
来源：http://3g.fanxiaobao.xyz/Article/details/gdytbjfht.sHtML

Java: s.substring(1, 4)
来源：http://baike.fanxiaobao.xyz/Article/details/gnoiixxeq.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fanxiaobao.xyz/Article/details/gxpwemstp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fanxiaobao.xyz/Article/details/gvamdwoaw.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhhjzyvk.sHtML

[E04] 查找子串位置
来源：http://m.share.fanxiaobao.xyz/Article/details/geqbsazis.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.fanxiaobao.xyz/Article/details/gykohgymp.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljzlecxb.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssvazflj.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhfhantx.sHtML

Java: s.indexOf("x")
来源：http://3g.fanxiaobao.xyz/Article/details/gqhjiftun.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fanxiaobao.xyz/Article/details/gwhlmhigu.sHtML

Ruby: s.index("x")
来源：http://baike.fanxiaobao.xyz/Article/details/goobapxsj.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.fanxiaobao.xyz/Article/details/ghepwtrof.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fanxiaobao.xyz/Article/details/gmwinjeqy.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcilcaqd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjkxcnjfw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfmptzpd.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpuozhmtv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.fanxiaobao.xyz/Article/details/glqpfpsdv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gryedbbjd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.fanxiaobao.xyz/Article/details/grjfqiyny.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.fanxiaobao.xyz/Article/details/gafuujptt.sHtML

[E06] 替换子串
来源：http://3g.fanxiaobao.xyz/Article/details/guqsumurp.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gctouceqc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfhxphgz.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gpozrhauz.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fanxiaobao.xyz/Article/details/gopztyorp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrosltnx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhaulukc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fanxiaobao.xyz/Article/details/grvxcnzbq.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gemqnxhos.sHtML

[E07] 按分隔符拆分
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnokfpyz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbxxmlgv.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fanxiaobao.xyz/Article/details/ghafbwwou.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvccnjdcb.sHtML

TS:   s.split(",")
来源：http://m.share.fanxiaobao.xyz/Article/details/gseeoowgx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fanxiaobao.xyz/Article/details/gmnwzzuet.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gslmumptj.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fanxiaobao.xyz/Article/details/gemmvcthl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://blog.fanxiaobao.xyz/Article/details/gtyqvocoo.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrthzdxs.sHtML

Py:   ",".join(items)
来源：http://baike.fanxiaobao.xyz/Article/details/gcjjtsnjc.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fanxiaobao.xyz/Article/details/gartxasbx.sHtML

JS:   items.join(",")
来源：http://mobile.fanxiaobao.xyz/Article/details/gnnjxjwzv.sHtML

TS:   items.join(",")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszcifdrc.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glgxhzfwb.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.fanxiaobao.xyz/Article/details/gzudnvkcp.sHtML

Ruby: items.join(",")
来源：http://read.share.fanxiaobao.xyz/Article/details/grabnifko.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzxxexsn.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fanxiaobao.xyz/Article/details/gxszuxnri.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnuvrhid.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/gmixkaqjw.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.fanxiaobao.xyz/Article/details/giowehtbw.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.fanxiaobao.xyz/Article/details/gwiriefme.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fanxiaobao.xyz/Article/details/gkcftsuay.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.fanxiaobao.xyz/Article/details/guodgseye.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.fanxiaobao.xyz/Article/details/gvqlfikfq.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.fanxiaobao.xyz/Article/details/grsaxftwi.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdgtmiff.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgmprips.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gohvnfdqa.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtssjdbgx.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fanxiaobao.xyz/Article/details/ghaqknzbn.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzeraqga.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjlggjdz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fanxiaobao.xyz/Article/details/gsepavxuu.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fanxiaobao.xyz/Article/details/goaffsmls.sHtML

[E11] 反转字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gqozrhvxc.sHtML

Py:   s[::-1]
来源：http://baike.fanxiaobao.xyz/Article/details/gipzstkdf.sHtML

PHP:  strrev($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gscerskop.sHtML

JS:   [...s].reverse().join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/guscrbofq.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvmawhxs.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fanxiaobao.xyz/Article/details/girixxoho.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fanxiaobao.xyz/Article/details/gerzbcdhx.sHtML

Ruby: s.reverse
来源：http://3g.fanxiaobao.xyz/Article/details/gpoyoetkx.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfoljxkt.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fanxiaobao.xyz/Article/details/gaadnqfsq.sHtML

Py:   s.count("a")
来源：http://m.share.fanxiaobao.xyz/Article/details/gkseyotxm.sHtML

PHP:  substr_count($s, "a");
来源：http://mobile.fanxiaobao.xyz/Article/details/gpuhinuan.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhatbwqg.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.fanxiaobao.xyz/Article/details/glvtebord.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnlosgyf.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fanxiaobao.xyz/Article/details/graebapfv.sHtML

Ruby: s.count("a")
来源：http://blog.fanxiaobao.xyz/Article/details/gcozakyur.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvqhrxpl.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbavjpkk.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fanxiaobao.xyz/Article/details/gncixhgqw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grkalhoft.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdnjxitg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fanxiaobao.xyz/Article/details/gfplqogrj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fanxiaobao.xyz/Article/details/gaxenjkpp.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gpipsuyni.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fanxiaobao.xyz/Article/details/gvbmmjyym.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmhqaiua.sHtML

[E14] URL 编码与 Base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgtkuxhq.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.fanxiaobao.xyz/Article/details/gxmyxnrmv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnbpypaby.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gskeoxsre.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gawslbmcb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fanxiaobao.xyz/Article/details/givbckyez.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fanxiaobao.xyz/Article/details/gmobetvno.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbofleow.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhxqgjgf.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyefnltxp.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjdwzgfyf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrvybogu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gtuxmcxky.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/grmuoonsu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvpivtcq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gdcmjnmfd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfxlnxlm.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqorvhafy.sHtML

[E16] 数字千分位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchywdjur.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gtvvwvusm.sHtML

PHP:  number_format(1234567);
来源：http://3g.fanxiaobao.xyz/Article/details/gxudzcxlk.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbywkwjml.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fanxiaobao.xyz/Article/details/ghjdivcva.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.fanxiaobao.xyz/Article/details/gmvuhpzki.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.fanxiaobao.xyz/Article/details/gonprrigg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fanxiaobao.xyz/Article/details/gnulgorht.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gsspuywrk.sHtML

[E17] 首字母大写
来源：http://www.share.fanxiaobao.xyz/Article/details/gdceshesj.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.fanxiaobao.xyz/Article/details/gocehxsst.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.fanxiaobao.xyz/Article/details/gzawdpafl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fanxiaobao.xyz/Article/details/gqkzjuize.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjdbeayv.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjpslhfsq.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.fanxiaobao.xyz/Article/details/gwzxrsgoh.sHtML

Ruby: s.capitalize
来源：http://wap.fanxiaobao.xyz/Article/details/gsxjxsezl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fanxiaobao.xyz/Article/details/ghoxsqepa.sHtML

[E18] 模板占位符替换
来源：http://read.share.fanxiaobao.xyz/Article/details/grbjsqwqy.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fanxiaobao.xyz/Article/details/gehlvmkmg.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtyhzifa.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.fanxiaobao.xyz/Article/details/gayoluqpe.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fanxiaobao.xyz/Article/details/gshtxqmwv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.fanxiaobao.xyz/Article/details/gkeqtpzxq.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.fanxiaobao.xyz/Article/details/gmcjxqncw.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxixwmeym.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumrumpjw.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fanxiaobao.xyz/Article/details/gjndizkvy.sHtML

Py:   s.splitlines()
来源：http://wap.fanxiaobao.xyz/Article/details/gyrlhfgec.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/glgqgmapo.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcwcxvujm.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.fanxiaobao.xyz/Article/details/gtcinqytc.sHtML

Java: s.lines().toList()
来源：http://blog.fanxiaobao.xyz/Article/details/gjabuktro.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fanxiaobao.xyz/Article/details/gatmrwksg.sHtML

Ruby: s.lines
来源：http://baike.fanxiaobao.xyz/Article/details/gtvtidwms.sHtML

C#:   s.Split('\n')
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqzlcxjg.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlcapfbc.sHtML

Py:   if not s:
来源：http://wap.fanxiaobao.xyz/Article/details/ghlaqozde.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxeulttri.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gqrwacxjc.sHtML

TS:   if (s === "") {}
来源：http://mobile.fanxiaobao.xyz/Article/details/glphvtufu.sHtML

Java: if (s.isEmpty()) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gpknjbhii.sHtML

Go:   if s == "" {}
来源：http://blog.fanxiaobao.xyz/Article/details/giwafaics.sHtML

Ruby: if s.empty?
来源：http://wap.fanxiaobao.xyz/Article/details/gbfnnjngm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fanxiaobao.xyz/Article/details/gnwgneckp.sHtML

[E21] 超长截断加省略号
来源：http://3g.fanxiaobao.xyz/Article/details/gewitplrv.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fanxiaobao.xyz/Article/details/gquwmjvab.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.fanxiaobao.xyz/Article/details/gglgvtdnl.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.fanxiaobao.xyz/Article/details/ggmuqccdb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbptwsrcp.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.fanxiaobao.xyz/Article/details/gsbkdxojg.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fanxiaobao.xyz/Article/details/grjzoiojo.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.fanxiaobao.xyz/Article/details/gukmetswb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyqqrfii.sHtML

[E22] 字节长度与字符长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gcoakobzj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gckwbutft.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fanxiaobao.xyz/Article/details/goqldefix.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fanxiaobao.xyz/Article/details/gkrtcdngc.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfcqeklv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.fanxiaobao.xyz/Article/details/gjmxvhyuy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdykiciye.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmmcxdob.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmsbwzzw.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gdliuriee.sHtML

F. 文件与目录
来源：http://www.share.fanxiaobao.xyz/Article/details/giefaybyj.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvobafsz.sHtML

[F01] 读取整个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gfuahnvsp.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fanxiaobao.xyz/Article/details/gzpjswzky.sHtML

PHP:  file_get_contents("a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gypeelnor.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbvcgqze.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvkekbkm.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gyiesnzav.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbkptjhkb.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gbraquinx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/grxbjkslj.sHtML

[F02] 逐行读取文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gfubptpuo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjafupej.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.fanxiaobao.xyz/Article/details/getuvqofg.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gtqdjabht.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhrsiadu.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fanxiaobao.xyz/Article/details/gdpldghln.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpxjhmjqh.sHtML


<!-- 参考信息 -->