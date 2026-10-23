代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3ibspzfjq.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3diafhnxx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3ridlzbkp.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3zaanytvt.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3xikdxivn.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3xlbgxuhx.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3jucspsuh.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ddrkdxfc.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3faktgius.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3tpbcgrqk.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3jhnjzryl.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3vckftgcw.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3qiactzui.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt3ujvpslgc.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fudsxaht.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3avminymo.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3wxgnpdvz.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3dcuzkyaz.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3tghlgxye.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3syzhukef.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3cxeihucj.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ldwcvtzr.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3txudfuso.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3chknkukz.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3azbxoxra.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gcntutqb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3izfbhftq.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3rhldrjhn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3zsxiwudx.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3jsmahrru.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3mdcbhkfr.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3sbpinvvj.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3tkrzxcya.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3swdwituo.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3cktmqpct.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3unvuqgyj.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3fkbplata.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3peiwvbam.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3sekogxsh.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3aiuetcha.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3gqeugmhy.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3fbnrqwpg.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3hqzqnnhe.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3xisqiehs.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3hwsdmwyv.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3bcvplbsr.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3wnifnojt.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kgbthneh.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3zneyceif.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3typjjwcl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3ijozhksb.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3otjxdtqx.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3rxctwfpu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3xgkiyxlv.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3lyuanozt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3lakmxeqa.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ofwqgmhx.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3tcgldsml.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3csovwvxk.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3ffdzguyf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3caumiipp.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3wxatqrrs.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3avnxtggl.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3bbwospku.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3apcvzeqi.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3qswsgdfi.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3ykuoqygt.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3xfyhxumy.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3ijmutujl.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3bgkqpvfx.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3urnkwdzc.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3raubmhxy.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dsgkbnkt.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3fjazphdp.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3poxhredd.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3kwiilqfw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3swzysacg.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3uyauncyl.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3ceukintf.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3hklcihir.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3goixjptu.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3iwnjrvqq.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3jjtzucgr.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vvtzetxw.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3oitlrsme.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3dwokxrls.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3uckhirtd.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3kpuazrxu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ulqoqbvu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3fllkjqhg.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ekqfomit.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3nzcamlpm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3ffcekkjf.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3hgrdkjgo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3usujratp.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hcgupyfe.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3lmjgrqni.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mtmsbdus.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3qkqydhmd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3dzdhzijg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ealpqveh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3hpjxgrhy.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3hegwumyh.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3njdfplek.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3xsndyium.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3roeevqft.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3gckxqbrx.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3yzmwfgjm.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3yfcwvipc.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3xunbmzcw.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3cpilnbbw.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xwlpwohh.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3dmdmqlhd.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3pnsqavdl.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3akxbwenw.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3cqkdzwxn.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3qvfulwoo.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3dqschzqr.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3wdnxgyme.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3zwullimr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iadhunof.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3axmrzgcj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gxjltnyj.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3dpcwdulb.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3dgevnaul.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3jpfrvvka.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3ehzenunt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3yfyfmule.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3vzfvazct.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3zunohufk.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3fhzyrula.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3oivhthbo.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3jslbwbof.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3rcyozlzk.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3ntxpgxtr.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3naliltyv.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3bpikpzni.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3prhjornc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3scpjfzmn.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3fmrjootu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3lsgfbxez.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3bkmufbmi.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3mijuwjnd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ihiaazcs.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xblvfzwa.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ckxllugo.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3prircfct.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3mxghfffv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3fucbhgya.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3jgqelltq.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3luqhdczn.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hyzfmtln.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3xpiycduh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3zrkjuftt.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3zcvooprl.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3uhieshtk.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3mtaforil.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vnhhghgx.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3wkatzztu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3vesctftu.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3daaljnnj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3nlfloeft.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3sfgnprtj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3pmgqfkst.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3sjzxksiq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3xzrpotej.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bqtmvmec.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3wlmchbol.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3pdqosrvw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mwhytbly.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xbedadwi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qptphufw.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kgzfsldv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zxlnzcen.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jnqfimho.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3iirwglso.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zqzpdbtp.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3pgpqhqcu.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3aiajshvj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ytftfqgx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3ivichgjg.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3wjlbobdq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3tivkkpax.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wiyynfir.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3pwdufpqn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3ulqsaxxp.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3nwnhomio.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3bmgoeykl.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3qlfchrje.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3pegnvppo.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3llbjodmz.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3qdayxkgp.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3wlnkekkj.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3zmklyiqo.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3pijfdfln.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3sxlsfhhx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3ljwhbtgy.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3uozgprdb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ggwpioaf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ttjdaxrs.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3hhrvbedy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3hzsagzpr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3orienoxm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3yjgrbjcf.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3jeikhgro.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nhrbawmu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3ewusxqvr.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3apikvnhr.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3exwtlhmq.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3tqrsnjqm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3khatjgqv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3mhdhnasq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3izxukuoz.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eyrtdhjo.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3uakxgtlm.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3raoirykv.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3tqxnmpjg.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3oaprmmzl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3awodsntq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3aripucqb.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vezpkvbe.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3pzxwvrem.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3bjjajeod.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3trryjeqn.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3rclimorh.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3gnitcrhc.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3akgeatqv.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3gnibbrhc.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3qzqpwefp.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kidchgey.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3mnoclden.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fhwefibx.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3mzstfidy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3anxeijem.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3dxijvmeo.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3cgsuiokg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3pkdkpwdu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3tmgmgwyr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3ichoiiuy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wtwqdkge.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3shvwcijj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3ghaigmcn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3kjmnoukx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3nugdjahm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3bffdkzfb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3mvlspgwo.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3sswatamr.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3qolimsip.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3tjgeuvaa.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3xzsbtjol.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jbnlwcqi.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3letkdyxd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3fxdxbrpf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3yzhotrgy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3rnuqgkax.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3amptvbda.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3vhmomtke.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3zisuhzin.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3agveysru.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3xragvhok.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3wqtyrcxw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3gtwkhwsi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ttckwiog.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3cirnqwhw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3dcyrwurp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3kshkpvva.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3stgqclkb.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3cpvzexov.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3aelanqbf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3foutoxgh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3laakhkqm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dagtzeiz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3itkdhwaq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3epobdaor.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3vzeakskz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3sokrypla.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3oczhbake.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3tipusroy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3qtvnfptn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mkodebtx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3rptycjeo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3maqcdzbm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3cprwvkox.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3nforzhub.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3hvtcjkds.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3dgnhrzck.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3tegctuhz.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3dxzyutyq.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3tvidmntw.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3xjlrfdyq.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3yzzlyzeu.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3fkqfhjwy.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3ixfkhhhj.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3blzzowkp.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3gprgjsed.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3ppbfeuxc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3ptiuuzjs.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wmraleiv.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3evrbtltd.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3snphhkjn.html


<!-- 参考信息 -->