代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/gzzcuggnt.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.hesvh.cn/Article/details/gbclxvssa.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/ginwmdeoh.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/gxkxbylvj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.hesvh.cn/Article/details/gpnnxdorn.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.fehbvm.com/Article/details/gsdwuncwf.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://blog.hesvh.cn/Article/details/gnhsmixei.sHtML

TS:   nested.flat();
来源：http://www.m.share.zdbjq.cn/Article/details/gxfyhusmh.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.zdbjq.cn/Article/details/grtwdabkb.sHtML

Go:   // 手写双层循环
来源：http://mobile.zdbjq.cn/Article/details/gdzkozvtu.sHtML

Ruby: nested.flatten
来源：http://www.share.fehbvm.com/Article/details/gmjlyralz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.fehbvm.com/Article/details/grmrojhrh.sHtML

[D19] 按字段分组
来源：http://wap.hesvh.cn/Article/details/guwrwvxaq.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://wap.fehbvm.com/Article/details/gyfomhdxx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.zdbjq.cn/Article/details/gjqsiflhn.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.hesvh.cn/Article/details/giqddmffk.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.share.zdbjq.cn/Article/details/gbmipiuat.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.share.hesvh.cn/Article/details/gntqsyjhp.sHtML

Go:   // 手写 map[string][]T
来源：http://read.share.fehbvm.com/Article/details/gqqvpidlt.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://mobile.fehbvm.com/Article/details/gmqcwigvo.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.hesvh.cn/Article/details/gurbfgrzn.sHtML

[D20] 统计每个元素出现次数
来源：http://baike.fehbvm.com/Article/details/gmsmsfpet.sHtML

Py:   Counter(arr)
来源：http://3g.fehbvm.com/Article/details/guhlycwzo.sHtML

PHP:  array_count_values($arr);
来源：http://m.share.fehbvm.com/Article/details/gfquizhnr.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.hesvh.cn/Article/details/gifhvdkdz.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/gxrmjntnu.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://baike.zdbjq.cn/Article/details/gawzuxccc.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fehbvm.com/Article/details/gkazxujkc.sHtML

Ruby: arr.tally
来源：http://baike.hesvh.cn/Article/details/gcclqixgo.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://3g.hesvh.cn/Article/details/gyvfdvxrl.sHtML

[D21] 判断是否包含某元素
来源：http://m.share.hesvh.cn/Article/details/gevuohjhr.sHtML

Py:   x in arr
来源：http://wap.fehbvm.com/Article/details/gsokalwgn.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.hesvh.cn/Article/details/ggthtnecx.sHtML

JS:   arr.includes(x)
来源：http://blog.fehbvm.com/Article/details/gzqlcbjut.sHtML

TS:   arr.includes(x)
来源：http://www.blog.fehbvm.com/Article/details/gwcguqieu.sHtML

Java: list.contains(x)
来源：http://www.blog.fehbvm.com/Article/details/gubhwtrdg.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.share.zdbjq.cn/Article/details/gwdtownns.sHtML

Ruby: arr.include?(x)
来源：http://3g.hesvh.cn/Article/details/guriteoel.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gkexdoozo.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fehbvm.com/Article/details/gnhoumzki.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.share.hesvh.cn/Article/details/gyfqjwrlr.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://baike.fehbvm.com/Article/details/gpeyepcrg.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gultqzsgb.sHtML

TS:   [...arr];
来源：http://blog.hesvh.cn/Article/details/ggluikvsl.sHtML

Java: new ArrayList<>(list);
来源：http://mobile.hesvh.cn/Article/details/gftfdxuov.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.blog.zdbjq.cn/Article/details/gdtiejlco.sHtML

Ruby: arr.dup;  arr.clone
来源：http://m.share.fehbvm.com/Article/details/gblvgqxqe.sHtML

C#:   new List<int>(list);
来源：http://blog.hesvh.cn/Article/details/gxfxsguva.sHtML

[D23] reduce 累积计算
来源：http://www.m.share.zdbjq.cn/Article/details/gqkllnpnk.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.hesvh.cn/Article/details/gjxuubldb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.fehbvm.com/Article/details/glckxeqyz.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://read.share.hesvh.cn/Article/details/ghhpkpssq.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gnuatfkke.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://blog.fehbvm.com/Article/details/gfltkynnj.sHtML

Go:   // 手写循环
来源：http://blog.hesvh.cn/Article/details/gqhudhmnd.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.hesvh.cn/Article/details/glsgpjdjh.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.hesvh.cn/Article/details/gfazttszv.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.zdbjq.cn/Article/details/gljcdfmdd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.fehbvm.com/Article/details/givqtlmxu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.hesvh.cn/Article/details/geajzinrd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://3g.hesvh.cn/Article/details/govzimywm.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gegzdjmpp.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.m.share.fehbvm.com/Article/details/gtfbpnrct.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.hesvh.cn/Article/details/gdytaguof.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.hesvh.cn/Article/details/gfhxnmssr.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://baike.hesvh.cn/Article/details/gtwzhmbcf.sHtML

