代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://wap.zdbjq.cn/Article/details/gwsajqtjp.sHtML

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://3g.fehbvm.com/Article/details/gzarbhgya.sHtML

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://3g.fehbvm.com/Article/details/gwladhxkp.sHtML

Go:   // 手写循环累加
来源：http://baike.zdbjq.cn/Article/details/gigokgyrk.sHtML

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://wap.hesvh.cn/Article/details/gxrhthakq.sHtML

C#:   list.Sum();  list.Average()
来源：http://baike.zdbjq.cn/Article/details/gduhzdynh.sHtML

[D17] 最大值与最小值
来源：http://wap.zdbjq.cn/Article/details/gwxwsgqpg.sHtML

Py:   max(arr);  min(arr)
来源：http://www.m.share.fehbvm.com/Article/details/gasnjvrzi.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.m.share.fehbvm.com/Article/details/geasvwzhq.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.blog.fehbvm.com/Article/details/gitqycgcz.sHtML

TS:   Math.max(...arr);
来源：http://3g.fehbvm.com/Article/details/ggzzksukg.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.hesvh.cn/Article/details/ghndhrbuj.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://3g.hesvh.cn/Article/details/gyuiyulwx.sHtML

Ruby: arr.max;  arr.min
来源：http://www.share.fehbvm.com/Article/details/gppyuejpe.sHtML

C#:   list.Max();  list.Min()
来源：http://3g.fehbvm.com/Article/details/gdwkpmwys.sHtML

[D18] 扁平化嵌套数组
来源：http://mobile.hesvh.cn/Article/details/gjgwwdbnu.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://m.share.hesvh.cn/Article/details/gnhknppbk.sHtML

PHP:  array_merge(...$nested);
来源：http://www.share.hesvh.cn/Article/details/gemdrmamz.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://read.share.hesvh.cn/Article/details/gnlssfsur.sHtML

TS:   nested.flat();
来源：http://www.blog.fehbvm.com/Article/details/gnlnhuyvc.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://3g.zdbjq.cn/Article/details/gitvyzexm.sHtML

Go:   // 手写双层循环
来源：http://www.m.share.zdbjq.cn/Article/details/gwixymkzm.sHtML

Ruby: nested.flatten
来源：http://m.share.zdbjq.cn/Article/details/gknsbmvta.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://blog.fehbvm.com/Article/details/gawbcvcay.sHtML

[D19] 按字段分组
来源：http://read.share.fehbvm.com/Article/details/gtpezglzu.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://read.share.fehbvm.com/Article/details/gbzvcfuye.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.zdbjq.cn/Article/details/gonooscgz.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://mobile.fehbvm.com/Article/details/gmbmnwcts.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://3g.hesvh.cn/Article/details/gbihxkpws.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://mobile.zdbjq.cn/Article/details/grsekqnoo.sHtML

Go:   // 手写 map[string][]T
来源：http://3g.fehbvm.com/Article/details/gckwfpqzr.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://3g.zdbjq.cn/Article/details/gmbxusupl.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.blog.hesvh.cn/Article/details/gekndfwzl.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.fehbvm.com/Article/details/gpkxtcyqn.sHtML

Py:   Counter(arr)
来源：http://read.share.zdbjq.cn/Article/details/gsjubizdt.sHtML

PHP:  array_count_values($arr);
来源：http://baike.fehbvm.com/Article/details/gudkhubqa.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.blog.hesvh.cn/Article/details/giibqoweb.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.share.zdbjq.cn/Article/details/guirmdwmv.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://mobile.zdbjq.cn/Article/details/ggibdxwdu.sHtML

Go:   // 手写 map[T]int
来源：http://read.share.fehbvm.com/Article/details/gvdwbsbqw.sHtML

Ruby: arr.tally
来源：http://m.share.zdbjq.cn/Article/details/gzxvcjogk.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.share.hesvh.cn/Article/details/gptqhultr.sHtML

[D21] 判断是否包含某元素
来源：http://baike.hesvh.cn/Article/details/gjbclpygv.sHtML

Py:   x in arr
来源：http://m.share.hesvh.cn/Article/details/gprdsbugu.sHtML

