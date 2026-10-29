代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://mobile.fehbvm.com/Article/details/gukudaopn.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.hesvh.cn/Article/details/gtpfytxgg.sHtML

[D17] 最大值与最小值
来源：http://3g.zdbjq.cn/Article/details/gfjipdbhi.sHtML

Py:   max(arr);  min(arr)
来源：http://www.blog.fehbvm.com/Article/details/gefzfvvpl.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.blog.hesvh.cn/Article/details/gzpafmylr.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://wap.fehbvm.com/Article/details/ghdfkjhop.sHtML

TS:   Math.max(...arr);
来源：http://m.share.hesvh.cn/Article/details/gskwpjdmw.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.hesvh.cn/Article/details/grlyeeysp.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gqninlapq.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.zdbjq.cn/Article/details/gthijlfmb.sHtML

C#:   list.Max();  list.Min()
来源：http://wap.fehbvm.com/Article/details/gkgirbhdu.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.fehbvm.com/Article/details/goeafuuvc.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.zdbjq.cn/Article/details/gkledvzts.sHtML

PHP:  array_merge(...$nested);
来源：http://www.blog.zdbjq.cn/Article/details/gmscyjrns.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/grydipsoc.sHtML

TS:   nested.flat();
来源：http://www.m.share.fehbvm.com/Article/details/gueqavixz.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/gsyrgfytl.sHtML

Go:   // 手写双层循环
来源：http://www.share.hesvh.cn/Article/details/grgdkrwms.sHtML

Ruby: nested.flatten
来源：http://wap.zdbjq.cn/Article/details/gbsyeqigw.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/gjhmpstyo.sHtML

[D19] 按字段分组
来源：http://baike.zdbjq.cn/Article/details/grktmqtvj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://m.share.fehbvm.com/Article/details/gkrgydtlj.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.fehbvm.com/Article/details/geoliaibx.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.hesvh.cn/Article/details/gxdzaxauk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gyadaphis.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.hesvh.cn/Article/details/gxuwrgcay.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.fehbvm.com/Article/details/gsbsdqwea.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.hesvh.cn/Article/details/gewoiysco.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.hesvh.cn/Article/details/gvaoqxxmw.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/gcaghczel.sHtML

Py:   Counter(arr)
来源：http://www.share.hesvh.cn/Article/details/gnnzvdfyl.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.fehbvm.com/Article/details/glvavqped.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.hesvh.cn/Article/details/gwmkhyija.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.hesvh.cn/Article/details/gggoeoaea.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fehbvm.com/Article/details/gbxbjfaiq.sHtML

Go:   // 手写 map[T]int
来源：http://wap.fehbvm.com/Article/details/grlzkjmee.sHtML

Ruby: arr.tally
来源：http://m.share.hesvh.cn/Article/details/gbpnjrben.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.fehbvm.com/Article/details/gkujckabq.sHtML

[D21] 判断是否包含某元素
来源：http://mobile.fehbvm.com/Article/details/gglbpxyze.sHtML

Py:   x in arr
来源：http://blog.fehbvm.com/Article/details/gtbjxznkt.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fehbvm.com/Article/details/gejvekujf.sHtML

JS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/gagmrqtfc.sHtML

TS:   arr.includes(x)
来源：http://www.m.share.zdbjq.cn/Article/details/gccosvpzd.sHtML

Java: list.contains(x)
来源：http://blog.fehbvm.com/Article/details/givoiaxhv.sHtML

Go:   slices.Contains(arr, x)
来源：http://m.share.zdbjq.cn/Article/details/gmwlxjqjg.sHtML

Ruby: arr.include?(x)
来源：http://baike.hesvh.cn/Article/details/gvefczzvh.sHtML

C#:   list.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/guekkuxbr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.fehbvm.com/Article/details/giujakwsi.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/gvdhiznmt.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/gaxqiyday.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.hesvh.cn/Article/details/gcbtdhwvz.sHtML

TS:   [...arr];
来源：http://m.share.fehbvm.com/Article/details/gyvxmyyke.sHtML

Java: new ArrayList<>(list);
来源：http://wap.zdbjq.cn/Article/details/gsltewcip.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.hesvh.cn/Article/details/gnghmcstj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.fehbvm.com/Article/details/gqkhztgtm.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gbfffaiyo.sHtML

[D23] reduce 累积计算
来源：http://www.share.zdbjq.cn/Article/details/gvhvxwvrt.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://read.share.hesvh.cn/Article/details/gzrdblwfb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://read.share.hesvh.cn/Article/details/gxvtniute.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://wap.hesvh.cn/Article/details/gfsguunkl.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.hesvh.cn/Article/details/gnefwihrd.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://baike.zdbjq.cn/Article/details/gfbmjufkt.sHtML

