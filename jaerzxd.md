代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://m.share.hesvh.cn/Article/details/gioxaqmtx.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://blog.zdbjq.cn/Article/details/gzvzvwrrv.sHtML

TS:   Math.max(...arr);
来源：http://wap.zdbjq.cn/Article/details/geiwlvrkh.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://baike.fehbvm.com/Article/details/gwnxqjrqi.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.fehbvm.com/Article/details/gaffiptph.sHtML

Ruby: arr.max;  arr.min
来源：http://blog.hesvh.cn/Article/details/geozylgfp.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fehbvm.com/Article/details/gjnlnzsnb.sHtML

[D18] 扁平化嵌套数组
来源：http://blog.fehbvm.com/Article/details/gzzuhwfcm.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.hesvh.cn/Article/details/gcnhfsqbl.sHtML

PHP:  array_merge(...$nested);
来源：http://3g.fehbvm.com/Article/details/gdhapjumg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.hesvh.cn/Article/details/gbxvzayrs.sHtML

TS:   nested.flat();
来源：http://mobile.fehbvm.com/Article/details/gmexyncxv.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.hesvh.cn/Article/details/gbnkqrfkp.sHtML

Go:   // 手写双层循环
来源：http://mobile.fehbvm.com/Article/details/goqitcmyf.sHtML

Ruby: nested.flatten
来源：http://wap.hesvh.cn/Article/details/goksreost.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.hesvh.cn/Article/details/gchbreyil.sHtML

[D19] 按字段分组
来源：http://wap.zdbjq.cn/Article/details/gtapavsll.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fehbvm.com/Article/details/gkdjeajdn.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://3g.zdbjq.cn/Article/details/gqqzcfdmm.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.zdbjq.cn/Article/details/gpfdetpmr.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/glupruauv.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.fehbvm.com/Article/details/gvybikvwl.sHtML

Go:   // 手写 map[string][]T
来源：http://www.m.share.hesvh.cn/Article/details/gcbmhbcdf.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.share.zdbjq.cn/Article/details/gpljannsn.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.fehbvm.com/Article/details/gblsxxdgy.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.hesvh.cn/Article/details/gzqeuqdsn.sHtML

Py:   Counter(arr)
来源：http://baike.hesvh.cn/Article/details/gloqsijgf.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/gjqwxqfoq.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gxhrcceaj.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gqhsdsays.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.hesvh.cn/Article/details/gxcogopyh.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.hesvh.cn/Article/details/gaaujxldt.sHtML

Ruby: arr.tally
来源：http://mobile.zdbjq.cn/Article/details/gdxnoelvm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.zdbjq.cn/Article/details/gkdbcojew.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.fehbvm.com/Article/details/gsnxtspxp.sHtML

Py:   x in arr
来源：http://www.blog.hesvh.cn/Article/details/gyxpfpxsw.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.hesvh.cn/Article/details/grhpvuqyt.sHtML

JS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gabrybwpk.sHtML

TS:   arr.includes(x)
来源：http://www.blog.hesvh.cn/Article/details/gzzjejyyp.sHtML

Java: list.contains(x)
来源：http://baike.zdbjq.cn/Article/details/gehhfpzbn.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.hesvh.cn/Article/details/gqrpmecvu.sHtML

Ruby: arr.include?(x)
来源：http://read.share.hesvh.cn/Article/details/gnhmfggrm.sHtML

C#:   list.Contains(x)
来源：http://blog.hesvh.cn/Article/details/gmfuhfaxg.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.fehbvm.com/Article/details/gjvbxxksh.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/gqtttiurj.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/gdlsoovur.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.hesvh.cn/Article/details/ggnrpnocj.sHtML

TS:   [...arr];
来源：http://www.m.share.zdbjq.cn/Article/details/gscgyyhno.sHtML

Java: new ArrayList<>(list);
来源：http://blog.fehbvm.com/Article/details/gdgcvkptv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fehbvm.com/Article/details/gnltzaxzu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/gkupueqbr.sHtML

C#:   new List<int>(list);
来源：http://www.share.hesvh.cn/Article/details/grrvutjvg.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/gxmuxobmb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/gjlfyojgg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.share.hesvh.cn/Article/details/ggghzazls.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/gyoiwyqry.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gktzkkfpw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.hesvh.cn/Article/details/gkpzaapzp.sHtML

