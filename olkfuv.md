代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3iakfsefk.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3bkrkbnyx.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3sbdyempe.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3jzcemxdy.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3wzwyzzcb.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3jgebswsw.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3znhlrbcw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3rizjrxmp.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3qukuabkn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3afwmlubu.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3zilflxnw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3zlinvugf.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3gamdyfth.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3uxkrehgk.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3dydkupwf.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3onlspnzh.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3ddajwqhg.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3poqxcage.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ulgoyixl.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3epxfmcdl.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3azybgpke.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3wssfunyn.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3cstmrwkk.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3okyoeknw.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3qtltoalj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3mzxcmttv.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3hobbfmkw.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3tgehcgco.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3inhtgkfy.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rjsmyarz.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fvatdhbp.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3oqhiahjt.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3shzunwlk.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lbsixdwg.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wdlmreem.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3qjsknegv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3tqvimgjg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3rftbbiyr.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3dpqyqgat.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3lbaqptif.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3psltisin.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3optkrngr.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3jrsiodmb.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3jwyqpxkz.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3ugshwcqk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3rmelvjuq.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3mfsscvat.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3griotizp.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3abrcpwqu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3lynlusks.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3rqcqvuqg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3uttptgib.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3nemxicda.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3agvnddhu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3bfbjjeyp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3blzosbkv.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3hsgsbkev.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3vlgulkoa.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3vskqemvb.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3gcalusva.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3qsamzqbs.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3gyuxzvig.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3bkkyeury.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3gcqmunvv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3aarpnike.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yarauokx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3esbljubn.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kuwyhdzp.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3myshycij.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xumjneap.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3odmwdxgh.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3imgnkjiu.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3mxtnolfc.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dyqnwnmy.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3cnqotklp.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3mimffnbv.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3arnhzmpp.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3vozuptpz.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hmmgpuxv.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3frnfzhwa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xdqwdola.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3khoqzvse.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ftagocxu.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3egxzsiwe.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3zglywsop.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3nxbqkhpu.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xzanecgf.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3zvxxztoq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3iotcidla.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3srzhzwbw.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3qcmggdik.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hvbqnvfi.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tbjsplpx.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3kypphbwl.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3sdiqbges.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zyhbzlss.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3iokrzxff.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3yzmtzcro.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3govqhnui.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3dkotwpzl.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ilsdyxaz.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3bvtlnzru.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3yayrekhi.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wsmgrmbf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3naraluoy.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3djbblajm.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3mkmioztw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3qjhedczs.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3lzpbdnhe.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3pzspxvuz.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3pozthtpd.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3udkztyqo.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3momusrtv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3tpjiotoz.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3brsiustn.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3yzueohub.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3qfsohlkv.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3vtfeefbe.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3pbfeqlib.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3rbitmtgr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3vkxfatdl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3mctofasm.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3pbvqggnw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3jtttmzkp.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dkpmkest.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3vfsonpmx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3cqlzqfmx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zdaihwkf.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3xodnelww.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3smjuqiil.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3kuvpdngx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3atbxqqbc.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3egquxufb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yhwzsndi.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3taehnmel.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qzjwpmst.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3glmllknr.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3yoqkplst.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3qynlbvvr.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3scubgpon.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3jajradmr.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ippiqyoq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3nywujpek.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3zaxfqygl.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3qushhxoz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3vortscvy.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3tnnxmdvi.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3cldlzpjk.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3ekvqyfib.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ypusftng.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rwtictey.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ddmwkpbm.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3iydtfllr.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3fpnikrfo.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3yqxyauld.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3urnnabvz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3pamkrsre.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vfcxxsps.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3louskern.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3bjzvoxos.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3dzyeatri.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3grvixrjl.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3zujkmkxu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3uonlxqcr.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3oidqouwf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3lqcmlryt.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3yvmdyiir.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3eewwlgcn.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3aliwbowr.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3nmrxjbtf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3mgtqjtpd.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3rnonrvux.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3pfyqtfaa.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lvnhilln.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3joobuuho.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3sjdabnbz.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3glmmibnw.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3oqhrcykk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3eyosispk.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3tfdksqxv.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nenrivma.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3yikeesxh.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3azdzlukt.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3cslvflhx.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3stgsassq.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3rqofezac.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3tolqraed.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3qqzhatvz.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3cggqxeht.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gopycwtb.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3kfudgois.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3djtwqaun.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3hczrcitu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqzorjpj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ciafwgva.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3kslpvxqx.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xhlkjinq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3oehgcyzs.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3codtyrdv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3cobpewqj.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3xddslobu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3eroeqxkb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3jjtkwabb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3xktwztpc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aeiodxfp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3zywfkgmw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3arxrodfj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3hjhjkowv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3tftptvvu.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3jhktzfec.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lmezahyu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3sycpsxsi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qkoyvqvv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3rhvmnxti.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3yocyyrvu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hxkqaqbj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yihhgknm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rrwenwmq.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3hqdlbith.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3iewbpjsc.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3vcpwzaae.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3xfhjgfev.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3vzjnrwkr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3yxrdcrpo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3qmikpzaw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3lbhtpchd.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3rlbgzteb.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3knjsgwoo.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3pycpgkvo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kuvlbjup.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xruuwmbp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vqhivjwf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3fknbtvfg.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3ublhuqhz.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3evhmquzp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3nvgueqgp.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3dlwlpfne.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3bctxofsa.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3zskxadmz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fxflutwl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jrcjbown.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3grxkieye.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ayqophfl.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3dujwwlux.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3elprjyzl.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3xismhqxw.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3tmnsphbq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nibwszkr.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3pezyhezm.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3rwhopcuh.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ntgyvdrj.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zgxnbfnf.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3fakuljmw.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3wthaaldt.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3hdlanovc.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3qvqtekxf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3btfnwkhk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3mahvmlfs.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3bmzjtvyl.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fxtorwkc.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3lugvvrop.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3ljgqosrr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vxuyevqs.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3gmbrgkea.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3tltzjidq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qavdhwap.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3otvgbrnh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wpakmhqs.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xhcrygcb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3xxddjjlp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zntuzegq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3miqncetp.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3ybhrkgcc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3dtevjrvi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3fggpuhsl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3hthmrzxo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3roggvvqr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3fjncefpl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3mcvpckka.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3fdphggcf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3sjzizbed.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hwovwmol.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3fzywqoka.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ukjqajmx.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ttzezrst.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3ybesjcua.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rrjindir.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3uzwvbhgk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3wbeknrhr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3xgdhmgve.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3hypxscee.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pyjfylan.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rpzhzlfp.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3dfcnmysa.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3qekfyaja.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3sotskmjs.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3zilazbpi.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3oaativld.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3pkvtdsse.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3vjugtkjp.html


<!-- 参考信息 -->