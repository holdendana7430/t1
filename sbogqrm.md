代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://blog.zdbjq.cn/Article/details/grccyyabt.sHtML

Ruby: arr.max;  arr.min
来源：http://www.blog.zdbjq.cn/Article/details/ghgezybtw.sHtML

C#:   list.Max();  list.Min()
来源：http://read.share.fehbvm.com/Article/details/gjdfblwen.sHtML

[D18] 扁平化嵌套数组
来源：http://baike.zdbjq.cn/Article/details/glxrzwdti.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://blog.zdbjq.cn/Article/details/gutijiarz.sHtML

PHP:  array_merge(...$nested);
来源：http://mobile.fehbvm.com/Article/details/gqxstpgua.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://m.share.hesvh.cn/Article/details/gibsaqdgb.sHtML

TS:   nested.flat();
来源：http://www.share.hesvh.cn/Article/details/godcjuunu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://blog.fehbvm.com/Article/details/gwautexrr.sHtML

Go:   // 手写双层循环
来源：http://www.share.zdbjq.cn/Article/details/gtynqxuut.sHtML

Ruby: nested.flatten
来源：http://3g.fehbvm.com/Article/details/gorffeziz.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://wap.hesvh.cn/Article/details/gnyymaeci.sHtML

[D19] 按字段分组
来源：http://mobile.fehbvm.com/Article/details/gpzdyvzih.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://blog.fehbvm.com/Article/details/gzewgtbzq.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://read.share.hesvh.cn/Article/details/gpoygmtjv.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://m.share.fehbvm.com/Article/details/gxytfactn.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://wap.zdbjq.cn/Article/details/gzrflkuqn.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://blog.hesvh.cn/Article/details/gkdtioime.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/gcumordkd.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.zdbjq.cn/Article/details/gfeojvcjl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.zdbjq.cn/Article/details/gjwzswvqy.sHtML

[D20] 统计每个元素出现次数
来源：http://m.share.zdbjq.cn/Article/details/gctmilowr.sHtML

Py:   Counter(arr)
来源：http://mobile.hesvh.cn/Article/details/gdjocivlw.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.hesvh.cn/Article/details/gxsoubego.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://m.share.zdbjq.cn/Article/details/gdfdbjoic.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://blog.zdbjq.cn/Article/details/gtfkiuyer.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://blog.hesvh.cn/Article/details/grfsmszub.sHtML

Go:   // 手写 map[T]int
来源：http://www.share.fehbvm.com/Article/details/glgeppusz.sHtML

Ruby: arr.tally
来源：http://mobile.zdbjq.cn/Article/details/gzvqfzkdm.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/gsztsygae.sHtML

[D21] 判断是否包含某元素
来源：http://blog.zdbjq.cn/Article/details/gqctopfyx.sHtML

Py:   x in arr
来源：http://blog.fehbvm.com/Article/details/ggyhunjmq.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.zdbjq.cn/Article/details/genzjoemq.sHtML

JS:   arr.includes(x)
来源：http://baike.fehbvm.com/Article/details/gdidcfayf.sHtML

TS:   arr.includes(x)
来源：http://mobile.fehbvm.com/Article/details/grzlpbsjp.sHtML

Java: list.contains(x)
来源：http://wap.zdbjq.cn/Article/details/gowkxhfib.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.zdbjq.cn/Article/details/gmdsqswxn.sHtML

Ruby: arr.include?(x)
来源：http://www.m.share.hesvh.cn/Article/details/goklsglyh.sHtML

C#:   list.Contains(x)
来源：http://mobile.zdbjq.cn/Article/details/gqanjumnr.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.hesvh.cn/Article/details/gaudwvaer.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.fehbvm.com/Article/details/godaezkho.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://mobile.fehbvm.com/Article/details/gensrcdej.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.fehbvm.com/Article/details/gftezyzqe.sHtML

TS:   [...arr];
来源：http://mobile.fehbvm.com/Article/details/gbnadoyxq.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.zdbjq.cn/Article/details/gtsvgvpsi.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.fehbvm.com/Article/details/gwpiacyxz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.zdbjq.cn/Article/details/gwalglgdq.sHtML