Go:   // 手写循环
来源：http://blog.fehbvm.com/Article/details/ggovnbcnf.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.zdbjq.cn/Article/details/grngckwjt.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.zdbjq.cn/Article/details/genepkzdx.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fehbvm.com/Article/details/glclmfqtd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.hesvh.cn/Article/details/gijjgbqma.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.zdbjq.cn/Article/details/gbpbzpwcv.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.hesvh.cn/Article/details/gvpsvbxzx.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gabipfyeu.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.fehbvm.com/Article/details/gdawhdlbx.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.blog.fehbvm.com/Article/details/ggtdanbdq.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fehbvm.com/Article/details/gfemnptwd.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.zdbjq.cn/Article/details/gxbkbsdfq.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.zdbjq.cn/Article/details/ghtthqzhk.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.zdbjq.cn/Article/details/gtopppjjc.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.zdbjq.cn/Article/details/gxfvkdwfp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.hesvh.cn/Article/details/ggknjtvnh.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.fehbvm.com/Article/details/geyjkvodg.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/gugdpkjsg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.zdbjq.cn/Article/details/gyytptkil.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.fehbvm.com/Article/details/gbsponiyg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.fehbvm.com/Article/details/goknjdjnr.sHtML

[D26] 数组转字符串
来源：http://read.share.zdbjq.cn/Article/details/gmuyfxdmk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.hesvh.cn/Article/details/gpymxfhdo.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gbdbqblug.sHtML

JS:   arr.join(", ")
来源：http://www.share.fehbvm.com/Article/details/gxxbpepmz.sHtML

TS:   arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/ganmgmmtp.sHtML

Java: String.join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gzdgsmkly.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.hesvh.cn/Article/details/gydvynkfr.sHtML

Ruby: arr.join(", ")
来源：http://blog.fehbvm.com/Article/details/gffcneakn.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gtiqxqkcj.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gfgccmdee.sHtML

E. 字符串处理
来源：http://m.share.zdbjq.cn/Article/details/grpdnhxus.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gqyyavqwr.sHtML

[E01] 拼接字符串
来源：http://blog.fehbvm.com/Article/details/gsticydor.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.fehbvm.com/Article/details/gpgzudjfo.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.fehbvm.com/Article/details/gicalvovv.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gkyaegnpk.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.fehbvm.com/Article/details/gnnnbmqqy.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.m.share.zdbjq.cn/Article/details/gxyeeeenq.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://3g.fehbvm.com/Article/details/gnosduaak.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.hesvh.cn/Article/details/gerrmaety.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gzlvjxylm.sHtML

[E02] 重复字符串
来源：http://www.share.fehbvm.com/Article/details/glpresphl.sHtML

Py:   "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gzweikrpb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.hesvh.cn/Article/details/geduszbud.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/gmziipcax.sHtML

TS:   "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gbshpncrn.sHtML

Java: "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gwauuuyda.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.fehbvm.com/Article/details/gginkmxvw.sHtML

Ruby: "ab" * 3
来源：http://wap.fehbvm.com/Article/details/gbmkpzobv.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.hesvh.cn/Article/details/gradejkzz.sHtML

[E03] 截取子串
来源：http://3g.fehbvm.com/Article/details/gkvcposyj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.fehbvm.com/Article/details/gmgdchxuw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/grrbcngnl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://3g.zdbjq.cn/Article/details/gurdtruhm.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gdvqbayjv.sHtML

Java: s.substring(1, 4)
来源：http://www.share.fehbvm.com/Article/details/glmxxobza.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gxetyiwyv.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.zdbjq.cn/Article/details/glxoyfdmd.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.zdbjq.cn/Article/details/gvcvwhbvf.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/gwjrbbfxt.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gqrbwataw.sHtML

PHP:  strpos($s, "x");
来源：http://3g.hesvh.cn/Article/details/gsgkhqbwx.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/gnynzmywm.sHtML

TS:   s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gyhysocqn.sHtML

Java: s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gxcbgamrk.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/gqfaowlok.sHtML

Ruby: s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gvexuzazt.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/guwgdahou.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.hesvh.cn/Article/details/gbryoamtf.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.zdbjq.cn/Article/details/gmyjozivl.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/gpjfhaiia.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gnhenreic.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.zdbjq.cn/Article/details/gxhcokrio.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gdevwxbig.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.zdbjq.cn/Article/details/grmionxfg.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.hesvh.cn/Article/details/gxhrcvmyi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fehbvm.com/Article/details/gdpmxnmpe.sHtML

