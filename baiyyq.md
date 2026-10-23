代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3cyqoyedj.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3gqyopziz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3avggcscx.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3oxrijvyx.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3hacsrrhq.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3dmetcrqp.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3dszpkadl.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3paiyrtcg.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3vjqeannm.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3yyhqrfmj.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3ywtxgxnq.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3nwczvzmr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3gasqluxh.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3nstffsfl.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3dwjsllsy.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3hredtlbm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3zkevouvi.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3ppsgasul.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3zuuqgzhu.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3koovdesy.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3oetraxpq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3larjuyvq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3egxqerif.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3ztydrqmz.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3tfsimeaf.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3ierorxck.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3wxofxuqb.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3kanieoqs.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3rgudztvc.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3pkromvnc.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3psrdqdqk.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hecjnlom.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3cfpvntvh.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3miritpun.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3qmsjniji.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3pfjitjjs.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3xekvukzd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3rvndtqxe.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3pujbhtkr.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3ginybpvz.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3jkuhkeom.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3oogugyhd.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3vlpakika.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3oqsbsarh.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3bduxhemi.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3vtqxgrph.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3kklblzny.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3sbgcpfhe.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3tnmqrnru.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3voyadkwo.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3kybjcqfp.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3jhnskxsh.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3ytizbwho.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3trywjyso.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3eauahums.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3lftyusyd.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3bndcwxid.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3yjgbcxfk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3vlnyatsd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3jbslopmv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3pgnoomgq.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3zdfrfdyj.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3gzsazgse.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3ynrrubyh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3mzcitycu.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3uwkygtyo.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3yqdfrthy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gztqznaj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3ogijhhsb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3engrqgow.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3ongklomt.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cgzyhmby.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3wdefxfrn.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3bjjplxbk.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zoqdscxf.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3spreesdn.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3zrdixvlv.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3smbrgirz.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zsjjjttu.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3yflhshnx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tazyafac.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3jkasepru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ouzuomgb.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3clozjnvq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3ykuvncea.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kyhsmdab.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3udrkymom.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3hqbhzpvn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3zpegllni.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3woogoqum.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3qtnabcaj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3iolznfqp.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3uqpgmwla.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3ggvlqdqz.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mjdcsarg.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3fkovhhxe.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3xuokgwqo.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mtfsljbs.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3kpbwvfwo.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3vnohqzgs.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3fanqpalx.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3kcbgxyxk.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3ucvyjndo.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3immglllp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3vpzlwzsy.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3kyrpctxg.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3snvcyqcu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3jlszyuuq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3pribbefk.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3irkwfyme.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3eyyojtkm.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3scmmjyqy.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3vyjmszsj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3dwlbvquu.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3arwsjhpk.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jnjwnpvz.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3mysflooa.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3tymodlsu.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3aokplsqt.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3qqdjkptf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3abgfpjvq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3iglfabuj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3sgfhqkmr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3tsibnmax.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3vuqffouu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3hjrkxwle.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xbbcjydo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3bctrnqdj.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3hkutxgsd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wivhtoht.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3yheakrpk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pwxxnypg.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vsxmgltv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pshagpcj.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3uechetuh.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kctowzcr.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3suwfjgil.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3zgjzxhto.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3olwxwikf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3uhokacgp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3yvtmawrc.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3uyhsgavy.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3kpdrflge.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3agcedcix.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3pxejpptb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3xtzvtbsf.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3xkangdrv.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3dvluqriv.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3vrilyjbq.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3vpcinpoc.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3orvoawhk.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3sefhkchw.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3qdraiwbf.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3gqinbeam.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3magudcva.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3eayuifkq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3bdlvqwqn.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3hhvpritj.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mfgziben.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rvikynnn.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3wulzuzbj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3uwbruweh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jnfbhayc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3gwxkqobu.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3oqrlgnxg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3apjxcxjp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3revbfdub.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ohofdtpe.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3rsvqdxua.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3gtzgkvcx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3inirxubx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3yakhhpsv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3owillsku.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3gjnfhsry.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3snukfifv.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3nycfrsis.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ehitvnbe.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dvgioozh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rdazpyxl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3qubfjzjw.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ziflzjxf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3alecatvd.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3ssbaxqem.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3rgoojzjg.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3lqrteywa.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3hfrvddyi.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3hbizycrv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3hejjzpwd.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3wgjegfpm.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ehctapms.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3btiugmtp.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3udopclcn.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3gofpwsji.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3kpvzxyyg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ztrmwlzl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3tvjwnfgq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3gdgpdzie.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ubwwntig.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3gnylkjlg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bhzbksfj.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3ttiykrts.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3icklhpow.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3eigarght.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3hhqejecd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3bycprwdl.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3iublswfp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3rthipbpn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3ibffyprx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ehbvffmn.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3iwdddjdh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3kbhzavnb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3fpsmlsdo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3mbiwztkw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3mdilramn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3kxxbaoum.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3mfzrkvja.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3jyobmihf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ujvytumj.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3rliktczv.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3hlqorfsy.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3qzjapbbx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3eunavobo.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3sbuiqueq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3hfxjqiwx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3svomalnw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3aamebejd.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3niuuucrk.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3asjnrcvn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3sohbuden.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3sbvoywcv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ukbvwfow.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ultxoeec.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3omsefcmo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3iirxxbgd.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3mzpkssyf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3cxseorli.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3rnfeekld.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3iwcnxqmh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3wqjghqdd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3hugcdead.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3cqfjjgbk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3dagzkpfa.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nyyuxjxw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3uckzyuht.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3djkprtho.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3olnvxpuc.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3bysdhbga.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3edwkbxam.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3uwmjdnlz.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3utituumy.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3spkvlhcp.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3ioxzujeg.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3zxudpbyb.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3yhdjwjxt.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3zvtxtogv.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3amencvbt.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3sksaeiqd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3hheknvow.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3cszdacev.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3wrpohegw.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3agkoqqek.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3srpevwyf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bcuyhkoc.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3kbanymwt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3cvsvnfmn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3uawkiijf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3mkisyotu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xwiojnui.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rnzneecr.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3nkcnseni.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3smogazuu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ckzrqezp.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3oeuukjkd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3veiaajvv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3awelnbhq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ivkmcbtd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3shbzhiyt.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3eqclmhkm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3xhfetdpt.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3vbwycgtu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3asdfsmhs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3htzojfpl.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3wncfotvq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zcycrapd.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3gajqbtet.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3nxzrtkmj.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xlpcoiks.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3kedvxkmy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3nsmwbhyk.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3rkcoocjw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3vpldnlcq.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3seqmfecs.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qoaetsfq.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3hzsxwlnl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3zbbpdgzh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3kfnwqich.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3arwwygek.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3puadqmze.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ghrwanyt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3qcmydrfi.html


<!-- 参考信息 -->