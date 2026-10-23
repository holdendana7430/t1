代发 wailian999

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.52xcode.cn/Article/details/gt3opldynwh.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.52xcode.cn/Article/details/gt3hnkxkspa.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3qdfswdzw.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt3alqdwygc.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mjuyswms.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3nvdeujei.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3xbwkwelw.html

TS:   arr.map(x => x * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zduhrbov.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tsqsvozy.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3wxrskdeb.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3slpssewo.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt3jrrznycu.html

[D15] 去重
来源：http://www.52xcode.cn/Article/details/gt3reoidsqs.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3rqsqfkry.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3duceklfh.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3dyahrtbe.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3ohpravcy.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3odkmasyn.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3hxrgknro.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt3sfupokeu.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3jvoliqjj.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3ckbqmret.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3blarraoj.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ncdkfwyt.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3txecfbiq.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3btrwzokv.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3mqgmkphg.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3pewurndy.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3dazmwsxr.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3wgylanov.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3chzdkfrn.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3fqgmvajf.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3ztgaxjlw.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3ucraqsfg.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3tilasiav.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3jwxhpzke.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3qwndvfuc.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3hzmrthhi.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt3lkrbbpyz.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt3grysdrnf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3rnxzpnfj.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3fjoybxkh.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3ryjuqwcy.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3gbumlgpc.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mbuoyhlp.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3rgmpyouy.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3aommevvb.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3aepuatmk.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt3nrwfxbli.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jhuktrog.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3zsmqrdte.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3mzkhwncv.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3rnpdnjku.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3pzdxncls.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3vguvhfey.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3kvwqpfcu.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3osqcwsia.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3tsbbrkmx.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3xtelwrff.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3plebbzfc.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3pnzhwrfh.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3utsxsymh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3kvdogccd.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3oawhuicq.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3octqvoof.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3wjddsvei.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3acxrvqij.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3zdfgkije.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3pqqebfqw.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3hepkmavx.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3rflwdrfh.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3najavtii.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3jmptsolk.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3svupmdlz.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ybcbaxps.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt3uzugpqqr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3csrhkeei.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3uiugchvi.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3sizzpedh.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3crniohxc.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3vsubhfjs.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3szpjhupc.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3wbuetana.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3kcewvhmw.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3vdpsvtur.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3fdgliakd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3bbawtbbg.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3hnuitpds.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3frlnnycj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3mhxrkvvi.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3tirneasz.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3cywelgnm.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3irifhhtk.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3wlzhgoeg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3sbmymers.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3kdezcugx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ldyivqlx.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pdcxlltr.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3kwoyogzh.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3wnbgomly.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3reaguzor.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3rqavhcrs.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3ecnyjacf.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3mlphiujx.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3qfhkuysa.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zepxnszd.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3nkkyddwy.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3uimxpisz.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3mpplvovs.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3ahcnqgvn.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vvgoglcr.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xndtpgyu.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3dnbavwxp.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3vsgdgkof.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3apqhtqct.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3udfqsgis.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3efiakqbx.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3oxwrdbnz.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3dlzsrdki.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3szwajprf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zpizvcpp.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3bejgvhha.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jlliomsw.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3tjczcmbg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3zdvdrrun.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3bbnzcdxd.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qoodosqe.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ywaamffu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3ayfpovuf.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3rjyhrswu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3dlzpahmz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xnabusev.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3ddrclxya.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3qynrjezq.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3jzaefwfi.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3afyozzwz.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3rtomciam.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3tpkjmczq.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3pzqowuck.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3pmumvmqm.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3jlrrqpcy.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3aleemnay.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3ivssmopf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3wnnphunu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3qmnrciwb.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3frkpzxjx.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3rwuooddl.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3vwdzsadz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3zkkdsjxq.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3zwbwkaoj.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3rrefzokc.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3mvddozsu.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3xhxamdin.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3kajurqlw.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zgmrwlxv.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wwcqdosu.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3bckjxmyl.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ardohrxx.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3jbhpxrps.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3zqzqnrzr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3bjuuworm.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3egdevmeq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3asooaqen.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3grwmpucc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3hytwcpmi.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3alfwrvtu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3kmtasone.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3tlqgkehk.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3khhtoqkj.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3iuryurze.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3unbswgdo.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cakcxgbt.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qpjcrafq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ikjucpse.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bprlkjrd.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3usmxolxn.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3okhobjgm.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3pxdafczw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3hbmcnexy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3eekxmxyl.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3lnululla.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3nybzaluq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3aoakyakv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wzfswsrv.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3vtwniayq.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3ejyazxco.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3ijlhuoxn.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3pciyhlmx.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3knoeqiqe.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3azunolke.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fhklityq.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3qcwhllbt.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3rifasdpw.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3osvtcrfb.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3nbozahxn.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3ewzrubsj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3ifneehza.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fuwjhrla.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3jmwtryti.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3lfcaeces.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3aawwdxpc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3eimczori.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3mcyevhqb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ylfniwja.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3bombrwjh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fksibjhh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3onlpzrhe.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ftngobud.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3xfvaalbm.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3bfddhckt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3cpsegmdw.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ukrqvzgy.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3aptyekof.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3zzbhemxq.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ytgohvdm.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ymhugxen.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ygpviikn.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vybfhlpf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3nhifwojs.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3hnabcotj.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ephwqtau.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3vnnuseuo.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3nhknecoe.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3dwkaozeh.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3mzsyghlf.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3jtqonkfz.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3znnwxuwk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3usnmvyzu.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3picxcnze.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ebwudkuo.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3nfgplfax.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gpldozzi.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3ykpjjdds.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3riarboig.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3fuupbkmh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3uzlapqof.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3fjgzjxut.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3wtrfstyy.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3zgveqyhd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3hkzkkwtl.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3haucprjn.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3ijgwpsox.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pgbqxdgm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3wrqmvzpn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3dducaoua.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3sngspkgv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3wurdxwla.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3zbjbgawk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3rqvcokgo.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3avckcvse.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3clljoqtg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3sxkmjqwg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sfcbpnll.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3lvqsbdzx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3lppbdgzt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3cmbkpadx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3utcbmmpy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3egsgazab.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3kwadtiea.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3itmjhomg.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3pbchhvsy.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3okxtpvns.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3jjrnzmnu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3smyekcuz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3tgeqemfs.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3cigqqrnm.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3qzzdjsnz.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3svxdjqea.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3cyinjqoc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3zzabuxqa.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3hjexmgpz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3aytsdlkm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jvtpfbql.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3qoewgvhh.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3adiegcyl.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3ifgmvyfu.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3crybplgk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3nvbmrlmw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3ucfavnqy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ubvfontx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jzaqzsex.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ilomzilh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3lyyqlpsl.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3ozmcautu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3qnhyzvmr.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3lttbbriw.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3pcukuxbk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3wudgcoyd.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3iajqlphl.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3toqjsmuu.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3otgsfuuk.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3ogaueupi.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3myzuwruf.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3kjhqnukf.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3oekwijxr.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3yxeliwml.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3eldecwst.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3raeaipas.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3zmaobari.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3gpniprcp.html


<!-- 参考信息 -->