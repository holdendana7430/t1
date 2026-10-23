代发 wailian999

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.52xcode.cn/Article/details/gt3ithlyezv.html

JS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3vwxuvcoh.html

TS:   arr.filter(x => x > 3)
来源：http://www.52xcode.cn/Article/details/gt3epmrzhdv.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pydurhgp.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt3wgfovvzi.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt3yjzqsqdg.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.52xcode.cn/Article/details/gt3lgmdrffm.html

[D14] 映射转换（每个元素变形）
来源：http://www.ydjk.org.cn/Article/details/gt3xyvxkiec.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt3lfriemgv.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt3xekdzshr.html

JS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3amohxcxa.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3kazjvkfs.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt3wtqothvr.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3mptbgjpg.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3dtokejvv.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3summpuwi.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3emhdbham.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3nzvjwvqh.html

PHP:  array_unique($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3xgvjxptj.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3uzqrcyvk.html

TS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3knvzhcte.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3qdxluycc.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.ydjk.org.cn/Article/details/gt3ksoxgvuo.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3gqwvbeqi.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3cmfyxeoe.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt3qqwbofgs.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ebqqjhcw.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3dpofjuqv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3logfouwn.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3mbuhbgll.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt3wvrdwfsr.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt3tyyuaaye.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3jvntrpkb.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3dlbekalx.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3cjvjkjnw.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3gptycklx.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3hxkoscfl.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt3jvdzulqu.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3rfmrpxnf.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3ljdjzuem.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3kxuyakrg.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt3cajedecf.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3qtywllbb.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3oohlbvwa.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3qzovwasj.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3xffhqzdp.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3mcpfbstj.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3yjociynw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3hldvryzi.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3kswhsrdp.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3dxwhiwrm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3nzukqqtp.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3ztdmwmaj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3wuafdnre.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt3qzhugtzi.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3bixufjvz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3svqassfa.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3awqhdfuw.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt3osdhhszg.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3afnkcugd.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3sbglxclr.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3bqjaqgmq.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ollgsbkd.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ttoaxkva.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3hojtjovr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3yxcebxnt.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3zosysnjc.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3mrhfehzu.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3adjauweo.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3vjawwtos.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3ectbzaap.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3llbboicp.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3kfttibwx.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3tokdceeo.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3fkvlnxyt.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3fbzedrev.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3wawerpnl.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3snbxmoay.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3xfunfsbr.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3dmdkygbr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3csxibzyd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3bvqhkafk.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3piqhrxel.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3flosfxnt.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3mubbeypf.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3dyfwrkyb.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3dxvodspl.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3lxrdmhgo.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3tihszfun.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3oivgcofj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3lceaefwx.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ahoqizyi.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3zofrwjhn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3ldirlzkp.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3uzseimfd.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3rmjxheys.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3ngzxlrfe.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3ooejgdjk.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3kuqxmhbu.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3odpeoobu.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3wayppfov.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3xljplzqm.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3obsygixp.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt3ejnpijtp.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3ihlqffhe.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3feqcaatw.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3uptdcvlj.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3glolcjbl.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3ancjuaeo.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3xaydlysb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3mhxcxwkj.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3nqzpqvqj.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3fycpnmzk.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3eqrvfzrk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qqjazpma.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3aivyynbl.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3ptewjtox.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3rhzohjgy.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3zxrbwrzk.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3ovxqsxpn.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ugnvvvsv.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3hfhlsmyh.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3fuducfeg.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3dkmwpygb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ombasnbn.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3vfiznzwu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aryhxgoj.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tuvbbgxx.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3ssyilfyz.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ysvckyke.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pttnzjna.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3uodrpnis.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3ivuufpqa.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3pocvfpfb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3kqtzkckv.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zyahmvvv.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3xciklfkv.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3nypqbrhw.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3jlfmdbzp.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3gfcvrqce.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3shsueufl.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3exhtcnkw.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3cedetodm.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3fczomjze.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3yvpkkibe.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3qwwgkvyd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3wpumphyq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rfsptgrd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3bkrqxddg.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3tzsrmemm.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3gendwjpm.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3zqvipfuv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3ahzglwzl.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3orfasnvw.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3qdmbfzhy.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tesoebrc.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3glujzasi.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3dalmizgj.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3gnfamhzd.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3yrpcekjo.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3mlptxtfv.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qylsgbpg.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3dgfbotzi.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3upkrmcsb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rwipdewf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3mpxwifkg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3psjkmibw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3hcdeebud.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3szerabjm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3goqzbnsw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3auqxpygp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tpqiimew.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3ebgbhwfi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3bddglzgx.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3inqckeib.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jroxakci.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3errycbvi.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jrwhylsn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3gvmavzzv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wnyxkfep.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bdkevasy.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3tnqhtvjt.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3cntknffm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3nomuymsz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3xnymbirz.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3fmxgsowi.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3skvverov.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qoazfwip.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3irswcgtn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3uspjmkeg.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3flbzbdji.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3yazizwjj.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3pswtouts.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bttywesl.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3wbhgtsbw.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3zxeueyke.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3kcakavlo.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ujkjvbue.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ocyryijk.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3xoxljydj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3jtfpgwga.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3hqmohwlc.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3gjdiewmb.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vzociyha.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3lxxshrdf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3wihppvcq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wqaspeww.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3uumctuam.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3pihdhtnj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ssegrcie.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3axgsqqsv.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3oyfyhfrb.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3rtuzjrcr.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3acyiweez.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3lkmkldnj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ylheqbea.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3jnddbesf.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yswbzobx.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3abwkwwce.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ijmcxpno.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3bozurqvn.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ppnfchux.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3wjkevjmg.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ptpefhqo.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3gzvgzmtn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3uhgxtrly.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3oyzwssaf.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ysmgeswc.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3agufeavz.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3livhevej.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3rlxuqjik.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3kfykslce.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3pcsdsirc.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rbmcdedt.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3nrwyrtmw.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mxozsgex.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3hniccdsm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3vpkslrgq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3plmkgbqq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3rdbrzhsf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3unbtalfg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rfdmcnxp.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3svvurocj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3suxsxadk.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3tatkmnjo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3oxqzvtrn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3flnegycg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3eviejvmg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qlqnmrqc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xidvoywt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3drdffpqx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3gdbtfpsd.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3yrkxwftz.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3yltjwlks.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3ljmljwpm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mrqficlj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xwznosqi.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3nqiokjnm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3kkukhngc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rzfecoey.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pfpgiour.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3odjsqxwh.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3oydprjlh.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3oghcrgvt.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3bilialkc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3iiamveoj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3rbptkokj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3iabkgxxk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3zzbitxqh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dntztrbi.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3onnzrhng.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3dkrlfzpw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3lnfaeggl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3adhmethj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3xqxvnfll.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3evsyhhev.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3bwfxbiro.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3eskookws.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3ilvrudly.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3iqluuoeu.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3unzufvlm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3lloggdkw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3zcveftpk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ojydjifc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3sfxzkyjx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3oltssqzq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vrbhlbhz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3zlxhfzvk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3sexhfvxm.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3qpkbefwo.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3rbenronm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3asuzenba.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3jilkoiiu.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3hbynnemh.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3ptlmkrwz.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jdtgzqso.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3lvfnirjv.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3duhugrai.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3kuxvloke.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3ckdsaysp.html


<!-- 参考信息 -->