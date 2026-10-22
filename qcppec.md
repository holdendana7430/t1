代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2hhfdbfwh.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fnchcjvj.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wgiucurd.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2dlgdfgrv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2cdkmrhfe.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2cjiezhwl.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2fdtwwkbj.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2dxxkfibt.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2wsirzsql.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2fgshptdr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2iijovftc.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2mkwlaxhk.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2rwblbwra.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2elyqbetq.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2czzwoili.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2cymtlmyd.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2pbzwjedx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2whlorflt.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2puwhoctg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2yrblnskf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2umvntero.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2zqjsziij.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2xjblievv.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2ihvtzdbc.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2osptxehd.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2qchilrke.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2geebnbvn.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2wlbrwzhn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2uhbzhmkr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ongytfrg.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2kgwhddnc.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2jodzshmz.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2tixcvapz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2emhnokrt.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2bucvrqtb.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2ahskxoug.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2hmoilhnd.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uuowelot.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2uvgxevyj.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2jtbadycr.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2gfypxjhm.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2umgstsjs.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fxxlgseb.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2ljxicjig.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2wnabibdm.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2olahjiwg.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2ofhskuro.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2smmkcvcj.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2yfkjdekh.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2dlhwbjsv.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2oilccati.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2kcijylkw.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2ehqrfnvh.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2fwyhhgck.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2xvmdtksd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2uhxvcuad.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2bgpqeojw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2lewudocu.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2dckejgmp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2fndzgbrq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2borzmeve.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2ichqejac.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2rwrbloia.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2qltfywds.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2xljldwzo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2bfeycwmm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2nbkeyjcs.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2sxapsqyd.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2jnpaihge.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2glzqbcsp.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2encrinmr.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2zzxgrglg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2fzqjjffj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fgikvype.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2lsrcjwtk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2oeruxaxh.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2wkiwnnbg.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qjnrpdpd.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lggsowvj.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aogpbicp.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2hwxypxnx.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2jvgrzmul.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ncuialtc.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2xyqcaruj.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2lvkztair.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2ryudjwey.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2umkmzvoe.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2sclcgwjd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ojdglzlr.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2kcsthvoo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2apwwmnwl.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vmwqjtjn.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2ewtyvrvy.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wwochdcf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mnqdrpag.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kzztwmyz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2iasshnlw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2wqtimpco.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2umalepqm.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2znqqwrir.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fbyicjmx.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ywujpuhz.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2lanbxacb.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2yhhfrqfz.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2jtbfuosl.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cjvifart.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2nwphjtav.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2tdmrdpqn.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2lcrcabqn.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2pfbfpful.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2plldtoqa.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ieqhqszg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2sucwmkal.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2aruyzguf.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2dtyzqfwp.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2fijarper.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ftkaunas.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2wfrmwmzo.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2buovjddm.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dlapmrdz.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2ohjzhcib.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ndulrqtv.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tlbypsbt.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2uovtowps.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2uaqdwzde.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mcqwgxtv.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jzkxfviq.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2qgkkssuy.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fwcxaahw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2clgqlfaj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2livgvpni.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2daubqswr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2qrjmfbop.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2sqfpptpg.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dqmczzkc.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kwrykulj.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2pzqzkrxp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2jukwmevk.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2hlanjqru.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dgpqnoxj.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xzepcekj.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2obairejb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2pewzzjfg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2agugzjax.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pzdsuoiu.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2bcdydgvf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2gipqhfxi.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2tjvikkbo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ayikxoca.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2cululcto.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ccercxfs.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sjpboyxe.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2hgsgntvg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2txbcbmpu.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2gzjiqvwa.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2msdrtryr.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2qwahvcsn.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2whywmngc.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2muelugew.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2mnisditx.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2zwfprpjm.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2aedzhspz.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2nyrhbnpc.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2wajbjekv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2kqqrchlo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mvkjaxum.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2mgtzwekk.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2baqoodlo.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ffefaxxv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2strfzuia.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2fenqhepp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2vnfwksch.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2medmwuko.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xxtmrbbx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2hxgaokzk.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qczfndjj.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2syjxqwjc.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2eaivczqb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2hshnbdds.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vyqyxxmh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2qqcoligw.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2zitezidh.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2bqumcgtp.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kjfobejm.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2dtzluvap.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fvrkuenu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2yjartczd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2szvwzqzg.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vhysbbok.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2jiqgtpjl.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2rqjnznvx.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2hpedmdme.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2mctaasqd.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2rfgwgynk.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2xjzajhad.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2tvfjahif.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2qtrrqjji.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jngscpar.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2jrtvkrew.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2slnqiuay.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2onogvjip.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2alzjaisq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2khomzsbp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2lmxkhwyx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2bfyosvmz.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2eyhabiwb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2evqqfvjm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mhmyyatm.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2pvsaxlpv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2bqjpickj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dwvjdgca.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2bejnhjpp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hifdvsoo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2loxugciw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2vqcmtlxf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2gzmhbcii.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ravlcysz.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2escbzhsl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kzoumbsz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2nlplfqml.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2lftegzqh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kzqafnil.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2rtkstaqz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2vpxxzpgr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gwgojzwx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2kuvxroaj.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2wskepdlf.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2thmreugg.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2jgxpfhao.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ksgszyob.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2kimbdyko.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2eztrhgvk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2lnkrchca.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ytafnskv.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2vgxtvyfc.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2bfjfntmu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2lwgoqqzz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vumwmidi.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lhdkhaqn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2axopwvev.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2biqlhojg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2bbizbdcm.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2jeoidgeq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2ueezsfds.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2uyhxoddk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2cjfqtrzu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2poonajxe.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2aksyqedr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2itassrli.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wuinxkhh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ftxjvtgl.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2gjcrhuwf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2elxagqdz.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2zrurihpi.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2hsrxpqfo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2tllhuexa.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2giicarmm.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2jbnpgvvx.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zoqbztye.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2iodmzqho.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2impfvpmb.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2xhntyrvt.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2wlabjdbl.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2dfjbtlul.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2dzljklnn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zqiergxj.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2uwcgifll.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nbvqbasq.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2dekaarpu.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2rudcoffm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2hzpqftfc.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2eegyfxnp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2anmzosur.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2jqacctao.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lrdqbwtb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zyxkvdgp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2zdkhgbuz.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2rwjxbroo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xamqdzqd.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gsbfgsbv.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ysqzkmqg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rljlypnj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2bungbbse.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2rtkdxmik.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2mclznrwa.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2jvnfzltz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2lkcopgrj.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2swkfkqbf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2rfttydqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kjkjxnkc.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2srdfopwk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dkiojial.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2wyvmuopb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2xggpnqbo.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2edafasxo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2gqwfvhdh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2hozczobh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mxhwedqx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2ucepdgzj.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rswvgqqf.html


<!-- 参考信息 -->