PHP:  in_array($x, $arr, true);
来源：http://m.share.zdbjq.cn/Article/details/gidntamlc.sHtML

JS:   arr.includes(x)
来源：http://mobile.hesvh.cn/Article/details/gydckgsfw.sHtML

TS:   arr.includes(x)
来源：http://wap.fehbvm.com/Article/details/gcawnvvuu.sHtML

Java: list.contains(x)
来源：http://www.share.zdbjq.cn/Article/details/gffcdyqfr.sHtML

Go:   slices.Contains(arr, x)
来源：http://baike.zdbjq.cn/Article/details/glurhmzpg.sHtML

Ruby: arr.include?(x)
来源：http://3g.hesvh.cn/Article/details/gkrevcnum.sHtML

C#:   list.Contains(x)
来源：http://wap.zdbjq.cn/Article/details/gcfghnrly.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.m.share.fehbvm.com/Article/details/gehlvoojk.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://m.share.zdbjq.cn/Article/details/gupqmjdwf.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://m.share.zdbjq.cn/Article/details/gtgkzvgxh.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.share.zdbjq.cn/Article/details/ghifmjarm.sHtML

TS:   [...arr];
来源：http://wap.fehbvm.com/Article/details/govypysqs.sHtML

Java: new ArrayList<>(list);
来源：http://www.share.hesvh.cn/Article/details/gdburrrms.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.hesvh.cn/Article/details/gouioxjcj.sHtML

Ruby: arr.dup;  arr.clone
来源：http://wap.fehbvm.com/Article/details/gdogsnhqt.sHtML

C#:   new List<int>(list);
来源：http://m.share.fehbvm.com/Article/details/gvrhiykhd.sHtML

[D23] reduce 累积计算
来源：http://www.blog.fehbvm.com/Article/details/gtzuqhmcc.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.hesvh.cn/Article/details/gmdkduduv.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://wap.zdbjq.cn/Article/details/gnrxodbcn.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/gdxyqudyn.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://m.share.zdbjq.cn/Article/details/gbbnkzqyj.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/gficjsduj.sHtML

Go:   // 手写循环
来源：http://www.blog.fehbvm.com/Article/details/gvefwrbbw.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.zdbjq.cn/Article/details/gqfiogvwg.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.share.fehbvm.com/Article/details/gyzusoqxm.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.hesvh.cn/Article/details/glbfixwxd.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://m.share.fehbvm.com/Article/details/geodzedtu.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://blog.zdbjq.cn/Article/details/gzzkvjyiq.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gucookaau.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://3g.zdbjq.cn/Article/details/grdkvdwit.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.zdbjq.cn/Article/details/gjjfqzipt.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.zdbjq.cn/Article/details/gomwqqejy.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.m.share.zdbjq.cn/Article/details/grntorxgo.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.hesvh.cn/Article/details/ghosrwloh.sHtML

[D25] Set 集合去重与交并差
来源：http://baike.fehbvm.com/Article/details/gydhwzrnt.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.hesvh.cn/Article/details/gdnlrudqx.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.zdbjq.cn/Article/details/gnhrrmrfp.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://read.share.hesvh.cn/Article/details/gworxonay.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://mobile.hesvh.cn/Article/details/gnjoavuje.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.zdbjq.cn/Article/details/grguweoah.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://wap.zdbjq.cn/Article/details/gtddrwahe.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/gvahhantj.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fehbvm.com/Article/details/gubzijiwy.sHtML

[D26] 数组转字符串
来源：http://m.share.zdbjq.cn/Article/details/geldqyaka.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.hesvh.cn/Article/details/gldaosihf.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.hesvh.cn/Article/details/gijphomrh.sHtML

JS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/gmbvlkukf.sHtML

TS:   arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/ghylkbubj.sHtML

Java: String.join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/ggjdhzdnp.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.m.share.zdbjq.cn/Article/details/gdycwcrza.sHtML

Ruby: arr.join(", ")
来源：http://www.m.share.fehbvm.com/Article/details/grdglvybu.sHtML

C#:   string.Join(", ", list)
来源：http://read.share.zdbjq.cn/Article/details/ggqbvpbcm.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/ghqjmzepo.sHtML