C#:   new List<int>(list);
来源：http://www.blog.hesvh.cn/Article/details/gwzbskhza.sHtML

[D23] reduce 累积计算
来源：http://blog.hesvh.cn/Article/details/gbixgazkx.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.zdbjq.cn/Article/details/gzveekrbs.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.fehbvm.com/Article/details/gkyvzqvhn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.blog.fehbvm.com/Article/details/gvsqnjfjp.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gorsfrznk.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.hesvh.cn/Article/details/gguccfoom.sHtML

Go:   // 手写循环
来源：http://www.m.share.fehbvm.com/Article/details/gohfogvlo.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://baike.zdbjq.cn/Article/details/gefjmvafm.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://mobile.zdbjq.cn/Article/details/gjkgazfaa.sHtML

[D24] 字典 / Map 基本操作
来源：http://blog.hesvh.cn/Article/details/gwfkbhvtp.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.hesvh.cn/Article/details/gbzlkkqnh.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://m.share.zdbjq.cn/Article/details/govryyfdk.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://read.share.zdbjq.cn/Article/details/glgjdmaep.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gdvyprwqe.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://baike.zdbjq.cn/Article/details/gxyhnmzal.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://mobile.zdbjq.cn/Article/details/gukvutjaf.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.fehbvm.com/Article/details/gedheinpp.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.hesvh.cn/Article/details/gkdglxlxk.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.zdbjq.cn/Article/details/galochdsj.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fehbvm.com/Article/details/gsjdhuspz.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.hesvh.cn/Article/details/gyoppmnxa.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.hesvh.cn/Article/details/gtnserepz.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://wap.fehbvm.com/Article/details/glkvsmtxh.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://3g.hesvh.cn/Article/details/gmdowovuv.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.blog.zdbjq.cn/Article/details/gdrelvbmf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.hesvh.cn/Article/details/govnevgzn.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://read.share.hesvh.cn/Article/details/gucbddzca.sHtML

[D26] 数组转字符串
来源：http://www.share.fehbvm.com/Article/details/gjhobtsld.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.fehbvm.com/Article/details/gcnnutbrt.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.zdbjq.cn/Article/details/gpywexslo.sHtML

JS:   arr.join(", ")
来源：http://mobile.fehbvm.com/Article/details/gnvzyfahp.sHtML

TS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gdahahpbm.sHtML

Java: String.join(", ", list)
来源：http://m.share.zdbjq.cn/Article/details/gvlbjcfmt.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.hesvh.cn/Article/details/gbxvlkzid.sHtML

Ruby: arr.join(", ")
来源：http://mobile.zdbjq.cn/Article/details/ggtvzgcoe.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gstjjolqu.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gfxfmsfqx.sHtML

E. 字符串处理
来源：http://mobile.fehbvm.com/Article/details/gxaueuqjv.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/guifujfbc.sHtML

[E01] 拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gnblkldqa.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.zdbjq.cn/Article/details/gdloaffor.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fehbvm.com/Article/details/gxdgvjnkw.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gxhkigaqd.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/ggqrwxnqj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.fehbvm.com/Article/details/grffzbyif.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.zdbjq.cn/Article/details/govgzslch.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.zdbjq.cn/Article/details/gpxzvzonr.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/grgcozemd.sHtML

[E02] 重复字符串
来源：http://www.blog.fehbvm.com/Article/details/gskussemv.sHtML

Py:   "ab" * 3
来源：http://www.share.zdbjq.cn/Article/details/gttjnyohx.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.fehbvm.com/Article/details/gwgbxsxpn.sHtML

JS:   "ab".repeat(3)
来源：http://3g.zdbjq.cn/Article/details/gtdehzhqf.sHtML

TS:   "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gekzpduby.sHtML

Java: "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gqdilkbfk.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://wap.hesvh.cn/Article/details/ggroqmldz.sHtML