Go:   // 手写循环
来源：http://wap.fehbvm.com/Article/details/gynpznkfq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.hesvh.cn/Article/details/gsgrvmfxn.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://blog.fehbvm.com/Article/details/gvpwjeexe.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.hesvh.cn/Article/details/gmdukpgps.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.fehbvm.com/Article/details/glinlvbxy.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.zdbjq.cn/Article/details/guvzyevdh.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.zdbjq.cn/Article/details/gingwyxrg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gmdznghfs.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.fehbvm.com/Article/details/gbfkavxcs.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://m.share.fehbvm.com/Article/details/gsfffsyra.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.zdbjq.cn/Article/details/goeapdzbr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://m.share.hesvh.cn/Article/details/gzbrjlbnk.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/gostnkqic.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://read.share.fehbvm.com/Article/details/gmstyrcyq.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://read.share.fehbvm.com/Article/details/gyfznppan.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/gtyxeoiqo.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.m.share.fehbvm.com/Article/details/gajvclttz.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.zdbjq.cn/Article/details/gjktpskbo.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/gonofhuiw.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://mobile.zdbjq.cn/Article/details/gxwotwchb.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.hesvh.cn/Article/details/grmofhwia.sHtML

[D26] 数组转字符串
来源：http://blog.fehbvm.com/Article/details/gfggvmkte.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.share.fehbvm.com/Article/details/glcxbrutl.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.fehbvm.com/Article/details/gsegtnwpf.sHtML

JS:   arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/gegvfzixx.sHtML

TS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gmknvxixn.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.hesvh.cn/Article/details/gjqoicfpz.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.share.zdbjq.cn/Article/details/ghabeoauu.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gbwkvbdmn.sHtML

C#:   string.Join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gekvidutc.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gdctkxsyd.sHtML

E. 字符串处理
来源：http://m.share.fehbvm.com/Article/details/gabqcdcbk.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/goidarmwk.sHtML

[E01] 拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gtfiqmath.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/gkbwlvtlj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.zdbjq.cn/Article/details/gopdxqgmo.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gngzrrvfn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gnjiyeygn.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.zdbjq.cn/Article/details/gkvrxsmma.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fehbvm.com/Article/details/gkxnxahcu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.fehbvm.com/Article/details/gzpxqduak.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.hesvh.cn/Article/details/gaaemviqh.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/galehuwzp.sHtML

Py:   "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gziqkrurr.sHtML

PHP:  str_repeat("ab", 3);
来源：http://3g.zdbjq.cn/Article/details/gfuzlhtle.sHtML

JS:   "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gzpufwvnr.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gevrxdsyf.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gjowrcyvg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://blog.hesvh.cn/Article/details/gnzekzybc.sHtML

Ruby: "ab" * 3
来源：http://www.share.fehbvm.com/Article/details/gecppxrpw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.hesvh.cn/Article/details/gjoopzjed.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gunqyyxsv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.zdbjq.cn/Article/details/gbgngqbcg.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gprsxujau.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gynfkruog.sHtML

TS:   s.slice(1, 4)
来源：http://blog.fehbvm.com/Article/details/gwarhmydg.sHtML

Java: s.substring(1, 4)
来源：http://www.share.hesvh.cn/Article/details/gccbflafe.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/gaqupnhvi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.share.fehbvm.com/Article/details/ghscrefkg.sHtML

C#:   s.Substring(1, 3)
来源：http://baike.zdbjq.cn/Article/details/gxehfpziv.sHtML

[E04] 查找子串位置
来源：http://3g.hesvh.cn/Article/details/glwjksdnz.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.fehbvm.com/Article/details/gcrgjzoic.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.zdbjq.cn/Article/details/gamccquns.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.zdbjq.cn/Article/details/ghruepvla.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gkjamyadl.sHtML

Java: s.indexOf("x")
来源：http://www.share.hesvh.cn/Article/details/gsxlszsyv.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.hesvh.cn/Article/details/gvevayvou.sHtML

Ruby: s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gzoqgxedg.sHtML

C#:   s.IndexOf("x")
来源：http://mobile.hesvh.cn/Article/details/gjdeqmygb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.zdbjq.cn/Article/details/giurnynkm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.hesvh.cn/Article/details/gfdnzazvt.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.fehbvm.com/Article/details/gwvdggmfi.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fehbvm.com/Article/details/gngyeopnr.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.zdbjq.cn/Article/details/gugbswggr.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gcttliptx.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fehbvm.com/Article/details/gykvasahd.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.hesvh.cn/Article/details/gaydxfylz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gquembdlm.sHtML

[E06] 替换子串
来源：http://3g.hesvh.cn/Article/details/glkspqepb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gqvynrkfc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.fehbvm.com/Article/details/gcvffyuat.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.zdbjq.cn/Article/details/gwxczrmqt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/gfupsfkyr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gjssqsekk.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gfrknhshq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.zdbjq.cn/Article/details/grxyvanpy.sHtML

