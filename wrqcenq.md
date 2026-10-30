代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.blog.zdbjq.cn/Article/details/gqdzvimig.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.fehbvm.com/Article/details/gveiypzbu.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.fehbvm.com/Article/details/gvngivymy.sHtML

TS:   nested.flat();
来源：http://baike.zdbjq.cn/Article/details/ghlnexsvl.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.zdbjq.cn/Article/details/goqmiawll.sHtML

Go:   // 手写双层循环
来源：http://wap.hesvh.cn/Article/details/ghmcztnyq.sHtML

Ruby: nested.flatten
来源：http://baike.fehbvm.com/Article/details/guyrhhdjf.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://mobile.zdbjq.cn/Article/details/gmccdpnzc.sHtML

[D19] 按字段分组
来源：http://www.m.share.zdbjq.cn/Article/details/gfasdppta.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.hesvh.cn/Article/details/gfriqzgpo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.zdbjq.cn/Article/details/gkxmralqn.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/gsdwvbsvx.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://blog.hesvh.cn/Article/details/gsfqxnugw.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.hesvh.cn/Article/details/gbqpywngt.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.hesvh.cn/Article/details/gduyobpev.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://m.share.fehbvm.com/Article/details/gvpyoeixb.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.m.share.fehbvm.com/Article/details/gdpmxwxft.sHtML

[D20] 统计每个元素出现次数
来源：http://blog.fehbvm.com/Article/details/gdtxoqvzc.sHtML

Py:   Counter(arr)
来源：http://blog.hesvh.cn/Article/details/gmvhnzdnc.sHtML

PHP:  array_count_values($arr);
来源：http://wap.hesvh.cn/Article/details/gdzkhngij.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.fehbvm.com/Article/details/giwmhfsbq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/grdetyykf.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.blog.fehbvm.com/Article/details/gkbcfrbaj.sHtML

Go:   // 手写 map[T]int
来源：http://www.m.share.zdbjq.cn/Article/details/ggltjbiwi.sHtML

Ruby: arr.tally
来源：http://wap.zdbjq.cn/Article/details/gmsakueaf.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://mobile.zdbjq.cn/Article/details/gcmdpmfgp.sHtML

[D21] 判断是否包含某元素
来源：http://read.share.zdbjq.cn/Article/details/gxecohhro.sHtML

Py:   x in arr
来源：http://baike.hesvh.cn/Article/details/gukllztzd.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.zdbjq.cn/Article/details/glmgsdlkb.sHtML

JS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/guxiddnnh.sHtML

TS:   arr.includes(x)
来源：http://read.share.zdbjq.cn/Article/details/gftanwfph.sHtML

Java: list.contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gizagmpcn.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.blog.zdbjq.cn/Article/details/goeqvogld.sHtML

Ruby: arr.include?(x)
来源：http://baike.fehbvm.com/Article/details/gmnvdzzue.sHtML

C#:   list.Contains(x)
来源：http://www.share.fehbvm.com/Article/details/giaqqaksw.sHtML

[D22] 复制数组（避免共享引用）
来源：http://blog.hesvh.cn/Article/details/gqwenjydx.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://3g.zdbjq.cn/Article/details/gbnimlrwk.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.share.fehbvm.com/Article/details/gvwvuknbd.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://mobile.hesvh.cn/Article/details/gccsgqagd.sHtML

TS:   [...arr];
来源：http://3g.hesvh.cn/Article/details/gkcmmbutx.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.fehbvm.com/Article/details/gtngqtlwd.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fehbvm.com/Article/details/gvariyljm.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/gjpunakdy.sHtML

C#:   new List<int>(list);
来源：http://read.share.fehbvm.com/Article/details/gqdikxcyy.sHtML

[D23] reduce 累积计算
来源：http://read.share.fehbvm.com/Article/details/gmbvplwzo.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.hesvh.cn/Article/details/gdddgiizg.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://blog.hesvh.cn/Article/details/gszaefist.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.fehbvm.com/Article/details/gerttivza.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gndjdemob.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.zdbjq.cn/Article/details/gztqvcgwc.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gfhcrdntc.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.zdbjq.cn/Article/details/gdoiizkas.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.zdbjq.cn/Article/details/gvcvvsmzt.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.hesvh.cn/Article/details/gvezgfuao.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://wap.hesvh.cn/Article/details/gwqoctuvj.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://read.share.hesvh.cn/Article/details/gdxigbssz.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.zdbjq.cn/Article/details/gsblzhdzg.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://baike.hesvh.cn/Article/details/guuzsizbw.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.zdbjq.cn/Article/details/gmmesnbul.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.fehbvm.com/Article/details/glhzptctr.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fehbvm.com/Article/details/gpvhhwrid.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://mobile.fehbvm.com/Article/details/gmtbdwrck.sHtML