E. 字符串处理
来源：http://www.m.share.fehbvm.com/Article/details/genmagxbp.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gjhuozxum.sHtML

[E01] 拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gqvtylrhn.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.share.fehbvm.com/Article/details/gbpsfifdb.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.fehbvm.com/Article/details/gyehwlvcd.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://baike.fehbvm.com/Article/details/grivmjdin.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gitavsscg.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.zdbjq.cn/Article/details/geysgerrg.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.share.hesvh.cn/Article/details/gvcqhspza.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.fehbvm.com/Article/details/gtkmzyjlz.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gfvvshqnf.sHtML

[E02] 重复字符串
来源：http://wap.zdbjq.cn/Article/details/gffmpwzli.sHtML

Py:   "ab" * 3
来源：http://www.blog.zdbjq.cn/Article/details/gczflcjqh.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.share.zdbjq.cn/Article/details/gikhsapao.sHtML

JS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gcdlyiehf.sHtML

TS:   "ab".repeat(3)
来源：http://baike.hesvh.cn/Article/details/gmbpqnwig.sHtML

Java: "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gzmjqcxbl.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.zdbjq.cn/Article/details/guqhykyhm.sHtML

Ruby: "ab" * 3
来源：http://m.share.zdbjq.cn/Article/details/gygfxnfwb.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://baike.fehbvm.com/Article/details/ggfhzggew.sHtML

[E03] 截取子串
来源：http://baike.zdbjq.cn/Article/details/gcmlvkxay.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.fehbvm.com/Article/details/googuzhks.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/grwvivrwd.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.m.share.hesvh.cn/Article/details/gkluvxmmk.sHtML

TS:   s.slice(1, 4)
来源：http://wap.fehbvm.com/Article/details/gtwrgtywt.sHtML

Java: s.substring(1, 4)
来源：http://www.m.share.fehbvm.com/Article/details/gbklwxhvj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.m.share.zdbjq.cn/Article/details/gssbuzfwx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://www.m.share.hesvh.cn/Article/details/govqstjcw.sHtML

C#:   s.Substring(1, 3)
来源：http://read.share.hesvh.cn/Article/details/gyjxsmsgb.sHtML

[E04] 查找子串位置
来源：http://m.share.hesvh.cn/Article/details/gxjuuslzb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.hesvh.cn/Article/details/gwwzqlcwa.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.hesvh.cn/Article/details/goacoijpj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.hesvh.cn/Article/details/gkzbumcne.sHtML

TS:   s.indexOf("x")
来源：http://3g.zdbjq.cn/Article/details/gsgffdybx.sHtML

Java: s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/grzwiqqnu.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.hesvh.cn/Article/details/gkkstilqg.sHtML

Ruby: s.index("x")
来源：http://www.blog.hesvh.cn/Article/details/gxhiofcwl.sHtML

C#:   s.IndexOf("x")
来源：http://read.share.hesvh.cn/Article/details/gfzumrwlm.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.m.share.zdbjq.cn/Article/details/ghabsmaqq.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/ganhlgypq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fehbvm.com/Article/details/ghhmidlgc.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gxtoljnsm.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.blog.hesvh.cn/Article/details/gpbwdrxrv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/ghcwbbwwr.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://baike.zdbjq.cn/Article/details/gerwnxieo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.share.fehbvm.com/Article/details/glccmcurk.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.fehbvm.com/Article/details/gjxtheknr.sHtML

[E06] 替换子串
来源：http://wap.zdbjq.cn/Article/details/gobrbujol.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gyabqsokt.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://read.share.zdbjq.cn/Article/details/gdpqyakqo.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gjkyjnibx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/grkrdgkde.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/ggiulsqba.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gpjfefwcy.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gjcculcsd.sHtML

C#:   s.Replace("a", "b")
来源：http://blog.hesvh.cn/Article/details/gcyumpkqb.sHtML

[E07] 按分隔符拆分
来源：http://blog.hesvh.cn/Article/details/gvoygjlar.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://mobile.zdbjq.cn/Article/details/gpekmvrlz.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.hesvh.cn/Article/details/gchjaiuze.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.fehbvm.com/Article/details/grkrqvbhl.sHtML

