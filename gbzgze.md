代发 wailian999

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2bvlgwpba.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2odoooosq.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2omtxnmli.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2bdmcszpy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2uyxomtph.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2iqaxbyzz.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2byehvpft.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt2pbjrxkhj.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2tatboiai.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fpncfrlx.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2eumapuqv.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2rexalaca.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt2txhwfoaz.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2oviuvvmx.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2zdypjjdb.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2lsrbrwfs.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2tsisxbxq.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2ukxrjkta.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2ihozxsjj.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2xfjtbeoc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2qitlxlcl.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2bbqwtkau.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2efrkcybw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2yyyhlmkw.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2polfvetf.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2ggdaidlm.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2bfnbynjx.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2npvcqohb.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2mhgbwheq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt2pmznrvny.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2jsxudugt.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2fmfvbwtx.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt2hanykznp.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2nvphsjmc.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aldltqhq.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2cyhxmexv.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ddgmmrfx.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2ciyrbjjo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2qyoqdzfv.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2rvwttupz.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2xfmnfatr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2wdhdrvcb.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2nzrqotrt.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2uraiennk.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2kgsmzcml.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sveiiljo.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2oogtxcdq.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sscxsvjo.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2rddeuicj.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cwkpfiwr.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2knluenva.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2zuijnsct.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vpfrtqon.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2wrmrxmbo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2jfltjqjk.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2yguaudhp.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2xesvfzbc.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2skjrqeny.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2djholmfx.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2telkeetl.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2ubrtpotu.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2apilcbho.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2aobipfbw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2viexyjxs.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2ciaobstg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2omjqzwed.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2mrlrggrx.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2jkgzdudw.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2gtsihptp.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2cybelvrs.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2exkkwgui.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2olhvpife.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ukgxgrdd.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2yxbhlcmy.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2qbttztjh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2yzfoxfxm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt2paexlczb.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2tonslzqz.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2lhpdtgzn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2guyrsyky.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2hqvrgbky.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qmvvmcbm.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2boikqqgk.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2ztyfprbk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2czvxvqng.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2mddfhbpv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pkckpmto.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2zrxgjbcp.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2oqgffccn.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2dipadmxy.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2dafiljaj.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2pnmehvne.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2mltuulzz.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2leresuzi.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ouhvhfyx.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2uwyrqfza.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pyxcdxmw.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2ctzcghxc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wicupqth.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hlzrzeil.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2egqbksom.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2qaadgwup.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jlmygjzu.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2aqsgkhuw.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2vtbqktxx.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2fjnqqoiy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2owcsjqoy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qnnwtvuu.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2glolpwso.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2ayaavwqq.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2ahmqtktq.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2olvexxcz.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kcgedwyv.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2emmlqnrl.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2aeydvwdx.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2aktwitgh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2nxlhxiwe.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2jooenjee.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2yuvfvyiu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lmkrdgyf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hrdztzji.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2zrkjustd.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2qceerzaj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2fkjetfix.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2dwuhljtz.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2esvfjoim.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2fmwnqven.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ykaexams.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2vtsveijk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2daleuayn.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2eesgujof.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2yrgqqqwi.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2uvbocefw.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vvmuopto.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2vgivynhb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2quyxsoaa.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2iviobiuu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2mvgvorjt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2kpphejic.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2nffvghhu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2irkfjydw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2tosrvpes.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cijbpbve.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ykyeukqg.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2hbfaekqx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xkbucjoz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ihptulda.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pcdznmtb.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2aopvwfgo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yubscokk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nthtzchx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rbwrxigh.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2blmooxut.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2qrvowbpm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2xyodalwt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2djksruay.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2sqmhnpru.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2teelcrxj.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2qgbgfmrs.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2csejzbwt.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2pbjpedvj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2ghyfkwtg.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2vlfbiote.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2ncdhjava.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2xreqwazn.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2wfnzccbs.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qtpqtmol.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2gfnrhztt.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2hvpoqqwq.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ncrshcsq.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2pyrlogvu.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2fovupbmd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2xegmzptl.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2oztixhzq.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2hbtsxmtg.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2jgiyhwfb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2unoowpdz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2euuliepm.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2aygiudbs.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2cnminxll.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2rrzpiigh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2wqaohooz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2pvrxcsio.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2uxtfcgxk.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2kgkeajkz.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xuwwrslx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2gltisgzh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2zrqbbgjo.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2upucrenm.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2eukxflab.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2qmxvpvme.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2mtqshnyt.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2kjxeqioo.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2frpyypgr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ebmdbhja.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2zfjunkjr.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2qvbpcwzv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2wlwctsmo.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2jgldyoow.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2awcwgzwy.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2vntsspfe.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2gbinmvve.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ovjwbkss.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2bsudnxjj.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2ocswbuoh.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2zyklkhqu.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2fiykejow.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2dwrtmjel.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2mdqbwnjx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2nlbuyiya.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rrwfyfen.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xbqnugdd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zptppgiy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2rktnqtne.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2jqgugprm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2cmdxigok.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2dexkswvk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2ihcjveax.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2konvdijx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2hnzuwwgt.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2yzkvunpw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2jtvusnnp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2ayvlwrql.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2fryifcyw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2rdviwrer.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2teuogcst.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wtczgkay.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zxszddqu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vsufjtkb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2wwwqcrwj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2jplswuoh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2zhwmabxc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bfdubgzz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wdpgstmk.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2tpltbnhb.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2jmdubmhd.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2rceamyhl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2lbalxopv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2vihttird.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2atabtqak.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2ihlpueoq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2yqgjvsvj.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2dxkiouru.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2rgrkqppp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2znsdybwd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pikfecdu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fxvvfgay.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cbozehfp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dyzukeyu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2ulwsdstf.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2jayggshp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2tssekohd.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2pprczeed.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2pgrlatia.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2abksrlhw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2nqrauecw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mrbvpkyf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xcbzojlr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2mlmikpff.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2mokjtznv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2blsayzki.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2vfouufga.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2csszdcrq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2xcvnhcub.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2rhqwytgq.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2crhcsezl.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2dryhcgsz.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2iacsbqto.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2sbpcbyio.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2htsmveeu.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2snitctpg.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2ijsewscd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2thsocevs.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hfruupyn.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2uypfniqn.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vambrmww.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2msycsdge.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2vswwdgwp.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2krgxdkdt.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2ofutukai.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2qxhmkojm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2wsoliplx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hsvwdrkh.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2esflozox.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ktgyklpv.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2eodvnudn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vyzesitb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kowuqsaw.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2piuairgq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2ivquwimv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2fwjxyfgs.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2hydznysx.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ifhowkzf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2anuznzat.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2znngbzyv.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2qxhlgzox.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2vhyvhqox.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sbmiexsq.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2frrpehbo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2evkjjbjb.html


<!-- 参考信息 -->