[D25] Set 集合去重与交并差
来源：http://wap.fehbvm.com/Article/details/gbirbvvfr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.hesvh.cn/Article/details/glznjivpk.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.blog.zdbjq.cn/Article/details/gmzwcvzjr.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.hesvh.cn/Article/details/gtcffnftb.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://baike.fehbvm.com/Article/details/gcdkeoyxv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gpepfoejf.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.fehbvm.com/Article/details/gnelekzjd.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.fehbvm.com/Article/details/gusximqgv.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.zdbjq.cn/Article/details/ggsugdbfa.sHtML

[D26] 数组转字符串
来源：http://3g.hesvh.cn/Article/details/gqmkhtkvo.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.fehbvm.com/Article/details/gidpvplmw.sHtML

PHP:  implode(", ", $arr);
来源：http://baike.zdbjq.cn/Article/details/gatqdkffe.sHtML

JS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gwmtxqdez.sHtML

TS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gyqxnrynf.sHtML

Java: String.join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gbdwbsrlk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.hesvh.cn/Article/details/guznfxnqh.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gnfhrmkme.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/gbagmmihw.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/geweervir.sHtML

E. 字符串处理
来源：http://www.blog.fehbvm.com/Article/details/gjiavgqxy.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gkwszjrue.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gxvmnrgyh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.zdbjq.cn/Article/details/gbqtqqrju.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.fehbvm.com/Article/details/gsuhtsmmw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.hesvh.cn/Article/details/glipspmqn.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.zdbjq.cn/Article/details/gaipancuo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fehbvm.com/Article/details/ghomltcuk.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://baike.zdbjq.cn/Article/details/gbuqwbeht.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://3g.fehbvm.com/Article/details/ggbxxsluh.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.hesvh.cn/Article/details/gpxrmrbcs.sHtML

[E02] 重复字符串
来源：http://mobile.hesvh.cn/Article/details/geglruocv.sHtML

Py:   "ab" * 3
来源：http://baike.zdbjq.cn/Article/details/gmvxitdkx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.hesvh.cn/Article/details/gywvyfupl.sHtML

JS:   "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gzqugicav.sHtML

TS:   "ab".repeat(3)
来源：http://m.share.zdbjq.cn/Article/details/gcenizryv.sHtML

Java: "ab".repeat(3)
来源：http://m.share.fehbvm.com/Article/details/glubmyhxn.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.hesvh.cn/Article/details/gfuspjmzu.sHtML

Ruby: "ab" * 3
来源：http://wap.hesvh.cn/Article/details/gfogvdwxu.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.zdbjq.cn/Article/details/gcvqttnim.sHtML

[E03] 截取子串
来源：http://blog.hesvh.cn/Article/details/giurdgoag.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.hesvh.cn/Article/details/gsjjpljlr.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gxyabayzk.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.share.zdbjq.cn/Article/details/gztwbcwmu.sHtML

TS:   s.slice(1, 4)
来源：http://wap.hesvh.cn/Article/details/gppjvrsux.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.fehbvm.com/Article/details/ggiysmdah.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.zdbjq.cn/Article/details/ghhhgilpt.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.zdbjq.cn/Article/details/gevqszerh.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.hesvh.cn/Article/details/glzdblyxl.sHtML

[E04] 查找子串位置
来源：http://baike.fehbvm.com/Article/details/gtiwcoaxr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.fehbvm.com/Article/details/gojdehuep.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.hesvh.cn/Article/details/ggzumekai.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.zdbjq.cn/Article/details/govwjmdpj.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fehbvm.com/Article/details/gqyurbnxc.sHtML

Java: s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gpzfznjkd.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fehbvm.com/Article/details/gaxaziwgu.sHtML

Ruby: s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gvtkxqpfc.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.zdbjq.cn/Article/details/gmjfyddby.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.zdbjq.cn/Article/details/gkjawohfi.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.fehbvm.com/Article/details/gtoettzcq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.zdbjq.cn/Article/details/gpzdmezkr.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gnlgqennk.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fehbvm.com/Article/details/gnkixcldi.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.zdbjq.cn/Article/details/ggochvusg.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.hesvh.cn/Article/details/gpkzfafhi.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://read.share.fehbvm.com/Article/details/gqgbvuuml.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fehbvm.com/Article/details/ghudqcdql.sHtML

[E06] 替换子串
来源：http://wap.fehbvm.com/Article/details/gvquwldob.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gkwpkvkfq.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.fehbvm.com/Article/details/gpsecfhnt.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/giixfkevg.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gbnbebpsv.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gsrpsimnj.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gwtlznuxg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gswiflgvi.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gshfbxrud.sHtML