TS:   s.split(",")
来源：http://m.share.zdbjq.cn/Article/details/gjryjupyq.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.hesvh.cn/Article/details/gknfkynrs.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.zdbjq.cn/Article/details/gbcwhnjlj.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.zdbjq.cn/Article/details/gjqxqzjki.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.zdbjq.cn/Article/details/gfkzmjrhv.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fehbvm.com/Article/details/guhzwlqat.sHtML

Py:   ",".join(items)
来源：http://www.share.fehbvm.com/Article/details/glghwlein.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fehbvm.com/Article/details/glbmqplnl.sHtML

JS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gvtstvxno.sHtML

TS:   items.join(",")
来源：http://www.blog.zdbjq.cn/Article/details/gzhsvilbc.sHtML

Java: String.join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gncfgculx.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.hesvh.cn/Article/details/gzsqcghwp.sHtML

Ruby: items.join(",")
来源：http://wap.fehbvm.com/Article/details/guklxiyus.sHtML

C#:   string.Join(",", items)
来源：http://baike.zdbjq.cn/Article/details/gwvmadjmz.sHtML

[E09] 去除所有空白字符
来源：http://baike.zdbjq.cn/Article/details/ggflgzpob.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.zdbjq.cn/Article/details/ghvzsmvxn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://m.share.fehbvm.com/Article/details/gqkybrobm.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gknjswptm.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gjvedlggd.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gwkownbrj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.hesvh.cn/Article/details/glcnlnoqr.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gsdvskrul.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gwfistkno.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.hesvh.cn/Article/details/gferepmzb.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gygdxjwwg.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.hesvh.cn/Article/details/gfohvuyup.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gpksizmly.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.hesvh.cn/Article/details/gkbuclymz.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/gnamerbso.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/geubroaer.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/glfaubujt.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.fehbvm.com/Article/details/gqyaquvne.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/gudeevonb.sHtML

Py:   s[::-1]
来源：http://mobile.fehbvm.com/Article/details/gxrvhopau.sHtML

PHP:  strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gkwwwgkas.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.hesvh.cn/Article/details/gzgkzuwhe.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gumddtbvb.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.zdbjq.cn/Article/details/gsskdgynt.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.zdbjq.cn/Article/details/gnxjxcatj.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/gjtwnnzhl.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.hesvh.cn/Article/details/gafoszqtj.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fehbvm.com/Article/details/gdkgfyvxq.sHtML

Py:   s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gijkrpjoa.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.fehbvm.com/Article/details/gsqdgmark.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gnneyvcng.sHtML

TS:   s.split("a").length - 1
来源：http://baike.zdbjq.cn/Article/details/gafrhizdy.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://m.share.fehbvm.com/Article/details/gdbfuvvor.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.fehbvm.com/Article/details/gfpdjatiy.sHtML

Ruby: s.count("a")
来源：http://m.share.hesvh.cn/Article/details/gmknagqrm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.hesvh.cn/Article/details/gfdvwoaeg.sHtML

[E13] 逐字符遍历
来源：http://mobile.hesvh.cn/Article/details/gzkxabkxe.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fehbvm.com/Article/details/gfdljbvxz.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.zdbjq.cn/Article/details/gxezehgrn.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gqfgcyhrd.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gmbtdlmsy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://wap.fehbvm.com/Article/details/gjwzvsrgx.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://3g.hesvh.cn/Article/details/gzrwylbrr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.hesvh.cn/Article/details/gxzwxhrnp.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gueymprbl.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/gnqvoyxmi.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://baike.hesvh.cn/Article/details/gpjioztga.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://read.share.fehbvm.com/Article/details/gcstgygxg.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.m.share.hesvh.cn/Article/details/goqnsvlzd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.zdbjq.cn/Article/details/gxxdhndtd.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.hesvh.cn/Article/details/ghmdkgyaj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.zdbjq.cn/Article/details/gyqhsqpvh.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fehbvm.com/Article/details/guilaxzlf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gjwbkggdm.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.zdbjq.cn/Article/details/gizygnrjr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.m.share.hesvh.cn/Article/details/gwpopadzl.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fehbvm.com/Article/details/gtdmjumno.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.blog.hesvh.cn/Article/details/gebfoectu.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.zdbjq.cn/Article/details/ggkhoewgb.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://blog.hesvh.cn/Article/details/gedcbvmhx.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.zdbjq.cn/Article/details/geaqxjtrh.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/gfskvbdjw.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://baike.hesvh.cn/Article/details/ghmpwowtt.sHtML