[D25] Set 集合去重与交并差
来源：http://read.share.fehbvm.com/Article/details/goptugisj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.zdbjq.cn/Article/details/gwmtiugnu.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.zdbjq.cn/Article/details/gnmcairhd.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://wap.hesvh.cn/Article/details/gckygupez.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.fehbvm.com/Article/details/gmopgyxam.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.zdbjq.cn/Article/details/gkjvczhsz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://mobile.hesvh.cn/Article/details/gdeteuzzh.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.hesvh.cn/Article/details/gwsgiexhl.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.fehbvm.com/Article/details/gbgdhjuqx.sHtML

[D26] 数组转字符串
来源：http://www.share.fehbvm.com/Article/details/gzewbqyln.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.zdbjq.cn/Article/details/gsfemkrkk.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.hesvh.cn/Article/details/gkomemlet.sHtML

JS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gwpngazqw.sHtML

TS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/grjjrufzk.sHtML

Java: String.join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gksavkabi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://m.share.zdbjq.cn/Article/details/glqtujraa.sHtML

Ruby: arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gqafwobmj.sHtML

C#:   string.Join(", ", list)
来源：http://www.share.zdbjq.cn/Article/details/gukwqyvih.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gevfoubnm.sHtML

E. 字符串处理
来源：http://wap.zdbjq.cn/Article/details/gqdvfycko.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grrtfadhd.sHtML

[E01] 拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gvjygpjmy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fehbvm.com/Article/details/gbvjvcikj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://mobile.zdbjq.cn/Article/details/ggwtoksee.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/gmnatyytp.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/glqhfgylh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.hesvh.cn/Article/details/gqaynezga.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.hesvh.cn/Article/details/gavtibdyq.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.fehbvm.com/Article/details/gnmoacoui.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gyqtdwbtt.sHtML

[E02] 重复字符串
来源：http://www.m.share.fehbvm.com/Article/details/gjtcwtabe.sHtML

Py:   "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/guwsfpqiu.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fehbvm.com/Article/details/gnjdjyjgz.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/ghkbmwykl.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gcfbsqlsm.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.zdbjq.cn/Article/details/gykxpuuua.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.hesvh.cn/Article/details/gohkrecii.sHtML

Ruby: "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gymmgdaai.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.zdbjq.cn/Article/details/gdlsmvkrz.sHtML

[E03] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gykfajvvb.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://read.share.zdbjq.cn/Article/details/geqgiisaq.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.hesvh.cn/Article/details/gummdjzzr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gqeomkxru.sHtML

TS:   s.slice(1, 4)
来源：http://m.share.hesvh.cn/Article/details/gmvzznmaw.sHtML

Java: s.substring(1, 4)
来源：http://read.share.fehbvm.com/Article/details/guwrdlxgr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.fehbvm.com/Article/details/guhhwqvjy.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.hesvh.cn/Article/details/gmzsuspze.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.zdbjq.cn/Article/details/gsvewuijc.sHtML

[E04] 查找子串位置
来源：http://read.share.hesvh.cn/Article/details/gescszpbe.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gnyfcqdqs.sHtML

PHP:  strpos($s, "x");
来源：http://3g.hesvh.cn/Article/details/gmfisxinx.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fehbvm.com/Article/details/gidakuzyr.sHtML

TS:   s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gnmhcsxsu.sHtML

Java: s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/glnxdkutb.sHtML

Go:   strings.Index(s, "x")
来源：http://3g.fehbvm.com/Article/details/gtuzxlvhd.sHtML

Ruby: s.index("x")
来源：http://3g.fehbvm.com/Article/details/gjjlbhywx.sHtML

C#:   s.IndexOf("x")
来源：http://wap.zdbjq.cn/Article/details/gsnvtophx.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.fehbvm.com/Article/details/gkkatgihc.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.fehbvm.com/Article/details/gvchiuuli.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.blog.zdbjq.cn/Article/details/gqdljbzsd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.hesvh.cn/Article/details/gzhlqcsqe.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://blog.zdbjq.cn/Article/details/gicoqnmzg.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.fehbvm.com/Article/details/gutcvqwuv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.fehbvm.com/Article/details/guymcosqk.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fehbvm.com/Article/details/gwitlzkdx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.m.share.hesvh.cn/Article/details/gbewelkbm.sHtML

[E06] 替换子串
来源：http://www.m.share.hesvh.cn/Article/details/gmkjulwzc.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.fehbvm.com/Article/details/gboeftjkx.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.m.share.fehbvm.com/Article/details/gbiehnpbv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gmcealhrm.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/gxbtyvjab.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gljgeyqbg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/ghkfkohyy.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gpjfmzldg.sHtML

