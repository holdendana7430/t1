代发 wailian999

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.ydjk.org.cn/Article/details/gt3ssvjdsqz.html

C#:   list.Sum();  list.Average()
来源：http://www.52xcode.cn/Article/details/gt3yftucsrs.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt3hgfvewib.html

Py:   max(arr);  min(arr)
来源：http://www.52xcode.cn/Article/details/gt3lobbkcoj.html

PHP:  max($arr);  min($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ubxljpgb.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.52xcode.cn/Article/details/gt3hphuvdwv.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt3bwpnscbt.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.ydjk.org.cn/Article/details/gt3olnwalsv.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.52xcode.cn/Article/details/gt3amuzjniz.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt3qdrxwaop.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt3jvbneztx.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt3sqcpiacd.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt3yntgnupm.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt3avujyllk.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.ydjk.org.cn/Article/details/gt3zkufbpit.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt3bikclidw.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt3djzeluta.html

Go:   // 手写双层循环
来源：http://www.ydjk.org.cn/Article/details/gt3bmrnifiq.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt3kiyixiih.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt3fmpplejo.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt3wktjrnib.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.52xcode.cn/Article/details/gt3vazcgubs.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.52xcode.cn/Article/details/gt3vxyatqjd.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.ydjk.org.cn/Article/details/gt3nosaxidn.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3xbstmilq.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3xjbdmfml.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3xgeftefo.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3nsrhbezs.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt3ngpctzeb.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt3zbhohocu.html

Py:   Counter(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3kndpdflu.html

PHP:  array_count_values($arr);
来源：http://www.ydjk.org.cn/Article/details/gt3qfadtqci.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3yrwjiool.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt3zgrfwsow.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3pnsblesg.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3ffmggmxl.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3ozbhdnms.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3bpkptlwo.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3ncqwumij.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt3fcyarzka.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3hohydjgf.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3qfpdejzl.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3wavrdbuz.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3kuxxdizp.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt3dncdnora.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3zqfmzbwa.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3gtqqbsgw.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3fqlwsehr.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3jvzrhnhh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt3oluybkpy.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3chemwccz.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3hvlvgxfz.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3levqnfhn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3idtgasal.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3fhodwgya.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt3mqdklsfv.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3lcjxksxc.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ohlmttnn.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3wvuitgyr.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3rqgjsuiw.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3xhibuuyd.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3juxkaale.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3tekggxvv.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3kafhxyyi.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3lkguamlt.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3mmahvzwf.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3zdatgbpc.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3wgsdfcdc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ydmitgyr.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ypvvqhni.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3oemrtwtd.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3lojyqqvm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3xkfrykrh.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt3knqrhfft.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3lpupadya.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3rnujnxpc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3fgbmpouv.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3qkqvxqlb.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3ssguyziu.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3enaoszxe.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3puluamuz.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3twfhgpup.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fhfjirfm.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3hmbrorme.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3sfnlezqq.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3cxbivyim.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3acpfzoxi.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3kbuzcbxc.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3fpsaqniw.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3wpwihlzx.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3uzdzzjmw.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3tujfcrcn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wcznjzyb.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3xyenwuyt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gjndyjik.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ahjsjebt.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3jkygjnsk.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3ssofryal.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pmsyqxts.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bymfrjug.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3ktvkqaca.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3odbrfjkc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3vapkqqgz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rmkrmnzb.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3cozgqzse.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3skcstewq.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3titfczce.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xxkivull.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3laccajli.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3jwtldnab.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3mdscynti.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3plxryowo.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3qqfutjvi.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3whmtynhy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3gshoijhm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3spqmecge.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3kpgyeksi.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3otyntfst.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3fvoajxtt.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3rtmgobjb.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3vfhdlabt.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xbtijtqt.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3cucnuryy.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3itkppwbi.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3xndvzedi.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3xfqzzwel.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3evzfxniz.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3puwazxjl.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3laeylasf.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3lovhgxqh.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3kmalztuy.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3tkcpngtj.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3phxwkwdv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3rucngtij.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3alfxhuzo.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3andxrych.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3zlawrrhz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3xnqzwunf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dahayvbo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3rmwuimuy.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3fbmrvtni.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3qpwhpvzw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3sjsyudac.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3stwxvcrp.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ivvhrvac.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jiysdrvs.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3vgpekvgn.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3aqkzijqb.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qvfxuzmv.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3caxzvjxl.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3badcfhfc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3oiteehmb.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3aeyfmpeg.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xcwpnfrf.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3qyslzubv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3hafvafqt.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3tpetqixu.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3tjoorefh.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3gdouyild.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3tqxykzme.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3unytdbcy.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3vglogcyx.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3dvultohu.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3cqyaaxpp.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3hnmwhofh.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3wwvqspim.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3urpzitsu.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3yvyqyked.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3zntenoks.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3cobfczjh.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jzikjbip.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3cuwcpqrh.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ikjqswlh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3wcwdgglm.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3lafndilv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3eqsxhssc.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3hxxxwdhn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3lgfyvsnm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3aisnxwia.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3csksaiyj.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3lmjjrivv.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3sjsylwmb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3gdyauoqn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3gggnxape.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3dqqtoduj.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3badopngn.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3oyhgxkrn.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pixwzwyw.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3bwmkcurl.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tbprdoku.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3zfyubegf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3gfpvgdio.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3csywoenh.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3cvwmfqgc.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3meqguhjp.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ogwkbdrg.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3mwplxqut.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3glcziyyx.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3zaffemwz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3daqtenqa.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3zytflqwk.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3bpncuzur.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3heowdvho.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3hgiwetbi.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3jrxfhphu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3nrebcyib.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ffrbypvi.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3eexinfvp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vonxskkr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ixxzuzwg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3xqbodoyy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3chhlmfnc.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3tjingyzk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3abjlhfck.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lgzvwxpa.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3fdjrwwoj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3bscwyxiw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3sjnkamxg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3ojfehfqf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3dqraybpy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3olqybhci.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ambcfbfu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3sbkwlgvj.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3zlgpcrpi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hronakix.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3jbqpgwwp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3uqbtuyvb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mnokioxr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3jqcfecrh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3lnxvsirz.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3mysahsni.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3hteglvhx.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3qjwcplhm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3wdfoybdc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3vqyqedrz.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3erwinsiw.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3ixfbxseu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3yodzuwvc.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3mfbgdoop.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3iepmqufp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3syjhhtlq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3umqpzopq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3cmxpnjrd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3pzpqqnrb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pdklcmjd.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3vffgpbct.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3shkojndw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3jqlldliu.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3gxjzints.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3fsrygtph.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ysghgfyk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3avfrcenf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qqiqlnqx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3fhgiwnhs.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3xfnysmeb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3pntqexyx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3cnehvbbf.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3bokglwvv.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3qftbxnfr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3tfzxmsst.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3lbgxkhsm.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3moesbqji.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3xbwukivm.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3uxbnohdz.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3zaexwvmt.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3djxygaow.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3tmmgzsfu.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3hylhyzpn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3wkhlltvf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3omeekszz.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3smgzqxfv.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zqstoxti.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3zgngwopw.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3ytsjnole.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3frxtzipc.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3xhjxtefl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3wezkzfwe.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qasegxum.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3osxhljnw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3gtqztdwr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rabxrplu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3glabkxqg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xyyzzazg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3awjwycmv.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3dvkncttb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ikvsibgm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ijougqnu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3igwltjli.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3upzhfvne.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3arxnbvfn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3zssunqce.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3igtnvfnu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3gvixnhoy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fkedvlxq.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3wtwxjhpf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xovxfvau.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3bzrmimww.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3gfhwveqt.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qyocxlcn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3rzeuybaf.html


<!-- 参考信息 -->