C#:   s.Replace("a", "b")
来源：http://3g.fehbvm.com/Article/details/gbweftlyi.sHtML

[E07] 按分隔符拆分
来源：http://baike.hesvh.cn/Article/details/gthkjojih.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.zdbjq.cn/Article/details/gnbpipuvp.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.fehbvm.com/Article/details/gwnpxnnpa.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fehbvm.com/Article/details/gbioaepzu.sHtML

TS:   s.split(",")
来源：http://blog.fehbvm.com/Article/details/gzhdpnhom.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/gtfosauxm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.hesvh.cn/Article/details/gneecbbep.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.hesvh.cn/Article/details/gepalvlcm.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.zdbjq.cn/Article/details/gqfrwqtie.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.hesvh.cn/Article/details/geshnwyie.sHtML

Py:   ",".join(items)
来源：http://blog.fehbvm.com/Article/details/gjbmjfdta.sHtML

PHP:  implode(",", $items);
来源：http://www.share.zdbjq.cn/Article/details/gxgtptxlm.sHtML

JS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/gfnudfeeq.sHtML

TS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/ggczggmdh.sHtML

Java: String.join(",", items)
来源：http://www.m.share.zdbjq.cn/Article/details/gzjizsdhm.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.zdbjq.cn/Article/details/goyfzjqgi.sHtML

Ruby: items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gesqxsljz.sHtML

C#:   string.Join(",", items)
来源：http://3g.fehbvm.com/Article/details/gcrtqseqy.sHtML

[E09] 去除所有空白字符
来源：http://baike.hesvh.cn/Article/details/ggucjmhti.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fehbvm.com/Article/details/gquwqgkus.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fehbvm.com/Article/details/gdxbffnbd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.fehbvm.com/Article/details/gntbrkxgr.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/gkossdfti.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/gqygivzpp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.hesvh.cn/Article/details/gugoqmddq.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.fehbvm.com/Article/details/gfmhiycdo.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fehbvm.com/Article/details/gaoifsort.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.zdbjq.cn/Article/details/gxgyooqpb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gbkdqesdn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.hesvh.cn/Article/details/gjfefrmzs.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/ggoiirklu.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/gffouresw.sHtML

Java: String.format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gbioavusc.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gsjfxlsgb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/geiaksraw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fehbvm.com/Article/details/ggnjinhhh.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/gvjkhdzwe.sHtML

Py:   s[::-1]
来源：http://3g.fehbvm.com/Article/details/gnbiachxg.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/gxmilqrfa.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gtriofuia.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gbcdzbdem.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.blog.hesvh.cn/Article/details/ggshihbrc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gpifkxubr.sHtML

Ruby: s.reverse
来源：http://baike.hesvh.cn/Article/details/glrjsrgqi.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gerhlywnq.sHtML

[E12] 统计某字符出现次数
来源：http://3g.zdbjq.cn/Article/details/gpgqhthrf.sHtML

Py:   s.count("a")
来源：http://mobile.fehbvm.com/Article/details/gzuftmtyk.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gaczvwllk.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gwkhrocar.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/ghxjrexhc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/ghzzauyad.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.fehbvm.com/Article/details/gailyrajr.sHtML

Ruby: s.count("a")
来源：http://blog.hesvh.cn/Article/details/gxlfwlyak.sHtML

C#:   s.Count(c => c == 'a')
来源：http://mobile.hesvh.cn/Article/details/gyyauxrcm.sHtML

[E13] 逐字符遍历
来源：http://read.share.hesvh.cn/Article/details/ggnbmayaz.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.fehbvm.com/Article/details/gkaauwcqy.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.hesvh.cn/Article/details/gomcqygtl.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gcwiabsvd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gsstgrzxy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.zdbjq.cn/Article/details/ghphnwfgw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.fehbvm.com/Article/details/gpfnyxiwc.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fehbvm.com/Article/details/gkgmkglve.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.hesvh.cn/Article/details/grpyeamin.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.zdbjq.cn/Article/details/ghrweuhxa.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.zdbjq.cn/Article/details/gblsvckfd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/gjbqilwiw.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fehbvm.com/Article/details/gafrhducd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.fehbvm.com/Article/details/gagzwtdpn.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fehbvm.com/Article/details/ggohynzqx.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fehbvm.com/Article/details/gukqkpawu.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fehbvm.com/Article/details/ggoqjeroj.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.fehbvm.com/Article/details/gypwjmxyy.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.hesvh.cn/Article/details/geohxnpei.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/gefmleipl.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.hesvh.cn/Article/details/gzyrcitxd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.fehbvm.com/Article/details/gjkgopaxu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.hesvh.cn/Article/details/gyfojqzfv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.hesvh.cn/Article/details/gatmcytfu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.hesvh.cn/Article/details/gyksapndy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/gbqvorrmc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gcdfhvaka.sHtML

