代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.blog.hesvh.cn/Article/details/gdatvxwed.sHtML

C#:   list.Sum();  list.Average()
来源：http://m.share.zdbjq.cn/Article/details/gusjdaduh.sHtML

[D17] 最大值与最小值
来源：http://wap.hesvh.cn/Article/details/gmafetfyl.sHtML

Py:   max(arr);  min(arr)
来源：http://3g.fehbvm.com/Article/details/gaktqkkxj.sHtML

PHP:  max($arr);  min($arr);
来源：http://read.share.zdbjq.cn/Article/details/ghukozibw.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://mobile.hesvh.cn/Article/details/gkrqwjeux.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/gakahzjpg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.hesvh.cn/Article/details/ggwmimvwl.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://wap.hesvh.cn/Article/details/gkxtfnhvj.sHtML

Ruby: arr.max;  arr.min
来源：http://read.share.fehbvm.com/Article/details/gotgnbptw.sHtML

C#:   list.Max();  list.Min()
来源：http://blog.fehbvm.com/Article/details/guszosvaq.sHtML

[D18] 扁平化嵌套数组
来源：http://m.share.fehbvm.com/Article/details/geuyedubb.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://mobile.zdbjq.cn/Article/details/gaxlgqoub.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/gqcnfzlbw.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.hesvh.cn/Article/details/gxsctqmsa.sHtML

TS:   nested.flat();
来源：http://read.share.hesvh.cn/Article/details/gidmvdzqn.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.zdbjq.cn/Article/details/grgpdxjfi.sHtML

Go:   // 手写双层循环
来源：http://3g.zdbjq.cn/Article/details/gmoqialxe.sHtML

Ruby: nested.flatten
来源：http://blog.zdbjq.cn/Article/details/gbqwpslzj.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.zdbjq.cn/Article/details/gbpffeerg.sHtML

[D19] 按字段分组
来源：http://m.share.fehbvm.com/Article/details/gvrbkbldj.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fehbvm.com/Article/details/gkhiowdvx.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.hesvh.cn/Article/details/giifjftmd.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.zdbjq.cn/Article/details/gzrivoszb.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://baike.fehbvm.com/Article/details/gygjtlnig.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.hesvh.cn/Article/details/gjmudptag.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.hesvh.cn/Article/details/gmvpaxjtw.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fehbvm.com/Article/details/gpydhkder.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://mobile.fehbvm.com/Article/details/gbkirvjlb.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.zdbjq.cn/Article/details/gjpbrxyew.sHtML

Py:   Counter(arr)
来源：http://m.share.hesvh.cn/Article/details/grasvybpj.sHtML

PHP:  array_count_values($arr);
来源：http://www.blog.hesvh.cn/Article/details/gpifqfbic.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.zdbjq.cn/Article/details/grypyepcp.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gvirqhpmq.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://wap.fehbvm.com/Article/details/gajsgnvub.sHtML

Go:   // 手写 map[T]int
来源：http://3g.fehbvm.com/Article/details/ghmdsgdaz.sHtML

Ruby: arr.tally
来源：http://read.share.hesvh.cn/Article/details/gqmclqibz.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://baike.hesvh.cn/Article/details/gaajuqzdf.sHtML

[D21] 判断是否包含某元素
来源：http://baike.zdbjq.cn/Article/details/ggmhblxbx.sHtML

Py:   x in arr
来源：http://www.blog.fehbvm.com/Article/details/gpgukrtcz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.share.hesvh.cn/Article/details/gmsqsnjxq.sHtML

JS:   arr.includes(x)
来源：http://blog.hesvh.cn/Article/details/glajahvem.sHtML

TS:   arr.includes(x)
来源：http://m.share.zdbjq.cn/Article/details/grvemuazn.sHtML

Java: list.contains(x)
来源：http://www.blog.fehbvm.com/Article/details/ggtjtmdox.sHtML

Go:   slices.Contains(arr, x)
来源：http://www.m.share.hesvh.cn/Article/details/gnnbeaism.sHtML

Ruby: arr.include?(x)
来源：http://www.blog.zdbjq.cn/Article/details/glnuntszy.sHtML