C#:   s.Replace("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/girzzpkza.sHtML

[E07] 按分隔符拆分
来源：http://baike.fehbvm.com/Article/details/gxeezcptu.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://baike.hesvh.cn/Article/details/gpxnmdcty.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.fehbvm.com/Article/details/grwslpizh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.zdbjq.cn/Article/details/gmewmseyi.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/girzfxrfu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.hesvh.cn/Article/details/gtzvwphrk.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.fehbvm.com/Article/details/grqsnjplx.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.zdbjq.cn/Article/details/gwovzjgjc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fehbvm.com/Article/details/gbxypteap.sHtML

[E08] 数组按分隔符合并
来源：http://wap.hesvh.cn/Article/details/gancebsff.sHtML

Py:   ",".join(items)
来源：http://m.share.hesvh.cn/Article/details/gomlgjtaf.sHtML

PHP:  implode(",", $items);
来源：http://baike.zdbjq.cn/Article/details/gvojkxviv.sHtML

JS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gzrxouytr.sHtML

TS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gidqlvofv.sHtML

Java: String.join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gybkhngpj.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.fehbvm.com/Article/details/giuxgdccd.sHtML

Ruby: items.join(",")
来源：http://blog.fehbvm.com/Article/details/gkfonyhup.sHtML

C#:   string.Join(",", items)
来源：http://3g.hesvh.cn/Article/details/gslttobqc.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.fehbvm.com/Article/details/ghbvdvvap.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.zdbjq.cn/Article/details/gvdhdtcrf.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.zdbjq.cn/Article/details/gcrachvlj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gifzcfrsx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fehbvm.com/Article/details/gglmsgndd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fehbvm.com/Article/details/gexnspyko.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.fehbvm.com/Article/details/gvafnnexx.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fehbvm.com/Article/details/gdcfifxzm.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://3g.zdbjq.cn/Article/details/gdkrleciv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.zdbjq.cn/Article/details/gacuvrxsw.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fehbvm.com/Article/details/glingogyp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.zdbjq.cn/Article/details/ggxlkddpt.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gpwaqflkr.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gerdxmygh.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/geqstlzyt.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.zdbjq.cn/Article/details/guntjopkk.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/grpidojvm.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fehbvm.com/Article/details/guyimpcxk.sHtML

[E11] 反转字符串
来源：http://www.share.hesvh.cn/Article/details/gblcattbj.sHtML

Py:   s[::-1]
来源：http://3g.zdbjq.cn/Article/details/ginhamxwl.sHtML

PHP:  strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gczxyujhs.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/ghcxwbnmx.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gtoqgmnpo.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.hesvh.cn/Article/details/gzytygnmp.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.hesvh.cn/Article/details/garxqgiup.sHtML

Ruby: s.reverse
来源：http://baike.hesvh.cn/Article/details/gxdhehctp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gjodphfzx.sHtML

[E12] 统计某字符出现次数
来源：http://read.share.zdbjq.cn/Article/details/gydwrrrhd.sHtML

Py:   s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gcbbvjczf.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.fehbvm.com/Article/details/gxjuxvuwa.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/gnpmsdvnm.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gefjnipyh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fehbvm.com/Article/details/gkbmenpuo.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.fehbvm.com/Article/details/ggeylsrqe.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gvsbewdvq.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.fehbvm.com/Article/details/geqohtkwu.sHtML

[E13] 逐字符遍历
来源：http://www.share.zdbjq.cn/Article/details/gkerrkjmq.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fehbvm.com/Article/details/gnsrqaeqz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.zdbjq.cn/Article/details/giqwzbpjx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gyblhsdce.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gpymqgggm.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gfqbxridk.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.zdbjq.cn/Article/details/gqcghsqqo.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.zdbjq.cn/Article/details/ggvgdhxtg.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/gjxbvtrfi.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fehbvm.com/Article/details/gxdjfnglp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.fehbvm.com/Article/details/gyyhestzy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.hesvh.cn/Article/details/gpgwpxipa.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.hesvh.cn/Article/details/geehzjxei.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.hesvh.cn/Article/details/gmusxpejt.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://read.share.fehbvm.com/Article/details/gtfdbvozp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fehbvm.com/Article/details/gqtfqhkiv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.fehbvm.com/Article/details/geqyewalq.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.fehbvm.com/Article/details/gvrcdhxve.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.zdbjq.cn/Article/details/gcilbpwux.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://read.share.fehbvm.com/Article/details/gqseaonaa.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.share.fehbvm.com/Article/details/gcgxsczlf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fehbvm.com/Article/details/gfydsjfzp.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.zdbjq.cn/Article/details/gqrblarep.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.zdbjq.cn/Article/details/gacugjgat.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gvzeccbch.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fehbvm.com/Article/details/gzzszxfao.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.zdbjq.cn/Article/details/ghvwplztq.sHtML

