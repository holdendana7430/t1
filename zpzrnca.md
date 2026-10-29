代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://baike.fehbvm.com/Article/details/gaguzxrus.sHtML

C#:   list.Sum();  list.Average()
来源：http://www.share.fehbvm.com/Article/details/gqmhxkrjx.sHtML

[D17] 最大值与最小值
来源：http://mobile.zdbjq.cn/Article/details/geweiymhy.sHtML

Py:   max(arr);  min(arr)
来源：http://baike.hesvh.cn/Article/details/gxcywafjx.sHtML

PHP:  max($arr);  min($arr);
来源：http://www.share.hesvh.cn/Article/details/gjkzylxor.sHtML

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.m.share.hesvh.cn/Article/details/gtejubufk.sHtML

TS:   Math.max(...arr);
来源：http://baike.fehbvm.com/Article/details/gqqcboxec.sHtML

Java: Collections.max(list);  Collections.min(list);
来源：http://blog.hesvh.cn/Article/details/gbkmdpgtc.sHtML

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.m.share.zdbjq.cn/Article/details/grnightvm.sHtML

Ruby: arr.max;  arr.min
来源：http://m.share.hesvh.cn/Article/details/gzgpnvrjv.sHtML

C#:   list.Max();  list.Min()
来源：http://baike.zdbjq.cn/Article/details/genzjtxlb.sHtML

[D18] 扁平化嵌套数组
来源：http://read.share.zdbjq.cn/Article/details/gjojgnbmx.sHtML

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.share.zdbjq.cn/Article/details/gxurrager.sHtML

PHP:  array_merge(...$nested);
来源：http://m.share.zdbjq.cn/Article/details/gyqaglvhy.sHtML

JS:   nested.flat();  nested.flat(Infinity)
来源：http://mobile.zdbjq.cn/Article/details/gsjfonmyk.sHtML

TS:   nested.flat();
来源：http://m.share.fehbvm.com/Article/details/grohwkumf.sHtML

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.m.share.zdbjq.cn/Article/details/gearrsltx.sHtML

Go:   // 手写双层循环
来源：http://www.blog.hesvh.cn/Article/details/gychpxybc.sHtML

Ruby: nested.flatten
来源：http://3g.zdbjq.cn/Article/details/gdsjastxv.sHtML

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.share.fehbvm.com/Article/details/ghruaracl.sHtML

[D19] 按字段分组
来源：http://m.share.hesvh.cn/Article/details/gujvlfmuy.sHtML

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://3g.hesvh.cn/Article/details/gcxwctkga.sHtML

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.blog.hesvh.cn/Article/details/gwmdzlkpb.sHtML

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://wap.fehbvm.com/Article/details/gzmqlfllc.sHtML

TS:   Object.groupBy(arr, x => x.type)
来源：http://read.share.fehbvm.com/Article/details/gtvlfqmcr.sHtML

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://baike.hesvh.cn/Article/details/gvaxwbedr.sHtML

Go:   // 手写 map[string][]T
来源：http://baike.fehbvm.com/Article/details/gnrnopxhz.sHtML

Ruby: arr.group_by { |x| x[:type] }
来源：http://wap.hesvh.cn/Article/details/gmtjelbnp.sHtML

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://m.share.hesvh.cn/Article/details/gqggxjrvl.sHtML

[D20] 统计每个元素出现次数
来源：http://read.share.zdbjq.cn/Article/details/ggmqoizut.sHtML

Py:   Counter(arr)
来源：http://www.share.hesvh.cn/Article/details/grijjlqad.sHtML

PHP:  array_count_values($arr);
来源：http://read.share.fehbvm.com/Article/details/gkurxbtie.sHtML

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://mobile.fehbvm.com/Article/details/gtrkcqcgi.sHtML

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://wap.hesvh.cn/Article/details/gjhcnqajp.sHtML

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.share.fehbvm.com/Article/details/gwkxsqmak.sHtML

Go:   // 手写 map[T]int
来源：http://mobile.fehbvm.com/Article/details/gwpzqrtox.sHtML

Ruby: arr.tally
来源：http://wap.fehbvm.com/Article/details/gltsttile.sHtML

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.blog.hesvh.cn/Article/details/glgdiegtr.sHtML

[D21] 判断是否包含某元素
来源：http://www.m.share.zdbjq.cn/Article/details/gqyfnpaof.sHtML

Py:   x in arr
来源：http://m.share.hesvh.cn/Article/details/giwavmsmf.sHtML

