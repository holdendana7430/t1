代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2bxrrkpsy.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2ymrbkwrj.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2dxuwsmtu.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2glzkybgs.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2rwgwpydq.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2dyzloxlu.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2gmwonqdc.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2wblpvoar.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2uhlohndb.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2hcsrhjrk.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2wccubldu.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2dlqxdsvi.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2olkkmrvj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wcrdyeon.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2dhdtferp.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2yrbcatcb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2nqplyppd.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2jktqinqq.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2cqpnnrng.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2kpalrzjb.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2hsczuufq.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2mkxpuktp.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2vbunyzmu.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2pgsrwuwr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2avkrkaza.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2sgzjdweh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2vuxzhxir.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2hdjbnjcw.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2tijqjrhh.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2vlrxtpis.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2nxzkbwwx.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2hwnxsnut.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xoeknrkz.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2gkqcbdvf.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2alpezpoc.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2mjlzably.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ultoeanu.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ncoxuxwr.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2pilccrls.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2weqffiux.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ynytxriy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2vjqwpdpu.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2teimvhit.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2diayvypn.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2vzhbkkpi.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2iooftgqq.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2kchrlrpr.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2btfpsvvl.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2bzfliztt.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2gosqsgfx.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2gjvjjuyw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nsvarwtl.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2kcrlfmsl.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2vsnzrgek.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2qgvonfmo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2kudndale.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2olormelw.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2ifyhflvt.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2suodrnqz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nmwlmkyp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rsjdtbhx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2eyzujytb.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2tcnxnpvy.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2bavhhlah.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2tnsptlza.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2mdrhkoru.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2mgtzcyww.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2vyffutfq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2kycfyhes.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rbwwgohb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2hzfmizdn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2szmoffnq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2tcsxfskc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2wkbryard.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2pkzxpzbu.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2brfddcgz.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2rhpcmwln.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2gxiazpxz.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kyjduptf.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2zluxwhxb.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2ypcraejn.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2wruibbnm.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2gshdgygz.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2rdggrefr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2svhmynjk.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2ieuymqcx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xxobjeyk.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fmssrcmx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2ubtvgqvu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2wwyfjkfy.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fuirccbk.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2niysgmnq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2ewpfquva.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2jumljwwk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2rwtpoaeq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kdhupece.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2yjpzcrcx.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2znkvzrcw.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2khervhqd.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tmklxbnp.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2dtpsbfzr.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2lvqxalur.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2bzuzuncv.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ykwkkhtg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2fampfrvg.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2imryqrkl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2xyecihqj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lbkfekaf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2oexdrlbm.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2chwyzxwm.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ffwysflq.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2iqcgxodh.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2edkduyqu.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jecqokdw.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2jpetkdua.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2kwmkntnp.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2tpdcfjyx.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2hiiljfvv.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2xjfwwzsz.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wgutmcrl.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2jupgyvoa.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ljocqjtc.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2imprfzou.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2wamxhwdv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2awqaoely.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2cxrcpyfi.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2netepwdm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2lrbefnjy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ibghnhfw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2zpbfjbmo.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2havrxfms.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mscziwbf.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2zhrptivv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2phiqucoq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ofsujuzu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pujqyirx.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2msigrusc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jjgpsuri.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ohipfwoe.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2iarqfpfw.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jzcqwzcz.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2ymewgwid.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2tbmvyart.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2abpgsvrq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2prlpqlkr.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2bjpztfkt.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2sdeihupe.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2jvwquaeu.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2hadctszw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2ofitockq.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2fcrocfyi.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2fftbiwuj.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2xbcbdhko.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jleciocb.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2zeizhgnu.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2nepdubad.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2kbuvinfd.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2cjhevhla.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2glgsnxgv.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2lwtgdiah.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2vhvuxckn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2kkufevsy.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ratwzcwy.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2wzycuxvc.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2xdgpckhk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2kwdeiavx.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mhwpzwds.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2qzwqmuti.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2owmnwryj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2plfhpdhy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2ftoilnwd.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2pevgqbtw.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xzcforyt.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2wwbkzakz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2sylbaefx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jrklugpw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2svpbvghe.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2jlslngtx.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2cstlphoj.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2smzvqrvp.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fskitvai.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zmslkfur.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2znzlzgfu.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2wavhljix.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2cnqxpkfk.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2sbdvuwiq.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2rzawyafb.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xzaiypyo.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2noyooyse.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2jtkbdeyt.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2aghnowdr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2sapjvadk.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2ilzmdxef.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2xnsofzzx.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2fnmfjzeq.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2zgvrsktn.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2akijllru.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2cbgwahks.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dyizmgtc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ldnsuatm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2yjpzrqgx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2jhhemnif.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2lkxxqocy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ocprtjfh.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2ugpipoii.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2ogsyhhtr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hixjmovs.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2nterffyc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2qxjxqvij.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2vspigcau.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2jdlartxs.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2hedhnkuw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2cocxuoas.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2ajdpthsp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2iokyvnsl.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2eufenmzo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2zivxsxmk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2yenrowwo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2aosbrxef.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2slgctuam.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hyvuyenm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2nbpuffed.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ahglvpyo.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2mkncwjyl.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2pstrmeaa.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2dhfhsvfi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2zovtcpac.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ofdpihqb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2wmckyteq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2rvamyskp.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2nqiyxszq.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2pspvfhvg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2caumfrnb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vvpjclmv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ehzcsmzz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2urqrhbox.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2fiyexngt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2veehmrcp.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ynuwhhqt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2uhlrrlvc.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2mjwvqlfg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2lbcmlqed.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2ehreqstk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2lbsxgnle.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gxcgxnqt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2gzmvopds.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2zstrpayu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ihfdyvwb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2wirpique.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2nnbyunim.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2miagwlgg.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ibdgocmg.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2euzatkyj.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2gotcgunp.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tfsgjjhz.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2setsctly.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2xspumopy.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2vgubwiek.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2iefvjovl.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2lmoxwcon.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2srsdgosm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2ivypewde.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2kptddkqn.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2xamhnjod.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2zjxsmery.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2cffgoxrb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2cqlrhorf.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2uxafvqwj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2xdiowhdq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2kpfskhlw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hnieneig.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jtlyorne.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gtyppgxp.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2ubtzaoun.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jfeqdtqq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gfsnxubb.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2ucxrydgp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vibcnzqn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gwonaknu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2gfmoxeti.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hbfqpsly.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2mjfrbboe.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2dlttmthp.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2yerwvbwu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ddsvivgt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vjertxai.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2meeqsaam.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2oussunkq.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2cpdtlftu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2bldaaoyc.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lspqzjrh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2bhwhcccp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2xupbfvpm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zxfmmwqj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2dikmcgxx.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2roortyth.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2avltyrrt.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2qqyulsju.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2bzyxhiaa.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ddudgmdg.html


<!-- 参考信息 -->