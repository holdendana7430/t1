代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bbkyxagc.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kxszfsid.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3klmkmzih.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3pqczblgg.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vysewmgb.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3dwchlauz.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3rtrhyizm.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3fyqymfou.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3sktfqjbo.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3dbvbrhoq.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3uteneuwi.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3yvravnsf.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3oftlyeli.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3ahgtamez.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3wenpsgxa.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3svpcgzoa.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3ijlziudh.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3vylvfpkr.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3utbpcsfc.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3jxavfzha.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3vedaqpvv.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3snxhraas.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3hywmaoqa.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3ommcomgt.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3fiofnppw.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3fdwbcfbu.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hctqqezg.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3uiilnnoi.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3qwhklklc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3yqolstwe.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3cbzpmixn.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3azxwwbkf.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3jrlffskp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3uwyolvkd.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3jyunhshp.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3zibqbsci.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ahvgdotf.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3sisjjelb.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xzelrefq.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ybaledfx.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3qrpjuusi.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3urhvlliu.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qcvszjbx.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3mejneuaj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3sjnyacxs.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3pflvffnn.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3gsdctbqi.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3vzlofmlq.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3nhxcwrbz.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3wskwyymi.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3gqcwsvzw.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3hpuwqzrx.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3pcbgpyrb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hpxmdlph.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3oqdmljsf.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3pombygrv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zczvbnhs.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3viqbsgmo.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3pdwvyexo.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3zmhuwljp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3pshjhsse.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3yhdefkbc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3pgazxpiz.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3fahfhaun.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zrvxgpgo.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3acqowatl.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3zxuiombk.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3kaclkjbg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3bwfbjlyd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3gyptdlxq.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3fjtclkjl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3htzguooh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3qlzngaqx.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3wxoqbajs.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3elenzlfw.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3iwmvgfmb.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3nhmycxqp.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3dzqcfvmz.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ggkgzxic.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ioqbdjqo.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3txugwcjp.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3sqdlntsb.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3kzyyuruz.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3tmdzuioi.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3brgtylls.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3blyjfktz.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3hytnkmwi.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3jkhhvydg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ggchxnkr.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3mzrdccbq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3twzvtzgj.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3valhychi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3lcymfahz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3lgybdcoj.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3fhewfuuo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xikvedag.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3vnkhkvhb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3biovyffx.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3dqjrkphq.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cdvpyqdt.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3lopcjoha.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3vwrplnth.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3ijsdfips.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3wldlrjjn.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rzcqokix.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3qzegydif.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3unwplbyw.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3hmngvfkj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3tkecnojl.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3mtkducnd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3zoucppyl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3huqrtpnc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3szeaftwy.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3nyampygu.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3kvkurgps.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3wxfpxxrb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3bjtwtwoa.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3nehizneu.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3tdwyseur.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ibycduyp.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3rjfqydyn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3wkytzvpt.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3nawlzpgp.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3rvcxmpot.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3pirglkkd.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gisywkzu.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ptjnkzfa.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3jlwctzpi.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3wixxuhlq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3cynarqsj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3wpnuncqs.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3swaqytdo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jufiqpjt.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3lsqfnpoj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3vzzzrirf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ibkpekfs.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3qkuocwpy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jgpszvzk.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3gfglfnyo.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wwolaqnc.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mymugphz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ivsphgzd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gtgmgitj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rumasipi.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rqlkvzle.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3lctlbgqu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3llcgjsnn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3qraurbek.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3ehyxebok.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rqzvynjd.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3cjelrsud.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3vybightl.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3ouqhmwvh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3vswzmxco.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3adqwxaov.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3retxhazz.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3ftruutaw.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3erbrmahy.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tjtizmai.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3nhvhuybk.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3rsyshwiu.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ibhpqekv.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3kmqjakyz.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3okxogowq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3wqtdvjxi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3bjvggvir.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3abfappmw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fxqflxgj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3qymzpgth.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3wkccvgix.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vtvvoddu.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3jmvjfrxf.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3cokienmu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3oczqspzp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3oorqedjn.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nzwtdcve.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qnmpjjzx.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3zbcrizhc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3yiohvbzy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3nhmotlod.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3tikwmcll.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3cilbbaki.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3pkirtjzm.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jxojepsb.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ypbcjjkh.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3cgevzckr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3lugvecvj.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3rfdntrdw.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3kxtdbgbu.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3fqmsdlig.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3iwwjvbsp.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kvhflgdo.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3qvfixwot.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3cziumsnc.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3zkbjrcuf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3cqnrurzy.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3ttrvysql.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3jdofbgwe.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3xxnxjfjt.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3kxacqikh.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3kukcpuhp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3aseynqlg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3oupsrfoe.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3viutskbf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wwddxmjf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3cnctjlzi.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3uumqgbpl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3xliuokys.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3cycjtsuw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3umlmmpkt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3liejphxc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3fzfgyzup.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zhlrxlqe.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3pvcrdktq.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3vgnhazrn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3agregdcp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3coszpfjk.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3wlberjei.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ajgjhvlm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3yjegljmj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3etjjstrv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3dxrvaswy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3fwakgjdq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3dizjecnu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3rhpwqlcc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3krtmjolt.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3evfzdwft.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3zzdgcgyx.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3dacpdtue.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3faayontj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3omhvqjtf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3sjiqrsux.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3iqgrqytc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3efqywrpi.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3dykztngh.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3mvhsdztv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3kwivoaxe.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ecjelmfp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ahtpfwsh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3pszjgmfe.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3zaphlbrq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3zocfvzaf.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3rjycbfsa.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3noldtpak.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3lbhyytii.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3vhbjitue.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3uavaipdw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3hofhjkqm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qqdtvpys.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3cpqausqz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wvfwzdgi.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3qdnisfxt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3fmeruxfw.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ngxomwbx.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3cadwmevc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3dyvnbsup.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3tuvcntfm.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3romcejvm.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gnieypew.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3tmvavytn.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3mmwusoqq.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3zxoomrnd.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3idrjwwns.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3tdricumw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3obgbwgyk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3ragveufz.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3qqxowlxi.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vxiziygc.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3anulmpsi.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3qkyawqsb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3ahvqonlo.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3jkzqjncx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3stvqzfnz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3uilkyeax.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gtlhmpuc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yqfzrcyp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nmuswvvt.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3lioxjqzq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3utjwjpvq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3oryykjxp.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3alstvjtq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3skorrcwy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3geewlkdc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3nifenonw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3legrfqzm.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3vdvdoapa.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3fpvknlfj.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3rrdqrcvm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3swknmnrr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bjyauekv.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3ibywwxns.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hzlperoh.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3zwsywfvc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3rpovkrdn.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3priglsdw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3wjmegqzf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3tszjrxuw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ysqnylmz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3tvfugniu.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yedvyeuy.html


<!-- 参考信息 -->