Ruby: "ab" * 3
来源：http://baike.hesvh.cn/Article/details/gkfcqprrn.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.share.zdbjq.cn/Article/details/greztizou.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gwjmjjgon.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/gpgenmvak.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/ghnzyaodv.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/guiqxsdad.sHtML

TS:   s.slice(1, 4)
来源：http://mobile.hesvh.cn/Article/details/gxhktrwmn.sHtML

Java: s.substring(1, 4)
来源：http://3g.hesvh.cn/Article/details/gxrljgjbi.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.hesvh.cn/Article/details/grllpsvqi.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.zdbjq.cn/Article/details/gmgipgfmq.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.zdbjq.cn/Article/details/gwkmcgmqb.sHtML

[E04] 查找子串位置
来源：http://www.m.share.zdbjq.cn/Article/details/gkrqzpwvf.sHtML

Py:   s.find("x");  s.index("x")
来源：http://read.share.zdbjq.cn/Article/details/gkejvcjil.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.fehbvm.com/Article/details/gtnvohawu.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.hesvh.cn/Article/details/gpwdhlghd.sHtML

TS:   s.indexOf("x")
来源：http://blog.hesvh.cn/Article/details/gufqfnkzm.sHtML

Java: s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gpktsmqyf.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.fehbvm.com/Article/details/gkweyzsiy.sHtML

Ruby: s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/gmzbzuvtn.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gvmnlhylb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.fehbvm.com/Article/details/gczxmlzys.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://read.share.hesvh.cn/Article/details/gaacstdbx.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://3g.fehbvm.com/Article/details/ggssbwcxj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/grmpjotqo.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://baike.fehbvm.com/Article/details/gtcjnrrca.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.hesvh.cn/Article/details/gseyyyxym.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.m.share.fehbvm.com/Article/details/gyjtpgvzi.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.m.share.fehbvm.com/Article/details/gueysexmj.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://mobile.hesvh.cn/Article/details/gkccqdbcn.sHtML

[E06] 替换子串
来源：http://www.share.fehbvm.com/Article/details/gvprandfv.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gavumtuwv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://wap.hesvh.cn/Article/details/ggnygnvda.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gdvjedpew.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gupihpymj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/ggsdmakmz.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gkllcxbpj.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gcyqgksuw.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gorbezphz.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.hesvh.cn/Article/details/gtpnqhwuf.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.hesvh.cn/Article/details/gptqmqvrl.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/gmgzjesow.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fehbvm.com/Article/details/ghxrklgfd.sHtML

TS:   s.split(",")
来源：http://blog.zdbjq.cn/Article/details/grfxptlcb.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.hesvh.cn/Article/details/gbdiukpad.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://3g.zdbjq.cn/Article/details/gzaabfncu.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/grwkopdba.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.hesvh.cn/Article/details/ghloohtjz.sHtML

[E08] 数组按分隔符合并
来源：http://wap.zdbjq.cn/Article/details/geeykddgp.sHtML

Py:   ",".join(items)
来源：http://mobile.fehbvm.com/Article/details/gxkvobyoz.sHtML

PHP:  implode(",", $items);
来源：http://mobile.hesvh.cn/Article/details/gnzbtplkq.sHtML

JS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gtxjutzon.sHtML

TS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gebfrbdnl.sHtML

Java: String.join(",", items)
来源：http://blog.fehbvm.com/Article/details/goohwlgon.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.fehbvm.com/Article/details/gfmroexmv.sHtML

Ruby: items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gxqvbeeqp.sHtML

C#:   string.Join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gsvdlclkz.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/gpfsorhps.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://3g.fehbvm.com/Article/details/gfjmyppkb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/golfvjpni.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.zdbjq.cn/Article/details/gymfknbvl.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gxvflwlzo.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.zdbjq.cn/Article/details/gkqieghhp.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.zdbjq.cn/Article/details/giegbybyl.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fehbvm.com/Article/details/gzerwaunx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.zdbjq.cn/Article/details/gjcyylnnr.sHtML

