代发 wailian999

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3godedcnc.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3izztgurx.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3szujrqkr.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3fjndompb.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3zlufcpla.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ovntlcma.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vtaohvhq.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3cwkzbnno.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3eifrnzox.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3cmdeftre.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3bmfuwqth.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3tupnkuyv.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3cwnwsivs.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3nldtekvl.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3chlxbejp.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3trcfxoyj.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3kkvpykma.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ubzpejsm.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3uwzgzajh.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3dikruulc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3dqczrhwx.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3iukjbpba.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3jqrsggue.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3qnqtojam.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3nhwiywit.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3dxmymkla.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3urlhenoc.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3ujyeskai.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3jhsxftgu.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ezqaadgq.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3njrkihie.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3xqduurax.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3apuckufl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3gmkyylor.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3nspfjqvn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3aconwkof.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3yxzfepvv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3pbtefrxv.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3vchlqjtx.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3fnnvgktm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3riywlxqc.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3rxswpevc.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3uykscfnj.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3lfggprxb.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3hypjfgfb.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3sdntwwul.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3hrprdyjp.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3wbebyqvz.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3akcpoarf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3xecyzegk.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3satbbtpz.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3dmvtixoc.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ihrgggoz.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3knuwzpej.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zsymwazf.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xhkkkbce.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3qdbitraq.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3vzodnhrd.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3feiingag.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3kpzagcpm.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3zxlcqsbk.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3dqzmlpeg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ajtgatkm.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3egqgtxhe.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3grcbrcvm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3iijfugqq.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3utghoakn.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3ruexonwq.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3xkyihmeh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3umqszpov.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3gqkcidnw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3hcekmbfb.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3wyybrpdt.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3usacxwmz.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3uaqfurab.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3zjurfody.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3rkdekdyh.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3abwjmkse.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3kwjtfwzg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3jfahpwzm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xtcgnjzo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3bmviidef.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3vdjyrned.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3xuwxlpcz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3ijggwmhd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3pbqczwai.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3zrjvcjzt.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3ogduavdy.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3kfgzaizp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3iblnnhjx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3nbhjshcx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3kqhqugyg.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3vdvpgfkm.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3onrogkcj.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3xbkpmuoe.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lpgpxfty.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3ujmavlbd.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3bvqmwhyp.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ugnvuknk.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3qpdhkngx.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3wuzgocbn.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3inzngrcm.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3sucqkslg.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3kcsoyqbg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zljyrhmr.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3nmpnardc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ednjuimv.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3omrqdxfm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3dccdzijr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3dmdqczwk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zhoqyoup.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3qkpudvtt.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3pxntrzbg.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3etstbxfa.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3emhvfguq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tgwcnqte.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3dwyxaiqd.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3yfrcnbjm.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3zmkjxvqv.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xttmlidj.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nxiiljzs.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rekfejoa.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3gncbhikq.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3bhhyfvir.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3bmthaxez.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3dcjcmtvp.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3tkbetegl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3etxkuvev.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3vwacqkcm.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ofpjwymk.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3gjianfxn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3helgdvqj.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3ldvcpiwl.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3aemjpeyw.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3carqjdoo.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3hqyctqsx.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3twridxej.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3dsyurmym.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3jichsnsl.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xjwzurwu.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3jcuxnfog.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vqjnawwr.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xeoykzkh.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3vmkvqimb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3zcjheklc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3zizlrrnr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rkamyokx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3arzkyjky.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3krcavlvf.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3tixrfdmg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3ggrizgua.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3iacsjxpy.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3ozumriow.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3efxysicw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3awoszxli.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dpflecop.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hekjjwpv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ncsdbehc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3tfimwtne.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xdcsjrmm.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bskzopdo.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3yxugxslf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3mgqrnupq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3kcguaypz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3tbbfgpmb.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3eeqnyipu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3rtxoolvn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kdmztiof.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3jclweenx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3fevedvzb.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3oscwpxpc.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3jqtzwesy.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3gtfagynv.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tjpmmzjv.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3pcmhggud.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3uiswvesr.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3wflxfhzt.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bifsbacq.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3mejaxuvc.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3znelhbzt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3efehtrfo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3lqrdueqn.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3xlbqnkos.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3oybcozpy.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3tmqitesz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3mvtuklxw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dpsuusja.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3kxumlduv.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3djuxzoaw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hqcischb.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3ingmhaau.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3omypaskl.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3nrrxoock.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3pqtatnwc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3vzyuwnnx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3jrbcdppr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3kblskhxb.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3vldwhbcs.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3felqvrct.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3scxepsve.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wlpukzyg.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3iprleysz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3qlpabiar.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3sofgyfol.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3xuuwqtop.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3lknbveid.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3agbpjipt.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3qpowumfo.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3igqlnhph.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3stysvfkl.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3laxvaalx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3kqaklaee.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3ldtdxdjg.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wumxbvfn.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3rgiserex.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3krfpdehz.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3jmmbmvhz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3ceknpvzb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nspqlfuj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3daijxolw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3rhwdzrht.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3cacemroq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3rentffaa.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3dacnjhiv.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3hhyymisd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3stzjjkpi.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3odvmgual.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3pmfknhsc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3kjjskgqx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3zplqmkhp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3jielimzu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3qawahmiw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3txxkwvto.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3djgkhpht.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3kasrwktj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3oqibhjul.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3htcsqbdk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3iyhnczvm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3vpeupvac.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3wbowyrno.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3mdiwrkhs.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3zbcbbrce.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3aaqocrfr.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ehxnwaoy.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3mtmrmkjt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3xoidwaql.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3bufjjldj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3pljtktqt.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3mrzfxgmv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3iudbctfd.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3wqnamuzj.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3nrchcrxw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3vuipfalu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3grsaayni.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cdnxrvbr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tajrgnbl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3sxsfthoz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3rslpipou.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3rceeikzf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3qeecswmw.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3ryzemshs.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3btidmvya.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3dijixqmc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3maapmoyu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3dzixoyfs.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hdjdvybk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3phrqztjx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3cbktxojc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3ugqwxfew.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3gxkepnwv.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3khqpuuln.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hbyvzbfv.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3qtfgnuzh.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3zzlzsbpz.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rsbdiaoj.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3udwmqtwb.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3rigbxeum.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3mnalltyr.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3eiucoxxx.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3dsdyzedz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3eewhnadx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xzzrgtsk.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3cihiglcx.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gixmtqbs.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3bcegqnsd.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3drdtxlck.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3quxkziiy.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3knsssjav.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3slnqwbde.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xjrqmnob.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wrueexbl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hzyhimee.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nevrnzij.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3iqtvshqi.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3tadowpqc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3snsdmdjl.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3nslaeyps.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3qsqjrbzm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3dxevvapt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3rpumtegm.html


<!-- 参考信息 -->