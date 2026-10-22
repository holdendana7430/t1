代发 wailian999

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2pckkrhpq.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2xolghesx.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2jcxogswg.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2axqmqzih.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt2nfhgtaun.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2zxbavunb.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2djptqsam.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2clwhqixa.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2hpxzqtrv.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt2rcxzblxh.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt2gibmjzig.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2rxnwotla.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2lnzzejkb.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2jqbmcqte.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt2sfcdptjj.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2ftxyxguz.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2vpnfvhdg.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2fdbxvdio.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2uvuncdmk.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mrxywclx.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2npbyhaxq.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2qklphyvk.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2tyqmchdo.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2xhzhcvcd.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2rkojeulp.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2intiojet.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2zsxmmkdy.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2ystftsfg.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2rmgizyay.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2zdhxhdcp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2oonlnwso.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2ppfkzyik.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2nmmsjvkv.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2sifcbhep.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2yljnshkn.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2michtcqy.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2tuamqbmb.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2cahfayrz.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2ckvnvezf.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2hyzvuusn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2zgbzrgkx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2ptpucsbe.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2ghpxntre.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2xvppdtnf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2ugcjchhm.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2kylhkkwi.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2omrsgqhv.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2uefjqoro.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2owqcrimq.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2qeymvlak.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2nfkxgyoa.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2yvhrcrxw.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2nrnkmfrg.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2kexwgrlw.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2vdhrcrnw.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2emjdjmxc.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2spadpgpl.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2busmlytf.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2xmtnjamc.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2bpxdarwd.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dexrckpu.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2pqfhtbzr.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yoguocnu.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2luqswhnq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2zfkaezwf.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2tvgqjpqy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2lpiqvvbf.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2samgazox.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2pznpvocj.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2kwfkqycv.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2epsshpbk.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2aememvky.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2xnztevpr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2sbievrzg.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2rroleuat.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2bfyovcrt.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2jxsvzkta.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2ighchses.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2xfukgczl.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2eogwtend.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2dtfzvuau.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2cuihofcp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2fdtohtwa.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2xvtzqhlx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bfimofca.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2cmxappkd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2nqzcxpft.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2phwuokbf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2hnddqfix.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2lovlxqbz.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2knjbpmjn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2rnkgaimp.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2thiztjab.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2clucswcx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2vbgtscwm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sgkmwsbl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2kywaxisx.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vykslgtp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2qlohtiur.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2djhnnoay.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2vfimtrod.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2rrpgvctj.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2kztrsncx.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2brckhirx.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2gjeeidjb.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2bzzsxzwa.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2defjhzcv.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2blxywpvu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kylbonpk.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2gcfdvykg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2szphdemd.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2aleukxzd.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2plldwmlh.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2iwiguirn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bacbzgrj.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dqkpcerj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2jfwsnlyi.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2vvwfwfju.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2jrstddjc.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xuhkoehi.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2vrgkbkqy.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2xpwuqaun.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2tgkkvtqd.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kpbgqgpi.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2itqoyggh.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2hibppzre.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2dtnfofwh.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2uazmjayz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2qgduxlzt.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2fcttqjss.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2pqzftexk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2pyiiuytk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hggjhqro.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2iajdeyni.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2yhtjazsj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2gfpuuijw.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2eaqytwlq.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2ksjijhnu.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2mhhuvkgy.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2misqprvl.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2bqqbjcwe.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2eobnrivz.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2gzyjpekz.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2gyhijzfa.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2dzytcxor.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tlgxldzs.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vsrwxiar.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2qqxjbvnx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2xhldtrmd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2bckjkrqa.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2jyldgedj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2swfywqxc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xqwukgpc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2cuinkxhx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pnwrhpzo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2mejloqyh.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2pagivvtv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2bqeoldzz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2fgtyzfrd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cggofwsk.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rchhvoja.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2foimutmx.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ijmoyqji.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rwochbpk.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nkfqsmqg.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2secrdkhi.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2dfryfisf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2sjugdbsm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2nslpecrt.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2pvhgnisb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2ixfolqna.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dltibizt.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2oyuclljy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2wccrymgw.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2dxfpomyr.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2bqyjyzwg.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2lukfohcn.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2holbfzgm.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2irmmpcin.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2flarebhy.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2dlrufzip.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wsbcntpp.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2nizocdrv.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2pccxbgzn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2hddubsxx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tijeobhc.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2eyzhgcyf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ycgxcmps.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2vgillyjd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2orqluykj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2wxzwuoug.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ywjxmbja.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2vekaaytp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rgyqqdus.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2hxuyqqga.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2uytvfgyj.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jphgehva.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2chtlsqrz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2jgrzuark.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2pfmdtrzt.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2bjdsxdqp.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2wmbzbxsy.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2pnwgukgy.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2jgqoiqkb.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2pmxrswtr.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2krappcte.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2ddqyblqq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2iouqtyew.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2lvbwpcyf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2rxjpjbmq.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2zsacalrr.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ubsfncnc.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2rlsceumr.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2cyukovgo.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2cgysguyu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2wwuluvqn.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2yebhedyu.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xwpqymbc.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2brczrxzf.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2fvpjtoev.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2jaaucmss.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2jhjhygyc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2bgdlcmgl.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2rwryzvvw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ubbcpbxl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2fsrppcnv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2mktowsmz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rqngpmut.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2uysuflso.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2kibjijqa.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2ideafsbe.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2pqwzgswd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2whlkevmf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2aendvfke.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2sagtjfjb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2nbccgvbz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2xgptibeo.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2ddxtvahf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jssososw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2olyfuxxr.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2rhcmfimd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2arpitvwi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2xegavmyq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2plbrorgf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2iqzybnao.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2kuzcbbjd.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2lgxgwoyh.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2iohgdkst.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2xslbzasv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2pnghsgvp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2hbhrfeqf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2colmjgkr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2fnetwzew.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2oyaunese.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2covfsasn.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2ibstvxzx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2hocnxjex.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nkzbeval.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2sjgtrfzt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2bwmngnge.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2ujkhecye.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2embskqbp.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2fmaolbko.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2keqgtaso.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2kmbavirr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2frysznup.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2dmgohxdh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2lviuvkgv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xfnjcckj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2iattpymu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2yubivzrz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2kmajqwiq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2vppyemll.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2dyxbbphf.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2puuaosrt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kqdltnds.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2lqnychya.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2clmmyxmc.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2qiovsbyw.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2allgbfby.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2cbfuawtt.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2puraxdvo.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2nqaminvg.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2nlyfgpwp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2mkhnhjzp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2movilcbv.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2ykhobnqs.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2nmmzlell.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2ddskdwer.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2uhatjkhy.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2ufycsiat.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2ronyzyzq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2dcsnrciw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xzlwfxtk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xvtpzffo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yzhslcub.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2krynegzl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2relvmdkt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gpsfhyus.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2oiogxqep.html


<!-- 参考信息 -->