[E07] 按分隔符拆分
来源：http://m.share.hesvh.cn/Article/details/guvoylyev.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.zdbjq.cn/Article/details/gjiyejxmx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gpsmjprus.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fehbvm.com/Article/details/gqtnmqaob.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/gwnjwbvhm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.hesvh.cn/Article/details/gctkcfivn.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.zdbjq.cn/Article/details/gopxpnqub.sHtML

Ruby: s.split(",");  s.split
来源：http://baike.zdbjq.cn/Article/details/grpkopxua.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://mobile.hesvh.cn/Article/details/gfnonzmzk.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.zdbjq.cn/Article/details/gpiskefgh.sHtML

Py:   ",".join(items)
来源：http://baike.hesvh.cn/Article/details/gsfuxeyyv.sHtML

PHP:  implode(",", $items);
来源：http://3g.zdbjq.cn/Article/details/gvmuaxcvt.sHtML

JS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/ggldnjfyt.sHtML

TS:   items.join(",")
来源：http://3g.fehbvm.com/Article/details/gvftmvcwl.sHtML

Java: String.join(",", items)
来源：http://wap.fehbvm.com/Article/details/gfsdsmaps.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.zdbjq.cn/Article/details/gjkofatqv.sHtML

Ruby: items.join(",")
来源：http://mobile.fehbvm.com/Article/details/ggmledxot.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gldysnzam.sHtML

[E09] 去除所有空白字符
来源：http://3g.hesvh.cn/Article/details/gmincdors.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.blog.zdbjq.cn/Article/details/gitcebjpo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://mobile.fehbvm.com/Article/details/gueosobdt.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gwzawupfl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.zdbjq.cn/Article/details/gnbwyjwlu.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gxbudyttc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://baike.hesvh.cn/Article/details/gtcgnggvd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.zdbjq.cn/Article/details/gcvapyccx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.fehbvm.com/Article/details/gunvaqtmk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.zdbjq.cn/Article/details/gcsqdhqjs.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gtxtbefyp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.hesvh.cn/Article/details/gaxlwnhhf.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gstmdtoof.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gfhkftewm.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/ghtcvqprq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gfitvzmxy.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gzalckgmb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.fehbvm.com/Article/details/guayenzcq.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gehkkezmz.sHtML

Py:   s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gewegpwqg.sHtML

PHP:  strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/gfgnmqvjv.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/gmcattdnq.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gczrbwhqr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.share.fehbvm.com/Article/details/gfburxxfe.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.fehbvm.com/Article/details/gqluvvzum.sHtML

Ruby: s.reverse
来源：http://baike.zdbjq.cn/Article/details/gizjvvtkl.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.hesvh.cn/Article/details/gxqcqnxaf.sHtML

[E12] 统计某字符出现次数
来源：http://wap.fehbvm.com/Article/details/giufumkek.sHtML

Py:   s.count("a")
来源：http://3g.hesvh.cn/Article/details/gccfkeljc.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.fehbvm.com/Article/details/gptzrqdaw.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/ghphxifar.sHtML

TS:   s.split("a").length - 1
来源：http://3g.fehbvm.com/Article/details/gyrwcrbfm.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.hesvh.cn/Article/details/gwisspqnq.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fehbvm.com/Article/details/gsaheunkw.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gzdttxoov.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.zdbjq.cn/Article/details/gpdadggrc.sHtML

[E13] 逐字符遍历
来源：http://www.share.hesvh.cn/Article/details/gieguyrml.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.zdbjq.cn/Article/details/ggggncnmh.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fehbvm.com/Article/details/gsbavltvn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gfasfkagh.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.zdbjq.cn/Article/details/ggnxnfsab.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.hesvh.cn/Article/details/gjluyyfig.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.zdbjq.cn/Article/details/gcfzagduf.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.zdbjq.cn/Article/details/ghaolnlvj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/gwdaxiqqx.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fehbvm.com/Article/details/gwxnxjghv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fehbvm.com/Article/details/gcaisyvho.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.fehbvm.com/Article/details/grxryixbk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.hesvh.cn/Article/details/gcjkmeemj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.zdbjq.cn/Article/details/guweiskaz.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fehbvm.com/Article/details/gxzxquvkd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.hesvh.cn/Article/details/gumjoujvh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.hesvh.cn/Article/details/gvhitssws.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://wap.zdbjq.cn/Article/details/gztiofgyk.sHtML

[E15] HTML 转义 / 反转义
来源：http://blog.fehbvm.com/Article/details/gwxezwzux.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.hesvh.cn/Article/details/gbyrfpzes.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fehbvm.com/Article/details/gbcntjtbx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.fehbvm.com/Article/details/guulplwiu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/guupiixde.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://read.share.fehbvm.com/Article/details/gaxitfxuq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.hesvh.cn/Article/details/gqqoxqesj.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/giffjjshy.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.hesvh.cn/Article/details/gmvpedure.sHtML

