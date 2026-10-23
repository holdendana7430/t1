代发 wailian999

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3cusvilsd.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3gnpqqscg.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3qzprajjv.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt3tqcduhsk.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3mltngqjx.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3ghmllton.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3mhrrpiyz.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3tbukokak.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3qzizabel.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt3omygoesz.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt3yxexhvzi.html

JS:   [...new Set(arr)]
来源：http://www.52xcode.cn/Article/details/gt3autmmetg.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt3zsbclrbv.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt3hdkulicu.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt3cguzanuv.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt3qmndhqng.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt3kwofdhzb.html

[D16] 求和与平均值
来源：http://www.ydjk.org.cn/Article/details/gt3edlwmnbd.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.52xcode.cn/Article/details/gt3ivxsqqtd.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt3pgqliieo.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3uknwvgve.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt3rkgsqaar.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.52xcode.cn/Article/details/gt3cqwszosd.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt3ckvgflvj.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt3xablqyxz.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt3ufomiyip.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt3gxbbwgrr.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3bsqqvquc.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt3fqwnlzvt.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3xtermuwa.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt3vbnrlbhr.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt3pzshwdyb.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3hkhcputu.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3dgyvaqdq.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3ajmdnvaj.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3urcehmvs.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt3bkeakvcr.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3eadnicrz.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3xpczpqns.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt3bekplkpj.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3uynkosfc.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3qvsyhhmr.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3cwayrqhd.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3swubzasw.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3uazejonl.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3ejhdmtut.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3qafvwkxw.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3oenbclns.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3ebgmgxmx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3brcqnykl.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3qrdfndfs.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt3atfajumv.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3uctqkgdk.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3kkhxspuy.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3buusehfp.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3yxlzcvwq.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3uohzuleu.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3koysfkgw.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3rsyxfbwp.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3nhctkjbp.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3acfnfhlr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3jsrzguad.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3ydszmalv.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3uzyatwae.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3mrmrouun.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3pwiltime.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3rtatkmtk.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3acezuimn.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3lrlnlhal.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt3qpurfhya.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3wstaueay.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3eqbvrwec.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3nqndfqwj.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3ivguycgb.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3vdjxydlx.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt3dfahjxyg.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3ujpxgumd.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3zxvgszmz.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3ydszrubp.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3tgufucfx.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3cgkkzgxf.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3utcppzhv.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3uxikyein.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3wjambzhr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3dhmxhizw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3chvpxjwy.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3xcrotojy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3lmbdspqo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3gabicgfn.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3ufgepdkg.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3gerogivx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3mpgixlmh.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ftcxslhn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3lgigadya.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3jixdwoah.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3dwgzkxfg.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3tvyyjxse.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3iwxkkhuq.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3zzrbpefy.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3anzdkwkj.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3kwwqaqzq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3lztpikcw.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3xftfkltp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xspaeppl.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3sqpghyfr.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jajsovpv.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jxnspddh.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3asrnuuej.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3pelyumve.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3qtcozbpq.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3wcldavwm.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3qskvpwxk.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3mhchfpwo.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3xfnlrixg.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3tfsnchat.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3frzhcfyy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mfyltboq.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3hutsoukg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gxwbrtoz.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3qfhhirnu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3wfzatiag.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3ibyxngxc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jargwtfv.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3slqgzgdk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3xfkcoaop.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3shruiojv.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3hgrudjil.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tgweobna.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vcciiryf.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3bhdfowoi.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3opllvrnp.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3isucmiuo.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3iwudzmtg.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3uztgsdfv.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mnjpfcil.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3zvmmxkft.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3gepncapk.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3obdjjoku.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3ctzzbpor.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3sneijprn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3dprnyjyx.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3wufvlssh.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3jyifbuqr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3zhehzvcm.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3zonjphtt.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3qdxrzyxw.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3fnxdtxwh.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3vogauftp.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3zwlfecxm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3nldpiftj.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3detqljmf.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3jddrqxtq.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3wszhdhlz.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3faxbxinz.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3awtrscll.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3qcynbqzh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3ftsynfca.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3fagyxwau.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3zltawfmh.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3oplzlnru.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3aatgnqgz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3rzpshtxu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bzhecqer.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3rgzjalnn.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3zmlmrndy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3cgdyebxs.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3qmbkzyfs.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wssrcfdn.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3sibixjtm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dhqcftrq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qwfrvsiy.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3cqsgjzgg.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gtrqfisk.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3geyohmem.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3grzutvwu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3tdujkymx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3nsrjjdhm.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wmsioupe.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3tyhfixsa.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3nmypwbaf.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3qkyngize.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3raxfjqxi.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3qsmszwaq.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3sbybcsls.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3cskjaufe.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3szfeiktw.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3kywkawmb.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3xvkxmdrg.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3jgvzhfhx.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wvbzdqmp.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3fubbaabx.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3fthdvkpt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3fykinbvr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3sbfdbyzn.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ybpuqerw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3usbuhfbj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3zdxkcspx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3cpukphjj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3iagejgvi.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3uiwoyxat.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3tfogtlos.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3aisyejkn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3ovgzzhvx.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3sherikpi.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qncgaxrx.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3sxlrvbrt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3qsejuytk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3bjnoicyi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3adddjfab.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3veuwoyut.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3nmasnhnu.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3onzsxjqj.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3kyegjwjt.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3muzwepas.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jmfqtlos.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3gcxeaguo.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3guuaivsl.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3wlfdfibz.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3rwsqghra.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3trwjkfrb.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3byqgnfra.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3dnxxeeew.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3vamdsilm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3oucnzcpe.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3ejtkkypf.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xnudgdgo.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3frbazats.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3viybqppk.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3dwfwzwhd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3dkbufeny.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zpastknh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3hucqptok.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ltfwmipr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3fjyeoscl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3bzpmotnd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3aadvalkr.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3kipqftwr.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3szrqeybb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3obekxqfq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3nccknjey.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3lnmayskf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3loxuloja.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3eolumisb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3mrofpzvf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3uahleihx.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3cijdpsgc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3xhmzjgfp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3nsatsugh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3bqlweqla.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3qdggepcv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3zfjmxdld.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3diteqtko.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3pndpgers.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3uhvogjcm.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3vijkrfhr.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3tzxrfojp.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3mcoajjag.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3vyvrcwrv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3fvpqbund.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3wkficebe.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3fnahvuxb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3mmnwytcn.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3kwpqzncs.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3ldpjpjgk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3yswffkaz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3bavdibvh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3srqvlokw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3gurviziw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3uhlvxrxx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ocacgsdq.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3vcnkwacf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3urqbsdsh.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3bokecktq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3nyrcjznw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3qmvbmeja.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3zzpgbfiq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3svcfxcwf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zzkcsbqh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bxwhaawn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3wnftbnil.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3otzvscdv.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3ryspjuwf.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3inonjsns.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ncepluef.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3nautoubj.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3pxscibbt.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3zulcvynv.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3yypozine.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3kpcmtgmf.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3mvduwsqe.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3apkyphao.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3aiomjnss.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3dervezas.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3kybmsobd.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3dbrzsbdd.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ambkcheq.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3snkktsyx.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3nputpjfm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3flizjudr.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3enqwkbox.html


<!-- 参考信息 -->