[E16] 数字千分位
来源：http://www.blog.hesvh.cn/Article/details/gkzoeardi.sHtML

Py:   f"{1234567:,}"
来源：http://wap.zdbjq.cn/Article/details/gjupghpjk.sHtML

PHP:  number_format(1234567);
来源：http://read.share.fehbvm.com/Article/details/gwnnhqata.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gqewespgy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fehbvm.com/Article/details/grkbxsubu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gqzsgphxa.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fehbvm.com/Article/details/gdqabuxjq.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.hesvh.cn/Article/details/gzivlxkca.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.zdbjq.cn/Article/details/gvwjdiegj.sHtML

[E17] 首字母大写
来源：http://wap.zdbjq.cn/Article/details/gpabkypnq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/gkkkrcyhs.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fehbvm.com/Article/details/gfafvcvxp.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gszzevyev.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/guodnyrxl.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.zdbjq.cn/Article/details/gxaltmvsk.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.zdbjq.cn/Article/details/gjyfqtrvq.sHtML

Ruby: s.capitalize
来源：http://www.share.fehbvm.com/Article/details/gozgkigcv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.zdbjq.cn/Article/details/glzhthbbn.sHtML

[E18] 模板占位符替换
来源：http://wap.zdbjq.cn/Article/details/giwwexgml.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://blog.fehbvm.com/Article/details/gqtmuesve.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fehbvm.com/Article/details/grfzwfioo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gntlpelqg.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gjxvmcoar.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.hesvh.cn/Article/details/glqezdvyt.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gopfpwhhh.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.hesvh.cn/Article/details/giuvzftvb.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fehbvm.com/Article/details/gqfdryerr.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.hesvh.cn/Article/details/gmianrrhl.sHtML

Py:   s.splitlines()
来源：http://3g.zdbjq.cn/Article/details/gwxphritm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fehbvm.com/Article/details/gpcedymld.sHtML

JS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gyuxfuzen.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gbwqxrrua.sHtML

Java: s.lines().toList()
来源：http://wap.hesvh.cn/Article/details/ghbrdohsy.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fehbvm.com/Article/details/gvcxamigf.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/grudysnoe.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/gsnyakgwq.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fehbvm.com/Article/details/gvxfulhhs.sHtML

Py:   if not s:
来源：http://blog.fehbvm.com/Article/details/geheuprkr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.zdbjq.cn/Article/details/ggnwytlrx.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/gvficuhcz.sHtML

TS:   if (s === "") {}
来源：http://m.share.zdbjq.cn/Article/details/gqcpmmopa.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gggmofgym.sHtML

Go:   if s == "" {}
来源：http://blog.hesvh.cn/Article/details/goifqyeyt.sHtML

Ruby: if s.empty?
来源：http://baike.fehbvm.com/Article/details/gykkrwvlq.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.fehbvm.com/Article/details/glhfobldk.sHtML

[E21] 超长截断加省略号
来源：http://3g.zdbjq.cn/Article/details/graalxqnc.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.zdbjq.cn/Article/details/ghdtixsca.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/guvjhexrb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gmrmshiss.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gmtgjimyg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/glenuipex.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.share.zdbjq.cn/Article/details/gathlfjdk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gtdbyoigt.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gsejgbtam.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.zdbjq.cn/Article/details/gsyflynri.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.hesvh.cn/Article/details/gytcbohsb.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/guaeeoczw.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gqkjstybp.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gmnsskwks.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.zdbjq.cn/Article/details/gmbngrmej.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.zdbjq.cn/Article/details/glzkyviae.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.hesvh.cn/Article/details/grwaptyax.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fehbvm.com/Article/details/gsqweobdv.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbzckzkgc.sHtML

F. 文件与目录
来源：http://blog.hesvh.cn/Article/details/gzyidbrpl.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gqyykpfqa.sHtML

[F01] 读取整个文件
来源：http://3g.zdbjq.cn/Article/details/gkfrilkhc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.fehbvm.com/Article/details/gfhkwejeb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gadiymhwv.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.fehbvm.com/Article/details/gfcafvqgk.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://baike.fehbvm.com/Article/details/gpydkuhuc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.hesvh.cn/Article/details/gilcajmfa.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.hesvh.cn/Article/details/gmfhgruts.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gatucldnj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://read.share.hesvh.cn/Article/details/gfonpxkfw.sHtML

[F02] 逐行读取文件
来源：http://wap.hesvh.cn/Article/details/guarwgxoh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.fehbvm.com/Article/details/guzswdkqy.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.hesvh.cn/Article/details/gqbtocbol.sHtML


<!-- 参考信息 -->