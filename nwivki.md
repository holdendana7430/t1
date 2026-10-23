代发 wailian999

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3woeeulik.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt3cuedbplq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3rjivkaoi.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3hufpcykc.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kgswseli.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3mzfyecvd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3szhezjfo.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gbcabdfd.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3gxoqtcce.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3uachtlyp.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3cfpgpjmi.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3vnouflqn.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3isledkma.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3abdsfeut.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3bjdwncro.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jurldyot.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3djevlsqt.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3eqsdorgz.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ctsktmda.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3tlknzthk.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jlacqbxd.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3dslnmuad.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3vdnnrcvs.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3uvsftldv.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3yzroozpc.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt3zbdmfvle.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3rcetbxre.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3dbgftxlu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3fdrhxvki.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3hvsaruzb.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3csfgmjfj.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt3qzuxopia.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3dlrmjkyf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3brcmgyjx.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3yoylfeoh.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3ywhmwqje.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3dbecscfa.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3qdnewtif.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3mucmnvei.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3zrdwgrcz.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3fotujued.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3dlujcknv.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3avcwqzbi.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3bvmmkywu.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3yephvqaq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3gffjcfka.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3qtkjqhtq.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3fraqcmho.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3xzdneslv.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3rpukldgv.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3slhminfz.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3mqtpjrhw.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3kwbnthjy.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fzsdewtm.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3xaoobann.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3dpogdokh.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3xedlyvdm.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3mohahdle.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3tlyuzglf.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3eyrnguff.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3tyywjuqe.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3dtgkvwvy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3gyjxfobw.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3lmyhlkjj.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3vznegmyx.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3bczhsiuc.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3jowdzyle.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3emtuljsj.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3rmjjhetb.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3jgfyqudy.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3ospcfrsu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3pnvzbdpf.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zdxcfafv.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3xpmblfww.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3bgtrmhwe.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3doagkbxq.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3fyqrjfbx.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3bjeccxuq.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3mvadqkbx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3ljcawvmb.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3mnrsmbda.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zcgupbqp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3jqdvriot.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3uoffmeat.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3lfyeinbh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3szawdgoy.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3bfbgipav.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3jllmuaol.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3mouxvudb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bhqrqcxz.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3ywwfdaje.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3fgtnzffu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3irzdgdru.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3ygpitjcm.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3enzamirm.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3lclzctaj.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3pivjokna.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3phzecprs.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ewssxjwh.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3zmtclzqn.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3dcilviwd.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3inxdqdkl.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ofemioex.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3dlcuorol.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nvgkomti.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3pjkpvakm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bhtcmqii.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3ouopbdwp.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3cwsuxyvh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3tttekdpk.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3khwjmmma.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3fdfkpgjz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3jbiofbmz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3gjfxzvjb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3jxsehqxt.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bttcowxd.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3xkpzoazq.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3ahpshkuj.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3gtwghplu.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3hdzimzkq.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3iujyinkn.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rflcnrse.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rwcdppur.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3xlrjthod.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3jlftxaxo.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3agjudgrg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3xsojmbsc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3gihnshhh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3hwfibbvl.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3fwyhhtyk.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3luclzazy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3srruxncw.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3krnfxqba.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3xurkhqkg.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3deucagmw.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ybnlohcq.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3zzidjjss.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3hkantmgz.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3xzkydxse.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rxdbrorv.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3jtfbejiz.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3jehkmmfz.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zlvetnyr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3jhxqrleo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3lmnuncte.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3mrcvrzpj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qxmaaqnz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mfydjkeo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3twglczvp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3slowzelm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vwdjwtsq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ehhlrjys.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3qxaragiu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3sqseddqm.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3rbgbhelw.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ncqodzhd.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lqzzqilp.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3prddasts.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ovhtbusl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gzkfqeoe.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bdbbbxqu.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3mzztwbaa.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3hoccggvy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3dxuxekzb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3vlzaqxbt.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3jclauhfc.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3duhcoaou.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3lqzrtcvd.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3osxftaen.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3wbapyynf.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3hbvvydqc.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3lybitjwt.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3tshjlmop.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ofklycnj.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3jidgwvvc.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3oghcxznc.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3oqvcadja.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3twbauola.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3tavwkbox.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3atwtzkbn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3ozmapggz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dhmoyjgd.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3pgxepwbb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ihtsrran.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3lnbiayca.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3nfepsdya.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3hequwwky.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3bktiipmp.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3ccipkccj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3furjcfdk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3gozdrxqr.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3javhykdn.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3enunroeb.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3uczxpvsp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3srdizuoh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3cumnfljm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3danxnswx.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xzenvhpi.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3dpdyiqic.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3qkjcjduj.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vvacljmb.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3xkruwrhf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fbpmouix.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3dgmwgwkn.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3spbtmgln.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3mcmuhfbt.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3rjtfdbil.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3zlskiiwq.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3ewytzyrg.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3uvitjzdf.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3mrebrltm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3ejzafgpd.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3izsvzicj.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3jcffnbem.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3bpkwrlao.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3oxqltzxn.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3ijvmlbci.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3cuniovsl.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3krllvamh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3lrkpfxpd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3eogjwmld.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3lxesiart.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3cetlmhpb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3xszxshad.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3umsmpekx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3dfiynovb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jhrshhtk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3gehxsuol.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3paceobnb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3slodharv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3ghzkgnrp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3wrdfknin.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3wfusobua.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3uuwsrevm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3afauwozi.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3sbxexhkj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3utcrmphm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3wockwlup.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3usagcchy.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3vwqzzyxv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3huyqydyf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3afnluajg.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3eiigezdz.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ngmblikn.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3szseqpxv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3hiqwmfvl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3yekdpire.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ckysfvyz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3opxponpf.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3lsapqjvp.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3tsamypcy.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3abhhvzcj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3bjulthap.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bozmxvwc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tgkpateg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3utlfdrjp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cgxsppch.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3uebtpyan.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3jtdksppm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3hgodnrog.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3cakzhwkd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3oxomgpcm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3nviahraw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vygwqvpn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ajyvichv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3nyfddsqw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3gkpquydw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3avzwnbnq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3wmskzblz.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3keojnuib.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3phmtanvd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3orztthvv.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3qgyucuiu.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3jpvbzlhq.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3wishmhjc.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ezahjxvr.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3bxqjqmvr.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3vywokifx.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3butjwwqu.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3hsyjnugg.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3imoslokn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3afhdgmmy.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3raysdbbp.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qihnzspv.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3ymdwmxzr.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3bskadkfx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zbsbcuhj.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3eclojbrp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3tixoeipi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3acddmmnq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3uxeqkgmm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3axsljumk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ipmqxnqk.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3tppspmmt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3myyumhwq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3usegohqk.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3ssjokshu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3izntdaki.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qwjjogty.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3jhlcheux.html


<!-- 参考信息 -->