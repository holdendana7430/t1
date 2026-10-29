代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://m.share.fehbvm.com/Article/details/gekksdsvo.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.share.fehbvm.com/Article/details/gnmsacyyv.sHtML

TS:   Math.max(...arr);
来源：http://3g.hesvh.cn/Article/details/grfgffjcj.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://3g.zdbjq.cn/Article/details/guwwxewtd.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://read.share.hesvh.cn/Article/details/ggwbekwwn.sHtML

Ruby: arr.max;  arr.min
来源：http://3g.fehbvm.com/Article/details/gmyxgkkft.sHtML

C#:   list.Max();  list.Min()
来源：http://www.m.share.zdbjq.cn/Article/details/glyhzfxoe.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.hesvh.cn/Article/details/gfegaeyvj.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://3g.zdbjq.cn/Article/details/gpfvnhzxd.sHtML

PHP:  array_merge(...$nested);
来源：http://www.m.share.hesvh.cn/Article/details/gabdsdikg.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.blog.hesvh.cn/Article/details/guxspzhpp.sHtML

TS:   nested.flat();
来源：http://baike.fehbvm.com/Article/details/gsxgvyuxu.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://read.share.hesvh.cn/Article/details/ghasgdned.sHtML

Go:   // 手写双层循环
来源：http://baike.hesvh.cn/Article/details/gbhpkvome.sHtML

Ruby: nested.flatten
来源：http://www.blog.zdbjq.cn/Article/details/gocdjrstl.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://m.share.hesvh.cn/Article/details/gaevlizli.sHtML

[D19] 按字段分组
来源：http://mobile.hesvh.cn/Article/details/gcqyakaby.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.m.share.fehbvm.com/Article/details/gbqvdntma.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://wap.fehbvm.com/Article/details/gsomktwzk.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/gpormswzj.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.zdbjq.cn/Article/details/gtvqvnzsa.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://wap.zdbjq.cn/Article/details/gpcaymmln.sHtML

Go:   // 手写 map[string][]T
来源：http://m.share.hesvh.cn/Article/details/gbbltekhe.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://baike.hesvh.cn/Article/details/gcijnbwfu.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.share.fehbvm.com/Article/details/gwprasjtz.sHtML

[D20] 统计每个元素出现次数
来源：http://www.share.fehbvm.com/Article/details/gagwqiayp.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/gupeuqyrl.sHtML

PHP:  array_count_values($arr);
来源：http://www.share.hesvh.cn/Article/details/gbhmolspm.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.fehbvm.com/Article/details/gutzebuhg.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://3g.hesvh.cn/Article/details/ggnjmuxuo.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.m.share.fehbvm.com/Article/details/gwlvhypzi.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.hesvh.cn/Article/details/gbuerwkds.sHtML

Ruby: arr.tally
来源：http://3g.fehbvm.com/Article/details/girgbpbli.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.fehbvm.com/Article/details/gritmkygh.sHtML

[D21] 判断是否包含某元素
来源：http://baike.fehbvm.com/Article/details/gausjkxjh.sHtML

Py:   x in arr
来源：http://www.share.zdbjq.cn/Article/details/gcbzmlclv.sHtML

PHP:  in_array($x, $arr, true);
来源：http://wap.fehbvm.com/Article/details/gtefpatmp.sHtML

JS:   arr.includes(x)
来源：http://m.share.hesvh.cn/Article/details/ghwceizmv.sHtML

TS:   arr.includes(x)
来源：http://www.share.hesvh.cn/Article/details/glodijhcx.sHtML

Java: list.contains(x)
来源：http://www.blog.zdbjq.cn/Article/details/guxxrclbk.sHtML

Go:   slices.Contains(arr, x)
来源：http://3g.fehbvm.com/Article/details/gjcoeijkd.sHtML

Ruby: arr.include?(x)
来源：http://blog.fehbvm.com/Article/details/gaasszpcn.sHtML

C#:   list.Contains(x)
来源：http://www.blog.fehbvm.com/Article/details/glkjsqwuk.sHtML