[E10] 左侧补零 / 定长填充
来源：http://m.share.zdbjq.cn/Article/details/gjuwbtixq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://blog.zdbjq.cn/Article/details/gjefdkiji.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://blog.fehbvm.com/Article/details/gozvgntnl.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/gvaotyfjn.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.fehbvm.com/Article/details/gwwbiyjqk.sHtML

Java: String.format("%03d", 7)
来源：http://www.blog.fehbvm.com/Article/details/ggiibhhao.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/ggisdxnll.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gpvrsockh.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.fehbvm.com/Article/details/gbunlnzbg.sHtML

[E11] 反转字符串
来源：http://www.m.share.fehbvm.com/Article/details/gitasydhf.sHtML

Py:   s[::-1]
来源：http://www.share.hesvh.cn/Article/details/gusbxgnqi.sHtML

PHP:  strrev($s);
来源：http://www.share.zdbjq.cn/Article/details/gsldkgwlg.sHtML

JS:   [...s].reverse().join("")
来源：http://3g.hesvh.cn/Article/details/gxedeyzjn.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gsgvnefwb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://baike.zdbjq.cn/Article/details/gpytfdmaq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.zdbjq.cn/Article/details/guvlbxrtf.sHtML

Ruby: s.reverse
来源：http://baike.hesvh.cn/Article/details/gdrtqvwkp.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gfspapslo.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.fehbvm.com/Article/details/gxaczaush.sHtML

Py:   s.count("a")
来源：http://www.share.zdbjq.cn/Article/details/gurqeynwr.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.hesvh.cn/Article/details/gbtxztfrr.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/grlsdnhmc.sHtML

TS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gcqmthkyj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.zdbjq.cn/Article/details/gnixppyvr.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.hesvh.cn/Article/details/gtsoehevj.sHtML

Ruby: s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gdlzjzqgn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.zdbjq.cn/Article/details/gemqcqafn.sHtML

[E13] 逐字符遍历
来源：http://blog.fehbvm.com/Article/details/gkjqxqxtg.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.hesvh.cn/Article/details/gspbdysmb.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.fehbvm.com/Article/details/gxlocblbp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/glmzekyii.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/glysimqkr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/gxnftsamc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://mobile.fehbvm.com/Article/details/gzxqpkaow.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.zdbjq.cn/Article/details/gzhnqokqb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.fehbvm.com/Article/details/gupdcmhsy.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fehbvm.com/Article/details/ghfgafjfw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.zdbjq.cn/Article/details/gsjbjekcm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.zdbjq.cn/Article/details/gdkkhtpqb.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.fehbvm.com/Article/details/gikiafqkp.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://wap.zdbjq.cn/Article/details/grmecndev.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gzmvrmdes.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fehbvm.com/Article/details/ghxedlesy.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.fehbvm.com/Article/details/gmdvxredb.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gtewkrmbs.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.hesvh.cn/Article/details/gaknepkld.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.fehbvm.com/Article/details/gygtqdppw.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.fehbvm.com/Article/details/gvtgmcrib.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.hesvh.cn/Article/details/gfmvpwtmg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.zdbjq.cn/Article/details/gvfwsbvbo.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.hesvh.cn/Article/details/gwiitgwnl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.zdbjq.cn/Article/details/gfpguasbm.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.zdbjq.cn/Article/details/gpndkgpdi.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.hesvh.cn/Article/details/gegumchej.sHtML

[E16] 数字千分位
来源：http://baike.fehbvm.com/Article/details/gpmerrhwb.sHtML

Py:   f"{1234567:,}"
来源：http://blog.zdbjq.cn/Article/details/gmsuxiiwn.sHtML

PHP:  number_format(1234567);
来源：http://baike.hesvh.cn/Article/details/gdlurnafz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gssvuerol.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.fehbvm.com/Article/details/gsybwylll.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.fehbvm.com/Article/details/grjjjvbij.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.fehbvm.com/Article/details/gwmvfcrog.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fehbvm.com/Article/details/ghoyjukiv.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.fehbvm.com/Article/details/gtzjbudoq.sHtML

