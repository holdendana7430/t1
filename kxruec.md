代发 wailian999

TS:   Object.groupBy(arr, x => x.type)
来源：http://www.52xcode.cn/Article/details/gt3inncidpc.html

Java: list.stream().collect(Collectors.groupingBy(Person::type))
来源：http://www.52xcode.cn/Article/details/gt3eutbwxdv.html

Go:   // 手写 map[string][]T
来源：http://www.ydjk.org.cn/Article/details/gt3mcnxugcp.html

Ruby: arr.group_by { |x| x[:type] }
来源：http://www.52xcode.cn/Article/details/gt3lmdfeksm.html

C#:   list.GroupBy(x => x.Type).ToDictionary(g => g.Key, g => g.ToList())
来源：http://www.ydjk.org.cn/Article/details/gt3ggoedkfi.html

[D20] 统计每个元素出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3euxbbbpb.html

Py:   Counter(arr)
来源：http://www.52xcode.cn/Article/details/gt3bhymbmxn.html

PHP:  array_count_values($arr);
来源：http://www.52xcode.cn/Article/details/gt3hljlxdrn.html

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3ymldxkpt.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3hfvokdce.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt3uurcsidf.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3rkfkkasb.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt3tobktmyz.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt3zobizetj.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt3ngycjswt.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3aozswdeg.html

PHP:  in_array($x, $arr, true);
来源：http://www.ydjk.org.cn/Article/details/gt3phsdjseq.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3dvxvklvi.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3ezxssdem.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3osjegntr.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3kmktehwa.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3aicokhwi.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt3eeyhwtuz.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3fewrplxy.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3xywljpib.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3acqgjvsz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3ljvailwf.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3uldwxdog.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3osyosjpe.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3zbgncrza.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt3ragkkxvy.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3pmlluzbh.html

