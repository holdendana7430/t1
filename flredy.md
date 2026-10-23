代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3ynvhvuev.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3bxxrtmxt.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3nrcubzxj.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3xsuapcrb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3viwjdinr.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3qccdfmtz.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3gebsscuq.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tiwyyfkl.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3xsdgwgir.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3xbexhlkk.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3ewebcldo.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3qxyfnrtn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3gzeimwub.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3ffijqyps.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3cozjwjjo.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3mvlibwru.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3ijdjvpjd.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3nilvjmsj.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ksciazwn.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3zbcflrzo.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3qapeywtd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3sbmopgxc.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3nyavqyeh.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3zejmxnia.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3ixbbfblq.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3yalfwyzr.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3jglrfbpj.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3svdhjlwy.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nowoavfh.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jjfzddaw.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3kysswmyg.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gdiqzgvl.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3cycztjtt.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3vilmhnza.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3atfpdckd.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3ouwesjdi.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3ahvvzoni.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3ppnvfzcn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3oxgnrhop.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3uxxhxlhs.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3lhtfhokn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3ukdjxpsu.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3ibzqwvnc.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3ghkqctuf.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3rsafsibn.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3geeimdzv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3hgzewaey.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ozbrrhdt.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3kgtbmomo.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3gevvthxs.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3zwswnbfk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3pgjaeogi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3vxqozuxm.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3awemirar.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3lduytnsl.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jwsrddcw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3vfbilosh.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3bsqrvspa.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3yxbrdwnz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3kstniqwb.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3wvnugjtq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3mbdzfell.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3ykbaxglg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3lfjcknxy.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3dqohdbko.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xydpodxz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3fpuxqjas.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3gemtbehd.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3twpgkxul.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3xrvkyxoh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bcqkwvsa.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ryeygjap.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3stumltlq.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ggzkcuhe.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3fuvsrskn.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3gdrltrfj.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3wwkvfknu.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ekubryxt.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3gycufxxb.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3pofjplvl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gxzlbwfs.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3vvdeeorq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3feuhlkvg.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3iwmnwavl.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3agvyqavg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3suwjtnva.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3wejakbbh.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3woawwugm.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3tudzmwcn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hqtteakd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3gjvbourd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cirnlndy.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3kojsyxuz.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3nlfqxvvt.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3gioiwupk.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ghqkzqey.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3iyfkgpuv.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3bdskmtjw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3uapfddxx.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3pizfaiyf.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3tmsklexy.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3rmqmadyb.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3wnknmyce.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3opoqonzj.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ottscrfc.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3hhbfqijh.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3hwsokpxy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3xvtpsiiu.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3uzasubnt.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3nqawmdyw.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3zckgbezh.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jjqlgule.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3pprwkemj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3vhculuqo.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rlcpwsdz.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zmvjlhnn.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3woxdzxqo.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3fmjicspj.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ggyqdvxf.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3xbhstdvx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3zwjnemkm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3nrzxoudr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3pjgbpggp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3jxtptnbl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dhohmllc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3koequhfh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vmznokqe.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3pgrahgms.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3uhtcwrsq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3hvqlyttc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3fabcxykt.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tphllmdh.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ojtlvhab.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ylbfqttd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3epwtmtgn.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3efsoyihb.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wzyenuwp.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3alwtacfz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3vdpavqdj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tmsctomk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3lptsflyq.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3kdnpoggn.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3ertcrvpz.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bswbelze.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3aosaafbi.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3cpssroys.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3lgxgglls.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3kgrdvzxo.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3pashowaw.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lahgxabp.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3gvutyvee.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3zzufzexq.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3daypnyla.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ufaryarv.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3iochbrvf.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3fpztcmwg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3kdransaj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yznwwvzq.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3zlepvdpk.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3dtpphwub.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ilpltvme.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3gutvevku.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3pyynzmjr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3oxvtkjvy.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3usovghlh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ijceyses.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3taymbnsa.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dtyxlqhp.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xqppibwj.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3cmziomae.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3vjypapjq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3yjlplncq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3lokgfugy.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3azrxqfju.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ucqjyucs.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nbsziyxr.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vnjqecll.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ujxvxysf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3owcaelwm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3nyzbqjkd.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3prxnsdak.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3vtujgjic.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3relnkoxe.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3pyquncwc.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3onqzstcc.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3lgvfyrqc.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3gdltlmfn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3wzczgfln.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3nbzidqjo.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mvsuxysf.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3uyxksvfo.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ufkvjrdx.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3apolfjvu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3tgohxlbd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ybegsfam.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3eliiabwo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3opsjcima.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3qssiised.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3bxnfwopq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3foobrgnj.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3mgdmxxnw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3qmlgbmfh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wfilkwdj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3dznqmsvz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qpengsho.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3amixrgla.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3xhttlibc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3mnjqkffs.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xigvwdnl.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3oztbcmsc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3pzdggwcs.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3alvzipka.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qyxrilmr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3txrxqzsl.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3niolxjck.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3xrmajdff.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3dhtoaqrt.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3ctbpavxb.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3htgisoqy.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3xcuszuyk.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3eayhvccd.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3dreqwbbw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3vjiyiwjy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3tgujdsnh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3ltwvverx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3oxwvatdm.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3zozwnetk.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3klgmzyqk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3hmoulhvm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cykzxdsb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3qeyukode.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hupynrqg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3taxyxznp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3jdxmxjfv.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3tsbwsxqo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3ocrbmyku.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3kvsqgbmn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3cqtfysox.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3vtkzfwri.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nznhwtah.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3umnugiih.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3wkhngwel.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3xhelstwx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3smrptvhh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3yyvxzifv.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3ojhfyqas.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3bblfdlcx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3jatxsdbn.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3adhwrmdg.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3bqqchntj.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ukyxxdnp.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vuieabfg.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3umphvkik.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3nmdkkbob.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3ehfvpdpx.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3mhcladfa.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3idplnmou.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3lqoqbdxp.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3jatvolyb.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3mgwehucz.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3ycinxgmg.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3kwgiknuu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3bmilizti.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3qrtienhd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3jvsxsxdw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3goabvwak.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hdxepqqs.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qbpmvmow.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3cdrdqfqx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3yrmqqoof.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tvupkmmk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3uzdvmopr.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3wylygqww.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hoimwzhu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3swjrfgww.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ynbcfkis.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jgufekzg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3mlxehsur.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3xycksslr.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3blfiwexc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3bqvfcxdr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ubhutnyp.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3yzhysoyb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jthnqogc.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3tpficacl.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3setswzdk.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lpffpsvd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3riobssae.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3zdftagtn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mnmeucfm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3nibqgwgp.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bugghvov.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vahriybi.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3efbkapfw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3xbxowqdu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3amvpkqxu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qdhgalcp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ihtnukcu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3fhpeiiqc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3qcmlnsrh.html


<!-- 参考信息 -->