[E17] 首字母大写
来源：http://3g.fehbvm.com/Article/details/gnvnzehef.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.hesvh.cn/Article/details/gbgltskho.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://3g.zdbjq.cn/Article/details/glhsdjaqq.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gezibeuzn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.fehbvm.com/Article/details/gnzbmpjmj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.zdbjq.cn/Article/details/gbemmljdp.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.fehbvm.com/Article/details/gwwtwuxrv.sHtML

Ruby: s.capitalize
来源：http://baike.zdbjq.cn/Article/details/gzkfooigg.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/gaufvbjke.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fehbvm.com/Article/details/ggaqokbvi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.hesvh.cn/Article/details/goeaujjsf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.fehbvm.com/Article/details/gqorcmcxr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gcsagvogy.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gmrpiutcj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gwvnxhhfz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gasgdkqba.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.zdbjq.cn/Article/details/gxyvtugaw.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.zdbjq.cn/Article/details/ghweknyog.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.zdbjq.cn/Article/details/gudadtugq.sHtML

Py:   s.splitlines()
来源：http://wap.zdbjq.cn/Article/details/gbktedvna.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gncjokzea.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/ghaawavgc.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gkreewtej.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/gzsrurspx.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fehbvm.com/Article/details/gymyoumil.sHtML

Ruby: s.lines
来源：http://www.blog.hesvh.cn/Article/details/grbfvumss.sHtML

C#:   s.Split('\n')
来源：http://blog.hesvh.cn/Article/details/gfbuzjczf.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.fehbvm.com/Article/details/gzqoqsehl.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/gvwbqidky.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.hesvh.cn/Article/details/gcxaseuog.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.zdbjq.cn/Article/details/gbpimykun.sHtML

TS:   if (s === "") {}
来源：http://www.share.hesvh.cn/Article/details/gdtdseloa.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.zdbjq.cn/Article/details/gobnsjdgj.sHtML

Go:   if s == "" {}
来源：http://www.share.fehbvm.com/Article/details/gtnjdihoq.sHtML

Ruby: if s.empty?
来源：http://www.m.share.hesvh.cn/Article/details/gnyqgjync.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fehbvm.com/Article/details/gryqajbod.sHtML

[E21] 超长截断加省略号
来源：http://m.share.hesvh.cn/Article/details/gjttsrdqp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fehbvm.com/Article/details/gajdxuvmy.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gcckmmpde.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/ggaixpdlu.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gxlyqjmcq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gvpiknsem.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.hesvh.cn/Article/details/gougrxszf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gmdlfapod.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/grponcprc.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fehbvm.com/Article/details/gxrzktikd.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://mobile.fehbvm.com/Article/details/gpvqvwzqq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/ggpcuatsm.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.fehbvm.com/Article/details/gtpcrupql.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gmhwyrmef.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.hesvh.cn/Article/details/gywmkeyqg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.hesvh.cn/Article/details/glkvcvbxw.sHtML

Ruby: s.bytesize;  s.length
来源：http://3g.fehbvm.com/Article/details/gromtfjgf.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/ghovaesgi.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gnekivzvi.sHtML

F. 文件与目录
来源：http://wap.hesvh.cn/Article/details/gixplnsum.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gkyqjpzjr.sHtML

[F01] 读取整个文件
来源：http://3g.zdbjq.cn/Article/details/gslhtbnba.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.hesvh.cn/Article/details/giyqcisnj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.hesvh.cn/Article/details/gfnmwhiyl.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fehbvm.com/Article/details/glppkgcek.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.hesvh.cn/Article/details/grgdnsyhv.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gqqyqlzyd.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.zdbjq.cn/Article/details/gykrxoeos.sHtML

Ruby: File.read("a.txt")
来源：http://wap.hesvh.cn/Article/details/gatmtnycs.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gemgbqysr.sHtML

[F02] 逐行读取文件
来源：http://wap.fehbvm.com/Article/details/gfnpwzeko.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fehbvm.com/Article/details/gfltnukew.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.share.fehbvm.com/Article/details/gupwfjlxw.sHtML


<!-- 参考信息 -->