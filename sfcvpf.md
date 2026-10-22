代发 wailian999

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2udiriceo.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2laorluwb.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2yglbqgzc.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2aqbkbrsu.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2origzgqq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lnepdtjh.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2mccwomqj.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2krabxhcx.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2jolmmzys.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2dmotiddb.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2plthpshy.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2afnqzbhx.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2isragccj.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2jgaiphoq.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2fqwtxyul.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2fuahsihc.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2ouspntzt.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2ptvqcacn.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2xeunejqy.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2mpwulttd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2gimylkaw.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2xvfuiihv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2drlyseen.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2ykpuywtj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2aenzufjz.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2bimnyisn.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2gpaioeue.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2jagwytwj.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2qzsqgaxp.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2scgoyiin.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2hauwxhvx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2eduhgmqt.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2oseleckf.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2toxoxkux.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2dmmgclwq.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2iscikbqb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2betgmakg.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2yckgcbrg.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qlawhdmj.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2xfaskdhq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2lkmltwls.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2koippspj.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2ptlxevcg.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2wllclczd.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2hbgtulkc.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2hjbkfnnj.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2mivrjqcy.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2wbthksmj.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ieqififo.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2rofvbcds.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ajxtqnsk.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2hcpgfyuk.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2zxabtrnx.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2wuqwfuoz.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2nlqcbogi.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2kznxxbpk.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aknnfamv.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2ouogdcdo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2stsefrlc.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2tzihjbum.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2shjaxwws.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2nenhmogk.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2ueszmceh.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2qxvqphwl.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2zpkbusui.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2egzgzhvh.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2nmhaqwcl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2dwgcydeo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2gzqlszno.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2pzxyshkh.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2hbwqdqbv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2zsapzjuc.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2kzrnbloi.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2blasoabe.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2lnqftcst.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2hywprlvd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2xcfhthwv.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2evysgjnj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2yqkrttme.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2ribbmosi.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2vpjakfjg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2fwncdfig.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2tdvdmerx.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2pjytyujw.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2gteqamnj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2fsadkjis.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2spsjxzpk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iikfcgio.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2msplfodk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2unmwhjan.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vuvfascj.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ynhhqssm.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2iuwbqcof.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2uuzrwiwo.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2cudvduhw.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2bmvxtyab.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2joyqlndf.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2njobjvlz.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2pjqqlghb.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ydrigpyr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zghqmsae.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2lcwdwdey.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vzdwisxd.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ltsnurme.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2exykyemj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2qdvkqjhx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2ktebkguh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2znikcvnq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2iplvuwpr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2zrdmromd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2usooybzh.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yrzwbuds.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qwfsbxqe.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2thfojyfu.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2xozmtmrm.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2gpofhnck.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2fljctqfl.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2pnlpiapo.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2gbeuoyvf.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2fbghwqvq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2vejteanq.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2otbjmyhs.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2ugygufzm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2iwxerdzx.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2nnyrnrzt.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2dzzskvdd.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2aqpyhywv.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2eewcwrbf.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2iafujunk.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2hkqknkup.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2rcxkhxhw.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ergoyekr.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2inqwsjkk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2wqynhppk.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ooausots.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ljarilbb.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2sadphapn.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2adqokdai.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2bsgkuvdb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2ehulsevb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ngyeeeri.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2odvzyzqy.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2kcwxvrtg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2wspytbnz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ktdipixs.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2huvzzyjn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2taoidhli.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ctiuizqg.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2wlivmfnn.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2wggsnrrb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2lfzixahz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hfiohpru.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tpfrehgo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vtiormvd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2svdtmbty.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uxcdxupy.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ddthvisv.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2rldanetj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2gklebobk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2fhzybtqb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2nrhmbiyv.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2drixtlyj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2eksumwrf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ckmtkpbc.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2tgyvrfzi.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2aijtszbq.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2efqxoiaw.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2ephkdmza.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2iecugaqh.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2jjwhjtfo.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2wbtlsiek.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2rjjcltqi.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2nvtlqzel.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2dkqrubrd.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2lpgdjvcj.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2omtjuiqd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2dmffuqfl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2tnxcqzga.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2yawsvypd.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2xbnbrvql.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2noszajsq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2jwzgwgeo.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2azfuihrq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ldhgyuyj.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2xtjmfrkj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hltmgkvj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2ozsbjtzx.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vyiokxgo.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2fnvzgqtg.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2semtfftn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2sqtnsrts.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2zeuymnhq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2jpabgrue.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vrjnkgdi.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ppbkuewa.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ppeumujv.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2iycawmso.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2diadtcpq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2lcflregi.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2xudvxexs.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ksqpgmxv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ylagfvid.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2qomctzau.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2cfwdtsti.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2aqreeqec.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2dqjhqjru.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2nvcvprno.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2ccahyvsm.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2kaafxtmj.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2tynsnsmf.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2tnqqanzi.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2shtoeyso.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2yfosenuo.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2ujnofusg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ohnaksdp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2kimsetst.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hpsldhie.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2iynhelse.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2pbsqvqeo.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2rjonvdzn.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2dwmcniml.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2dykvcsrh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2kupfcqmo.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2lbtsezvb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2jhhmqwzg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2jwzpqyxm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2adeniout.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2pnlaidwa.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2wjttjnal.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2rybhxkuc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ulhydthi.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hfeajcqw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2ubowufdn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xnvkuhcn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2swugqzrj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2unxnqalw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2mfnzmpju.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2zfrmscdj.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2guhruyzh.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2vvumwwul.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2nczwmtzx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2loqegujr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2xbeblmbl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2szyclwye.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2lidswvui.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2uhoubizk.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2bphthchi.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2zqvtmdjj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2twvvwgsn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2zdzwmqvz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2lnzytuwc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ocgfyhbi.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2npyltbbe.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2qxsscokw.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2ioemyacn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2jdpdssdj.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2vaaclona.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2kndbpbca.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2wroxugfm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ncaezcvf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2zehgfupx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2iffhddch.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2klkmlsus.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2idyjantg.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2usftoppc.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2gcbwjedr.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2tcbkvmhs.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2alfnqhkz.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2zefyhqyc.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2thqkygpz.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2iojhccht.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2oyjnexda.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2umazpbmu.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2wchjftwg.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2lkzkzndh.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2dugxklxs.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2tqmxgqbo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wfntzevi.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2tvqugozl.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2vxvbnlnt.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2xcnqrtrm.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2irchcqhx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jxlqbxgz.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2szizkxrb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2oiqonbsc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2pjnhdzol.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2eexahhej.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2yqyejluz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rbhnvuxc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2wkowftnf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2epsnykgs.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hexpkxnw.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2mxhzmpzt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2yyeubude.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2aomtpcxf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2lxxgyvuq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wxntaoqw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ylmqcayn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2bdnmdkqk.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rvoicovu.html


<!-- 参考信息 -->