代发 wailian999

Go:   slices.Max(arr);  slices.Min(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2mxjvjjvn.html

Ruby: arr.max;  arr.min
来源：http://www.ydjk.org.cn/Article/details/gt2ehuawxcd.html

C#:   list.Max();  list.Min()
来源：http://www.ydjk.org.cn/Article/details/gt2dzwaenrv.html

[D18] 扁平化嵌套数组
来源：http://www.52xcode.cn/Article/details/gt2cqgrzwdj.html

Py:   [y for xs in nested for y in xs];  sum(nested, [])
来源：http://www.ydjk.org.cn/Article/details/gt2vjqsxhfw.html

PHP:  array_merge(...$nested);
来源：http://www.52xcode.cn/Article/details/gt2mkddtbat.html

JS:   nested.flat();  nested.flat(Infinity)
来源：http://www.52xcode.cn/Article/details/gt2xllgsvho.html

TS:   nested.flat();
来源：http://www.ydjk.org.cn/Article/details/gt2olytictm.html

Java: nested.stream().flatMap(List::stream).toList()
来源：http://www.ydjk.org.cn/Article/details/gt2srytfkdr.html

Go:   // 手写双层循环
来源：http://www.52xcode.cn/Article/details/gt2ztynowgo.html

Ruby: nested.flatten
来源：http://www.ydjk.org.cn/Article/details/gt2tjshiham.html

C#:   nested.SelectMany(x => x).ToList()
来源：http://www.ydjk.org.cn/Article/details/gt2uowpvfbt.html

[D19] 按字段分组
来源：http://www.52xcode.cn/Article/details/gt2qefazfzx.html

Py:   defaultdict(list)：for x in arr: groups[x["type"]].append(x)
来源：http://www.ydjk.org.cn/Article/details/gt2wxfybuuh.html

PHP:  // 手写 foreach，归入 $groups[$key][]
来源：http://www.ydjk.org.cn/Article/details/gt2umfbxxkn.html

JS:   Object.groupBy(arr, x => x.type)    // ES2024；旧环境手写 reduce
来源：http://www.52xcode.cn/Article/details/gt2zojylety.html

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt2bbiulguu.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.ydjk.org.cn/Article/details/gt2mxpiwtvz.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt2ugkrjbza.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt2vvyausdf.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.52xcode.cn/Article/details/gt2atnxfvdh.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2wvioyjyg.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt2mnawwiqf.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt2myvgfpva.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2jkiexuao.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2mopyajfq.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2kyiwvfla.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2cjqzmvsc.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2vjjmwhfu.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2lrxvdzxu.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2ffgmymxm.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt2qakkdtwg.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt2dlyfjyzx.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2qhyzhzhy.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2agxrgifw.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2egrdfjdq.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2vapmquob.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2tgatydsd.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2lcalpxef.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2pfckwuzj.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2xpwgpaik.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2mupngwel.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2jkstlmhd.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2rxzbmjvd.html

Java: new ArrayList<>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2altnumvb.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2qrblusud.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2xudbbigw.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2jtnlnqcc.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2rtpjicwl.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2nlxoeulw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2unffxzew.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2cxmagcku.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2hcaeysas.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2kkddypxk.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2hppdeqdc.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2hfumruhp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2cklzcypy.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2lzwdqzsa.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2dxzrakzg.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2ljpydhfo.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2sycnfzti.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pldcuhdi.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt2eoxsdjcr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2uewuxbvl.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2oukkwnug.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2rtynoqtc.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt2iqyvlchn.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2kuilhnzm.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2avkgslbb.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2outkznpx.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2qwukdywz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2cxtpxfxq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2ebzffxes.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fblpsfiq.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2fotdwprd.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2jhiygsut.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2khxttrjk.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2nyfzvaqv.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2dfdsdjik.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ysvfvbbk.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2fbgrpipv.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2eifwaylt.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2tsiwhmvg.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2hdksawym.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jlmizamp.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2wwbafexc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jyeilpur.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2oaapphdg.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2thaepoht.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2avbnjdki.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2pphcbsmg.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vgdxdalo.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2hgyhezbh.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vsidttjf.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2hmqpoqjz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2usmbvqkl.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2kpiwirtq.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2vmlqsbib.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2eynbjntr.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2tpmkfdlj.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2exnhljug.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2liqxrsgo.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2dkovfkds.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2uksrhqos.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2gbatqdlt.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2emldswfg.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2cculqdry.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zkqkbkxn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2rhazsxjn.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2mpuhwfdy.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2jmzwibzy.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2jeokwcqj.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2zuuaqbfg.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2mkhtefsx.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2xsuzwmsy.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2fiojnjlg.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2yhbahhjo.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2ovnplloq.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2cpmvrmxx.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bmnkides.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2hlgdhbxr.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bziolgqt.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2rbqxgmwl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2uohfwnqn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2epreylcl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2utavzgfu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ldlmoxff.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2jnzecark.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2crhdauws.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2imwauunn.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xmtojwwy.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ztdphsbk.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2qojtxznh.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2chtgjlyt.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2ovsazngi.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rscbygah.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hhlfercv.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2wotvdknw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ozitucux.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2eolfridg.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ttmntvpr.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2nmacdndg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2htknmpir.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2srocoiyh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2rmxowotf.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2trnuupxx.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2udvkxdqa.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yvqddevj.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2emlieaug.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2zraukvvt.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2jpmtekfj.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2kexhdjwh.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2kedtquun.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2hcbqbqvc.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2uwderses.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2oimddrhj.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2wmdsmekq.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ydgudaay.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ldurhsjz.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2ivkinxyh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2mlekrfpx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hkrojevq.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ceroejsr.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2dxznyypn.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2qoxfiywi.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2rjbjryhu.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2utrnerdy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2mepnoqvz.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2gefuwpbh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ywyafgzc.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2iebyjldq.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2dnmrcpqy.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2iknpevnq.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2kbrvwvuq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2eirlqjzk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2uofsgjcn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2blsciyhd.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wphvfuuu.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2rwxpmejc.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2sorskyrm.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2qauvbdyn.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mbzzauol.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2pnzcqlto.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2bqvduvfb.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2zgzfvtcf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2vxwhprzz.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2keuoxesr.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2imbbhaxm.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2wbveaswm.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2pxywcldt.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2tnikorcq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2ibzufhno.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2zfzpleif.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2grchjiqf.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2urchogyf.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dvhgpxdu.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2brkflonx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2jlciypkt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fkkmoklr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2bhbeqkzr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dxallfjp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2sxzhjwvh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2zjjsvtya.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hfopqwlt.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2fkvtdwuc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2hichxyum.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2szufzwsg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2uucbrjga.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2chzoudnc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2vbzkhjyv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2rmahwzdy.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2vaselzcx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2kkduljxh.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2hdmxlsvo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2moxpgduf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hmnqjapw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yqfoczjn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2tvdwsxbj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2epzmheoh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jbvtunxj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dnzgnvoo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xupoubot.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ipnkqone.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2udqspzop.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2wcfbrdwx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2dtbfkaje.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2uovwmpul.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2srmfxaac.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2ydhkmkqd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2addabbnj.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2lwjbkbdq.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2kfcznqbe.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2tvwgzhcs.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kdlfjiab.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ihpvwlpz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2pltxqxhr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sjphyvdx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2nemajpzo.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2trnkntpm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2skiyjtlu.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2rnbmoxkj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2dysyewak.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2zovrojuv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xovfclup.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ywuatxaq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2hsmqpkga.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2sclapyly.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2vygmwfbx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2iijbwrnu.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2aumyzvhc.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2ceahlamv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ronflhco.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2agufmkka.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2zwtkatqy.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2mkubcfpt.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lsqhkamo.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2eoebqqvq.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2xdytpqhq.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2suxqfabb.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2qqurtdxp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2mtnturau.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2twtffrxu.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2aztncrwy.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jledjgpb.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2diqfvwbh.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2nhppsese.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2pxegfcca.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2lzdvqpoj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2egdamnuy.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2axhqjjxq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tpdpbsou.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zixclkji.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ahkggryd.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2nmvokcer.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dzegymin.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ywqyqsfq.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2kzjzxbbr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2ymtacqib.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2szbtukyz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ufvhorht.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lobqrwxe.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2opfpdlxg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2xeltecbf.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2gbcakama.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2vfqskkdw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2obekaxfn.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2mwkieead.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bfmfhbze.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2iddaemol.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2kcgintww.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nfetqsfg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2ynfymdhz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rmykykpl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2azzdznhf.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2ivyubwan.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uoaxfeng.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wwexiufp.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2jdrleafm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2isptsmjt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2kyimpkvh.html


<!-- 参考信息 -->