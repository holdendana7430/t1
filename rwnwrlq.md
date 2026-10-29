代发 wailian999

Java: nested.stream().flatMap(List::stream).toList()
来源：http://m.share.hesvh.cn/Article/details/gcnvffmqb.sHtML

Go:   // 手写双层循环
来源：http://m.share.hesvh.cn/Article/details/gjttbpehh.sHtML

Ruby: nested.flatten
来源：http://3g.zdbjq.cn/Article/details/gmjitzewg.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.blog.zdbjq.cn/Article/details/ghrcitozp.sHtML

[D19] 按字段分组
来源：http://wap.hesvh.cn/Article/details/grpvqcuax.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fehbvm.com/Article/details/gsyeussgw.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://m.share.hesvh.cn/Article/details/gvlvccumv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.blog.hesvh.cn/Article/details/gwvljxmfl.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://mobile.fehbvm.com/Article/details/gpmenuzpg.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.m.share.hesvh.cn/Article/details/grzfwycoy.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.zdbjq.cn/Article/details/gzupqnafv.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/gcamxznqg.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://3g.fehbvm.com/Article/details/ghvlicenj.sHtML

[D20] 统计每个元素出现次数
来源：http://wap.zdbjq.cn/Article/details/ggakpfanj.sHtML

Py:   Counter(arr)
来源：http://www.share.zdbjq.cn/Article/details/gvmrqbibt.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fehbvm.com/Article/details/gyzhqdifu.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.zdbjq.cn/Article/details/golyfzekm.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://read.share.zdbjq.cn/Article/details/gjovooznv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://3g.hesvh.cn/Article/details/gqbxrcjqi.sHtML

Go:   // 手写 map[T]int
来源：http://www.blog.zdbjq.cn/Article/details/gmwqwibww.sHtML

Ruby: arr.tally
来源：http://mobile.fehbvm.com/Article/details/gwsjvpcfi.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://m.share.hesvh.cn/Article/details/gnfxueaxq.sHtML

[D21] 判断是否包含某元素
来源：http://3g.zdbjq.cn/Article/details/grqsrpwup.sHtML

Py:   x in arr
来源：http://mobile.zdbjq.cn/Article/details/gvoeiizfa.sHtML

PHP:  in_array($x, $arr, true);
来源：http://3g.fehbvm.com/Article/details/gavzhnpjq.sHtML

JS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/grjwhhxxa.sHtML

TS:   arr.includes(x)
来源：http://www.blog.zdbjq.cn/Article/details/grulhvdij.sHtML

Java: list.contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gtrhikbef.sHtML

Go:   slices.Contains(arr, x)
来源：http://read.share.zdbjq.cn/Article/details/gvlmuoirw.sHtML

Ruby: arr.include?(x)
来源：http://read.share.fehbvm.com/Article/details/gxzuekibu.sHtML

C#:   list.Contains(x)
来源：http://baike.fehbvm.com/Article/details/gjmsumfci.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.zdbjq.cn/Article/details/grtbgoxqc.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://blog.zdbjq.cn/Article/details/gxwtacoay.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://blog.fehbvm.com/Article/details/gvdoxlcnk.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.fehbvm.com/Article/details/gsujolrqn.sHtML

TS:   [...arr];
来源：http://3g.zdbjq.cn/Article/details/gkvwhpbxa.sHtML

Java: new ArrayList<>(list);
来源：http://3g.zdbjq.cn/Article/details/gdoxcglzr.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://wap.fehbvm.com/Article/details/ggqhzdyhn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://blog.hesvh.cn/Article/details/gkewkqagk.sHtML

C#:   new List<int>(list);
来源：http://blog.hesvh.cn/Article/details/grgnvnlir.sHtML