[D22] 复制数组（避免共享引用）
来源：http://baike.hesvh.cn/Article/details/gempsdzst.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://mobile.zdbjq.cn/Article/details/grbiytudt.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://wap.zdbjq.cn/Article/details/gcrxpzvrl.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gpgkgxjeu.sHtML

TS:   [...arr];
来源：http://www.blog.fehbvm.com/Article/details/gnjoosikt.sHtML

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/goosjwocv.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fehbvm.com/Article/details/gzjrukclu.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.blog.zdbjq.cn/Article/details/ghjrbdiaf.sHtML

C#:   new List<int>(list);
来源：http://mobile.fehbvm.com/Article/details/gsmgoslyx.sHtML

[D23] reduce 累积计算
来源：http://wap.zdbjq.cn/Article/details/gdkxkljeu.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://baike.hesvh.cn/Article/details/ggowdihgp.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.zdbjq.cn/Article/details/gjouhokwy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.hesvh.cn/Article/details/gsnlfffiu.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.fehbvm.com/Article/details/gmvdpdtqs.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://read.share.fehbvm.com/Article/details/glbuibbrx.sHtML

Go:   // 手写循环
来源：http://www.share.fehbvm.com/Article/details/gjxxatyij.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://m.share.fehbvm.com/Article/details/gxfnoujdg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.fehbvm.com/Article/details/guhcirbks.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.blog.zdbjq.cn/Article/details/gicitcudu.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://3g.fehbvm.com/Article/details/guqyvhxxe.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.share.hesvh.cn/Article/details/gfkludumt.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.fehbvm.com/Article/details/ghiziirbj.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://wap.fehbvm.com/Article/details/gfftqsogn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://m.share.hesvh.cn/Article/details/gyzxdlprs.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.zdbjq.cn/Article/details/gmarckkbg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://baike.zdbjq.cn/Article/details/gbtpduaur.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.share.zdbjq.cn/Article/details/gngajhhbf.sHtML

[D25] Set 集合去重与交并差
来源：http://mobile.fehbvm.com/Article/details/ggjzehimr.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fehbvm.com/Article/details/gaevnrrdp.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://blog.fehbvm.com/Article/details/gitegdkyv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.blog.fehbvm.com/Article/details/grirkolxa.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fehbvm.com/Article/details/guxghosvw.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.zdbjq.cn/Article/details/gfzkiqpxn.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fehbvm.com/Article/details/gauykftlk.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.blog.hesvh.cn/Article/details/glydgtzvs.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.zdbjq.cn/Article/details/glervxxbj.sHtML

[D26] 数组转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gfgokbtsi.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.hesvh.cn/Article/details/gdwinuonf.sHtML

PHP:  implode(", ", $arr);
来源：http://3g.fehbvm.com/Article/details/gbxwvzeyk.sHtML

JS:   arr.join(", ")
来源：http://m.share.zdbjq.cn/Article/details/gmfvvzqsn.sHtML

TS:   arr.join(", ")
来源：http://3g.zdbjq.cn/Article/details/glmmqhuvg.sHtML

Java: String.join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gkkqvyrzc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/gewyeilwt.sHtML

Ruby: arr.join(", ")
来源：http://wap.zdbjq.cn/Article/details/ghxvqvnim.sHtML

C#:   string.Join(", ", list)
来源：http://www.blog.zdbjq.cn/Article/details/gekbzloly.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gnfwhjuqd.sHtML

E. 字符串处理
来源：http://www.blog.hesvh.cn/Article/details/gcykwkige.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gcqnykxlk.sHtML

[E01] 拼接字符串
来源：http://wap.zdbjq.cn/Article/details/gidytperu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://3g.hesvh.cn/Article/details/gqvgpdqgg.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://blog.hesvh.cn/Article/details/gxpqmsypj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/grobhsyzd.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.fehbvm.com/Article/details/gswclsvet.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://3g.fehbvm.com/Article/details/gfhvtfkyd.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://m.share.fehbvm.com/Article/details/gfbgvnwpr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.blog.fehbvm.com/Article/details/gdkyvngjb.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gbuujumqd.sHtML

[E02] 重复字符串
来源：http://www.m.share.hesvh.cn/Article/details/gpxrrgrcb.sHtML