[D23] reduce 累积计算
来源：http://www.ydjk.org.cn/Article/details/gt3dfaxwlqp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3ashgrolw.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3dkbijrsw.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3hjqlqywg.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3bppbbphz.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3qqoppvjy.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3mlsycnan.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt3dawjbrti.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt3vaorumri.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3jbqommdp.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3lgksrgei.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3ygtttjfp.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3euslbadq.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3gubqfupt.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt3yrzapyfr.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3wfjnnmtr.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3bbgyutfu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3tvaawhza.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3ybsthgbo.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3azbhtpoc.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt3hnipayah.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3gdybmpxy.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3tbzzphrp.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cmrwzvuf.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3ijavrjyd.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3oujgzrui.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3adnzjbhz.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3ewkypkdn.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt3ljniuvos.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3ystzdphh.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3fccyeidb.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3fgaaliuk.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3vkwlpiml.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3nfuksmfc.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3kiydiawh.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3gxxwaspp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bpcginpt.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3cpxuqsix.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rmhedswa.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3avbyjwps.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3vnssikue.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3pokefrxg.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3zvjhxofw.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qknbvnaj.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3wojdpeoa.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3oojsxshq.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3rrynpajr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3nxvsvihi.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3hbszscwq.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3hprpvcxs.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3ouwkyxik.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3lmwoisyu.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3nbbmangw.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3qvsdhevk.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3kswcxuro.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3xwltpikj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3gpnhitzh.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3bjlifjso.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3ssrsyhfz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3blhsohxg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3efunljhs.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dxvbjwbu.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xctvflav.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3czpeoeoy.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3nanhqwts.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3lcpvsgqe.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3exwvjtxb.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3blmivaor.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3svrznofj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3nctmerno.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3cdprrydm.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3yfaxbbty.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3nepubplr.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wpegsyjb.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3uwgokebs.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3jyvvxcza.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3huzufvlw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3ruzlmnns.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3oxgrazov.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3mdhabmig.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3jxeohmng.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3vdswjpaz.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3iqkfeemk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3atckzduv.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3jppwfuet.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ttgstddd.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3attqegbh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bqekvhjs.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ovyedydq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3iembdmcf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xvzqelcm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ivinkjpf.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zwztogln.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3yxcnmgbc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3ykatfcsg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rkcvxurz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3mzzdwtiv.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3tuwjeqyt.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3kmumicak.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3lwnchdqk.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3umfgnnzh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3xudbqhqh.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3amuinecs.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3rykvetjz.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3twuorfcq.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3dzldnplf.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3njhslqug.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3wnbeprwz.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3wzfyoltu.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3cxpcstdb.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3nmjkvvmv.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3czjfquux.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3aygkfeyt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ohqsecey.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3hequqwvp.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3tntgtomm.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3nbuldhmu.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3rubjgsms.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3cfwohrin.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3oqejbobr.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3cseoujpz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3anbqkljf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3vizcssoq.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3afitnzyv.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3nucwtnuw.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3mejdaepd.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3gtctttpt.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xjuajsue.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3guhpaiyi.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3hgxbfslg.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3fudrjcfx.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xlbbajpo.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3unedywss.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3jyceaiyc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3tviznvjf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3skjofmhi.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ikmolhav.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3xzxvcykk.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3jiajlzli.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3whghjvqa.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3irzjzvlt.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3qisxoyoy.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ofvbkjjq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3svsqwcyz.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3mlcpetec.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3uiocttcs.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3udaoqiqk.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wdhosgwr.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3nkwkrmtt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3semrewim.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vomketmi.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3lkxfzeny.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ylgutikp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3kggjziky.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3codukqka.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3lxgtdejr.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3pvqewpqw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3azadstza.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3eylfisog.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3evqvuiqo.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3hsfoyxvk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ogtexcps.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3yypwrtvw.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3koinluyc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3eruqosal.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3atfwxbpb.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3cvdqnubk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3flqyotjs.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wsxrkrju.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3scfbivzo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3yayuwboe.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mugumwsz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3iyvtfpxq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3jcwigcrj.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3qdbjhtes.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3divzqbnm.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3sxambheh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3jxbztczg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3yvfuejgf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3usdcjjnf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3chqdeudk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3mxqlebeq.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3mgevpxap.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3evigeytq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3jbfgodpj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3sfuqsjxr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3krbtotmy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3sfuhryvm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3tllivatc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3kikjxksl.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3rslrtitz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3hhetbzex.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3qhinzpcr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3mkoqcxrz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3rprxkxlb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3inyctiaq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kkxgncim.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3enfqvuhe.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3wbnwouad.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3iaoyiewr.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3yetpojtx.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ikfsnauz.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3skqmewbi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3fwkhgtex.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3vxcgxwca.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3andundbj.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3sresgrwp.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3lqgxyqxt.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3hebicfxv.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3crgoxpla.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3rcbaktmg.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3bchilbxr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3nylpasvp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3thintiht.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3xmkvswxk.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ayamiglf.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3cvcnflpq.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3yjkcegbw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3uwpzaxwc.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3djgjhdrd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3kherzgle.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bpxvcnax.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3tarriftz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3drpakkyx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xvnsszzi.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3xzdcxyjv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fryurkvf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yqiwryqq.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3kmiismks.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3khdyeqfp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jxclvbxr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3eqtbssnq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3pjnqwrlr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3sczaqrdb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3nzdozkmh.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ruvbarys.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3llgenjlh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hkvrftey.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3wkfpysbt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iscwyatc.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3ivumbask.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3jdilvyth.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ygmtenpf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3refhdchr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3aauwjeyv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3qozadbih.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3ajlqbkfd.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yizpwxcv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vhgximgp.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3qhedjjbf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3gfinjtji.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3adqgxzrq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3wfafvbql.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3wlzjpohk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3hlhcokuh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3vgcnbhqb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3xbvdgktw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3gnobogdt.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3isznglgd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3bdbfudez.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3fwrriyko.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3dcwynjqs.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3hmdgrfob.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3ubrzowxd.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3izoaimpd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3tvoloptg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3nvovxjlu.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3bioetvju.html


<!-- 参考信息 -->