[D23] reduce 累积计算
来源：http://read.share.hesvh.cn/Article/details/ghccozdyd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.zdbjq.cn/Article/details/gfxnyuvum.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.zdbjq.cn/Article/details/gbpticgyr.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gkdanjuvd.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.hesvh.cn/Article/details/geeyofibp.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://wap.fehbvm.com/Article/details/gnuevzpeh.sHtML

Go:   // 手写循环
来源：http://blog.zdbjq.cn/Article/details/ghvmczuix.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.share.fehbvm.com/Article/details/gbxgbzbei.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.zdbjq.cn/Article/details/gfkmsgbqj.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.zdbjq.cn/Article/details/gojbkrfnu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.zdbjq.cn/Article/details/gbabsfvlo.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.fehbvm.com/Article/details/gsrijufud.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.zdbjq.cn/Article/details/gobmhepyo.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gikcicrtq.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/gkcxxours.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.zdbjq.cn/Article/details/gepivhpyp.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://3g.hesvh.cn/Article/details/gqijvrnio.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gyknofesg.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.fehbvm.com/Article/details/grwwspybz.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://baike.fehbvm.com/Article/details/gqeuzpdnd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.fehbvm.com/Article/details/gzxojacyo.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://m.share.fehbvm.com/Article/details/gtvfsnymk.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.fehbvm.com/Article/details/gtnbngmuu.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.hesvh.cn/Article/details/ghsumrgtj.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://m.share.fehbvm.com/Article/details/gzfcjcfjl.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.zdbjq.cn/Article/details/gvnxkopgg.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzsolejsi.sHtML

[D26] 数组转字符串
来源：http://m.share.fehbvm.com/Article/details/gcairyjtx.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.hesvh.cn/Article/details/gqmrzrmhp.sHtML

PHP:  implode(", ", $arr);
来源：http://mobile.hesvh.cn/Article/details/guttykjgu.sHtML

JS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gwnzlwwom.sHtML

TS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gjsnuxqap.sHtML

Java: String.join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gajuzrzsk.sHtML

Go:   strings.Join(strs, ", ")
来源：http://3g.hesvh.cn/Article/details/gzfhbcnlr.sHtML

Ruby: arr.join(", ")
来源：http://m.share.fehbvm.com/Article/details/gluwsekjz.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gybeteiem.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gvfnfcahg.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/grjcweucv.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gdkvxxczt.sHtML

[E01] 拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gwgzpbyxy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.fehbvm.com/Article/details/geeutjwnl.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://m.share.hesvh.cn/Article/details/ggezabmwd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.hesvh.cn/Article/details/gjdqzilyl.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.share.fehbvm.com/Article/details/gjkwnllbh.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.zdbjq.cn/Article/details/gkixaqpdb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.zdbjq.cn/Article/details/glyczywvh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.hesvh.cn/Article/details/gmdyzsuad.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://blog.hesvh.cn/Article/details/glnfqhcoh.sHtML

[E02] 重复字符串
来源：http://blog.fehbvm.com/Article/details/gjsfwmrro.sHtML

Py:   "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/geyirvgnn.sHtML

PHP:  str_repeat("ab", 3);
来源：http://read.share.fehbvm.com/Article/details/ghodgaopz.sHtML

JS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gheerldyo.sHtML

TS:   "ab".repeat(3)
来源：http://wap.zdbjq.cn/Article/details/gmzmsfchv.sHtML

Java: "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gveamvqqg.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fehbvm.com/Article/details/gcahsqdik.sHtML

Ruby: "ab" * 3
来源：http://wap.zdbjq.cn/Article/details/gtoewvnmg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://wap.hesvh.cn/Article/details/gdyotyobl.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/goxqmxkqn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fehbvm.com/Article/details/gvajsinvb.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/gxlooidvt.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gdrpxjbvt.sHtML