[E16] 数字千分位
来源：http://baike.zdbjq.cn/Article/details/gjophlylj.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.zdbjq.cn/Article/details/gwbunsszb.sHtML

PHP:  number_format(1234567);
来源：http://read.share.zdbjq.cn/Article/details/gppdghapt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.hesvh.cn/Article/details/glrpwcjzo.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gzuqexcof.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.zdbjq.cn/Article/details/gtibrubnr.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.hesvh.cn/Article/details/gbdhoeysw.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.hesvh.cn/Article/details/ggabaauym.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.hesvh.cn/Article/details/gzjakhbei.sHtML

[E17] 首字母大写
来源：http://3g.hesvh.cn/Article/details/ggkfodwrx.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.share.hesvh.cn/Article/details/ggfdmrxao.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.hesvh.cn/Article/details/gijalosmo.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gmgfoyvse.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gmoqhzzit.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.zdbjq.cn/Article/details/gvtfzlysw.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.zdbjq.cn/Article/details/gkjzxkjad.sHtML

Ruby: s.capitalize
来源：http://blog.fehbvm.com/Article/details/gdxzwsyka.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.hesvh.cn/Article/details/gayckqbmv.sHtML

[E18] 模板占位符替换
来源：http://m.share.fehbvm.com/Article/details/gbaacmjbl.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.zdbjq.cn/Article/details/ggjmvydmn.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://mobile.hesvh.cn/Article/details/gqznahvsp.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gxgbddxkf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/goarqygvy.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gmwqkjubw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/geipvhlds.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/giuerpkdq.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.hesvh.cn/Article/details/gstemidwr.sHtML

[E19] 多行文本按行拆分
来源：http://blog.hesvh.cn/Article/details/glrqonlpc.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/glzjjbqsl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gqcdpepqn.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gzvrpzpci.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gfaamzcdl.sHtML

Java: s.lines().toList()
来源：http://m.share.fehbvm.com/Article/details/gmvibtxil.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.share.zdbjq.cn/Article/details/goycslsdo.sHtML

Ruby: s.lines
来源：http://baike.hesvh.cn/Article/details/gyoscchqy.sHtML

C#:   s.Split('\n')
来源：http://baike.hesvh.cn/Article/details/gmoezyayg.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fehbvm.com/Article/details/gmfhjvybg.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/gujdbemsf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.hesvh.cn/Article/details/gzickiuwq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fehbvm.com/Article/details/giloyyktg.sHtML

TS:   if (s === "") {}
来源：http://www.blog.zdbjq.cn/Article/details/gauffegba.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gplgnbjcc.sHtML

Go:   if s == "" {}
来源：http://www.blog.fehbvm.com/Article/details/ggpoeclos.sHtML

Ruby: if s.empty?
来源：http://blog.zdbjq.cn/Article/details/gwkgqxnrp.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://wap.zdbjq.cn/Article/details/gkimoqtxq.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fehbvm.com/Article/details/gzxqauyjc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fehbvm.com/Article/details/gskzljozd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gcvdqusls.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/ghsvugsbl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gdnqvlvcm.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gelnpdqkq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fehbvm.com/Article/details/gulplziyx.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gkhdfwguv.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gsuubdpfu.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.zdbjq.cn/Article/details/goyegbvzc.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/gervefvlf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gemtojfob.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/glmvskkid.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/goeloegpo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gnpvwqjjz.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fehbvm.com/Article/details/gujdlmnrb.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.hesvh.cn/Article/details/gpjtwdrmy.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://mobile.hesvh.cn/Article/details/gyujwdhos.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/glptberkc.sHtML

F. 文件与目录
来源：http://www.m.share.hesvh.cn/Article/details/gnapyjvzp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvaqvxdnh.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fehbvm.com/Article/details/gyyqkezth.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.zdbjq.cn/Article/details/gvtsenkch.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.hesvh.cn/Article/details/geguudfpr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://3g.hesvh.cn/Article/details/gcvumatai.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gcytyvuep.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gjavudokr.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.fehbvm.com/Article/details/gfdzwwvcx.sHtML

Ruby: File.read("a.txt")
来源：http://3g.fehbvm.com/Article/details/gtwnnzasz.sHtML


<!-- 参考信息 -->