PHP:  in_array($x, $arr, true);
来源：http://www.blog.fehbvm.com/Article/details/gjxfxifdc.sHtML

JS:   arr.includes(x)
来源：http://3g.hesvh.cn/Article/details/gldnzjlve.sHtML

TS:   arr.includes(x)
来源：http://baike.hesvh.cn/Article/details/ggensrbft.sHtML

Java: list.contains(x)
来源：http://baike.hesvh.cn/Article/details/ggnrvhlgm.sHtML

Go:   slices.Contains(arr, x)
来源：http://mobile.fehbvm.com/Article/details/grhpugzba.sHtML

Ruby: arr.include?(x)
来源：http://m.share.fehbvm.com/Article/details/gxmvkcyix.sHtML

C#:   list.Contains(x)
来源：http://mobile.fehbvm.com/Article/details/gvxaopggs.sHtML

[D22] 复制数组（避免共享引用）
来源：http://www.share.hesvh.cn/Article/details/gsohvulvz.sHtML

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.blog.zdbjq.cn/Article/details/gkafxjmej.sHtML

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://3g.zdbjq.cn/Article/details/ghpcfucwn.sHtML

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://3g.zdbjq.cn/Article/details/ghzohcyig.sHtML

TS:   [...arr];
来源：http://mobile.zdbjq.cn/Article/details/gqrsrgybc.sHtML

Java: new ArrayList<>(list);
来源：http://blog.zdbjq.cn/Article/details/gtytuifuz.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://read.share.fehbvm.com/Article/details/geutghwwv.sHtML

Ruby: arr.dup;  arr.clone
来源：http://www.m.share.fehbvm.com/Article/details/gpxfqnbwl.sHtML

C#:   new List<int>(list);
来源：http://www.m.share.zdbjq.cn/Article/details/gbjwwhcdb.sHtML

[D23] reduce 累积计算
来源：http://mobile.zdbjq.cn/Article/details/ggrzugstd.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.m.share.hesvh.cn/Article/details/gotglnpiy.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://m.share.hesvh.cn/Article/details/guhdelawa.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.share.zdbjq.cn/Article/details/gjnybaxjr.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/gerqflaof.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://3g.hesvh.cn/Article/details/gylvjxbvm.sHtML

Go:   // 手写循环
来源：http://3g.zdbjq.cn/Article/details/goantjqvl.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://wap.zdbjq.cn/Article/details/gjiwuqmiz.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.zdbjq.cn/Article/details/gvnkhdapt.sHtML

[D24] 字典 / Map 基本操作
来源：http://mobile.fehbvm.com/Article/details/gnraprzwm.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://baike.hesvh.cn/Article/details/gypfszefm.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://baike.hesvh.cn/Article/details/gicjalbeb.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.zdbjq.cn/Article/details/getdynbla.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://m.share.fehbvm.com/Article/details/ghjdisjna.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.share.fehbvm.com/Article/details/ggtbpgaap.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://blog.hesvh.cn/Article/details/geoknxdxw.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://m.share.fehbvm.com/Article/details/gxidtavgc.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.m.share.hesvh.cn/Article/details/gfhjlshss.sHtML

[D25] Set 集合去重与交并差
来源：http://www.blog.zdbjq.cn/Article/details/gtfrqwxjb.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://3g.fehbvm.com/Article/details/grqiyrzqw.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.share.hesvh.cn/Article/details/gzdfjqzuq.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://baike.hesvh.cn/Article/details/gsmpnbubl.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.zdbjq.cn/Article/details/gplcdrkdm.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.fehbvm.com/Article/details/gghznteem.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.zdbjq.cn/Article/details/gbzcyggpo.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.m.share.fehbvm.com/Article/details/gykfstqyu.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://wap.fehbvm.com/Article/details/ghaydudyc.sHtML

[D26] 数组转字符串
来源：http://read.share.fehbvm.com/Article/details/gormacmbd.sHtML

Py:   ", ".join(map(str, arr))
来源：http://mobile.zdbjq.cn/Article/details/gxdtvebfv.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.zdbjq.cn/Article/details/gxostzfyx.sHtML

JS:   arr.join(", ")
来源：http://baike.zdbjq.cn/Article/details/grvgfabci.sHtML

TS:   arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/gqvfqxytl.sHtML

Java: String.join(", ", list)
来源：http://3g.hesvh.cn/Article/details/gnwzutycr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.fehbvm.com/Article/details/gkgeovgcc.sHtML

Ruby: arr.join(", ")
来源：http://baike.hesvh.cn/Article/details/grmrbnafc.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.hesvh.cn/Article/details/gtrjrzvst.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/golurfpzx.sHtML