[E06] 替换子串
来源：http://m.share.fehbvm.com/Article/details/gwbxltsya.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gzxpkirhy.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.fehbvm.com/Article/details/gebtanxct.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gezdlvjny.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gwxxubows.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.zdbjq.cn/Article/details/gvbqxubym.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gyhnbrdru.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.fehbvm.com/Article/details/gfgxvulwr.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gqlgmfilr.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fehbvm.com/Article/details/gsgktecbw.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.hesvh.cn/Article/details/gqwvrxpfs.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://mobile.hesvh.cn/Article/details/gwxpcsbrp.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://blog.zdbjq.cn/Article/details/goxxbybzl.sHtML

TS:   s.split(",")
来源：http://3g.zdbjq.cn/Article/details/goxtrkuwj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.zdbjq.cn/Article/details/gnapucdzi.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.zdbjq.cn/Article/details/gswuhrtez.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.hesvh.cn/Article/details/glirjgtqz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.hesvh.cn/Article/details/gjikmbwbq.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.zdbjq.cn/Article/details/gldqsbeok.sHtML

Py:   ",".join(items)
来源：http://3g.zdbjq.cn/Article/details/gueyznjxk.sHtML

PHP:  implode(",", $items);
来源：http://3g.hesvh.cn/Article/details/gpoygdkck.sHtML

JS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/giluajtlm.sHtML

TS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/ghbbnjxft.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gxyyjwrnc.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.zdbjq.cn/Article/details/gyfveecxo.sHtML

Ruby: items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gbjvutsmh.sHtML

C#:   string.Join(",", items)
来源：http://blog.fehbvm.com/Article/details/gzyucnuns.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fehbvm.com/Article/details/gmagxzcwg.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.zdbjq.cn/Article/details/gmyjzavjn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.zdbjq.cn/Article/details/gpbdrzpob.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gfcxjbvrh.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gfgljfmrc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/gjukgqhtd.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fehbvm.com/Article/details/gfovjjvvm.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/gzgxyajqo.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.m.share.fehbvm.com/Article/details/ggcosbdys.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.zdbjq.cn/Article/details/gjkpflwoz.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fehbvm.com/Article/details/gyhsfrcpa.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.hesvh.cn/Article/details/ggiaolgmh.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gpjxqlihd.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fehbvm.com/Article/details/gimzkrpeb.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/ggsixorze.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gzekfdjer.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gixpmdvbq.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fehbvm.com/Article/details/gecddqqhp.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/gsaffgjao.sHtML

Py:   s[::-1]
来源：http://blog.fehbvm.com/Article/details/grvdagdnq.sHtML

PHP:  strrev($s);
来源：http://read.share.zdbjq.cn/Article/details/gezseixtr.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gvtljvsrq.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gwottbeua.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.hesvh.cn/Article/details/grdeoxklv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/gtvftwhpz.sHtML

Ruby: s.reverse
来源：http://www.blog.zdbjq.cn/Article/details/gfgvbvtpd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.zdbjq.cn/Article/details/giavvrjki.sHtML

[E12] 统计某字符出现次数
来源：http://www.m.share.hesvh.cn/Article/details/gdbyjzlnv.sHtML

Py:   s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gvivuxynu.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.hesvh.cn/Article/details/gdkudbere.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.fehbvm.com/Article/details/gsztmjanx.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gbwargtrj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/gigjjdytq.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.fehbvm.com/Article/details/gqzuvssip.sHtML

Ruby: s.count("a")
来源：http://blog.hesvh.cn/Article/details/gnldaltzt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.zdbjq.cn/Article/details/gstnubyww.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/gscnqsuee.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.hesvh.cn/Article/details/gjzxtyggf.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://wap.hesvh.cn/Article/details/gqhpyuhqa.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gqtxalxjo.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gnftjscgi.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://read.share.fehbvm.com/Article/details/gojtkisrw.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://baike.fehbvm.com/Article/details/gxxpetudg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fehbvm.com/Article/details/gbatrmamn.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.zdbjq.cn/Article/details/gdttgpbvp.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.zdbjq.cn/Article/details/gtqhrofia.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.hesvh.cn/Article/details/gvrlqyias.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/gjvsiskou.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.zdbjq.cn/Article/details/gjxwdsuvs.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.zdbjq.cn/Article/details/ghvfzsvhc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.fehbvm.com/Article/details/gckcppiuf.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.hesvh.cn/Article/details/gpvykboqy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fehbvm.com/Article/details/ghxoxttrn.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.fehbvm.com/Article/details/gkcswmvtq.sHtML

