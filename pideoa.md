代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2wzmpumxn.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2diexmksm.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2ejjwmabx.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2fhbursfm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2cmmtjyve.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ognclxgp.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2kvwuvaeh.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2opbguaqt.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2ekuhvnyh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ujbrzake.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2blmxuvdj.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2jcpypifg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2jcepskhu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2qgbtwyko.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2wfxlevmg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2ixzgfvbh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2ibjnmjcf.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2dpwluszh.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2esukqjhq.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2cvkwaeko.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2nohnqyrz.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ppjttgup.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2jtiuxhrj.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2lxvxsxqm.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2kohdnlpo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2ydpwrczf.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2lrkpgkxw.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2pbffdlpy.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hvpoebiy.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qtcstohd.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qplhipyo.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2emohcnet.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2wsbcuaik.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2epiutfjx.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2qdayzuei.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2wnfjnosg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xeardmvd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2jhddxhjn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jdbjresx.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2uxvrctlh.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2ergentnp.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2pttrkmpd.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2nhshbzgx.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2ennpdypb.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2xetywrwt.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2xaitreqy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2zvgoimlk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2uxzfrmoz.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2bjjjtecd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2pwsyfrlc.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2iyeszirq.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2pwbbmnkv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2vrlkfjau.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2ebydapjb.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2arxzisfk.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2hylmvkek.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2prntzlrt.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xrwvkyet.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2umgkbary.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2ybtyymaj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ofsaervx.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2ofqremjd.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2prnblymz.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2nknihpru.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ipauwihn.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2rhpcoavx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2hjvqpebe.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2oyzjnciz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2fdnbjrfp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2yawbdhit.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2qctobfxp.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2yanlxgtq.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2jmmxkapy.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2jxgdgtdc.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ljnunzhm.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2ydwjzark.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2ykuuvurj.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2uirwfvbi.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2psdckgdy.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2zyredety.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yqxooaqv.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2mlvnbgrj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cxxvrzao.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2zrgapwns.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2bifaylar.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fwwxynhk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2rkzgwbrl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2epvwmeqh.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2nmzabmzr.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2wmxegcoc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2achpbtzd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vrvlsafu.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cjggtcfp.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2lmpcdzyb.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qfmhwyld.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2tjvtteyx.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bwnmmtxw.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2mmrfuclz.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ulcbhprl.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2mzowxugp.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2bjuqnmuw.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2efavmgiv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2mxlswrjs.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2nvomlill.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2lonunhzg.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2kfmvwyxw.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2jqaoxchu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2qdrariiq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2cvqpjbbs.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mqigouzj.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2oukvulqi.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gqnxsdew.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2gamxmahr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2impwojqg.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hbhvthlb.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wignrouy.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2xooiaoxw.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2bktbcxbs.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2bkcqjymy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2acdnfwmz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2fqtkpxoe.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2skjaystt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ddaxfrcc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mxepsmtr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ilfwiewp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2izuiptry.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vcbfqdzf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2glsfwdzi.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2suqzofxe.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2owknnthn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2yrkoafml.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2oggtmtgi.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ygfskoqf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2bhihbhzp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2hryaacbw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2iriwiesn.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zraltmde.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2aurleobu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2habzizia.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qiwdoiph.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2yxujhbqs.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2lkyyjepe.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2hdycfmay.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dwvwcamn.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2wrqgqiqs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2gscpocbl.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2ymseumvi.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2dvbtojlf.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2glghgsec.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2qwflrooq.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xwlkvvmn.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2doavbblq.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2susxfdfs.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jkujrwdn.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2deetjfos.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2qxbujgjg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2sgxvfxqo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2mfbjpoii.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2pybpwocr.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2mfqyqgyh.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2upqpjnlh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2sjsyfcmb.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ynhyesnb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ogkpvsku.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2zbartnif.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2lstmjpvk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2fmqinhga.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xgsbzzmk.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2tcjfbnrs.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xccpvkdx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2exsmmwxq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jkjqxnsa.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2uqnifbyh.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jxcxbaps.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2yixnogfn.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2oqlcxvls.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2agdlwrbc.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2hujfzqjf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2frmhkgmh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2fvmvjjae.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2lqntiypd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2hovrfire.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2gwatreco.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hbeyapcm.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2difbvokr.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2gnsmbgjm.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2fpxxngjl.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2acrnqmxr.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2uaqdkjju.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2fhmzerod.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2jzciatzy.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zdqbtjgi.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2tdikvyje.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2fdzgzpdw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2gmzsesst.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2klbgfduu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xhfsqdgr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xwfaqcie.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2oygkoscx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2lexukkgf.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2pyfdqxzb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2refiatxg.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2hwqdhhpw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2yjyxkmpf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dlmwjnvi.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2dssuyxss.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2zqhemvna.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2kossitom.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ugwwcpmw.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2tcnabwdl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2lfyihatu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2youafmyt.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2ehzpaisk.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dpxzboce.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2uyayjchr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2suaxjiqm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2ohlhwuao.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2faujffra.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2fzuqqzdz.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2jqqbemvm.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2zwhijzds.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2bjuftyjf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2lkqexlsg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2faanlxlm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2zewmcomr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zcuugtds.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2ffiksftl.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2ajbbvkkc.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2odjszkok.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2xuloiwks.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hhsvstxn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2asgafjvy.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2noxmkzii.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2lyuzzcic.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2nrtnnanz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2datbuvkk.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2bjegsgvp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2eifpmywm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2gxaabtuy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2zabiesxs.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2utxbucqx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2yhntkqtr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2hwvwhmri.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2dihqvtew.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2orqopspc.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2idnygzgd.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2rlxruert.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2icsugdsz.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2tafyqkdk.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2elqmwyml.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2jirhpmjo.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lbmlhmak.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2ysueqdjf.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2gecdqyzx.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2twmnvzux.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2kabjgbnw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2vilsrvzm.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tcnhwuwl.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2qmxegomf.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2qwiviszf.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2vpkoefbn.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2daqbmtss.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2qbbpwhiw.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2wmtnngfr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2wlqigapm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ylaxvyqg.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qnumocyu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pwbwgnet.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hztyglfq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2hajbmtiu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rozfeuzo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2oeymmaci.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2rkcxlmdp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2jfaekcoa.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2dyguikpa.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2eiqftkut.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2uqlyawat.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2jlpqrncz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2bdtqqzne.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2xjqdheke.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2iztcejhv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ssbghysj.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2tusdfimz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hqzfbhix.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2kcjmzowy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2gmprgtvh.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sqlrspmd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2vbepzgvt.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2vkitqbfp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ydrzulzp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2nmolcwkt.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dtrphgbq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vuijrrls.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2gamyxcgy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2zlpmhcnu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2ximrzdeo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bovwerzv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2owpxygzr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2cfmumxne.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2gmzgddle.html


<!-- 参考信息 -->