E. 字符串处理
来源：http://wap.zdbjq.cn/Article/details/gqcesvkqg.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gjrrjwfbu.sHtML

[E01] 拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gvahpnznh.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.zdbjq.cn/Article/details/gsupzeeos.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://3g.hesvh.cn/Article/details/goxgadjxc.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gytlxsuwm.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/gqzkwstpc.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.blog.zdbjq.cn/Article/details/gmuldwhkt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.fehbvm.com/Article/details/gmwdbfxsi.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://blog.hesvh.cn/Article/details/gwpmisobs.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://wap.fehbvm.com/Article/details/gwmqjuxhg.sHtML

[E02] 重复字符串
来源：http://www.m.share.hesvh.cn/Article/details/gglfteuki.sHtML

Py:   "ab" * 3
来源：http://www.m.share.hesvh.cn/Article/details/gpsozycob.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.zdbjq.cn/Article/details/gumkuudin.sHtML

JS:   "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gyimzhvqi.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/gobwmrojx.sHtML

Java: "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gxmlhceck.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.blog.fehbvm.com/Article/details/gwxkwtslh.sHtML

Ruby: "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gsfepikuk.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.hesvh.cn/Article/details/gwopkicww.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/gbtbiflhs.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://baike.hesvh.cn/Article/details/gymuwoqvl.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gkmdkfckn.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gkkkpcrbw.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.zdbjq.cn/Article/details/gnqsjeqji.sHtML

Java: s.substring(1, 4)
来源：http://blog.zdbjq.cn/Article/details/gpbnsvkvd.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.hesvh.cn/Article/details/gblrrbjhl.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.fehbvm.com/Article/details/gtwfsyfmo.sHtML

C#:   s.Substring(1, 3)
来源：http://blog.hesvh.cn/Article/details/gllngtwzn.sHtML

[E04] 查找子串位置
来源：http://www.share.hesvh.cn/Article/details/grplbhrio.sHtML

Py:   s.find("x");  s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gsbpyvtse.sHtML

PHP:  strpos($s, "x");
来源：http://read.share.fehbvm.com/Article/details/gekkyqsui.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://mobile.zdbjq.cn/Article/details/gqojmbjdv.sHtML

TS:   s.indexOf("x")
来源：http://mobile.zdbjq.cn/Article/details/gesaknljs.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.zdbjq.cn/Article/details/glfntuivh.sHtML

Go:   strings.Index(s, "x")
来源：http://read.share.hesvh.cn/Article/details/gajxxtnsf.sHtML

Ruby: s.index("x")
来源：http://www.blog.fehbvm.com/Article/details/gbunlbecy.sHtML

C#:   s.IndexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gdjezcdnk.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.zdbjq.cn/Article/details/ghmbqqwcj.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://blog.fehbvm.com/Article/details/gmexfhasy.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://wap.hesvh.cn/Article/details/ginaxlgbs.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gpuheldfh.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://wap.fehbvm.com/Article/details/gwosbspnh.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gkkwabvnz.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://3g.hesvh.cn/Article/details/gzgirknez.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.zdbjq.cn/Article/details/grltovnpi.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.blog.fehbvm.com/Article/details/gerhwgyni.sHtML

[E06] 替换子串
来源：http://read.share.zdbjq.cn/Article/details/gthlfcecr.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://blog.fehbvm.com/Article/details/gbpsuqrds.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.fehbvm.com/Article/details/gybyhzjrv.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gbgdjjcwt.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/grkwwybve.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.hesvh.cn/Article/details/gvxvaqugd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gpaaguxfm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://baike.hesvh.cn/Article/details/gtzaazkdh.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gziqaazez.sHtML

[E07] 按分隔符拆分
来源：http://baike.fehbvm.com/Article/details/gsdwhjwad.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.hesvh.cn/Article/details/gutanccvg.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.zdbjq.cn/Article/details/gyxydvcei.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.fehbvm.com/Article/details/gwjfthech.sHtML

TS:   s.split(",")
来源：http://baike.zdbjq.cn/Article/details/gzrivmyep.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fehbvm.com/Article/details/gsxieoldu.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/gvopcegfr.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.hesvh.cn/Article/details/gccaeyccm.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.zdbjq.cn/Article/details/gvvnkavxx.sHtML

[E08] 数组按分隔符合并
来源：http://blog.zdbjq.cn/Article/details/gfvkgmfxa.sHtML