[E15] HTML 转义 / 反转义
来源：http://baike.fehbvm.com/Article/details/gmhnhlglv.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.zdbjq.cn/Article/details/gahtfcrsj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.zdbjq.cn/Article/details/gbgxkrmfj.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.fehbvm.com/Article/details/goxyjymgy.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.zdbjq.cn/Article/details/gdlzahoya.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.hesvh.cn/Article/details/ggltmgqvx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://mobile.zdbjq.cn/Article/details/gjyjmbjoz.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.zdbjq.cn/Article/details/gvimwntpr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.zdbjq.cn/Article/details/gjzzzkbkr.sHtML

[E16] 数字千分位
来源：http://mobile.hesvh.cn/Article/details/geyhxuqju.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.zdbjq.cn/Article/details/gswsxuymc.sHtML

PHP:  number_format(1234567);
来源：http://wap.hesvh.cn/Article/details/gwmptcfax.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gewsknizt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gzsafwdob.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/glwgxhomy.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.hesvh.cn/Article/details/gyymwxier.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gcczcaxhd.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.hesvh.cn/Article/details/gsgwhkskj.sHtML

[E17] 首字母大写
来源：http://www.m.share.hesvh.cn/Article/details/grumgjhcw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.hesvh.cn/Article/details/gpuhkftyp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.zdbjq.cn/Article/details/grrbqkyrx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/galwuplcc.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.zdbjq.cn/Article/details/gkrmtyzfm.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://blog.fehbvm.com/Article/details/gzcszztol.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/gkjktjgdt.sHtML

Ruby: s.capitalize
来源：http://mobile.hesvh.cn/Article/details/gcfcrwfgq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.hesvh.cn/Article/details/gtkdnsieb.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/gdpruupef.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.hesvh.cn/Article/details/gowiaoowm.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.zdbjq.cn/Article/details/gykmhyixh.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gkwinfife.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gsohmoocu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gxyqrvxok.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.hesvh.cn/Article/details/ghmactwgj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.zdbjq.cn/Article/details/gdgwiiwae.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://wap.fehbvm.com/Article/details/gmkgmcexi.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/gdcuxppmn.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/gtvixeann.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.fehbvm.com/Article/details/gagccjrbm.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gqpnofrnd.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gmravwkiy.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/gawbqwmzn.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fehbvm.com/Article/details/gowzaniht.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/gyiassrlf.sHtML

C#:   s.Split('\n')
来源：http://blog.hesvh.cn/Article/details/grlvngscp.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.hesvh.cn/Article/details/gsrlathbi.sHtML

Py:   if not s:
来源：http://3g.fehbvm.com/Article/details/gnkzodjui.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fehbvm.com/Article/details/glxqwvuba.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fehbvm.com/Article/details/gkwnpotih.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.hesvh.cn/Article/details/gfviiursj.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.hesvh.cn/Article/details/gngnxbysj.sHtML

Go:   if s == "" {}
来源：http://www.m.share.fehbvm.com/Article/details/gxhbbjvyh.sHtML

Ruby: if s.empty?
来源：http://m.share.hesvh.cn/Article/details/gcgtfyozi.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/gyfjzvlnk.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fehbvm.com/Article/details/gtuhpciaz.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fehbvm.com/Article/details/gogupbogd.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/ghnzgdtml.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gyoyfviji.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gstyagqwk.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gehndnwyr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/gegthulbv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gnehdyoez.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/giqwjqmfc.sHtML

[E22] 字节长度与字符长度
来源：http://blog.zdbjq.cn/Article/details/ggjzbpmnd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.hesvh.cn/Article/details/gbvhrrrln.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/gvihabqrf.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gvktjkhfv.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fehbvm.com/Article/details/guckqbmow.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.hesvh.cn/Article/details/gdrztjjbj.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fehbvm.com/Article/details/gedpqspse.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.hesvh.cn/Article/details/giyjstdmq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.fehbvm.com/Article/details/gbkqxwbbo.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/geqsrlgrk.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/gtqxzyinn.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gtnbsrkff.sHtML

[F01] 读取整个文件
来源：http://m.share.hesvh.cn/Article/details/gjayjlvph.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.zdbjq.cn/Article/details/gwihriued.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fehbvm.com/Article/details/ghtjnjrnr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.hesvh.cn/Article/details/gvxzhbiiz.sHtML


<!-- 参考信息 -->