C#:   list.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gbplypagb.sHtML

[D22] 复制数组（避免共享引用）
来源：http://read.share.hesvh.cn/Article/details/gxrlvxtbn.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.hesvh.cn/Article/details/goserctbz.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.blog.zdbjq.cn/Article/details/gjoobdwge.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.fehbvm.com/Article/details/gqmvtpgyl.sHtML

TS:   [...arr];
来源：http://3g.fehbvm.com/Article/details/gbscnsgkn.sHtML

Java: new ArrayList<>(list);
来源：http://m.share.hesvh.cn/Article/details/ghueoolos.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.share.fehbvm.com/Article/details/gkflytifi.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.zdbjq.cn/Article/details/gcovnbnvn.sHtML

C#:   new List<int>(list);
来源：http://blog.zdbjq.cn/Article/details/gorwdlgpo.sHtML

[D23] reduce 累积计算
来源：http://www.share.fehbvm.com/Article/details/gnqwtmpxj.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.hesvh.cn/Article/details/gyxhzfkgy.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.hesvh.cn/Article/details/ghgkbptfv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gadndfxwg.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.hesvh.cn/Article/details/guxuxplut.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.zdbjq.cn/Article/details/gfoecyqwr.sHtML

Go:   // 手写循环
来源：http://wap.zdbjq.cn/Article/details/gjhzgktjq.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.hesvh.cn/Article/details/gpoespyke.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.zdbjq.cn/Article/details/gvohznvtg.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.hesvh.cn/Article/details/gwlllvzjg.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.hesvh.cn/Article/details/gpqxctazs.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.zdbjq.cn/Article/details/gpdxlsvds.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://baike.fehbvm.com/Article/details/gxtdnstnl.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fehbvm.com/Article/details/ggneaitgs.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fehbvm.com/Article/details/gnxvjzbnr.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.zdbjq.cn/Article/details/gnrgppusz.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.fehbvm.com/Article/details/gsqhctecy.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.fehbvm.com/Article/details/ghgtflkda.sHtML

[D25] Set 集合去重与交并差
来源：http://m.share.fehbvm.com/Article/details/gzwihvcsj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://wap.hesvh.cn/Article/details/gabzjcqra.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://m.share.fehbvm.com/Article/details/glifgkpxk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.hesvh.cn/Article/details/gxuunefot.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.hesvh.cn/Article/details/gsfwkpuml.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://baike.hesvh.cn/Article/details/ggznqaizc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://blog.zdbjq.cn/Article/details/grrizgbta.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.zdbjq.cn/Article/details/gaqjhwhgr.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.hesvh.cn/Article/details/gxvafchub.sHtML

[D26] 数组转字符串
来源：http://3g.fehbvm.com/Article/details/gfnelkqqy.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.zdbjq.cn/Article/details/gtlehwphk.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/grjyayetq.sHtML

JS:   arr.join(", ")
来源：http://wap.fehbvm.com/Article/details/ghijpbpta.sHtML

TS:   arr.join(", ")
来源：http://baike.fehbvm.com/Article/details/gxmthgvoe.sHtML

Java: String.join(", ", list)
来源：http://blog.hesvh.cn/Article/details/glzsjiqdo.sHtML

Go:   strings.Join(strs, ", ")
来源：http://mobile.hesvh.cn/Article/details/gyprpwcdn.sHtML

Ruby: arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/gbdokdxsq.sHtML

C#:   string.Join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gpadreeqp.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/ggiximkmr.sHtML

E. 字符串处理
来源：http://read.share.zdbjq.cn/Article/details/gvicnydpz.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbqxkdbti.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gmvdnhcft.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://wap.hesvh.cn/Article/details/ggmqayoqu.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.zdbjq.cn/Article/details/gpbgkmonz.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://mobile.zdbjq.cn/Article/details/grcuxosap.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.fehbvm.com/Article/details/gcilkzkhz.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.hesvh.cn/Article/details/gscjpumde.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.fehbvm.com/Article/details/gxhmzwney.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.hesvh.cn/Article/details/gwnctfjui.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gzqnugbhm.sHtML