Py:   ",".join(items)
来源：http://www.blog.zdbjq.cn/Article/details/gwcxidtvb.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.hesvh.cn/Article/details/gqxnuxvgi.sHtML

JS:   items.join(",")
来源：http://wap.hesvh.cn/Article/details/gycqhcfli.sHtML

TS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gsvkdlxqv.sHtML

Java: String.join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/gkbkcpdiu.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.zdbjq.cn/Article/details/ggtrjalvr.sHtML

Ruby: items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gblurstvy.sHtML

C#:   string.Join(",", items)
来源：http://blog.hesvh.cn/Article/details/gqkrzetgj.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.hesvh.cn/Article/details/gflfrvzet.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.zdbjq.cn/Article/details/ggnzzgfvg.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fehbvm.com/Article/details/grdxyvmvr.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/gdawptaqx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://m.share.zdbjq.cn/Article/details/gznfrgifh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.hesvh.cn/Article/details/gcypowgva.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://read.share.zdbjq.cn/Article/details/gyekmlbtv.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://m.share.hesvh.cn/Article/details/gjmhpctjd.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/gfhhfuxsc.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.zdbjq.cn/Article/details/ggfuinuba.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gvgpcoyzk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.hesvh.cn/Article/details/gtahyesfm.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/ggqtbsnei.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gpycyubed.sHtML

Java: String.format("%03d", 7)
来源：http://wap.zdbjq.cn/Article/details/gygttcpwz.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gpqqzallj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gfoaketzk.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.share.fehbvm.com/Article/details/grqanlecv.sHtML

[E11] 反转字符串
来源：http://baike.hesvh.cn/Article/details/gtbsqlioi.sHtML

Py:   s[::-1]
来源：http://3g.zdbjq.cn/Article/details/gdrsmjzsk.sHtML

PHP:  strrev($s);
来源：http://mobile.zdbjq.cn/Article/details/grqykavwc.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/gbjtwxepc.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gnnjobvzg.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.zdbjq.cn/Article/details/gooeaedaz.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fehbvm.com/Article/details/gloqogohl.sHtML

Ruby: s.reverse
来源：http://mobile.zdbjq.cn/Article/details/gpmxjxdgv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://m.share.hesvh.cn/Article/details/gjpbetuwf.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fehbvm.com/Article/details/gkfptuwof.sHtML

Py:   s.count("a")
来源：http://wap.fehbvm.com/Article/details/gfmcfijmh.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/grqzpikpq.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.hesvh.cn/Article/details/gnwexslqj.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gwqhibdus.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.hesvh.cn/Article/details/gshcqrhsu.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.hesvh.cn/Article/details/gwcfajtlr.sHtML

Ruby: s.count("a")
来源：http://3g.hesvh.cn/Article/details/gnxbihnga.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.zdbjq.cn/Article/details/gukcnlhva.sHtML

[E13] 逐字符遍历
来源：http://wap.zdbjq.cn/Article/details/ghptgwwou.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/guhhyxkdp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.hesvh.cn/Article/details/gtoaxamvz.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.zdbjq.cn/Article/details/grogvvqpg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.hesvh.cn/Article/details/gzixrfctr.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://baike.zdbjq.cn/Article/details/gjhcsnqhm.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/guljumcty.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.zdbjq.cn/Article/details/ghdyetmpx.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/gheeqiiiq.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.zdbjq.cn/Article/details/guqwbmfiw.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.blog.hesvh.cn/Article/details/gjwfrkyif.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.zdbjq.cn/Article/details/gdjrnojoa.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.zdbjq.cn/Article/details/glcshjgkr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.hesvh.cn/Article/details/gatejjpaa.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.zdbjq.cn/Article/details/gzmhcmubr.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.zdbjq.cn/Article/details/gknjwqzpi.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.hesvh.cn/Article/details/gaiysttek.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.zdbjq.cn/Article/details/gxhjdhklo.sHtML

[E15] HTML 转义 / 反转义
来源：http://wap.hesvh.cn/Article/details/ggtvnkgfo.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.fehbvm.com/Article/details/gwjktgozg.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.zdbjq.cn/Article/details/gecjmidxk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.zdbjq.cn/Article/details/gyrruzztl.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fehbvm.com/Article/details/geytfkwfw.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.zdbjq.cn/Article/details/gmihlfipc.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.fehbvm.com/Article/details/ghdsxdqqd.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://m.share.fehbvm.com/Article/details/gxprleaam.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.zdbjq.cn/Article/details/gpbnldoni.sHtML

