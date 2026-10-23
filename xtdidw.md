代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3azqzdkeq.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3xtimjrwf.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3hrxyvxaz.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3asxvftiy.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ioknxkhx.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jwlydksu.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ixmavpns.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3cstyjhbh.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3zyrxvgtm.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3nkbvoyjp.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3dvzhodzu.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3vbtfaegi.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3ilqyqrla.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3ylnqndmv.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3xpdfgpwd.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3oszdunbu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3bmmllqcs.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3zfhljjcy.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3fevmqcay.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3msqtixhw.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3ukalsmpt.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kfvydgwf.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3wipkvwju.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3gbuqbfje.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ntwdlwtw.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3hehbzasj.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3ajafnfid.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3nopcrujn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3aqjkxglr.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3piookala.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3ougimmeh.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3qnkpyyhh.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3objsdwfr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3ekdzpoky.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3jgkiedjs.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3mocwfmyg.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3xgoswehj.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3ervzvwga.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3ouwoufcm.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3lqvkeabh.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3diflamee.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3trdwxddm.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3nwfndexu.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3nwkeclkj.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dsqbqmlr.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aaghbyoj.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3cvaxtfbf.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3gezdylfu.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vkeouxcr.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3bddvbzzc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3nzyeadzv.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3jognnklo.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3xgjysopn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3qvkpvwjg.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3igtjfpjb.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rskulxyd.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3jjymilrd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3zkuracxi.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3drjphsxl.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3hzeezhkq.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3tstmpluz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3blhczkgl.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3qpxhqgjg.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3raluoegd.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3eapturoy.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3jbeiroio.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3loyqtjnw.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3wmkgelrw.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3yrscvbby.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3izxzbllk.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ylghnhog.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3clyqtjlk.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3lgccvrmf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3foikfnyy.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3itkybqhq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3rufdsycc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3wammmpyh.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3ndwtuizc.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3smbdhvqp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vhcmrcyi.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3dzbglort.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3qdkcbqij.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jtastqtn.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3sevhyisp.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3teomzxjh.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3yzgdovwi.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3lriwkjfo.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3yxmiukxf.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3fxcftwhh.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3spvxvxqw.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3pwrxzgob.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3wzzexxnt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mkhosiub.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3xipmcqaa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bkyyvklj.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3bjsmcxol.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3olklhgdo.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3kpyurqwl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wbtszmbu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cpapyicf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3rvhvbyde.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3qlxgyznp.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3eeiejjql.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qgsghuaj.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3aopqpfos.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3oojvwuuk.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3wggdyhni.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ukwtqshg.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3vxhhqqhm.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3jfeufymp.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3zmheccku.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3eghttohz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3wssdoztd.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3dtrwxvrz.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3lecnwcio.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3sjojmthe.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3dfzopokf.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3tpcfbwwa.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3cwaeibdx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3gnljqfbq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3acaykdik.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3praobgtf.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3lxnrlzds.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ddhogsmm.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3tiwbpwez.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3snicjoqw.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ddyltrnf.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ojmvcjcv.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3zvzpeyyz.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3fjcsbohw.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3akqjxglc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3nofellva.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3pigkgtzp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3lurdwtbr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3tgexjqah.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vphbbnye.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3zotljjek.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3ahetmokf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3gyuhzeqb.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3wlfiuzyg.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3lcvnifqo.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3yogefadw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3fkqqxcsn.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hnziqvwm.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ltslsuyp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ljvzswsp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3euycogem.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rvtzetvr.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3daoijkjr.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3wmpivatr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3yotlwkxw.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3zddmpywg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3amnlssro.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3jfjtfuzt.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3yshdwqso.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aklzdbvs.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3rrgbirpr.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3jqjglwmc.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3rqjypfbh.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3fbcukvjg.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3ryhumyyd.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3avysszmt.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3mzhktcos.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3jeffhejk.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3rnfmqfpj.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ucytizok.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3vqtkyzba.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3ogdjvsce.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3xozybyeg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xuarhnes.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3akysmplo.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ttianksa.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3bnjqwgta.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3ggamrvfd.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3rcggkwpr.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3rmawbutq.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3wprnqxxh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3jueuaeid.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3ntqskvxy.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3mqajfset.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3pyaawayr.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3pllirijl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3yqxdlrwu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3lyygufji.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3spaxstyu.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3uxsfkdoh.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3nutzosdr.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3cszctsup.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3izzlaodu.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3cuphwkuc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3ukvvawyw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3abtjnxvp.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3qaonitet.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3wymyidrp.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3fiujjkfb.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3xbiallbz.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3qzulsrfn.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3nogwzazf.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3dzkmwzvc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3avkekmwo.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3hervpgyo.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3xivgfgct.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3zdismflr.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ieeeyeub.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3xinnoeic.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3vkogqgaq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fjcwkmfi.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bdahxnkb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3guwwxfpg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3wyvfgzxp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3lhbbmqmh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3hzyqhanq.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3yuloobxi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3obuqwsxi.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3qnfwaong.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3ajywnrgw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3txwfxrmy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3bgoxmrup.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3fngczksc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3ybkonnht.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3jvjxgbtw.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3jbvsjmtz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kqakmhjr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wxbvjxtl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3exmwjblg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3phxlkclz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3fdobueyj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3iroatord.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3swdmieyr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yawoakcg.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3wssokcow.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3lpwgdjwi.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3rftjilsg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3eckgaldm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3lwfhzaeq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3xbbystbb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3nymcnano.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qzzrxhda.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3ytuegqms.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3ksqbsxyx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3zedrthnh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lpphodca.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3nevxmxkt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3vvqsokwl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hcssduwq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3hhhusvgm.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ywphjsos.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3bsiemgie.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3jajvszfi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3emesatqi.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3bdoqvjwn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3yqqlbnpk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3iycevmrf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3cyrkkfkv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3chziigzy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3hjhlxtno.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3zbxzpzwv.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3gkvkrnpr.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3wiimkylo.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ohdhrknd.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3kogxkigc.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3jwposkbc.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3jshxabpf.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3htbteevb.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3vutbcmln.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3ohociwcp.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3aivrfdhr.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3xbnduido.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3edloiuih.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3znzsjwnl.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3idicbtbc.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3omxgxzwx.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3rzbpnylr.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3uwnoadke.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jqqeuiom.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3tdntuvte.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3povxlchl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3tyqsurze.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3wjittavo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3fnbnyely.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yvpptefi.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3ptoxzqrm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3srlhmhjr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3typzazqt.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3yvabzuog.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nbwewywb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rkvdvsyt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3epxieplp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3cvsjagbe.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3voihqnom.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3eujgvelr.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3buuuyxoi.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3betsshfj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pakhwwms.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3mdezsmza.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tcjesluh.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3gdhwdpxb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3mmmvqkdz.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wdemjntq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3xkvjqnwy.html


<!-- 参考信息 -->