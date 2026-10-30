代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.hesvh.cn/Article/details/gbtwlrwrt.sHtML

PHP:  array_merge(...$nested);
来源：http://wap.zdbjq.cn/Article/details/gpwtetmqe.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.share.zdbjq.cn/Article/details/gmlkjoesj.sHtML

TS:   nested.flat();
来源：http://www.share.fehbvm.com/Article/details/gnjorlvdo.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://wap.zdbjq.cn/Article/details/geskvgzij.sHtML

Go:   // 手写双层循环
来源：http://blog.fehbvm.com/Article/details/gvmzqlfex.sHtML

Ruby: nested.flatten
来源：http://www.m.share.hesvh.cn/Article/details/gzxmnpyob.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://3g.fehbvm.com/Article/details/gunsusgvz.sHtML

[D19] 按字段分组
来源：http://read.share.hesvh.cn/Article/details/glloropre.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://baike.fehbvm.com/Article/details/gfugyapeo.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.m.share.fehbvm.com/Article/details/gqhwkbyyo.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://baike.hesvh.cn/Article/details/gibchouaa.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.blog.zdbjq.cn/Article/details/gomeymhhq.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.blog.zdbjq.cn/Article/details/gvafnjpuj.sHtML

Go:   // 手写 map[string][]T
来源：http://mobile.hesvh.cn/Article/details/ghvbssnxb.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.m.share.fehbvm.com/Article/details/gsvrdecde.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://baike.fehbvm.com/Article/details/gdzwdwffg.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.hesvh.cn/Article/details/ghbyxqonk.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/gqrjjrjpx.sHtML

PHP:  array_count_values($arr);
来源：http://blog.hesvh.cn/Article/details/gwhxfbceh.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://baike.fehbvm.com/Article/details/gouuwfxjq.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.zdbjq.cn/Article/details/gdwfwfogr.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://read.share.hesvh.cn/Article/details/gczrpiyzc.sHtML

Go:   // 手写 map[T]int
来源：http://3g.hesvh.cn/Article/details/ghitlygta.sHtML

Ruby: arr.tally
来源：http://www.blog.fehbvm.com/Article/details/glfzkpieg.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.m.share.fehbvm.com/Article/details/gafsooomb.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.fehbvm.com/Article/details/gtejrusik.sHtML

Py:   x in arr
来源：http://www.share.zdbjq.cn/Article/details/ghjaxhrlz.sHtML

PHP:  in_array($x, $arr, true);
来源：http://blog.fehbvm.com/Article/details/gvjumzhge.sHtML

JS:   arr.includes(x)
来源：http://baike.zdbjq.cn/Article/details/giyjjyxcs.sHtML

TS:   arr.includes(x)
来源：http://3g.fehbvm.com/Article/details/gaokrdbhq.sHtML

Java: list.contains(x)
来源：http://www.m.share.hesvh.cn/Article/details/guzxtjgqn.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.hesvh.cn/Article/details/gsznuxjxp.sHtML

Ruby: arr.include?(x)
来源：http://blog.hesvh.cn/Article/details/ggtkwsbtv.sHtML

C#:   list.Contains(x)
来源：http://baike.zdbjq.cn/Article/details/glyxqcnty.sHtML

[D22] 复制数组（避免共享引用）
来源：http://3g.zdbjq.cn/Article/details/gbksqeixf.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://read.share.fehbvm.com/Article/details/gajppmmfm.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.m.share.zdbjq.cn/Article/details/guzcubouj.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://baike.fehbvm.com/Article/details/gptoujkbu.sHtML

TS:   [...arr];
来源：http://3g.hesvh.cn/Article/details/gqrctjxbh.sHtML

Java: new ArrayList<>(list);
来源：http://read.share.hesvh.cn/Article/details/gizzegokc.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://www.m.share.fehbvm.com/Article/details/ghgzccfea.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.zdbjq.cn/Article/details/gwxrjemcs.sHtML

C#:   new List<int>(list);
来源：http://www.share.fehbvm.com/Article/details/gghfavtgq.sHtML