[E16] 数字千分位
来源：http://wap.hesvh.cn/Article/details/gubejwrpv.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fehbvm.com/Article/details/gnaguqotx.sHtML

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/gkiayhgmb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/grlmsilnk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gxwyhxwvy.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.hesvh.cn/Article/details/gpseywzzi.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/gduqmxpxd.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.zdbjq.cn/Article/details/gyiocacbu.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/gbsdvttxy.sHtML

[E17] 首字母大写
来源：http://www.share.fehbvm.com/Article/details/ggpwuelwu.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://wap.hesvh.cn/Article/details/gqswnivtx.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.zdbjq.cn/Article/details/gskgvpbjm.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.fehbvm.com/Article/details/gvzakmogt.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gfivzbxro.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.hesvh.cn/Article/details/gwhvaeytc.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fehbvm.com/Article/details/gbuvdgsjc.sHtML

Ruby: s.capitalize
来源：http://baike.zdbjq.cn/Article/details/gbxtfgtfh.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.hesvh.cn/Article/details/gxaqcpqza.sHtML

[E18] 模板占位符替换
来源：http://wap.hesvh.cn/Article/details/gtrpvzmez.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.zdbjq.cn/Article/details/gdsedbrpf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.blog.zdbjq.cn/Article/details/gyilwjpsq.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gbyquveut.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.zdbjq.cn/Article/details/gwuxuixri.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gqknpxwvh.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gzxsgrtdp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.share.fehbvm.com/Article/details/gbxfihvfr.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.fehbvm.com/Article/details/gdbkusxsx.sHtML

[E19] 多行文本按行拆分
来源：http://www.m.share.fehbvm.com/Article/details/gdscbgqlj.sHtML

Py:   s.splitlines()
来源：http://3g.hesvh.cn/Article/details/gmxpryuzv.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.fehbvm.com/Article/details/gwdqynoey.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.hesvh.cn/Article/details/gecajepih.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/giwoydplf.sHtML

Java: s.lines().toList()
来源：http://blog.zdbjq.cn/Article/details/ggafzncxu.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.hesvh.cn/Article/details/gbhipwszv.sHtML

Ruby: s.lines
来源：http://www.blog.zdbjq.cn/Article/details/gcbotgmdk.sHtML

C#:   s.Split('\n')
来源：http://blog.zdbjq.cn/Article/details/gembbsabb.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.zdbjq.cn/Article/details/gjeorccqu.sHtML

Py:   if not s:
来源：http://www.share.zdbjq.cn/Article/details/giaaadbkh.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://m.share.zdbjq.cn/Article/details/gfohukrkz.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.hesvh.cn/Article/details/gpjmsmypc.sHtML

TS:   if (s === "") {}
来源：http://3g.zdbjq.cn/Article/details/gxbyydlfp.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.zdbjq.cn/Article/details/grqbadwhg.sHtML

Go:   if s == "" {}
来源：http://mobile.fehbvm.com/Article/details/gimwmbfuv.sHtML

Ruby: if s.empty?
来源：http://baike.fehbvm.com/Article/details/gipxjuagx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fehbvm.com/Article/details/gufoppzvp.sHtML

[E21] 超长截断加省略号
来源：http://m.share.zdbjq.cn/Article/details/gfinypbmf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.hesvh.cn/Article/details/gkgypbqoz.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.fehbvm.com/Article/details/glxzdzmfo.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gtbbshqxx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gxuidrnbq.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gfbcpluvi.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.fehbvm.com/Article/details/ggexjpbat.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://mobile.hesvh.cn/Article/details/guzxalcpc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/ghbrzmmlh.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.fehbvm.com/Article/details/gqqyaurtp.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.hesvh.cn/Article/details/gnhmbikqq.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://read.share.zdbjq.cn/Article/details/gwulgdltd.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/ghsxpatby.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.hesvh.cn/Article/details/gpqzqwphc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.zdbjq.cn/Article/details/grusbgaul.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://blog.fehbvm.com/Article/details/glxdqwywi.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gjxvsqomx.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://wap.fehbvm.com/Article/details/gldsyxagf.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzitkdorz.sHtML

F. 文件与目录
来源：http://blog.zdbjq.cn/Article/details/gpyvbomod.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjtcxvxgv.sHtML

[F01] 读取整个文件
来源：http://3g.hesvh.cn/Article/details/guzhztvjz.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://m.share.fehbvm.com/Article/details/gjbiprblt.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gklvzursd.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.hesvh.cn/Article/details/gvgtkatcs.sHtML


<!-- 参考信息 -->