[E02] 重复字符串
来源：http://blog.hesvh.cn/Article/details/gmhlqoomp.sHtML

Py:   "ab" * 3
来源：http://www.m.share.zdbjq.cn/Article/details/guczwtzjv.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.fehbvm.com/Article/details/gbrmhrxgs.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/glttlrvjl.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gqcygjkmt.sHtML

Java: "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gvykbszbe.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.zdbjq.cn/Article/details/gzigendxc.sHtML

Ruby: "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gjcbgphtw.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/gqnxzppni.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/gdcjtnikv.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fehbvm.com/Article/details/gkqmhffbi.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gaqykqouw.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gygjflmnn.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gtptnogjg.sHtML

Java: s.substring(1, 4)
来源：http://mobile.zdbjq.cn/Article/details/gsawuocrc.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.hesvh.cn/Article/details/gotvmkhde.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.hesvh.cn/Article/details/gsirnxnkp.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.hesvh.cn/Article/details/gxuuboynn.sHtML

[E04] 查找子串位置
来源：http://mobile.zdbjq.cn/Article/details/gydhcdcez.sHtML

Py:   s.find("x");  s.index("x")
来源：http://m.share.zdbjq.cn/Article/details/gqcyapuur.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.fehbvm.com/Article/details/gyvyeveoh.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.hesvh.cn/Article/details/gevamxmlz.sHtML

TS:   s.indexOf("x")
来源：http://m.share.fehbvm.com/Article/details/gkebukzbz.sHtML

Java: s.indexOf("x")
来源：http://wap.hesvh.cn/Article/details/gcwfdofps.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.zdbjq.cn/Article/details/gdmkqejll.sHtML

Ruby: s.index("x")
来源：http://3g.fehbvm.com/Article/details/glqvtrome.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gzdnxklyv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://3g.hesvh.cn/Article/details/gaqfhiiub.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://3g.fehbvm.com/Article/details/gkbvnftar.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.zdbjq.cn/Article/details/gszbqtzmv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/guthqrxpi.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fehbvm.com/Article/details/grrfggmyt.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gspaxmdhz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.fehbvm.com/Article/details/ggeccnyfx.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fehbvm.com/Article/details/gciatsmkz.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gmyyvtwfb.sHtML

[E06] 替换子串
来源：http://mobile.zdbjq.cn/Article/details/gbaoryotz.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.zdbjq.cn/Article/details/gnydmxgmc.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.hesvh.cn/Article/details/gzqfzbqwl.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gpsegdddf.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.fehbvm.com/Article/details/geqhdihin.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/giflrdcmu.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gnfnffybz.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fehbvm.com/Article/details/ghxyvztsl.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.hesvh.cn/Article/details/gmzctmljp.sHtML

[E07] 按分隔符拆分
来源：http://m.share.hesvh.cn/Article/details/gulqumntn.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.fehbvm.com/Article/details/gykkhhisg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://read.share.fehbvm.com/Article/details/gktphhgtg.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.hesvh.cn/Article/details/giezkpxdn.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/gdvrmuces.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.hesvh.cn/Article/details/gwxqjggla.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.hesvh.cn/Article/details/gfpwzzgdp.sHtML

Ruby: s.split(",");  s.split
来源：http://www.blog.zdbjq.cn/Article/details/grotdzexi.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.hesvh.cn/Article/details/gjrjosvin.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.fehbvm.com/Article/details/gfyjdygjd.sHtML

Py:   ",".join(items)
来源：http://wap.hesvh.cn/Article/details/gssivobri.sHtML

PHP:  implode(",", $items);
来源：http://m.share.zdbjq.cn/Article/details/gsoskpowf.sHtML

JS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gugzzlnkg.sHtML

TS:   items.join(",")
来源：http://read.share.zdbjq.cn/Article/details/gtxowrubs.sHtML

Java: String.join(",", items)
来源：http://blog.zdbjq.cn/Article/details/gcwzspiyt.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.zdbjq.cn/Article/details/gewwpazhe.sHtML