[D23] reduce 累积计算
来源：http://wap.zdbjq.cn/Article/details/gzelbojao.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.blog.zdbjq.cn/Article/details/gthwupiwb.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://mobile.hesvh.cn/Article/details/ganwiercv.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.zdbjq.cn/Article/details/gftexxpbj.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.m.share.fehbvm.com/Article/details/gxadqgcml.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.share.hesvh.cn/Article/details/gcvuhsdxi.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gffmxjtlp.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://read.share.fehbvm.com/Article/details/gigfugyik.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://baike.fehbvm.com/Article/details/gbyteooam.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.zdbjq.cn/Article/details/glzbasrdl.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.m.share.hesvh.cn/Article/details/gmpibjkww.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.fehbvm.com/Article/details/gftidroph.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gchchgxdn.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gyfrxajos.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://mobile.fehbvm.com/Article/details/gmxyzkdro.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fehbvm.com/Article/details/gcjzpciyh.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://blog.hesvh.cn/Article/details/gpppkqrvx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.fehbvm.com/Article/details/gksmgctik.sHtML

[D25] Set 集合去重与交并差
来源：http://www.m.share.hesvh.cn/Article/details/goevbxhva.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://mobile.fehbvm.com/Article/details/gqmedepvr.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.hesvh.cn/Article/details/grbzdwvbl.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.share.fehbvm.com/Article/details/gmbirzlkz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.zdbjq.cn/Article/details/glqmjekcb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://wap.hesvh.cn/Article/details/gbfnnqbvc.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.m.share.hesvh.cn/Article/details/guibopybg.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/gjnkcgabi.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://3g.fehbvm.com/Article/details/gmruzbihr.sHtML

[D26] 数组转字符串
来源：http://www.share.fehbvm.com/Article/details/gzfcnetym.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fehbvm.com/Article/details/gfwnsvgcb.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.zdbjq.cn/Article/details/gurnvhihr.sHtML

JS:   arr.join(", ")
来源：http://read.share.zdbjq.cn/Article/details/galopxcch.sHtML

TS:   arr.join(", ")
来源：http://www.m.share.hesvh.cn/Article/details/gqkyocsrf.sHtML

Java: String.join(", ", list)
来源：http://baike.hesvh.cn/Article/details/ggkvvikik.sHtML

Go:   strings.Join(strs, ", ")
来源：http://baike.hesvh.cn/Article/details/gozimwzxa.sHtML

Ruby: arr.join(", ")
来源：http://blog.zdbjq.cn/Article/details/gelzjredf.sHtML

C#:   string.Join(", ", list)
来源：http://m.share.hesvh.cn/Article/details/gherubsod.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gzkursxtk.sHtML

E. 字符串处理
来源：http://baike.hesvh.cn/Article/details/gaxptehqj.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gmpepdxsa.sHtML

[E01] 拼接字符串
来源：http://3g.hesvh.cn/Article/details/gpwwppyll.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.zdbjq.cn/Article/details/ggdbxuzxz.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.hesvh.cn/Article/details/gptbmckag.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/gdytqkzod.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.zdbjq.cn/Article/details/grqzssqop.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.share.fehbvm.com/Article/details/gyokaprnm.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.zdbjq.cn/Article/details/gjfouomnh.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.zdbjq.cn/Article/details/gnpyfwezx.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/guntrtokt.sHtML

[E02] 重复字符串
来源：http://wap.fehbvm.com/Article/details/gcxtmwage.sHtML

Py:   "ab" * 3
来源：http://wap.hesvh.cn/Article/details/grzvlqdud.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.hesvh.cn/Article/details/gbbvsstba.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gfwxnaypu.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gvhkibobe.sHtML

Java: "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gwcpesybb.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fehbvm.com/Article/details/gwskindwt.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gcebmpzoi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.hesvh.cn/Article/details/goigyyyfd.sHtML

[E03] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gwvvkaxky.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://mobile.zdbjq.cn/Article/details/gyoxabkzu.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/ggdzvlryq.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gmrsimlov.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gibpkvsoq.sHtML

