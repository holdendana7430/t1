代发 wailian999

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3bhnpdhkd.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3qposomua.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3hhwaxdkz.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3zazeisgc.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3vqzpafve.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3tvggnjyv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3hkgmwdre.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3uertceru.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3zefkstzn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3tkfjpfif.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3pejtejpk.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3bgomgiqg.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3vaixslgz.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3cyadaruu.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3opptnhcl.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3ockabrzn.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ylvukptb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3wnyvumly.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3ozrhfnsw.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3cirbevtw.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3zzpdkjqo.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3vazraobc.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3cegfqqjv.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3vndexmsk.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3yugjybgx.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3jktglzyn.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3npjcmrzm.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3zfsjwjcn.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3ntqpflza.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3tsxbrljw.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3nbzelenz.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vvivqdke.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3uixbjzyj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3irwqmjji.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3mdhiiwmw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3upjqrove.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3zibgkpbj.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3niwvsrpp.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3erkgeheq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3pdosyouw.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3bufjiasb.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3gkukhzsa.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3wtubumha.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3anuamlib.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3eridfunp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3vajzzcaf.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3uuhecerr.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3iwcyxivm.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3cmucikei.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3cxqhgsxm.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3yzhwogoo.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3bqdgsucm.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3acnbleiu.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gtxnulet.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3kwdekupw.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lzjmyvuy.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3eydnqdup.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3kyiyprxl.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uhicxjbn.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3unjpzksd.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ylvnwans.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3ddsubqwl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3ddhhfcxh.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3kfglkdiw.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3pudvdmjg.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3cwjrtsjb.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3hwvgdmjw.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3atsffsdu.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3efqevqok.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3dmpenamq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3guxgelnp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zprjjgsf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3qqdjvzyh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3ghgcwjnm.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3kmoduryb.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3epeuzhsc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3blokbeyw.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3yhmsmltb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3detfubel.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3tirgztob.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3wgugykgf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3cgljxncf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3rndrlaot.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3zbskwzkj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3nqgjrhlf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3jmhdzxbk.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3nxmiijms.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3dsnplmke.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3xrzlbkpq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3aqqcqlaj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3uggmlvjo.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3icryjaeh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3hurtjzbt.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3zbdukuyq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3pbvbzvkb.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3uqgodxxu.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rcsyqnoj.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3omuzsrnl.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3kapqmjoo.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3zqrbhrmz.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3bfqmckgt.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3monucuaq.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3hxwaryov.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3crenmlak.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rocjhvdb.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3ihkkswow.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ugukbdyj.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jmuimzlo.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3nsvrkicy.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3imeswhol.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3iizyehun.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3krmshuze.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3htcpzwei.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3mjuwypqv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3bpacffps.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3neseigak.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fqgzkzmp.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3fhpbkwwd.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3xifwmaes.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3tbekdrsc.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3kxbskceb.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jmvbndtx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3zvwvkkvb.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3teslhfyu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3tmcaqiws.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3txzowicr.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3lsssngom.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3hgacrast.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3fzvrwmbz.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3nsugbwbo.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3lesdwoat.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ygnvgrvq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3mhlrifgs.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3wiwxjsae.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3xvrewgrs.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3tjstnirs.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3lkljwrmw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3gshqjpur.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3xsljbbyk.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3qntkbtcr.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3nksxawez.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zsrjwtbm.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3sidoeohg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3zimyxvuj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3nwmgxlra.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3kcxrcghy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ccowmokm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ecauquxc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dwxhxaam.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3vexghvlv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3uvmomakp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3sesjtgfk.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3cfogfzxb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3hejxdhed.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zulxrbge.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3oooucazb.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zdwkigxh.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nfnmgijj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3aerflyzy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3awwfmcbh.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3trqevqhw.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3thxvvfde.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3vtwxtfaz.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3swsnikno.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3zoahdadd.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3uxsvjglq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3lmpplrma.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3gmlksyyu.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3sqohifri.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3ltqrbvxi.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3tooqqejl.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3zmaevbsf.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3kkbmiwnu.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3cdmbjryw.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3knpamhsu.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3nuqqqtmw.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3cqadtolt.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bowtxzsh.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3azjkzowi.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3zrfrocvk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3lgbgdkxp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3crbqsqov.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ahgwqhaw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ypxugkos.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3jxbpvaaf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3vmdgpvjh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3zjfcmtjz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3harxnjch.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3tpoqzduk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wodjktdk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3mvfpajbg.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3cujjbrxd.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qyishfwz.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3mrxddxrq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3vbhfixky.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3dcgjgfjy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3cvcujcza.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3mluwibci.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3lsyxgwec.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ngrglnlb.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ioyopzqz.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3rsybftej.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wkoqqpho.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3cdjnmcff.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ocofxjgu.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3bpxhndzz.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ttogkomb.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3slvtbupb.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3wwbkamhn.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3fxurkhip.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3xgdiefcz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3ahstmyvu.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3nuzddzlz.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3eqbwscqv.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3zwzrvmhr.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3yaoiqrtb.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3hormtbhp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3wczeoncv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ajxlxbmq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jxpubjak.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ljqrpubu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3eixznxwx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3hqqkagbp.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wdpsyhml.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3jxhylvqg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3ghtafodq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zmomhxuv.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3bziebxyb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3jtkgnnoj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3oebygvnw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3czajgrym.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3kjarigxk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3acjopwkm.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3iqozzfml.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3trrvxxtn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xbwcksjq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3istgouzu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3jzmguxnf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3waakbbct.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pavhbcrq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rlodqume.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3jqvtgpke.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3cibqjwda.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3piquxira.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3lgswzquw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3gpvqwysl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3xazugbeo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3upxbxbwm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3pfjjwtxg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3wdqsnlzo.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3zhhslbzj.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3msmjwuix.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3snrhohxe.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3krmmjpru.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3tesjopnj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ipryffez.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jjldrlzs.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3vqyebqlj.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3jpmwdwnw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3bzrarqag.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3xfiqfkfq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3cqolbkxe.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3knofakyj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3tbtgtznf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3mqocghtt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qnavplxd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fnhenjka.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3omzevjys.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3msfkgepj.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3rgrdtfhz.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3motcmcte.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3fpovmvec.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3rogdumpm.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3jfrxbsxl.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3qvrnokys.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3pxrrtrkl.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3nbsxemds.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3cmmwrdth.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3cxzhkvgq.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3rygkhfbm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3dhfgpuaw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3gahdsayt.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3xhtcztrz.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aknzdvmu.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3otrhsssl.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3eafrqpnk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3txichpim.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3tjakogmy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3itukbysw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3oujjwskx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hcskdjtg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rzoxxptw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jxxbkvvm.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3pxtmsipf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kdxswetk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qxqojksc.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3olhmiglt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3zrzosjqn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3kttdtejm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ugrcfsjs.html


<!-- 参考信息 -->