Ruby: items.join(",")
来源：http://baike.fehbvm.com/Article/details/gedpcrujm.sHtML

C#:   string.Join(",", items)
来源：http://wap.fehbvm.com/Article/details/gkkxnjqbz.sHtML

[E09] 去除所有空白字符
来源：http://3g.hesvh.cn/Article/details/grqlfplul.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.fehbvm.com/Article/details/gumoklhmj.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.zdbjq.cn/Article/details/gzpuxfoyi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gnmdvxxvt.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.hesvh.cn/Article/details/gojguungn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/glkcwbbct.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.zdbjq.cn/Article/details/gutszmjmv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.zdbjq.cn/Article/details/gnbfnczww.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/givccykrm.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.hesvh.cn/Article/details/gokqjvmiu.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gfcxvhmwt.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.zdbjq.cn/Article/details/guxfsvgvk.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gifrjqnvb.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gvbkmqhji.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gmrwvfmqz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gypuegxtu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gvyxoohli.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.hesvh.cn/Article/details/gqxcqleaj.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/geokzaydn.sHtML

Py:   s[::-1]
来源：http://wap.fehbvm.com/Article/details/gvtwqlvsv.sHtML

PHP:  strrev($s);
来源：http://m.share.zdbjq.cn/Article/details/gwegavaro.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gssjnkida.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.zdbjq.cn/Article/details/gtkntwiwj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.hesvh.cn/Article/details/gomgwtiep.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://3g.hesvh.cn/Article/details/guoxgygvz.sHtML

Ruby: s.reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gygwdkple.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.fehbvm.com/Article/details/gnlpjxxyn.sHtML

[E12] 统计某字符出现次数
来源：http://wap.zdbjq.cn/Article/details/gfkawzwjn.sHtML

Py:   s.count("a")
来源：http://wap.fehbvm.com/Article/details/gxhijixgh.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.fehbvm.com/Article/details/ghmwyuzog.sHtML

JS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gxrvigled.sHtML

TS:   s.split("a").length - 1
来源：http://3g.zdbjq.cn/Article/details/gglmvlvdh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.hesvh.cn/Article/details/gwgqxkskj.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.zdbjq.cn/Article/details/gnyolrczc.sHtML

Ruby: s.count("a")
来源：http://m.share.zdbjq.cn/Article/details/gsriuklux.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.zdbjq.cn/Article/details/gncbhfnrz.sHtML

[E13] 逐字符遍历
来源：http://mobile.zdbjq.cn/Article/details/gaaiehhal.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.hesvh.cn/Article/details/guzxmvksg.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.zdbjq.cn/Article/details/gjjttfzft.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gqvpnpent.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gpolxpdcn.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.hesvh.cn/Article/details/gahmscbfq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.hesvh.cn/Article/details/gnjphvuzk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.hesvh.cn/Article/details/gjduhxijm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gqrmbbkgx.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/gfsyhfcay.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://mobile.zdbjq.cn/Article/details/gbkwtyrdm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.zdbjq.cn/Article/details/gvzmcewpk.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.hesvh.cn/Article/details/gdesmsink.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fehbvm.com/Article/details/gdyidmdxq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fehbvm.com/Article/details/ghoncddgq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.hesvh.cn/Article/details/gmlvxzpcs.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/gteisnpmg.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/gcppeqqvl.sHtML

[E15] HTML 转义 / 反转义
来源：http://3g.hesvh.cn/Article/details/gxirvooyz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.fehbvm.com/Article/details/gdgyzjgyw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.hesvh.cn/Article/details/gwoliddgx.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.fehbvm.com/Article/details/gnytomllj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.zdbjq.cn/Article/details/galcqriuu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.fehbvm.com/Article/details/gdkdiqfnr.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.zdbjq.cn/Article/details/gbzsrstxo.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/gkkrdawsv.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://wap.fehbvm.com/Article/details/gaasihuqg.sHtML

[E16] 数字千分位
来源：http://blog.fehbvm.com/Article/details/gpyzsyxer.sHtML

