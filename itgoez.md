代发 wailian999

TS:   [...new Set(arr)]
来源：http://www.ydjk.org.cn/Article/details/gt2pakzcgce.html

Java: new ArrayList<>(new LinkedHashSet<>(list))
来源：http://www.ydjk.org.cn/Article/details/gt2vtlcpjiq.html

Go:   // 用 map[T]struct{} 手写
来源：http://www.52xcode.cn/Article/details/gt2wbqtruiz.html

Ruby: arr.uniq
来源：http://www.ydjk.org.cn/Article/details/gt2rtngzsna.html

C#:   list.Distinct().ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2qvexerey.html

[D16] 求和与平均值
来源：http://www.52xcode.cn/Article/details/gt2yihxpsek.html

Py:   sum(arr);  sum(arr) / len(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2stytopis.html

PHP:  array_sum($arr);  array_sum($arr) / count($arr);
来源：http://www.52xcode.cn/Article/details/gt2dijewyxv.html

JS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2ggmmhius.html

TS:   arr.reduce((a, b) => a + b, 0)
来源：http://www.52xcode.cn/Article/details/gt2otsqcgbb.html

Java: list.stream().mapToInt(Integer::intValue).sum()
来源：http://www.ydjk.org.cn/Article/details/gt2yylohzig.html

Go:   // 手写循环累加
来源：http://www.52xcode.cn/Article/details/gt2dkhdwble.html

Ruby: arr.sum;  arr.sum.to_f / arr.size
来源：http://www.52xcode.cn/Article/details/gt2emeivezh.html

C#:   list.Sum();  list.Average()
来源：http://www.ydjk.org.cn/Article/details/gt2jzomrmcd.html

[D17] 最大值与最小值
来源：http://www.ydjk.org.cn/Article/details/gt2jchhxvck.html

Py:   max(arr);  min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2djdlkfrz.html

PHP:  max($arr);  min($arr);
来源：http://www.52xcode.cn/Article/details/gt2slokwksp.html

JS:   Math.max(...arr);  Math.min(...arr)
来源：http://www.ydjk.org.cn/Article/details/gt2zgbkogsa.html

TS:   Math.max(...arr);
来源：http://www.ydjk.org.cn/Article/details/gt2btsxtyha.html

Java: Collections.max(list);  Collections.min(list);
来源：http://www.52xcode.cn/Article/details/gt2rsitlwos.html

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2dfhbakmj.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2wmrashgq.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2uoxogiet.html

[D18] 扁平化嵌套数组
来源：http://www.ydjk.org.cn/Article/details/gt2xmysgjen.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.52xcode.cn/Article/details/gt2vupaevxs.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2viknhbgr.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2sjhwlvvj.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2beqylfhe.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.52xcode.cn/Article/details/gt2nlmlslob.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2hnesrbic.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2qmwmfjlc.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.52xcode.cn/Article/details/gt2fudrqljf.html

[D19] 按字段分组
来源：http://www.ydjk.org.cn/Article/details/gt2ybaamzwx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2fyfuowhd.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2lrwrjvqm.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2djozxfhr.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.ydjk.org.cn/Article/details/gt2ziubppky.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2swmcqbej.html

Go:   // 手写 map[string][]T
来源：http://www.52xcode.cn/Article/details/gt2dozafrdw.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.ydjk.org.cn/Article/details/gt2bvtnkcsg.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2qxoopeyl.html

[D20] 统计每个元素出现次数
来源：http://www.52xcode.cn/Article/details/gt2blztziud.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2sbodyxcz.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2smuipmzf.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2fooywzbl.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2cqaenumb.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2aeztwfdd.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2vbykckru.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt2porodexr.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2auyupqdx.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2rrvorwqv.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2djuhswnu.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2pmmqbxra.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2jaabprey.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2yjhrjksq.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2aqulwcoh.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2ogxgwwxr.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2fwizlxix.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2twxxnbuy.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2cvzkngbs.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2pqdmzefy.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2vwnxyrgo.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aeevfeyt.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2tcxspgfr.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2hpiqzckf.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2ayzqctjr.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2jvzvuytd.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2birudpfz.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt2iudcqpvk.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2toqkasnj.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2brdcpxse.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2xahnwoiv.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2ozmvikkw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2cfgjutrd.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt2dvbmkvme.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2nwhjwquo.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2yhgvandx.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2oywbtebc.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2ebbtakns.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt2ggboxxlg.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2cbnenaxm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wfydsrjo.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2aisbtelf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2qofijntf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2djnvvxfm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2uggwjvpq.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2rrlomatl.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2cvmxfqdh.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2dmgiomcj.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bixokuzj.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2nxxpaucz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2emsitngu.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2ffwockve.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2trrdgryh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2qwgbtfqi.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2ljtgqnjp.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt2lddcozyn.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2idyofper.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2qofmzcsx.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2nmvynrue.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2hmeouzgd.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2epcpanib.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2wjcweceu.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2tjtmjbxb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nzxjkate.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2aprhqkfq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2klvstnxa.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vsyhrugg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2yiynugpq.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2gddskmzf.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2mreimtxy.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bflfalzx.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2wccxyvzw.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2kbfbayua.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2tbuarrve.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cnvoxfqw.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2hwwrpcca.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2vmkjuixm.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2nevdwfcc.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kdblanvn.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2mmzzvlde.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ewvkzsug.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lrrdhgyy.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2crpibmbq.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2cjxfbhde.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2buqewavs.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2vhditruj.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2kfmjnumt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ujlkkvki.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ymkzomyj.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2trndkila.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2nvasxnmj.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2xvhfcubw.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2xcoztvmw.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2dsvfmden.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ogplupjz.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2fmlabjgw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2yrztnmtm.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2eqcghjxw.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bmlkaxfq.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2xgtpqmks.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jsdmklaf.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2aupzurgt.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2hjupjmic.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2xegletia.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2upjrdkzu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2exiubujx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2jceubsvv.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2yveqdiwt.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2reaoguyi.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2nqqwhhjw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2orypvrrw.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2spogbzht.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2cuaafpxy.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2eclarckl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jruryyvr.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cjijzurd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cgyqopdv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tpwcyzzp.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nysomdxq.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wblswwmr.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2brrnajrv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2xutxwfuq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2dtkguqel.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2sjjdcfnp.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gjipujeu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2utjqtqsd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fwlnveik.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2txvjgbij.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2nfagybww.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2rvftysjr.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2rvjywjro.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2vnsvotwy.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ebfiblsv.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2rxawpcfk.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2gwahpitv.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2kvaihwfg.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2dqbzwfsx.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2vpplmddk.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2hmgqcmik.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2rhqxyoeu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2brmeuzyx.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2kjhxddzd.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2lbzxazeu.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2mcidhrer.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2xbavcxcz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2sadkecah.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2fmojslew.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2bmknkycj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jjqdkluu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2ydjnsgbs.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2emklrfzx.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jquwmydl.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2dpsgzcfx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ncoflijv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2qdazvymx.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2rzoypelr.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2nmjymczd.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2kequkfpx.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2dulawdcc.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cdpufvsl.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ppsvcqez.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nicshqty.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2zucszzzr.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2frefujfu.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2wzvhmdvz.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2gtrquzta.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2kkfohmgq.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2tvxfibmv.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2yxnozeih.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2slruzikx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2qxpuccbt.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2fceotyjt.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2eaabedqx.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2pvnakguc.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ouyppdcv.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2ghrbdqca.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2swvfycrx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2pdtjtznd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ndtnvkmw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2absacgjn.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xolsjtsi.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2bjocdxdq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rnuuptfm.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2gdrojncg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2xgyipyln.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2iodxwfki.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2fmcrrvcd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mnoqpmjx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2emxccpqt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2rjwxejjo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2xaubjltg.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2txqwlwif.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2pmkarwho.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fqtnotlz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bqyhmpvz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2tnihqxnw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2daqodcuc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2nupofmtg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2wamokell.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2gfisjvno.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ljkppvas.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2kkdkqcsf.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2rvmwqqbe.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2levbdozf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2carlipuw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2hbjmszec.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2vmhxupad.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2rlvthhzl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2crvcnnnl.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2pjihpiln.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2unqnuwqb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2jbomynce.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uhpguojc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2fdjktqyw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jzghviep.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2spcygnnl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2omkvuyva.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2rrfcddsj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2lhvurnta.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2uotneecc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2skgvcwag.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2qbdsvuix.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2hpzspgxh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2nlkisbew.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jtuntate.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2yxcncsqn.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2wnyaiopo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2rqubolrs.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2foeqhyth.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2cfdukvxq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xfbwzqvs.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2iltcgtbl.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2hrcdmnhr.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2rhekmzls.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2qcjewxza.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2crvlubwz.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2ueobluvn.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2zpbhbccw.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2tuhmctac.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2rpzobqkd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2sztehjdp.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2ipkvvujn.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2jfjtnpwp.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2zuipngjd.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2cndppbmt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vzwzbiwl.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2hrbtieyb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2nfubyfeh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2asqqgatx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mvjexddw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2yjblqhbb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hzmkduje.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2uyyhjeup.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2clpkqpqi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hstrkqql.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2mmtunwsy.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vmcjjmjk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2gslnkjom.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2anyoxgik.html


<!-- 参考信息 -->