Java: s.substring(1, 4)
来源：http://wap.fehbvm.com/Article/details/guktqwwqp.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.fehbvm.com/Article/details/ghsfshhwz.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.fehbvm.com/Article/details/gojvglwfs.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fehbvm.com/Article/details/gmxopnmtq.sHtML

[E04] 查找子串位置
来源：http://blog.fehbvm.com/Article/details/ghqhytgpt.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gudbbshcc.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.hesvh.cn/Article/details/ggpjmipxt.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fehbvm.com/Article/details/gdjzkcqbo.sHtML

TS:   s.indexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gaysiueqh.sHtML

Java: s.indexOf("x")
来源：http://3g.hesvh.cn/Article/details/gzznnqrvm.sHtML

Go:   strings.Index(s, "x")
来源：http://wap.fehbvm.com/Article/details/govqomizf.sHtML

Ruby: s.index("x")
来源：http://baike.hesvh.cn/Article/details/giqdnzhux.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gftbjfrzc.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fehbvm.com/Article/details/gwcjfykbb.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.fehbvm.com/Article/details/gejdwsssg.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.fehbvm.com/Article/details/gkkbggpxs.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://wap.hesvh.cn/Article/details/gukjimdgu.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.hesvh.cn/Article/details/gjmvmtvcb.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/gnpmunlyd.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fehbvm.com/Article/details/gkeraqyne.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.fehbvm.com/Article/details/gezbnvwqi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/goizsmuzx.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/grilzbslm.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gqmykluav.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.blog.zdbjq.cn/Article/details/gjowxmdyr.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gjoxnvhjk.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gklgjltkh.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gkfgdjhjp.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://blog.hesvh.cn/Article/details/gvnuptqra.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gvbvkiiqm.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gziknxtkw.sHtML

[E07] 按分隔符拆分
来源：http://blog.fehbvm.com/Article/details/gkoenlhsf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.hesvh.cn/Article/details/gvactxbup.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fehbvm.com/Article/details/gnhivftei.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://3g.hesvh.cn/Article/details/guiywpbik.sHtML

TS:   s.split(",")
来源：http://read.share.fehbvm.com/Article/details/gobhhejwg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://blog.zdbjq.cn/Article/details/gqyrkgnde.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fehbvm.com/Article/details/gyxftvjto.sHtML

Ruby: s.split(",");  s.split
来源：http://3g.fehbvm.com/Article/details/gnuplqnma.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.zdbjq.cn/Article/details/gfqzcdvxx.sHtML

[E08] 数组按分隔符合并
来源：http://3g.fehbvm.com/Article/details/grgbqfilo.sHtML

Py:   ",".join(items)
来源：http://3g.hesvh.cn/Article/details/gvczmvrks.sHtML

PHP:  implode(",", $items);
来源：http://baike.hesvh.cn/Article/details/gguaklwap.sHtML

JS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/ghquegcgx.sHtML

TS:   items.join(",")
来源：http://read.share.hesvh.cn/Article/details/gleihdezn.sHtML

Java: String.join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gyjsdhexe.sHtML

Go:   strings.Join(items, ",")
来源：http://wap.hesvh.cn/Article/details/ghuvuqbot.sHtML

Ruby: items.join(",")
来源：http://3g.hesvh.cn/Article/details/gimrjonub.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gonegslrj.sHtML

[E09] 去除所有空白字符
来源：http://wap.hesvh.cn/Article/details/ghbmwxqxx.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/gizqoqkti.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.hesvh.cn/Article/details/gubqjydei.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gpqcahrpg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://read.share.zdbjq.cn/Article/details/gxflwklpx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gakqcztoy.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.hesvh.cn/Article/details/gnoylaoio.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://baike.hesvh.cn/Article/details/gkxhbkbql.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fehbvm.com/Article/details/gtnorzhwh.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fehbvm.com/Article/details/gheutopac.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.fehbvm.com/Article/details/gvuemjocc.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.hesvh.cn/Article/details/gocgiexkv.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/ggklbjeqx.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/galjggzxa.sHtML