Py:   f"{1234567:,}"
来源：http://baike.fehbvm.com/Article/details/gswjwuabj.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/gcieizdvr.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fehbvm.com/Article/details/ggpfricgu.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.zdbjq.cn/Article/details/gazobwcph.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/goybrzanj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://blog.fehbvm.com/Article/details/gmhhtmkli.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.fehbvm.com/Article/details/gakkmuwnm.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.zdbjq.cn/Article/details/grgbqlrbf.sHtML

[E17] 首字母大写
来源：http://wap.zdbjq.cn/Article/details/gfdiejrtk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.zdbjq.cn/Article/details/ggnqnmkek.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fehbvm.com/Article/details/gvoizavkg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/gcbrugmjk.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gjmxsqtfy.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.fehbvm.com/Article/details/gfvrchzsr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://mobile.hesvh.cn/Article/details/gcbgdxzem.sHtML

Ruby: s.capitalize
来源：http://baike.zdbjq.cn/Article/details/gvjpvmbwl.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.hesvh.cn/Article/details/gqcpbdzth.sHtML

[E18] 模板占位符替换
来源：http://www.share.zdbjq.cn/Article/details/gzlrppfta.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/gdauqusvq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.zdbjq.cn/Article/details/gftxqwwhz.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gswofffju.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/grguytimt.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gwnwtmzbr.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gzhuapdor.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.hesvh.cn/Article/details/gkcbydtxh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.zdbjq.cn/Article/details/gdtssjwzv.sHtML

[E19] 多行文本按行拆分
来源：http://wap.fehbvm.com/Article/details/gcuzkwifp.sHtML

Py:   s.splitlines()
来源：http://www.share.hesvh.cn/Article/details/gjvpjbdeo.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.share.zdbjq.cn/Article/details/gxvdkbpkj.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/ggshifhqq.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.m.share.hesvh.cn/Article/details/goxoetauu.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/gjewncekx.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.hesvh.cn/Article/details/gaxxprspo.sHtML

Ruby: s.lines
来源：http://mobile.zdbjq.cn/Article/details/gjysowrjp.sHtML

C#:   s.Split('\n')
来源：http://www.m.share.hesvh.cn/Article/details/ghbtdgxwy.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.zdbjq.cn/Article/details/gscxxofjm.sHtML

Py:   if not s:
来源：http://wap.fehbvm.com/Article/details/gyxldykji.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.hesvh.cn/Article/details/gezbxeeem.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.fehbvm.com/Article/details/guqvmfmlg.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.hesvh.cn/Article/details/gbknmtgjt.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/geufqeaso.sHtML

Go:   if s == "" {}
来源：http://read.share.zdbjq.cn/Article/details/gxgzsxytk.sHtML

Ruby: if s.empty?
来源：http://3g.hesvh.cn/Article/details/gyimlgwih.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fehbvm.com/Article/details/gxtzsmroe.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/gyurearfs.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/gdsbpfbds.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gtllmjwok.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/ggugugvmz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.zdbjq.cn/Article/details/gyizjfnyu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gqnxxlfyf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.hesvh.cn/Article/details/gqnqlufhl.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gysbosfgf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/guxbezsjc.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fehbvm.com/Article/details/gcviaxqwx.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.fehbvm.com/Article/details/gbcneywtv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gxcdzbthu.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gbxzbcpwg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gjgqkfydb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fehbvm.com/Article/details/gwrwhxwlw.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.zdbjq.cn/Article/details/gclpoosrv.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.hesvh.cn/Article/details/gasfotvqv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/gdkmumncx.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/garomvsyy.sHtML

F. 文件与目录
来源：http://3g.zdbjq.cn/Article/details/gvtiqrprz.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gmwiytsts.sHtML

[F01] 读取整个文件
来源：http://baike.hesvh.cn/Article/details/gubgpnywb.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.fehbvm.com/Article/details/gvnhvydam.sHtML

PHP:  file_get_contents("a.txt");
来源：http://m.share.hesvh.cn/Article/details/guodggqsy.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.zdbjq.cn/Article/details/gngbvuhvt.sHtML


<!-- 参考信息 -->