Py:   "ab" * 3
来源：http://3g.fehbvm.com/Article/details/glondknjb.sHtML

PHP:  str_repeat("ab", 3);
来源：http://blog.hesvh.cn/Article/details/gijfgfusq.sHtML

JS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gtbdupfdx.sHtML

TS:   "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gulzdlhfd.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.hesvh.cn/Article/details/gqxjilmpf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.hesvh.cn/Article/details/gneglpjbk.sHtML

Ruby: "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gbamccegi.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.zdbjq.cn/Article/details/grypxnakr.sHtML

[E03] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gnwldujoh.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.fehbvm.com/Article/details/gwkayacov.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.zdbjq.cn/Article/details/gjnxvgteh.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gigphqxmk.sHtML

TS:   s.slice(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gmarsqnhw.sHtML

Java: s.substring(1, 4)
来源：http://wap.zdbjq.cn/Article/details/gatkkcjed.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.hesvh.cn/Article/details/ghqffgcut.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.hesvh.cn/Article/details/gbauhkbxh.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.fehbvm.com/Article/details/gqcioigxg.sHtML

[E04] 查找子串位置
来源：http://www.m.share.hesvh.cn/Article/details/ggajglejr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gnnjrtgti.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fehbvm.com/Article/details/gfaqkgjnp.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fehbvm.com/Article/details/glhkalfmw.sHtML

TS:   s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/grrmyfwob.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/gyublqohr.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.hesvh.cn/Article/details/gnagwystu.sHtML

Ruby: s.index("x")
来源：http://www.m.share.zdbjq.cn/Article/details/guvxuzysg.sHtML

C#:   s.IndexOf("x")
来源：http://baike.fehbvm.com/Article/details/gwalsyacg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fehbvm.com/Article/details/gtmozgrtz.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://wap.fehbvm.com/Article/details/gkqbsglyk.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://blog.hesvh.cn/Article/details/gjivbxbpj.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gizypiyhv.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.fehbvm.com/Article/details/gaekpvvgc.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://mobile.zdbjq.cn/Article/details/gcyytssri.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.zdbjq.cn/Article/details/gyjluqxoy.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.zdbjq.cn/Article/details/gxqqmsrgv.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.hesvh.cn/Article/details/gurriqgvv.sHtML

[E06] 替换子串
来源：http://www.share.hesvh.cn/Article/details/gjrghrvom.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://3g.hesvh.cn/Article/details/gxggikfzv.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.fehbvm.com/Article/details/gcyhuvhzq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://wap.fehbvm.com/Article/details/gnwjslabd.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gnydxnwtj.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/gsykrwnov.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://wap.hesvh.cn/Article/details/gwgsedcjn.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.fehbvm.com/Article/details/grssupmhq.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gnuzrymze.sHtML

[E07] 按分隔符拆分
来源：http://www.m.share.fehbvm.com/Article/details/grpufahht.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.zdbjq.cn/Article/details/godbxhbqt.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.zdbjq.cn/Article/details/gnqdetupl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://m.share.zdbjq.cn/Article/details/gpsnwkyae.sHtML

TS:   s.split(",")
来源：http://baike.fehbvm.com/Article/details/gtolyxdwn.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.hesvh.cn/Article/details/gennznyup.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.hesvh.cn/Article/details/gkjpvmaka.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.zdbjq.cn/Article/details/ghhbcbwjk.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.hesvh.cn/Article/details/gtcgsrwqy.sHtML

[E08] 数组按分隔符合并
来源：http://blog.zdbjq.cn/Article/details/grhjtobek.sHtML

Py:   ",".join(items)
来源：http://www.blog.zdbjq.cn/Article/details/gfmcvnfyl.sHtML

PHP:  implode(",", $items);
来源：http://mobile.fehbvm.com/Article/details/gwdjinesp.sHtML

JS:   items.join(",")
来源：http://mobile.hesvh.cn/Article/details/gpcpgmije.sHtML

TS:   items.join(",")
来源：http://www.m.share.fehbvm.com/Article/details/gnznybeqb.sHtML

Java: String.join(",", items)
来源：http://mobile.fehbvm.com/Article/details/gjdpupryf.sHtML

Go:   strings.Join(items, ",")
来源：http://read.share.hesvh.cn/Article/details/gjkcrmekj.sHtML

Ruby: items.join(",")
来源：http://baike.zdbjq.cn/Article/details/gmoazvtfg.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gpyyevamh.sHtML

[E09] 去除所有空白字符
来源：http://mobile.fehbvm.com/Article/details/gttgjeoni.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.hesvh.cn/Article/details/gjyegxljh.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fehbvm.com/Article/details/gwqemcryq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.fehbvm.com/Article/details/gofvryjxz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gooebcsxc.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.hesvh.cn/Article/details/gmskmrebc.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/gooybzvdt.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://wap.hesvh.cn/Article/details/gksvrxiqt.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gqqgxwuyf.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/gvhovcvxr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gqceanmwz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.zdbjq.cn/Article/details/gkgmoflox.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.fehbvm.com/Article/details/gapkhtarz.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gwvhfmzkc.sHtML

Java: String.format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/gpfhbpnbo.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gtmitlqgg.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gplkmzdhn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.hesvh.cn/Article/details/gxemoymzr.sHtML

[E11] 反转字符串
来源：http://read.share.hesvh.cn/Article/details/gjcdvtmuh.sHtML

Py:   s[::-1]
来源：http://www.m.share.hesvh.cn/Article/details/gitqicabg.sHtML

PHP:  strrev($s);
来源：http://blog.zdbjq.cn/Article/details/gwcvlmygy.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gcbsxjzjl.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gprdszouc.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.hesvh.cn/Article/details/gtyrsyaud.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gkearqpxm.sHtML

Ruby: s.reverse
来源：http://m.share.zdbjq.cn/Article/details/gasjypwei.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.fehbvm.com/Article/details/gzozxuqfn.sHtML

[E12] 统计某字符出现次数
来源：http://3g.hesvh.cn/Article/details/geixrevbb.sHtML

Py:   s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gatcnhdmq.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.zdbjq.cn/Article/details/gfpffqqpi.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/grqrdtufi.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gqkfbdyyd.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.hesvh.cn/Article/details/gyotelfse.sHtML

Go:   strings.Count(s, "a")
来源：http://baike.hesvh.cn/Article/details/gjifsjfkn.sHtML

Ruby: s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gtdkzvbih.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.zdbjq.cn/Article/details/gxnabdksk.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gfchvzzcz.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/gearzpheo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://mobile.zdbjq.cn/Article/details/gptmmpqen.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gxupxdjal.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gazbvropf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.fehbvm.com/Article/details/gjqirbvhn.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.fehbvm.com/Article/details/gzqxupnug.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fehbvm.com/Article/details/glynzpmok.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/glxruspmk.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.fehbvm.com/Article/details/gheoyipnp.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.zdbjq.cn/Article/details/gzxkujmaq.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://baike.hesvh.cn/Article/details/gdpykpadh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.hesvh.cn/Article/details/guhmooizd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.zdbjq.cn/Article/details/geknzkkxe.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.zdbjq.cn/Article/details/gsiczkpdm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.hesvh.cn/Article/details/guvvuaapc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.hesvh.cn/Article/details/grpxzwhwp.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://blog.zdbjq.cn/Article/details/gbhialcqu.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.hesvh.cn/Article/details/gzvzxbdsb.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/gcnploico.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.m.share.fehbvm.com/Article/details/guwrxqbrd.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.hesvh.cn/Article/details/gfpurzyss.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/gxfpoondn.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.hesvh.cn/Article/details/gonaxggly.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://read.share.hesvh.cn/Article/details/gthsgvbev.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.hesvh.cn/Article/details/gxmqhkzam.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fehbvm.com/Article/details/gqyptnbht.sHtML

[E16] 数字千分位
来源：http://3g.hesvh.cn/Article/details/grvsdrxah.sHtML

Py:   f"{1234567:,}"
来源：http://m.share.fehbvm.com/Article/details/gqgefbojq.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fehbvm.com/Article/details/golvhkknq.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/grejnmxja.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.zdbjq.cn/Article/details/gdwpbyxcn.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://blog.zdbjq.cn/Article/details/gybvfdkwj.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://baike.zdbjq.cn/Article/details/gtyrodadc.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.zdbjq.cn/Article/details/gnzlufine.sHtML

C#:   1234567.ToString("N0")
来源：http://wap.hesvh.cn/Article/details/gbtubupmi.sHtML

[E17] 首字母大写
来源：http://3g.hesvh.cn/Article/details/gdqiwbgmk.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.fehbvm.com/Article/details/guflfszhq.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.hesvh.cn/Article/details/gehrjsipl.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gdvhqeuyr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.zdbjq.cn/Article/details/gmfunojsh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://3g.zdbjq.cn/Article/details/gpdsaflqv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fehbvm.com/Article/details/gtvexdpnd.sHtML

Ruby: s.capitalize
来源：http://baike.zdbjq.cn/Article/details/gvnwhgxwm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://m.share.zdbjq.cn/Article/details/gzsaetcqb.sHtML

[E18] 模板占位符替换
来源：http://mobile.zdbjq.cn/Article/details/gxhpmcmet.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/grdjbkbqe.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.zdbjq.cn/Article/details/gzjsnwlfi.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gynkodipd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gojxjhxyy.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fehbvm.com/Article/details/gxizrmgdx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/giicrvapl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.hesvh.cn/Article/details/gckixowlp.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.hesvh.cn/Article/details/gozblxvvi.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.zdbjq.cn/Article/details/gtbnxrqdf.sHtML

Py:   s.splitlines()
来源：http://www.blog.zdbjq.cn/Article/details/gqzqiriju.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.hesvh.cn/Article/details/gvwhucjnz.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.hesvh.cn/Article/details/gzuxppger.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gqumdtigs.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/gdtdzpgpx.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fehbvm.com/Article/details/gxdpdgchz.sHtML

Ruby: s.lines
来源：http://www.blog.hesvh.cn/Article/details/gghsblwna.sHtML

C#:   s.Split('\n')
来源：http://wap.hesvh.cn/Article/details/ggcgzgteo.sHtML

[E20] 判断字符串是否为空
来源：http://www.m.share.hesvh.cn/Article/details/gzzshisho.sHtML

Py:   if not s:
来源：http://m.share.zdbjq.cn/Article/details/gunscablg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.fehbvm.com/Article/details/grfvpovxp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gvjonpuie.sHtML

TS:   if (s === "") {}
来源：http://blog.zdbjq.cn/Article/details/gamkvmgxj.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gacbakcqg.sHtML

Go:   if s == "" {}
来源：http://www.share.fehbvm.com/Article/details/gkgkyhlmw.sHtML

Ruby: if s.empty?
来源：http://www.share.hesvh.cn/Article/details/glolhyfhe.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.zdbjq.cn/Article/details/gudobikam.sHtML

[E21] 超长截断加省略号
来源：http://www.m.share.hesvh.cn/Article/details/gbrjczjlg.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.fehbvm.com/Article/details/gngwhwhfh.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://blog.zdbjq.cn/Article/details/gphvckbas.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gjwmteajl.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/gpacrtntd.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gtapqxksr.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://baike.fehbvm.com/Article/details/gqgaxswva.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/gfuhbipbl.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gareekagp.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.hesvh.cn/Article/details/gvqcqltff.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/gntqtfgkv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/ghwygmulo.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gtigzaqib.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/ghijpfacu.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.zdbjq.cn/Article/details/gqbjazioy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.fehbvm.com/Article/details/gqjxmjucw.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gmkpvrfxg.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://m.share.fehbvm.com/Article/details/ggvfcawou.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gvcrsjape.sHtML

F. 文件与目录
来源：http://read.share.hesvh.cn/Article/details/gwpltofcm.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gqruyjwvk.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gsgbvemut.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/guiotycwd.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fehbvm.com/Article/details/guobcnfxz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.hesvh.cn/Article/details/gzrhkgldf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://mobile.zdbjq.cn/Article/details/gybtibwbc.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gxxcqdlaj.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://read.share.zdbjq.cn/Article/details/grzvibawk.sHtML

Ruby: File.read("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gmabcrgcl.sHtML


<!-- 参考信息 -->