代发 wailian999

TS:   [...arr].reverse();
来源：http://www.52xcode.cn/Article/details/gt2vrijovlz.html

Java: Collections.reverse(list);
来源：http://www.ydjk.org.cn/Article/details/gt2kwcffxxi.html

Go:   slices.Reverse(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tgwxtxwz.html

Ruby: arr.reverse
来源：http://www.52xcode.cn/Article/details/gt2whsixpmy.html

C#:   list.Reverse();
来源：http://www.ydjk.org.cn/Article/details/gt2hjzynrnl.html

[D12] 查找元素下标
来源：http://www.52xcode.cn/Article/details/gt2vmdvixma.html

Py:   arr.index(x);  x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2wogjwjdl.html

PHP:  array_search($x, $arr);  in_array($x, $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2bsgdxddw.html

JS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2fsjynuhq.html

TS:   arr.indexOf(x);  arr.findIndex(v => v > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ccbqkwbz.html

Java: list.indexOf(x);  IntStream.range(0, list.size()).filter(i -> list.get(i) > 3).findFirst()
来源：http://www.ydjk.org.cn/Article/details/gt2pvakxrnl.html

Go:   slices.Index(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ypprcwcj.html

Ruby: arr.index(x)
来源：http://www.52xcode.cn/Article/details/gt2iepqngok.html

C#:   list.IndexOf(x);
来源：http://www.52xcode.cn/Article/details/gt2igktgvxt.html

[D13] 过滤（保留满足条件的）
来源：http://www.52xcode.cn/Article/details/gt2rlnfffmf.html

Py:   [x for x in arr if x > 3];  list(filter(lambda x: x > 3, arr))
来源：http://www.52xcode.cn/Article/details/gt2tzvpocan.html

PHP:  array_filter($arr, fn($x) => $x > 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ijsndrvz.html

JS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gcugalvo.html

TS:   arr.filter(x => x > 3)
来源：http://www.ydjk.org.cn/Article/details/gt2duknohoy.html

Java: list.stream().filter(x -> x > 3).toList()
来源：http://www.52xcode.cn/Article/details/gt2imwjvsnk.html

Go:   // 手写循环，把满足条件的 append 到新切片
来源：http://www.ydjk.org.cn/Article/details/gt2waevugaa.html

Ruby: arr.select { |x| x > 3 }
来源：http://www.ydjk.org.cn/Article/details/gt2ybvsjntx.html

C#:   list.Where(x => x > 3).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2lqdvvdir.html

[D14] 映射转换（每个元素变形）
来源：http://www.52xcode.cn/Article/details/gt2nexvyuwj.html

Py:   [x * 2 for x in arr];  list(map(lambda x: x * 2, arr))
来源：http://www.52xcode.cn/Article/details/gt2pwgjztjk.html

PHP:  array_map(fn($x) => $x * 2, $arr);
来源：http://www.52xcode.cn/Article/details/gt2cyuiwpys.html

JS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2bezkclsv.html

TS:   arr.map(x => x * 2)
来源：http://www.52xcode.cn/Article/details/gt2vtowfsvg.html

Java: list.stream().map(x -> x * 2).toList()
来源：http://www.52xcode.cn/Article/details/gt2kheauddk.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2rnjokhrz.html

Ruby: arr.map { |x| x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2zzekwsxj.html

C#:   list.Select(x => x * 2).ToList()
来源：http://www.52xcode.cn/Article/details/gt2rijvezws.html

[D15] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ipjyfhpb.html

Py:   list(set(arr))        # 不保序；保序用 list(dict.fromkeys(arr))
来源：http://www.ydjk.org.cn/Article/details/gt2nkrozcoo.html

PHP:  array_unique($arr);
来源：http://www.52xcode.cn/Article/details/gt2ofrxcyew.html

JS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2ppblnjgg.html

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2qcyrtipx.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.52xcode.cn/Article/details/gt2enkqwvds.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2wwvikjze.html

Ruby: arr.uniq
来源：http://www.52xcode.cn/Article/details/gt2atumfghn.html

C#:   list.Distinct().ToList()
来源：http://www.52xcode.cn/Article/details/gt2wkuulzlu.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2qnbvfklt.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2gjiwksbi.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2xdaebivc.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wmpqprvo.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zszpciul.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2afcvpcqh.html

Go:   // 手写循环累加
来源：http://www.ydjk.org.cn/Article/details/gt2kdcgrmma.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt2kqvganky.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt2yvyyvthv.html

[D17] 最大值与最小值
来源：http://www.52xcode.cn/Article/details/gt2mczqhhak.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2vxbfisgd.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2fpywrfhs.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2uzdlijfw.html

TS:   Math.max(...arr);
来源：http://www.52xcode.cn/Article/details/gt2ehtnfyye.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2bdqhnmtr.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2bzxjpdcs.html

Ruby: arr.max;  arr.min
来源：http://www.52xcode.cn/Article/details/gt2ewakmufe.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2lohxcxoi.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2zlctprwh.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2hnpkdwxm.html

PHP:  array_merge(...$nested);
来源：http://www.ydjk.org.cn/Article/details/gt2rmqclqct.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2mfcxybge.html

TS:   nested.flat();
来源：http://www.52xcode.cn/Article/details/gt2uwifzwsb.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2uyyvbtyg.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt2ugcufamo.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt2smocessw.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2aemegnzr.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2wouidzmj.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2lioimfdp.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt2nuumjebg.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt2ufusrxeg.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2isnwhjwq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2axofxjwy.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2vfjptqmp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2rhvmdsql.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2vgrngdvg.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2wgaaetxc.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2honjldjf.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt2nclkhsgp.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2lukewobc.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2vnlrpxnp.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2kvlvqsls.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2yenvwifj.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2ssxbeeip.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2yypinbrl.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2esztpnam.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2jjhcekkc.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2bfedpfvt.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2pyvisxlr.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2mgipthft.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2hofhhufq.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2afwidksu.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2qcqzryoz.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ljgujybt.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2shscjgzx.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2nimrescn.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2ziomshqm.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zljifsfb.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2mlczrqqo.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2pvkmoedi.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2cwpuhhpd.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2ettbkkll.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2likdvltj.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2vsrqagij.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2zbzznghd.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ychbcapq.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2msmmsjuy.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2mkeclvyk.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2joqbqqxj.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2loomlwop.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2lckpsjmr.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2tagormmw.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2rcqosggo.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2nllpzirj.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2vbidcqfc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jujaljfn.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yyrijgaa.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2lklzwwql.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2ciasdtlz.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2sxnfacul.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2xjkjxhem.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2qpeqznir.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2pupawxug.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2wlutpdni.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2yyazkras.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2nxbnxyfq.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2uldmbudc.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2rizlyjuw.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2gvkjddjh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lofjfvnu.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2raibsgyr.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2kscjzrua.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2owkglybz.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2mhuyfmmw.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2plfbjkxm.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2dwxngdeo.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2adyjzcio.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2swqmncfx.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2nffxtibm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iskggldc.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2tfoaskvr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wwjwhfmw.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2kxhhcowg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2iehjecwa.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ojknlweq.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lfnxpddi.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2mzkwtagn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2mcuftucj.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2svgjnphe.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2qxomrjtz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ljsnyrur.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2iewjckgl.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2zgwdstvi.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2bvwagikv.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2wqjjpbko.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2asdfasnv.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2cqylqgzu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2szjlxntk.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2lrbboqii.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2gylfxmxq.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2fhecubbd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2yzijvlrl.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2wmrghsoy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2stiaxqnq.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2kfbexjdm.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2pdqejlbf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2rhhhhmiq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ipbprntu.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2vlavgkep.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2rigmkzqq.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2qwvqajap.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2ftvhpnbn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2etwyarym.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2sjxofaas.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2dekougxd.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2efuixijq.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ospiijke.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xyezjtck.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2ysoxxpsx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2imzbbtxv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2tojosaea.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zsxwdygr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zyulrvul.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2twosjlon.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2obipjedv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2xgtkjxkf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2veqjyadp.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2lmhrgyyt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2noigtkpa.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2whcqtokr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2urlqahaq.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2srlfdvyo.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ncaqlcfk.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2vebmgycr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2omkjcwpj.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2drefagjy.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2xdzxhyej.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2qxzlbehl.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2hzwbdxcv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2mdgyfaoa.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2haefrpce.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2qpesxpug.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2alzkqcma.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2ljjrpjog.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2srnfdrwa.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2iesndrls.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2gbciqnhg.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2dznbvqov.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2krqhvirv.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2qsrgltpw.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2nvnbtowo.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2fnucdjnu.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2izhkguug.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2jikvgmeb.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2sxdkqdei.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2mhqngsje.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2etkxtgkw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hlfpxqhn.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2mctrprsc.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ijmwydrt.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2fjdbnggy.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2trzjnknn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2wnqsijzo.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2uzjodmrj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2gnoiszhx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2mcrifezz.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2svxgvrtx.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xzvhkqjx.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ntuobqzh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2gngnfafp.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2vmdterta.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2jhznbdbz.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2rffmaptf.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ivosgyqg.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2nvdrjgah.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2laoyrobb.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ofkuqxrf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2glioovnp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2gbqpsidc.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2sugedhhg.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2npzhkjws.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2cswwhlbp.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2omwxgghg.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2vcvukhcl.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2semrwkie.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2vpqxfpfo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2apcewmkv.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2rfsspynx.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2lgwvyorh.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2lqswoikj.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2aedjhwba.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2bxucprdy.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2dxykkapk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2udgjztsc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ufpvloss.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jpyytffu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2oszqdhdd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2umyrehiu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qvcupgoj.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2zkbkoxqi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2kflhlkva.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jbwjwlux.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2xqjgdivl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2wefkttro.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2fmyroxly.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2vrqdxmeg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2fxtditss.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2fwfrnsvi.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2xrguypnn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2wxvyrxek.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nytwvikn.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2rwwwomro.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2hmsghbuj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2isawksgy.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2qsettrbe.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2ztboxqlt.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2epgiermm.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ltlxbgft.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2ztrsuqut.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2rvtamdoh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2nrbdbfyh.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2kijhtqmi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2yykddvgm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2umxvdnsb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2cpjrfreq.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2gjtatogl.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2yxehlofm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2ahidtezc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2gnastqzj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2alyfaowq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2plisfogt.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jwxdjmpf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2htfzaxuq.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ylchgidm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2khbwsaow.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2fkjdbvkp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2sygdjsgq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2cvebghrh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2eyncbmng.html


<!-- 参考信息 -->