[E16] 数字千分位
来源：http://m.share.fehbvm.com/Article/details/gygboqnlq.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.hesvh.cn/Article/details/gbozawrbf.sHtML

PHP:  number_format(1234567);
来源：http://www.share.fehbvm.com/Article/details/gouiapdqh.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gltgijojt.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gfhhjqrri.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gedmqwqet.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.fehbvm.com/Article/details/gjdcynagr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.zdbjq.cn/Article/details/gdjdsvaxk.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/gletulicp.sHtML

[E17] 首字母大写
来源：http://3g.hesvh.cn/Article/details/gjfetnkyb.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.hesvh.cn/Article/details/geystlmjz.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.hesvh.cn/Article/details/gcnlsprve.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.fehbvm.com/Article/details/gvxzpcpwo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/gbkpvpgrw.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.fehbvm.com/Article/details/gtjvvkpgv.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fehbvm.com/Article/details/grpbnakip.sHtML

Ruby: s.capitalize
来源：http://read.share.hesvh.cn/Article/details/glpawkndq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.fehbvm.com/Article/details/gdnkoswjv.sHtML

[E18] 模板占位符替换
来源：http://read.share.fehbvm.com/Article/details/gsekloroe.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fehbvm.com/Article/details/gaztxatqw.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.hesvh.cn/Article/details/guumpsldi.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gwjznaehu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gwdalubll.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gpyioioho.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gsnjlndhf.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.zdbjq.cn/Article/details/gkplqevhv.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.share.fehbvm.com/Article/details/gwopdwnej.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fehbvm.com/Article/details/gpdtpclme.sHtML

Py:   s.splitlines()
来源：http://www.blog.hesvh.cn/Article/details/gdnfhmsqr.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/gewvnobdb.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gglamhnxe.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.hesvh.cn/Article/details/gmmwqdiop.sHtML

Java: s.lines().toList()
来源：http://www.share.fehbvm.com/Article/details/gezxorlyn.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.fehbvm.com/Article/details/gphccnzfk.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/gsgazvefg.sHtML

C#:   s.Split('\n')
来源：http://blog.zdbjq.cn/Article/details/gzbjczhtg.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fehbvm.com/Article/details/gwdeovyaj.sHtML

Py:   if not s:
来源：http://wap.fehbvm.com/Article/details/gnfodygnk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.zdbjq.cn/Article/details/gogildofy.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.zdbjq.cn/Article/details/gajatwzyk.sHtML

TS:   if (s === "") {}
来源：http://www.m.share.zdbjq.cn/Article/details/gprifmhon.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/ginyrqryu.sHtML

Go:   if s == "" {}
来源：http://m.share.hesvh.cn/Article/details/gzfiewjnm.sHtML

Ruby: if s.empty?
来源：http://www.share.fehbvm.com/Article/details/gekhhwppk.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fehbvm.com/Article/details/gioukptyw.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/gafvwxsui.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.hesvh.cn/Article/details/goqjgbhmr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fehbvm.com/Article/details/glcsoafxq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gsvoxagup.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gkbisbbqf.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gvahcoirs.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/gdkmeupyc.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.zdbjq.cn/Article/details/gmzlsrauq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gpbbwxgxw.sHtML

[E22] 字节长度与字符长度
来源：http://read.share.hesvh.cn/Article/details/gosljixrs.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://baike.zdbjq.cn/Article/details/gogiitiui.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/gppwsztnk.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gippyscya.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.hesvh.cn/Article/details/gjfxqdkuz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gxpxxxbpa.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fehbvm.com/Article/details/gikvqneii.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gsdlcqjro.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.zdbjq.cn/Article/details/gjirbplkn.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gysfolgtz.sHtML

F. 文件与目录
来源：http://www.share.fehbvm.com/Article/details/gtsjncasc.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwwlizhps.sHtML


<!-- 参考信息 -->