代发 wailian999

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3nsqclnzn.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3nsicwsom.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3snkjnqpn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3hghfbkif.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3krzlgsam.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3zhwerfmg.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3tcvawehb.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3xnbtcavf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3lwqiuivj.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3ulvbzgbq.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gmfprdrk.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fewiwpxw.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3qqqibcdm.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3nsmcwulv.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3hzoygcbb.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3xbijxepm.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3rgqoojiw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3mmpxehjk.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3hqkyaztv.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3djryguwo.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3blgdpbym.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3utpsjspc.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3taezbzco.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3gxckfwfx.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3gcodvfav.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3ylelwbsk.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3gfohbmfe.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3tlqbmver.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3codwlcco.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3ujkzsmwi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3juhjookl.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3zbkczcox.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3qqhuldtz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3hytffsoc.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3nyrjohiw.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3edqoyqaj.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3dffnljdp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3vazccqaa.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3mtuohxts.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hrteggix.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gznhbpgt.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3zxoccacv.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3mixxjrvk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3hcnnphru.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3jwowhfbz.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3mkfyczrw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3wcynjxuj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lfhlhegd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qpholnvi.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lhuimyaj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3wqnatpsj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3zyglqvdk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3ceqaaicg.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3qpvnkuwn.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3aiewlmop.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3bwgqmxei.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3txmvlujs.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zpvdzius.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3orkifsqu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3wuirelpy.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3fbkbukab.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hbufkytl.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3esfvuuee.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3micdmqgg.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3idwsdfte.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bkbblpye.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3pogjcwan.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wdygcfvc.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3zywkbuos.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3lrnyecyh.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3vjqzwqpx.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3iziextlg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3acofrbqa.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3cowhjmzc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zudiffiv.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3gfyvsyqa.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3ewqqzqay.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gdvrodty.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3yktrdxqb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ilqrfuhg.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3sihipjzv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rhremzrk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3rznyyqzv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fvbjanmp.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vcrktiga.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3mancjtdx.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3iwsyjahy.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3iphnhkjr.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3eqbkkfrn.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3sjpqpskn.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ladkgbhu.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3xblaidxd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3valyynhy.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3oeihkcvm.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3hrzvlnru.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3mxvftcod.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ylrhzjfu.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lebiywva.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3qgqcfjye.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3uxcydobz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3lfxuokjx.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3qmagmtok.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3etsjqdha.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3jssguodd.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3dfpunirj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3dnmgsqbn.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3utsyswzt.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3bkfqkkrf.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3bzheimjo.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3zmgsciyb.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qylpvwlr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3yxfhtnvn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3jitxnkwa.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3tojiwhku.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3vpwjthoq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3dfsflxph.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mjunccnu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3lskubiwy.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xxkuntua.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3slomlnrl.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3litiisrr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3fmgxhojk.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qwlgjujc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zoezdifc.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ikbemzlu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mqmwsctk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3dtzcrvgk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rqxveika.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dydwjyyt.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ktyyxuee.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3malibngj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3iqoenpsk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3qkfglzcl.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3vcxllhjy.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3kgrgpnpf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3chrhirdr.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3bckccxkp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3spanamsa.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3tjgulvyk.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3scbechzk.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3jacajbil.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3jexuesyk.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3inziaczn.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3dudpjqtf.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3gsjigwjk.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3zcrrblyz.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3pseraxmt.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3csskmljt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3ixcldgeu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3ahytdsqk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3luszuuhf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3zulsgvdq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3dmvdtvyc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3mddlrfsc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fmeefmdt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3nzhijzav.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3amavndbr.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3smwuztkh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3hlatyjgz.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3cevsmudb.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3aompihfz.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3slxcjpsl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ftroidri.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qefqfvwe.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3xtjqfbdy.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3lopbvtjf.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ucmpemuu.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ryoxvxnx.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3isnkkawz.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3oleptzaj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3ifpvzdfv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3iiiogrld.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3tipafoau.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3fzwaiqek.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3kefoxpkz.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jbnymbqk.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3gfwuaesy.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ojechqxn.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3tbiqsrpv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3zsclxpkx.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3xicsviaq.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3dezelpfm.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3warqokmo.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3pwikgkci.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3wtrgbqpj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3eqlsnytp.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3lhpkhsbd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fbnxldke.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3tskqhlme.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lfhluejm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3zyaicyaw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3hulbdggg.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3hkjbewoh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3hujtocwn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3dmqueigm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3gggipzgh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uzwykzvx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3wehxbgfr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3hsqylpga.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3xuuudhwg.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3lstwexxc.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3qpbotuml.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3ctjgszhf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qkiufibm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bsfpkwde.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3iqsohrbt.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3brzbvmgg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3qjnamhuy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3paalbcyk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dhbshyww.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3swzsyxgv.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3rtdbzxpx.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3yfsfkegp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3zzncahgf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3gulocwvt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3kgbgptfa.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3kzkivbcq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3gaeftcqb.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3kzzymwfq.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3vdrlwusz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3fotoqemc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ewusjmzy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3fvcnaquk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qkioxfke.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kuwtrlva.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3kcskpdzg.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3mohgvoyy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3lkbvdnty.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3gkvcpbbl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3kugxcppx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3giuggzrj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qwqldgrm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3edncxoak.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wsgcjdlm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ariqykko.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3ldbtpyqh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3xpsugube.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3ywraoeqk.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3lxxkintm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dbuivbmh.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3iaoxnmqf.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3rmfxiozf.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3chybealv.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3jtcxmhoo.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3mhlrukfk.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3khbqwqkj.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3ytxlioxi.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3wtbdkxke.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3rmxvhoti.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rfztninj.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3buglwyiq.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ubsakbfp.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3tziyvlgx.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3kbxjriqh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3uydaejgz.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3lmpkesbb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3bonytgho.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lxwtdjss.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jmfemlpo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ekenjahs.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pxkiwsap.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3shrgpaun.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gvobqqkx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3eewtbtyd.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3usntfcvx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vcqygxlr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vvlorjej.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3atnpnhtb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3lecdkvkm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3jzgyolgp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3mnligfpk.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3xewyvohb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3evxbdpjl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3szslznio.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3fynjefax.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rentufmb.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3apzeacyj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3mquwyvqq.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hxeppcyr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3llctaejl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3cnbkoxtc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mzxoyypy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3srtymmrq.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ppbofdrd.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bnqdrvuu.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3uwwogiun.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3nqcfrcdp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3zxxviyro.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3qpcqzpnx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zjnlygum.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3eioatenh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3dioyxlpb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3fofmfvjz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3ijsrwgup.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3skdvopsq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3tgasomwy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3unuuohda.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3oiollbrv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3pbzapzxs.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3uyzfwrfk.html


<!-- 参考信息 -->