[E16] 数字千分位
来源：http://blog.fehbvm.com/Article/details/gaqzrpefh.sHtML

Py:   f"{1234567:,}"
来源：http://3g.zdbjq.cn/Article/details/gzkgjswlf.sHtML

PHP:  number_format(1234567);
来源：http://www.share.zdbjq.cn/Article/details/goxbpmflp.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gzygyhrgv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gchuredkn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.m.share.fehbvm.com/Article/details/glkecfyxl.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/gjqisanqq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.zdbjq.cn/Article/details/gpozsibyc.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.zdbjq.cn/Article/details/gxdrhcnuf.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/gwcffaqyc.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.fehbvm.com/Article/details/gofbdgwgp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/glmsghmzz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gfqfilylh.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.fehbvm.com/Article/details/gkqcvecsy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.zdbjq.cn/Article/details/gpuykmpuj.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.zdbjq.cn/Article/details/gdkvsszth.sHtML

Ruby: s.capitalize
来源：http://www.share.fehbvm.com/Article/details/giycjouol.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.fehbvm.com/Article/details/gdqjzimfa.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.hesvh.cn/Article/details/guszpssob.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.hesvh.cn/Article/details/gchzcknss.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://wap.fehbvm.com/Article/details/gxmdbjjlv.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gnhpcwibp.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gsomhzzzv.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/ggghxanjd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.zdbjq.cn/Article/details/ghmmnzscs.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fehbvm.com/Article/details/gjrvlgccl.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.hesvh.cn/Article/details/ghrlfnmok.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fehbvm.com/Article/details/gyxyalvcy.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/gwekckoxw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gblayquzp.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/ghalpvvvi.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.hesvh.cn/Article/details/gijkjmiit.sHtML

Java: s.lines().toList()
来源：http://m.share.hesvh.cn/Article/details/ghtxhzuco.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.zdbjq.cn/Article/details/gxxxbbzwu.sHtML

Ruby: s.lines
来源：http://m.share.hesvh.cn/Article/details/gzlhmhsxl.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.fehbvm.com/Article/details/getxgxgrw.sHtML

[E20] 判断字符串是否为空
来源：http://wap.zdbjq.cn/Article/details/gaxsaqdcy.sHtML

Py:   if not s:
来源：http://baike.hesvh.cn/Article/details/gjuzqymhq.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/glwxlvwcq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.fehbvm.com/Article/details/gaytncypk.sHtML

TS:   if (s === "") {}
来源：http://m.share.hesvh.cn/Article/details/goyhsqzce.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gwqjlehqh.sHtML

Go:   if s == "" {}
来源：http://blog.zdbjq.cn/Article/details/guibtkvul.sHtML

Ruby: if s.empty?
来源：http://read.share.zdbjq.cn/Article/details/guazbhgth.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fehbvm.com/Article/details/gcxyvnknf.sHtML

[E21] 超长截断加省略号
来源：http://3g.zdbjq.cn/Article/details/ghjgxrubj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.zdbjq.cn/Article/details/guicwrffg.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/glkcpedaa.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gmkwevrqa.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.hesvh.cn/Article/details/goezenlex.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gpevikhsq.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/gdnuzvaio.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gwnarhdsu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gflirbzvt.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.hesvh.cn/Article/details/grbntsodt.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.zdbjq.cn/Article/details/gvjrsassu.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gfzaujare.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/ggzyqdyit.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gpwlctrij.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/gxvekocom.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fehbvm.com/Article/details/gihqdnyec.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.zdbjq.cn/Article/details/gcbrwbhki.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fehbvm.com/Article/details/gcpvecrkh.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvggfiydx.sHtML

F. 文件与目录
来源：http://www.m.share.fehbvm.com/Article/details/gmtfowfke.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gulyfinng.sHtML

[F01] 读取整个文件
来源：http://www.share.zdbjq.cn/Article/details/gzrxndivn.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.zdbjq.cn/Article/details/gghsfwnnx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gyfgxhezp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.fehbvm.com/Article/details/gfxkyfrlh.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gkkhxktip.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gxtseebgp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fehbvm.com/Article/details/gcwlfrnpj.sHtML

Ruby: File.read("a.txt")
来源：http://wap.hesvh.cn/Article/details/gbgbufqva.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fehbvm.com/Article/details/gmlwjdfcr.sHtML

[F02] 逐行读取文件
来源：http://baike.hesvh.cn/Article/details/gqdbqfvmm.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fehbvm.com/Article/details/gpwszznpq.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fehbvm.com/Article/details/gdwwhisgt.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/ggvlybxkt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.fehbvm.com/Article/details/gkrtfyxqv.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/gargioabj.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.m.share.hesvh.cn/Article/details/gesajtpfu.sHtML


<!-- 参考信息 -->