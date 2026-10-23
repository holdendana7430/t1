代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3ngkjslfi.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3zcjbszxq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3nmmdstqi.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3zdynfbal.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3yfyqfxnd.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3beesxror.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3hqoypaxd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3xfeijejw.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3tjxodujo.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tgrfbrla.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3jfmrdwhi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3qpvlsere.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3rtmbxfnw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3zubtsbig.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3yrafemtw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3yudncado.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3sfmacbfp.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ztbqnjpz.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3pggogyuu.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bqxegimr.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3pmvgvmul.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ufxtytcl.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3ixpjcruq.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3stjqcfmt.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3zbhrsohl.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3zllkxpyz.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3xthsgdga.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3qowrzmio.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3gzwcrcpo.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3owcuhdge.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3nqaokndm.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3avbctznd.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jtkdgjjh.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3iqrgbhgs.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3kbajsnzz.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3psxdxtmg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3kvbqwwuc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3pdachyko.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3kqtgsnxb.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3giylumkl.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3khxcllxx.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3yfclixat.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3xgznpdqn.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3esmdglhg.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3lkojxcig.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3qxotdjvr.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uggcszvs.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3cqknoxyf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3fuadzhna.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3nsskshey.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3gzhcllkk.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3ooahydlp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3zisoetsk.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3mvyompnc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3okzpdqdi.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3dudekflp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gmorgvpk.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3egwnmcqj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3bfyopcbr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3uczgbnjj.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3ggiyodro.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3qtiqgrth.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3fwpfaldh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3eskqbvld.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3ujbefdxo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3gigvqsce.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3vfhodlkf.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dkcerfwa.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3vfwoojjl.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3lqqlqjhg.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3sntjghsl.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rqfrwfdc.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3psrwpdzw.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qzjirbva.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3mmorprne.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wguuezkn.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3weejgfqc.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3fajmaruu.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ymodtcpz.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3gnrpsyzg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jfyoyjgj.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3nrowftxc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kdtkhysa.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3leupxxwa.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3sykovbnn.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jxmaspsm.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ghfequgb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qbsurzxz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3ducpsifi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vjimkbsd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3kyqmmiee.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tpbteafz.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rqxihmif.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3kfcqszxz.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3zpkdbman.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3opdieejc.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3cryganuf.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3hhcvfrzq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3zfuwtgsv.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3azooozda.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3kitvgnbx.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3tqwexedc.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3novzvxid.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tishhaud.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rlaygawq.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3uyubfjoj.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3wgbsfbxg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3raqbccdt.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3vkxlxkro.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3aisnseyc.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3qtwqllvn.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3gqcqvika.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3oeanucyz.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3sgagfgst.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3fxosggnq.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mnzebvca.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3fvlxjvub.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3xupogcnp.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tujdjcny.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3ozlnguud.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3piyffcxu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3nibbhqvv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zdyivoxm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3xbjjmzqa.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3crwegous.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3aigjjnqa.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3gfwiigme.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ohzapacs.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3ejqwmnaf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3drlbuehq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3vtzkyrga.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3matnbwwt.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jmkzsexg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3osvvobvk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3hknmnsef.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wvyerlcv.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bskbgtwb.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3jkbkfnma.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3jafvictm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3stupcbqw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3fajhfznq.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ojjbgvdc.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3wfavnyoi.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gprtnhyd.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3ttqttldz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3msobhhpp.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3elwldzrp.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3zfreljsb.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3syzdzphi.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3xjgiqbci.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3lltvfgsb.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3umrwnath.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3bxkhqxzg.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3hzlujbrl.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3htqdgziz.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3wntgqgbn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3ekvlqiwy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vfmonpcs.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hzunfnya.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3bzdsssop.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3iaivofhm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3alvxrkno.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3uiuvzdgi.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3eyveyzmu.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3btqvtmvs.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wvyxkoxl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3qstbijdc.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3egzacqvq.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3saustwmv.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3zoshkweg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3nsjzzyrb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ozmetxbi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3blipggry.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3yvacpyur.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3chnccxwa.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kgmethes.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zfszfwlr.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kbuibyqj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3tflpytrp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3fxsgeyla.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3inolbvzt.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3kurxvcjs.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3wnrsvkgg.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3qgluopdd.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3nfjqdrar.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3olfvsevp.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3vshzqxxo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3tvhebmfj.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3erktyacj.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zkhyoada.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3cltheqiw.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3esxmctdo.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3stnfaexw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3vfbeakji.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zqigrqlp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3sstemvth.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ojecnerv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3hakakldq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3jmlmoqdz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nmwnpxqv.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3apcdgsax.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ouzrixud.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3jrtrluuz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3iyquniln.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3ndzsjvgs.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3volyrcer.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3btnyuzib.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3smvkgflk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3tnmhafbz.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3kbahmmgp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wupknqku.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bsqtrslu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zwyregyf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lfhblxgn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3kyfzeiln.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3ihpuyvet.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3nfklfixr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ocxqmxvl.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3wjpgzcop.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3rxchjhtn.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3zfbktobl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3kpbzxckk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3qzhaxziw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3aujhulnw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3tkjmliut.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3uubqheff.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3wocpfeur.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3krejxmvi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3ynenrvhe.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3sokhtiiv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3oixcyutl.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3iwxpnwyw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3oaosgdrx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3bvfhrahz.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3qjzjiovw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3xzymuhwq.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3ctlmfdwf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3jqldvayu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3arntlhre.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3zfwgdvvt.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3hfopxnim.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3azdrwzgf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3tucsbial.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3fqltlxil.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3rxomowvb.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3gielpyrx.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3ubrsuwwq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3cwgobmvm.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3iejgjxak.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ekepdpit.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3tvybntcp.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3keyrsvle.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3phuyjdvg.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3xkbrlbgk.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3uwzwzirg.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3ewaqhzqw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3mnrdeqhn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dqizjwtu.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3bhxfqkww.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ctzkquyv.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3xejnbjuj.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3bxwinqjk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3xncncxwc.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3sxujrljl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3jnfocvbb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jscrcezj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pvnlgxxs.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3myliurhu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jfwvrtqc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3sxhjpycu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dvozrbai.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zhqosqai.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3mxwkxsld.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3crvikcri.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3kpvmydgv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3uskigcwh.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3vkhgktxx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ndmcudjq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3dwcnxrtr.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3oepqofct.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3lxkxvgog.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3sbnesfzp.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3uxlquepy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dsxuzmkv.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3naqviasp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3kkjtqqfp.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3goozbdif.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3mdwyfyxf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3jxzoszzu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3mgrebloq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3hzzardgh.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xwfqjcmr.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lmmeubxn.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3ahplfzeq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3qtoszhsp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3jajfetqg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bfhpuyaz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3xrapwkbt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ozvqglfl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3bumjgawm.html


<!-- 参考信息 -->