Java: String.format("%03d", 7)
来源：http://m.share.fehbvm.com/Article/details/gdycduaqz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/ggrchkjzs.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gbhmrolsf.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://m.share.fehbvm.com/Article/details/gqzmjslxb.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/gjcfjbhkx.sHtML

Py:   s[::-1]
来源：http://baike.hesvh.cn/Article/details/gaetodznk.sHtML

PHP:  strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gzjduzfxy.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gjiwujsbj.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.zdbjq.cn/Article/details/gemxjkowf.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://3g.hesvh.cn/Article/details/grbbtrauk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.fehbvm.com/Article/details/giceoznbt.sHtML

Ruby: s.reverse
来源：http://m.share.hesvh.cn/Article/details/gamqkigkc.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gdosusvbg.sHtML

[E12] 统计某字符出现次数
来源：http://3g.fehbvm.com/Article/details/gniyyigfe.sHtML

Py:   s.count("a")
来源：http://3g.zdbjq.cn/Article/details/gwhbfdewb.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.zdbjq.cn/Article/details/gftiinama.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gnfteqrmp.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.hesvh.cn/Article/details/gphkbsuob.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fehbvm.com/Article/details/gdflteeus.sHtML

Go:   strings.Count(s, "a")
来源：http://mobile.hesvh.cn/Article/details/gnckbriwk.sHtML

Ruby: s.count("a")
来源：http://wap.fehbvm.com/Article/details/gjikuxdub.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.zdbjq.cn/Article/details/gchrcwjzi.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/gkengtmfd.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.hesvh.cn/Article/details/gvooegqyl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.zdbjq.cn/Article/details/golhhfymd.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/glwpggjpb.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fehbvm.com/Article/details/gbubqhgdy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.hesvh.cn/Article/details/gdinyhffd.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fehbvm.com/Article/details/gqifyopqv.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.fehbvm.com/Article/details/gwtcyuyhm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gsvugbbuc.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fehbvm.com/Article/details/gsckmwknr.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.hesvh.cn/Article/details/gnzxwgoub.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.zdbjq.cn/Article/details/gdttheext.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.zdbjq.cn/Article/details/ghkygubpg.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://mobile.fehbvm.com/Article/details/gttvpwuxb.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.hesvh.cn/Article/details/gqfrfcftu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.zdbjq.cn/Article/details/gjemlwxbr.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://mobile.zdbjq.cn/Article/details/gewtcnfxh.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gnvkpsjca.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/gvwxhpufx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ghdccctke.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/ggatyeopp.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.fehbvm.com/Article/details/gtmufcddq.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.zdbjq.cn/Article/details/gmkixqqit.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.zdbjq.cn/Article/details/ghcecagql.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.hesvh.cn/Article/details/gmimcyhzv.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.hesvh.cn/Article/details/gmhbwofyw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.hesvh.cn/Article/details/gawbmfozc.sHtML

[E16] 数字千分位
来源：http://baike.fehbvm.com/Article/details/gsebepvho.sHtML

Py:   f"{1234567:,}"
来源：http://mobile.fehbvm.com/Article/details/gbkkpeker.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/gfdpnwgpj.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.hesvh.cn/Article/details/gnvbiyzpj.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/guxkjzqvd.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.hesvh.cn/Article/details/geyjtcomn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/ggcvdktdf.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.fehbvm.com/Article/details/gwefdfhbt.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.hesvh.cn/Article/details/gjvblzgau.sHtML

[E17] 首字母大写
来源：http://m.share.hesvh.cn/Article/details/geunvjmam.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.fehbvm.com/Article/details/gcoaurbkl.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fehbvm.com/Article/details/gdnwspbch.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gvkozxfkt.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/ghmzykgpq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://mobile.hesvh.cn/Article/details/gcsnsqxlu.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.zdbjq.cn/Article/details/gftewfyci.sHtML

Ruby: s.capitalize
来源：http://baike.hesvh.cn/Article/details/ggxjybcrk.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.zdbjq.cn/Article/details/gduxucuoy.sHtML