TS:   s.slice(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gptbbvewv.sHtML

Java: s.substring(1, 4)
来源：http://baike.hesvh.cn/Article/details/gcplybmxu.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fehbvm.com/Article/details/gqvkuefnd.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.fehbvm.com/Article/details/gvwwlrphi.sHtML

C#:   s.Substring(1, 3)
来源：http://www.m.share.fehbvm.com/Article/details/gqwruqojv.sHtML

[E04] 查找子串位置
来源：http://baike.hesvh.cn/Article/details/gxvfhqshf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.zdbjq.cn/Article/details/gaxdakkpr.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.zdbjq.cn/Article/details/gwyjuhvua.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.fehbvm.com/Article/details/grbtucjfg.sHtML

TS:   s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/glbxghzvn.sHtML

Java: s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gmiroyofa.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.fehbvm.com/Article/details/gbewlbdob.sHtML

Ruby: s.index("x")
来源：http://blog.zdbjq.cn/Article/details/gnechnmgi.sHtML

C#:   s.IndexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gldljwqux.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fehbvm.com/Article/details/gqpfboieu.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://baike.hesvh.cn/Article/details/gxlbtosjf.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.hesvh.cn/Article/details/gsznafopx.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.fehbvm.com/Article/details/ghpjbsbbi.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fehbvm.com/Article/details/ghpydwghy.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.fehbvm.com/Article/details/gqiqygppa.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fehbvm.com/Article/details/gpcoyknnc.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://baike.fehbvm.com/Article/details/grmowvufn.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.hesvh.cn/Article/details/gcxizsncu.sHtML

[E06] 替换子串
来源：http://wap.fehbvm.com/Article/details/gceimqzpv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gptciibxa.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.hesvh.cn/Article/details/ghmizlfyf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gcttwpvjk.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/ggmgokgpp.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/grsbckmig.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gtfosetyb.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gasyfbdlh.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gxbbyweqc.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.hesvh.cn/Article/details/gqpttmshm.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.fehbvm.com/Article/details/geknfbwal.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.hesvh.cn/Article/details/gcaxxckpd.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fehbvm.com/Article/details/gcxugwxfq.sHtML

TS:   s.split(",")
来源：http://mobile.fehbvm.com/Article/details/gqbeycqze.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.m.share.zdbjq.cn/Article/details/gargheckh.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.hesvh.cn/Article/details/ggozwnnph.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.fehbvm.com/Article/details/gqaxtphcq.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.zdbjq.cn/Article/details/ggturaxxp.sHtML

[E08] 数组按分隔符合并
来源：http://3g.zdbjq.cn/Article/details/gcqksxnpe.sHtML

Py:   ",".join(items)
来源：http://mobile.hesvh.cn/Article/details/gwzihzthm.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fehbvm.com/Article/details/gruqfqxwu.sHtML

JS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gjxcgewjm.sHtML

TS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gobjnpavn.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gvocibfkx.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fehbvm.com/Article/details/grqoldvuk.sHtML

Ruby: items.join(",")
来源：http://baike.fehbvm.com/Article/details/gskhotkhe.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gvtfwxfjy.sHtML

[E09] 去除所有空白字符
来源：http://read.share.hesvh.cn/Article/details/gzzmyixvi.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.zdbjq.cn/Article/details/gyeecrvyo.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://baike.fehbvm.com/Article/details/gafxpdbnm.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fehbvm.com/Article/details/grcmqvdef.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gkijawkxn.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gethocieh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.zdbjq.cn/Article/details/gzmvmfkdg.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.zdbjq.cn/Article/details/grkbboymn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fehbvm.com/Article/details/gbmssbklb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.hesvh.cn/Article/details/gsfmpynkf.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.zdbjq.cn/Article/details/gmavoqsxu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fehbvm.com/Article/details/ghouigwwn.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gmxsblpro.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/ghgaqlosb.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/grlykcahe.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gmyqmdiov.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gmrjgcucl.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/grdveuxcd.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gwmotmhar.sHtML

Py:   s[::-1]
来源：http://wap.zdbjq.cn/Article/details/grltztmkw.sHtML

PHP:  strrev($s);
来源：http://read.share.fehbvm.com/Article/details/ggjhfxomu.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.zdbjq.cn/Article/details/grgrsqqhl.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.fehbvm.com/Article/details/gxzwxekpn.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/gvjhrbnqb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/gcxzyqtsl.sHtML

Ruby: s.reverse
来源：http://m.share.hesvh.cn/Article/details/gfraxvphm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://3g.hesvh.cn/Article/details/gonmgjlmj.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.hesvh.cn/Article/details/grtndagfv.sHtML

Py:   s.count("a")
来源：http://read.share.fehbvm.com/Article/details/gtviqwhmv.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.zdbjq.cn/Article/details/geiatjtgh.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gmjzonmyr.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gmidpznbo.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.fehbvm.com/Article/details/gyezrwrni.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.zdbjq.cn/Article/details/geagiopan.sHtML

Ruby: s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/ghojqutsi.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.zdbjq.cn/Article/details/gkrvkdsgb.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fehbvm.com/Article/details/gruzbfhjy.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.fehbvm.com/Article/details/gsesvvsvd.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.hesvh.cn/Article/details/glxnyafwf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gwptithvj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gquoaqafl.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fehbvm.com/Article/details/gevkcacrq.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.hesvh.cn/Article/details/gjzcsotjx.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.zdbjq.cn/Article/details/gnaxuiktr.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://3g.zdbjq.cn/Article/details/ginmlihvt.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.hesvh.cn/Article/details/gzgkvgucz.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.zdbjq.cn/Article/details/gzkhxbrcz.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.zdbjq.cn/Article/details/gaacrumbg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.hesvh.cn/Article/details/gqoqvzcch.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.fehbvm.com/Article/details/glytzjdma.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.hesvh.cn/Article/details/grsxymzzo.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://blog.fehbvm.com/Article/details/giyxpjrbj.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.hesvh.cn/Article/details/guibnlkam.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.fehbvm.com/Article/details/gidvflzcj.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.zdbjq.cn/Article/details/gahqaqvuf.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://blog.zdbjq.cn/Article/details/grmydvnxs.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.hesvh.cn/Article/details/gbduomwnf.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fehbvm.com/Article/details/gwteftsge.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gdejtjulx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.zdbjq.cn/Article/details/gbjmueyjs.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.fehbvm.com/Article/details/ghspvnzet.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/gmzwwmecg.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.hesvh.cn/Article/details/gxzwxzpro.sHtML

[E16] 数字千分位
来源：http://baike.fehbvm.com/Article/details/gwddpqxve.sHtML

Py:   f"{1234567:,}"
来源：http://www.share.fehbvm.com/Article/details/gwmgvqvnf.sHtML

PHP:  number_format(1234567);
来源：http://m.share.fehbvm.com/Article/details/gftruehno.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fehbvm.com/Article/details/gaqqrbhdp.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gysjltocw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gvhoaatvm.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.hesvh.cn/Article/details/gjcjvyuxk.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.hesvh.cn/Article/details/gqhhzonxd.sHtML

C#:   1234567.ToString("N0")
来源：http://blog.hesvh.cn/Article/details/gocodiieb.sHtML

[E17] 首字母大写
来源：http://m.share.zdbjq.cn/Article/details/gnnxskrir.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fehbvm.com/Article/details/guqliyjda.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.zdbjq.cn/Article/details/gdihedybs.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gfdkrkrio.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fehbvm.com/Article/details/gikryuabw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.hesvh.cn/Article/details/guxrohbep.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.hesvh.cn/Article/details/gjdoqdknw.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/ggjpdlfkz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.zdbjq.cn/Article/details/gqcjootdq.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.hesvh.cn/Article/details/gzmcglsfu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://mobile.zdbjq.cn/Article/details/gatujjobi.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fehbvm.com/Article/details/gxcmnyfpd.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gyysnycxr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gactagyky.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.zdbjq.cn/Article/details/geoutgdht.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gpmoeoadu.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fehbvm.com/Article/details/gqcrcmkbd.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.hesvh.cn/Article/details/gaxrslazt.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.hesvh.cn/Article/details/gmdntysno.sHtML

Py:   s.splitlines()
来源：http://blog.fehbvm.com/Article/details/gnbpzrkoi.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://blog.fehbvm.com/Article/details/gvhhkluyd.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gsisfnxif.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.hesvh.cn/Article/details/gkbrxkpws.sHtML

Java: s.lines().toList()
来源：http://www.m.share.hesvh.cn/Article/details/gmvmkopjd.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.hesvh.cn/Article/details/gxwgzlamt.sHtML

Ruby: s.lines
来源：http://3g.fehbvm.com/Article/details/ghpcyfmcp.sHtML

C#:   s.Split('\n')
来源：http://blog.zdbjq.cn/Article/details/gigrzsjva.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fehbvm.com/Article/details/gdpdaegzz.sHtML

Py:   if not s:
来源：http://m.share.hesvh.cn/Article/details/gicmoxxsb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://baike.zdbjq.cn/Article/details/gotsqysgu.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.zdbjq.cn/Article/details/gqtmqtilk.sHtML

TS:   if (s === "") {}
来源：http://3g.fehbvm.com/Article/details/gvolgjhhh.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.hesvh.cn/Article/details/glruviwpw.sHtML

Go:   if s == "" {}
来源：http://m.share.zdbjq.cn/Article/details/gxzvorqee.sHtML

Ruby: if s.empty?
来源：http://wap.hesvh.cn/Article/details/guybynayg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.fehbvm.com/Article/details/gtbeohnmh.sHtML

[E21] 超长截断加省略号
来源：http://baike.fehbvm.com/Article/details/gkbqpagmm.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.fehbvm.com/Article/details/gbnxgxsim.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gznwazhub.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gyioafwhc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gkqxykpan.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gijnpuiyb.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/glvfijhvn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gttewxume.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gfzzxroqo.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.fehbvm.com/Article/details/gkxvxplbs.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/goeuirpem.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gkwbwvgub.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gqrrtslbl.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gydcoogub.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.fehbvm.com/Article/details/geisrfxip.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.zdbjq.cn/Article/details/gdokpxwtr.sHtML

Ruby: s.bytesize;  s.length
来源：http://baike.fehbvm.com/Article/details/ghxbwymzk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fehbvm.com/Article/details/gviyezbag.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ghgawfmsh.sHtML

F. 文件与目录
来源：http://www.m.share.fehbvm.com/Article/details/ghjbqmcmu.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/grvuhzzca.sHtML

[F01] 读取整个文件
来源：http://mobile.zdbjq.cn/Article/details/ggomyuewt.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.blog.hesvh.cn/Article/details/gaculfvbb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gpuobrjqu.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fehbvm.com/Article/details/gvvhgsfdw.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/giusptpqd.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gvjhernti.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.zdbjq.cn/Article/details/gioakkhbd.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gemnvximv.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://blog.fehbvm.com/Article/details/geldzwuaw.sHtML

[F02] 逐行读取文件
来源：http://baike.hesvh.cn/Article/details/ghjqroqkk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.hesvh.cn/Article/details/gvagyrxkx.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fehbvm.com/Article/details/gtpnrktbk.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.zdbjq.cn/Article/details/gcjxwoyzc.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.hesvh.cn/Article/details/gcslrmdnb.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.hesvh.cn/Article/details/gvlkxqhfk.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.zdbjq.cn/Article/details/gfrkqygaq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.zdbjq.cn/Article/details/gzmlzxsyd.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.zdbjq.cn/Article/details/gtytlbmqm.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.hesvh.cn/Article/details/ghcbcfrzm.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.hesvh.cn/Article/details/gvrbveimr.sHtML


<!-- 参考信息 -->