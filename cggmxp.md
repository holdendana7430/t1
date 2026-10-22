代发 wailian999

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2yvuxltib.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2pgibznbh.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt2ngvisyrm.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2vgkyvkdz.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2tkoxrukb.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2pdbaeuke.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nfkjugju.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2kkljhlev.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2etiyzxej.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2myqfubgf.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2vwthqldo.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2glwzlfax.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2msefremh.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2lbjvigzn.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2cydzjtng.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2iqcjbkhv.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2idthdnds.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2njspmoth.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2miigeflg.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2pdykuqul.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2vwgjdqqz.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2dbdgdkjc.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2xmvdthpc.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2rauzamom.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2qdshyopa.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2rkhvuoox.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2qvpdmrsi.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2pydnqfzg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wblyuszz.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2flfnyzsi.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2nkafyaee.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2kfbwlnbd.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2uahihlmo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oovhyqnq.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2urwiryit.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2hnytewkc.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2yyamdgnn.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2bkyfxhad.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2tadzocah.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2eljposhg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2lspixibz.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2jlmekbkv.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2xsqghtck.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2ijthrvbp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2gqyfrmvo.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2erbzbaxl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2otajddlj.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2mgyemhvr.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2vmsoyaxw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2uewrpwpm.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2skbwntdf.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2cpvrxtyv.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2zqdlpujk.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2ouuvqjph.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2yohvllxn.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nekjtyfd.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2ewcnfkur.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2yiznhprf.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2qvosmyjo.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2xjihmojf.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aeidzvuj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2oherdthq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2cjslpfpe.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2bierrcyf.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2ebgceuys.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2nsrilnja.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2ndmfekww.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2hwzbfkoy.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2yosypbjz.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2hgffuxnv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2zcrmnqlc.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2nbutqznc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zwragrde.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2rbqigsfw.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2jhaqwvvt.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2svzuxauv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2gaxpotyg.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2pcigphvw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2nyrvvtvy.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2gvbqbxxy.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2omyvmyxz.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2dhlewngf.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2fxjgpyhl.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2juzvhlnh.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jzoyzttd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2plntejew.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2soubxsnr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2mimjgjar.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2sdbonkrf.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2odycxagx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2qtionhxi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2wvmsjsvh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2jlgpnrcb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2wqjkcemw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sdaukwqv.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2nktlvshu.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2qxlxtgtk.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2fsqrutzn.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ovzudlve.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2pggipmre.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2hblrfgtq.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2htogcgvx.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2dudmbmwn.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ylpmnrrz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2viywuzro.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2amyqwdyv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sigcddpj.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2svgmgmlf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2xefwzudk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2zjtagbqr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2bicaypsz.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2godyhwas.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2smfzsskv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2thcqvphh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2iildlakf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yiafzfmh.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2slidbcnh.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2leruxeiq.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2auwspksa.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pyhnfexq.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2rlssjdkf.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2wzoyjrse.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2njcummyq.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2wreczoph.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2qwrhwkoj.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2xkjloqya.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2ffzeafum.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2faxnqgpn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2hflswvkc.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2xdufxkzw.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ovgwrqrj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ujisvyfw.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2tauqgdcn.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2auswimir.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2lekgmkqz.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2duklxcha.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2naaicuzb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2pmrleruz.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2xdarqapt.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2qigrlxxt.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2cvxtcodz.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lrtljcey.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2mkvenzwr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2xggrbdnw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ipwdzakx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2qqbwavkn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vlovcivd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ggabmkca.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rqrqeylo.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2pnwfvrjw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fscxyvov.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ylbrvkay.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2pkilfrdw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2wpoetmnw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2fldupqzd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kvrjbxor.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nowkuhsi.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bdjgerig.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2pjkwkqxg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qyljqucr.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xeywahhp.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2sbdhfcei.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2yqklejmj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2dfidmkoy.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2zibilthl.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ctmfiiju.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ujlpekgf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2spuczdok.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2ogbkqytl.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2iepiumie.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2ppitobof.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2cyuyhdrv.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2irnongan.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2vhgztxqk.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xuxvfhyu.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2iodqrxmz.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2tllfdaiw.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2fserswzd.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2kjlijgbi.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2liscdevr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2txrovxii.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cillcopf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qyzdnluf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ixksckcp.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2htogbhbi.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2fvjmkere.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2nlciauya.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2mxgqxnfe.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2jrwgjtdy.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ugxotdex.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2psuqjajj.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2egleklgq.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2uppywlll.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2gyimslsp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2lkrdbqld.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2fqvaqykn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2khwhvdws.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2kunmrxif.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2byomrjqu.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qbpuasjp.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hkqydixe.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wjomapol.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2llaenbvu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2usaadnal.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2luiipazd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2djhsqvjg.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2vgepznst.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ziwrvcrp.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2lraqraou.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2taqsdxji.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2mgrjirqw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2winulabe.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2onadvspq.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2loawmlnn.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2etcmtasf.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2kdrfecyw.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2eignnmel.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2zkexvgnf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2wlcyupum.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2myrdzcri.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fgvxwgjh.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2nmomqxxb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2txfliflf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zaiyrptx.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2svdiscyv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2boijotjb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2gfadlzyr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2rmtddbll.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kqkpwbqd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2nywrwutm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2jrhbvoms.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2evnnpdce.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jieagyoz.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2pkjquded.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dfbyqtxx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2erpdmwgq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2jpfawqpn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cdkjqqiz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2raipwknc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2tgcabbmm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2llibngmk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2svpmpkoo.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ogvppdls.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2xmdbujlq.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2lbnnciay.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2vvwohcgj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2fuhabkzj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2lburkurr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2gselqpcc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2eezigspm.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2qvbcfgjm.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2ngssefgj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2dmhhtdxs.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2hdoyaeot.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fibgewvi.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yfpimtni.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2sohwawjw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2qhmayhmu.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ttckhxyl.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2ksupizwe.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2dtuaxydx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2ohdasuxy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2dcwdgjfr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xufuobhf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wfmdhijw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2meqkyxvf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2keoanfbp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ykgrzqco.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ouwaagjb.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2losmyuxr.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2yswwmpjl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kpdgcgkr.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2bpqslvzb.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2omzhldpe.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2abxsnhna.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fccdhsht.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2ynjseefv.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2llyxhkfu.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2silolxww.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2xvhrycsf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2gzrffexj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vywwlzgf.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2tbeqmjpo.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2liyzuuut.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2jpxsfjpx.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2tqnusept.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2nbzskfbj.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2gmnwxzzj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2ncznfazb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2vhgotkgo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tudegrlg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ezunownz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2upxdxedo.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2abtmuhue.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bhvmtmyo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rcuwjjgj.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2evlwpasx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2obnbsrxm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2hiiosndy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wzdekcbz.html


<!-- 参考信息 -->