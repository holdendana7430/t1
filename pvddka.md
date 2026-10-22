代发 wailian999

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2rtwccvrq.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2zeelawaa.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2wuulmsgd.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2uzfrepaw.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt2fpianata.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.52xcode.cn/Article/details/gt2nglrehbq.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2jxqrecgl.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2dlaomndg.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2pbhpgeon.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2muiogsud.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2yqoznzyb.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2yvgbhuiq.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2upbrfewo.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2qsgotkyv.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2nifovzir.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2ufdzogxr.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2dmjimulr.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wiozgnfg.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2vsubiyir.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2zjawfrjo.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2uoymieml.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2zxbyazhd.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2snutwtal.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2jtklvzgo.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2swuatdho.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bxcaksbt.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2arvbhyzs.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2oqpckbeb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2izbdeuba.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2vtjbbkfl.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2uagijpoo.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2mcnwpluj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2mzxdolzx.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2ozytuyhz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2vgcmxlru.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2vqyicuxd.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ddjiykle.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2cqfshddy.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2zuvbmfpw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2tyvsghmj.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2dyqarpef.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fclcryje.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2qgezgnax.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2jfmthejg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2kkwbtwak.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2lbtrfjfl.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2gogcmdvg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2picwxdwl.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2ilrviagi.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2xkqmltag.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ahsravxq.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2vsvfqwgj.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2kqojofup.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2mwfaqzsu.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2rsgmfucb.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2nzhzzwaz.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2awjkjupz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2wfddhmgu.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2ohefujec.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2rvobfztb.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2coeknhti.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2nykedtjj.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2igpdppuj.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2tzvvvvew.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2leagafai.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2xjrwvtij.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2crphqmto.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2giofvbtc.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2unsbfpwz.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2kyhholuy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2fzlbyotk.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2sowywxnr.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2ajoltovv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2bqxgkcvb.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2uqogipes.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2sflfrfoc.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2vyxtxaqa.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2oqdxekpm.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2likuncif.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2jclarubx.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2cadmoluh.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2arwbkqsx.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2ycsvqmap.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2revuartk.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2vptuvzuz.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2czlwelyo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2fowugtms.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2uacsvhpf.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tzeddpit.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2bpaognky.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2wygwqzqh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2dthsftvi.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2pnosoglf.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2wvlebpsz.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2bjiajwkm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2wbdrvyno.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2ogkybprd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bwkonkab.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2yrlgoloi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qjzkyypi.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2xvjmrmfj.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2eqshprqo.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2wlulzitf.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2ewkjnmfb.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2psymbqby.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2qkxcseju.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2wwpghsdd.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2trhvgiin.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2pprturtg.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xnlziglo.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2caafzaad.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2yztxtcco.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pxblhwre.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2gxpikzwz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ucnduzdm.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ekksolbe.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2pmnvzjoc.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2fqwgglhe.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2jvcdmtrb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qvqpykwd.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2yudjbqbp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mgumlxoy.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2kqwvimbf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zjtgrwnt.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2bufhswth.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2uzoeesof.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2vynsaroq.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cdagruud.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2dfcqfjzv.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2tugmadzk.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2sycrqxny.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2wupuajsh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2ksnuisov.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2eotbvzbq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2dwzsugcd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xttyxuia.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2djwcduik.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2pzazraes.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2kecqvrql.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2lzuaisqz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2qhstwrgk.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2shmhxrsm.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2vfzprhkt.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2xjokztme.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2urmnidxu.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2llbxtkvc.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2cwrffavp.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2pgoksgdg.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2qxmcqliw.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ecthlnit.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bzzsdcsp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2xuonhnxq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cfjwgwjw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2mtdwjkvp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2syaxulep.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hvahnafv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kpileaej.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2vradmwbc.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2umuthmht.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2eahvseks.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2zvqmpgzh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fuhlvzgr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2ehbvdykl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2sgadmqzf.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dmzazdcc.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2deruoojk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2tyxjlxdo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2vqbyrqzv.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fovzvmei.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2oascqncc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2nhmrtiev.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gzzszvmh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2xttamqer.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qdsepbvi.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ujhzkqsx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2qeipmsem.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2qiverlka.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2xttycpks.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2zpkapdni.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2xujpnlnt.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2mhakuxpr.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2geqhsuxw.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2itkixkwu.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2lpwofyee.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2gdcbezdl.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2sgpfgvaa.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2abhdwldz.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2isaeerqy.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2nktzpbwo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mposxexj.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2hduzpqik.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2sbmwtxxr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2igrofvge.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2hetjknxn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2kuyjwpbb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ycxgaggq.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2jymqyoyv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zozehanq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2wrgqwtmp.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2uxvyqyrk.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2cuzjxavd.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2sgbvqnrb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2wezdadup.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2mnxqjmck.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2jjtjlwmv.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2ypiepjvw.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2vfboakde.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2tipxitnp.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ortcrnpm.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nznkzkcn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2bbtxkvni.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2paseahvu.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2izgxecng.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ustxupez.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2spgnrphx.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2opasvyhl.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2hptwixuh.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2wxikhslq.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2zwosetlo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2ygnxgwyh.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2etfdbqoi.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xgqheqab.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2lwriwzho.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2duzdstjg.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2rkejnpow.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2fzfmahjv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2uhmugzcf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zxbeoszz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2whjakrlg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2fedmbzji.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2xpiojwje.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hkrakink.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2ascyripa.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2xmbrfvpy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vjdsyhel.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2qlslulhx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qgqtkxez.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2dovbwscc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2wwqhyfwi.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2cnwwfdxu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2shgrjkml.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2tksijasn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2qsysryta.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gwjujfma.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2usdabuht.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2weldubqf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2mmdmeyfj.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cfrutorj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zmsyaxjt.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2svxznmiz.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2rtpfltfr.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2qvwfozhc.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2tbwyuequ.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2hvjpuohz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2dawbgctq.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2udsptahr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2qhsisnhh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2eoeltyju.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2qmegypav.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2aujtfhjo.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2xusyrnyz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2dodywwrt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ztfwiaaa.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vaqzwkzx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2jwssfliy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2johxlxau.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2fuiptqvm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2bgxtpnaz.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2dngclcqp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2welhgfvd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2ifyarzdk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mpyiuvgq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bdoyuofp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2degrerbs.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2kcgazgqw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2isjhwdkh.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2tuqyutxu.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2lvrwjojp.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2lewdutzm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qbrotawl.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2dezgedjc.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2rhpqgyid.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2ebcqfpub.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2rpdehgyd.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2ocmjmwqf.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2emijgqko.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2dhesktwn.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2dfdlyufy.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2ffbtyyog.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hzewcrif.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2qrverlxy.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2pxuwrupy.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2jfalcnxj.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2zrirmlvo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hnahbypw.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2cphlokwc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2uoljefxe.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qlcorqrx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gxcgqmtk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qwuzpcup.html


<!-- 参考信息 -->