代发 wailian999

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nabnpsrd.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt2ffysikdu.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2portgwjt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt2rotzoyip.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2flmkpuns.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2buomziaz.html

C#:   list.Max();  list.Min()
来源：http://www.52xcode.cn/Article/details/gt2xjfpzrpf.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2pbpdegaf.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2minlcnfy.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2gefetila.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt2wpavagbx.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2bvhobpgg.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2diqyuwlm.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2yccfyrux.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2qvyglucr.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2gyuvvyuc.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2jprdptsi.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt2pkgfurtw.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2dhtfapws.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2scmwuxtr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2ajfalzrk.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2zcskayoo.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2vbbdhfno.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2wtoohfyn.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2gprfhzrd.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2kbisabqx.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2ksvaettb.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2lsbkzzbz.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2ffwqmcqg.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2msovxljy.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2pifcqtrw.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt2daylwgzl.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2yyadjtls.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2zyyrptiy.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2sowtwicl.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2ctwausjq.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2aahlzwee.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2nnbmnnvr.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2bsueluxe.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2icrmvhsz.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2qugdofzn.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2sgfnhqrw.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fwonefpd.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2xsptjkir.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2eqylyukc.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2xnhfrtcv.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2yqdqhwdt.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2dxlicoxn.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hjxjtwwt.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2olcgdtjt.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2rkkbxvrq.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2brgfjlpm.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2iksuoycc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2vdytlaon.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2zbkvoipj.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mjrorphc.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2dabgqnyo.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2zmovcgjt.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2kabdnojj.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2dlwyklns.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2erumufee.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2rgwsbehl.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2fyrzlvcx.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2awqbpwdj.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2cjbvjffr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2sejermfx.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2suavvpoj.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2daurmrzm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2xvhqrdek.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2ixyzbvih.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2egsoyzdm.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2jscjvmwg.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2dgewehcd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jlpcnhct.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2pchokvcq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2edqadgmr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2hoazifkb.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rojlugdu.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2oxesgihy.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2aespobew.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2wcxgenfn.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2nobjpnkp.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2itoegogt.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2tthwfxvq.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2wmfmesgg.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2zzhmxdtc.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2dggecwvv.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2bvlwfdaj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bckrygzy.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2titlqcmd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yaldtrtp.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2rxdnxxtm.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2ojbvtalu.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2mulnmqll.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lzwcfxhs.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2wqovjhlf.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2gttswcpv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2zsjmjwjb.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2rjjjcfge.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lyuysmdb.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tmvgfrsn.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2qpbtivbb.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2zezhhczb.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2eracdoty.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2iszvlmrr.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2dzgskmxy.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2jgxlmlsm.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2gncqlspx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2raywsvjv.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2jnvmnwfg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2vadqyeum.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qlwuwmns.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2cozwwgkk.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vadidnma.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2pbubccod.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2aqqokkwe.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2gkxjxuht.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2uungegch.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2axmrssuz.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xhesmarw.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2eyhntojj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2tmtejosh.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2uohiwzbb.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2pvybhmig.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2bodvniud.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zigabtzg.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fgqnimag.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2gyigrhwk.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2injewpko.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2ncuxoumf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jqbqodpn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2oogvhoua.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2gveogawv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2qfmyzwfx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2wmvuomil.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2rjnitkge.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2tggqlsqc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2eeegoruv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xmhnodse.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2emfoalvs.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gwlmhprt.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qcyhtqxk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vimgwdqo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2opmlpcls.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2oskqwrhs.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2bhktpgan.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2ovezsfru.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mahcywvz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2kpjhbyke.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2xpcvhhbx.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2aalrffzc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oqtfwqdp.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2pdnzsqsw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2fuyuylmt.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2ibyeowsl.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2ivbnnxge.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2nrfeimpg.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ecncydwh.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2thrxahrg.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2wjfuisuu.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2zqexluaf.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2sywcpyoq.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2wvkvryvh.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2kovoecmz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2mvtfvxci.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2dfprhxtl.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xxepvrdv.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2qqglhhbm.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2snyqoqxp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2xpgpwilg.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2cliiwnzk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2vdvuoyyy.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2fqnrdscx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2fxlzkmoj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2nnigxhxh.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2xvoujkga.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vncmjcfa.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vicnntvg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2dngixjfs.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2qobybeot.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2ktlvjvlb.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gfpoionk.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2zcgyrnyi.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qyxupqse.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hfyhveyz.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ydwtgyuu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2puzdozaa.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2bkgjgtvo.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ndeqvpsa.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2hkljeqny.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2qgwnvdcw.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2lguejrww.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2jrihuwfj.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2entyhlun.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2bihgpsdc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2qkstxzvq.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2elpnfkuk.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2lobngonm.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2baafkhlm.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2akpjdcey.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2wunargql.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2qztqttos.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2jnkhlaax.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2pkbimdal.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2pahbvyxx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2ewmsbkdb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2rnvsztqh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2bnhdmzeu.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2ekvfzxbs.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2vcaposqe.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2rcfoelcl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2jmjjbair.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jxgxbhwf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2xhrbgcyi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2dubbmqxf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2tvqobxen.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2vcwgaojo.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2oligimbc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2bqkmnuft.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2tpaqefpc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2zfzbnzbr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2bemushtj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2owfhgdkz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yxamsvwc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ypdtosky.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ecfvoeap.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2thlbyldm.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2gjormhio.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2skjzlxnv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2zjttuvkh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2cwkuvkfo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ehmmogwb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2wqoimltw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2akqcceaa.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2chjveakb.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2twjrfuok.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2vrdtygbo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2rbyzaite.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2rwpsjecq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dxkzvrje.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2mnmecnrn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2krntljbr.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2mbmligmk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2lodmlmfl.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2foaxwwny.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2hnzfwvlc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2zktfzkcr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2vgyyenez.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bjgjmfpm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lpotxkxz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qpdxykty.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2gupgpuvj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2tcvlyooh.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2fgbcgvcm.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2afsuudsd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qjeqtpvu.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2djzjmwmk.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ugcjbygm.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2vbobsgqx.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2kutkfjrk.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2zxjaetxb.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2eamebiaj.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2hmaeotul.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2eldjiuet.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2qyvhtbes.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ehjhsmun.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2vedaztvr.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zmwfadks.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2unfincpi.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2fnnkqdrt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dhlwkkpu.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2dsifsvqe.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2kzvoqxml.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2bjtdkpqb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2metauwwb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2txfmtecn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2fzdqpopc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2ujwlbexx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vpciubpb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ddavplly.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2vfjlrkuc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2auyjbrzx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rzivhmzr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ezjgmdze.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2nvxvefiw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2elyjoouc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2qsefsrsl.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2kezlpljs.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2wukoqpmx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pqonpsoy.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2jtxkupsn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pwcocexn.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2wsyjohhr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2dczqrebr.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ytvzvdzn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2uukxjnnu.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2towfnewm.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xxwwbtyj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2fjbjyjyu.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tnpasyfk.html


<!-- 参考信息 -->