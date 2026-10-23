代发 wailian999

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3bpqiwuhh.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3dhmpnyta.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt3cuxnctbp.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3hofrvclu.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt3yuzqwqyc.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt3ryxtydno.html

Ruby: nested.flatten
来源：http://www.52xcode.cn/Article/details/gt3ufxpymqm.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3kijmtfuh.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3lmbvdvoq.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jsbtfbfl.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3qouigzql.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt3vmaybibz.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt3prousdxx.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt3dceiwubo.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3geqzdsdd.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3otnhgxcs.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3kndhdtnr.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3widqtnrp.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3ixprahim.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3szcvxbnx.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3fmtdthwd.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3gnjcprgo.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3ofkbgttk.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt3ujctoxvj.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3ekjykkta.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3pggrefjg.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3qiwzgpxn.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3flpwzgod.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3hmiletic.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jmohekov.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3uafdjnwn.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3uespkxvx.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3odkibrto.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3tdbgpxnt.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3gmxhwvii.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3fnzejfyw.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3olzurwap.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3zmvpmwrw.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3rycuhqfo.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3qjeltgod.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3kxucvqpu.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3hsulkiip.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3icgqxqrt.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3nuvdpcuw.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3lhimfwxl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3euoubsli.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3uuioqcrp.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3glrbeoqi.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3rbvwkltu.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt3lmqrrbve.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3balkwiwt.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3omtyymjy.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3bkwkkurt.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3cjewkfea.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3jibakhyc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3habwcisg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3vvbdehif.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lajmtmqi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3bijayjiu.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3bapknksa.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3fwkdmkgd.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3gkbepokf.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3wunnrjxi.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3heegjodm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3vpfumklv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3hxgankhl.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt3fftiysgd.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3cblffflr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3qjujxcra.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qcbosmsk.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3xujujslw.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yicvvuxz.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3nskaoial.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt3jbxcslja.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3ywjrlllw.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3auqavyzx.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3anotcjbe.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3vyzvwlno.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3shrnoato.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3izdwpssy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nsjyanrh.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3tthuolkl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ecidofer.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3fsnymbcq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3fttmvghg.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3bhpedupw.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3piipokkr.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3wxscsqgz.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3yamspbgb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3cjaycpdd.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3jfwuizdd.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ukngqkwe.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3recnjdov.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3qzrlouio.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3weczlkbn.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ntwabnaz.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3uihzxpyr.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3nlidemja.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ovihvozj.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3isgllpnh.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3xwxactux.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3mwdixkww.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3mqkmskyu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3frunmixd.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3smuqjmre.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3bszhsjsv.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fceaidqw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3aelimftt.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3efdkkrxv.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3bpuyejma.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3shhnsgak.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3xybhmqsh.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3lhsifwjr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3wnblfnvk.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3wscqhmqk.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rvtopuwa.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3iwdggywr.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zhnvcpxd.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3uwalzwrm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3uwxunhhs.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3ffvaymkx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3yeswwsxo.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ztpwatha.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3qdzqyzgu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yodsiepw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3mmcgngqz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3ekvdfbhf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3fcoxbpvy.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3pndvptnr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lcbuxyyl.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uesthvmk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bozjhkzr.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qlifvspf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kdkuzgpd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3gkdjciqn.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kwokfrcd.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3myvkanyb.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3hbeccjmk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3zopjgbgh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3yjzvnark.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3cmbjmavp.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3iozemnlt.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3cmcthleg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3macaulpt.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3iyifjpgo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3orucitbq.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3ppvmnopp.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3byqubasg.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3ltiiucww.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3olctpeso.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3oueskqlo.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3npndquvk.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3lonvrmdz.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3irrlwerb.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3nfjccwvb.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3ddksbgcg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3dkliljai.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3aoqyvigz.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3tfdkcmwt.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3feoryatv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3acdynfrx.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3bzfngcoz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rpzzvbrx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3xxqcyrjc.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3ivloyjdm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3whrjooqg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3iexlteyz.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ffqtdpmw.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ulhmlnvz.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3lxyctdlh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3qgprdspc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3msxvxkes.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3tufttchg.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tolrwqlf.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3foljwtds.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3zyrhilol.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3plnjvduw.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uaosbzzi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3oheedpay.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3qvvjtzho.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3irkdkvpp.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3bqasnlvb.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3rgsaiqly.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3mkssksfd.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3dqmssowv.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3gsfnshah.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3gjnkbszx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3whjaezsc.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3oonakekr.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3nasxvwiz.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3vsbgsdhq.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3eyvhbkdl.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3nuynyuiq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3hujagvfq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3clausqdg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3tixmddkj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3uhaktwee.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3muocelbd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3nsujtjgz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3srioeuzx.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3eukosvvp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3anxviznm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3jplbucqp.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3nzieofjk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jnpjqgid.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3agojuupp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3jiweesmn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3jgmbiqcx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3sntqsujg.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3lwlsztmw.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3qegtknpv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mzmaaldh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hpvwabhw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3svwcghyw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3fyghwvso.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3feenwrgl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mblqoaaw.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3dtxwpzrr.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3hodztnmk.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3aqhsolis.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3cifcrfmk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3zyxwnzvc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3dznhxvak.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3fqjqokhr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3dzzyipjn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3humhflpn.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3obrjdlsr.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3kaqnutlh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3ssdculie.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3kawswlbs.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wbkmmwes.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3kihejzce.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3skzvwskw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3ucsjadkl.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3pchnrbgk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3ijjluocl.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3ptfqehvy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3vbbagxbw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3rhczkzrt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qwhwraba.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jrpwtjzo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ikrpzyrm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mlibkqbt.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3sndwrbxo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3dxfxnons.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3qenanndx.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3faoebylw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3eizbbtmb.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ygckfyxl.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3mdgobkgp.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3dnrpgkhk.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ukhbbbrz.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3iwxzomho.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3aincgrkg.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3ztvcxxty.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3oufsbbyl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3detwebki.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3iypiwucw.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3jhdmasdb.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vayyqqqb.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3ruwnbuor.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3cpbfijnd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3wsftibgz.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3lenfzdvv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3jzmvplit.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3pahtrwkd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3istggwpq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3vwnajodw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xjqermvp.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3qutfremf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ryvmglkb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xaukkcwd.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3sjsdgmhb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fjbihaaa.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3gjsthjiq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3tzlvxkcn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3vtepzqgk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3grkxfxfw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3prlkysjz.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3urkhkeng.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3qpnomeca.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3spqxrenu.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3sctpuogi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qubuwnbl.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3dxupwyka.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3vbzsgxjg.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pyqguatb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3hxyudnpq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3qnmhiwqp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3cqzioifo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3dbvqwtja.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jpzfgwik.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rlnnlomn.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3xokecwos.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3yvupmyhd.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3pflsnyrm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3uzztreml.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lbccgrxn.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3tcobgqoq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3wdjziqtp.html


<!-- 参考信息 -->