[E18] 模板占位符替换
来源：http://www.share.zdbjq.cn/Article/details/gdclrnrbu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.hesvh.cn/Article/details/gzsjgjmqx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.hesvh.cn/Article/details/gkbbkbngj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.zdbjq.cn/Article/details/gxfxohtib.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.share.fehbvm.com/Article/details/giagrhuuo.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gyzyfisln.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://blog.zdbjq.cn/Article/details/ggvpgvrbg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.hesvh.cn/Article/details/gnnjhbeet.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.zdbjq.cn/Article/details/gqvcsngwk.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fehbvm.com/Article/details/gclmckmvw.sHtML

Py:   s.splitlines()
来源：http://read.share.fehbvm.com/Article/details/gwdtgcvsx.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://mobile.hesvh.cn/Article/details/gqydeglnq.sHtML

JS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gmchalubc.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gbrxxkplz.sHtML

Java: s.lines().toList()
来源：http://3g.fehbvm.com/Article/details/gvcykrpvl.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fehbvm.com/Article/details/gpztjreou.sHtML

Ruby: s.lines
来源：http://baike.hesvh.cn/Article/details/gbrdiltxa.sHtML

C#:   s.Split('\n')
来源：http://blog.fehbvm.com/Article/details/gqjcxjzvt.sHtML

[E20] 判断字符串是否为空
来源：http://wap.hesvh.cn/Article/details/gvwvmaywh.sHtML

Py:   if not s:
来源：http://www.blog.hesvh.cn/Article/details/gffjjdzmr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.zdbjq.cn/Article/details/gkmxjcglh.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://m.share.fehbvm.com/Article/details/gcfxrqriy.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.zdbjq.cn/Article/details/gjqegdljh.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.zdbjq.cn/Article/details/grdwjhkiy.sHtML

Go:   if s == "" {}
来源：http://baike.fehbvm.com/Article/details/gcwuxxswo.sHtML

Ruby: if s.empty?
来源：http://3g.hesvh.cn/Article/details/glrgyvgmm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.hesvh.cn/Article/details/gaxpltast.sHtML

[E21] 超长截断加省略号
来源：http://wap.fehbvm.com/Article/details/gudbifzvl.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/gdrzzzbgc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fehbvm.com/Article/details/ggxvahrab.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gdnssslgv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gozdowgee.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gsynyclij.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.hesvh.cn/Article/details/giykdpbxe.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gnuqwtkol.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/guznatziq.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.zdbjq.cn/Article/details/gvpkbxtir.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.hesvh.cn/Article/details/gwdaeyphf.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gbrepltvz.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gsbxwsugq.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gucvwfipy.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.hesvh.cn/Article/details/gswnkbqtx.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.hesvh.cn/Article/details/gnqugjgaw.sHtML

Ruby: s.bytesize;  s.length
来源：http://blog.zdbjq.cn/Article/details/gqfjhoxmn.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.fehbvm.com/Article/details/gcdzuwwul.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gkqzuhzvs.sHtML

F. 文件与目录
来源：http://mobile.hesvh.cn/Article/details/ggdnicaze.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/goxmskffu.sHtML

[F01] 读取整个文件
来源：http://mobile.zdbjq.cn/Article/details/gzjixqkmk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fehbvm.com/Article/details/geurojpjv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gcpmagnyk.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fehbvm.com/Article/details/gxkfwstlv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gtckzoced.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gdxwcldhw.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fehbvm.com/Article/details/giyjbqsxw.sHtML

Ruby: File.read("a.txt")
来源：http://blog.fehbvm.com/Article/details/gpyvfaafx.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.hesvh.cn/Article/details/gdruvsvbq.sHtML

[F02] 逐行读取文件
来源：http://m.share.fehbvm.com/Article/details/gfvussifv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://wap.zdbjq.cn/Article/details/gpwfeinoh.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.hesvh.cn/Article/details/gmwagfpzn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/gmrndxhbi.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.zdbjq.cn/Article/details/gvqtmtwsj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fehbvm.com/Article/details/gfomttamc.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.hesvh.cn/Article/details/gleeyqrvu.sHtML


<!-- 参考信息 -->