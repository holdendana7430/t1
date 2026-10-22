代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.ydjk.org.cn/Article/details/gt2wnqtrzau.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2zwbkqdeh.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt2jcjnwlsj.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2irdbqrti.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2bpgrvidp.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.52xcode.cn/Article/details/gt2dislmbdr.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt2mdjnintn.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2wxdggifg.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2vaxletyv.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2omckkhsv.html

TS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt2bufgdvxl.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt2sscnvgms.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2oaiyozkc.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2mvbdighd.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2uspervcx.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2cabbbotg.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2lwfxbllb.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2mqfejylz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2uqnfuqor.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt2wyaaejqz.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2vmrnaddd.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2mywjgxob.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2hoibxqqm.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2zzaopzzb.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2npzolopx.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2wwcnjyvf.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2htomxpov.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2xxdksphm.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2yknxitoq.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2ojfzensd.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2vwdrgndy.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2lglulxdn.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2cfsjcgvm.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2guujypav.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt2bswvfnuo.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nrwhlsdz.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2aewanxih.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xdaitith.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2erghmivz.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2czyivvix.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2muioolsu.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.52xcode.cn/Article/details/gt2ljbaenok.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2mdyshwsi.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2jendipcq.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.ydjk.org.cn/Article/details/gt2abbwyvuq.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ithbmiry.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2cpfeyvom.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pgkonwdr.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2akwuxqen.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2uqyjyhva.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hnmaejll.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ktpkself.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2qbevbnvd.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2jehqxxnl.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ltiswodl.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2hdcycizf.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2nweigbxk.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2sntnlfxs.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2kufmqtnp.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2soianhcl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pudgrcev.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2jdvczhop.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bwtmcbuw.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2knhskflf.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2bamwoplw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2qyqlqevr.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lvzajqwa.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2guaurayk.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2wopuvabl.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2wshdwivm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2dqpbusle.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lbnqxfnc.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2lbnvvkil.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2tsbxlcxa.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2vxeqgdhv.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2aydkcawf.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2argfodff.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2bwnucmrg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2pdflwjqb.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2sndorfjt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2mefwtqhk.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2lcpxncmy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2vukkeutf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2mbunlwqq.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2ejsowidv.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2iaxjdnvn.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ygpivqzu.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2pojinlrc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ybqkpmip.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2cnsfsazd.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2kiubidaz.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2uiognlch.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2dpnkevwy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2glixtopi.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2joryicyf.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2hvsomhkb.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2larxture.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2pmgummtl.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2vjltuemb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2emjdjxyd.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2smqfmyrs.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2istxrrfa.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2rjpuqhxi.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2kujvtafd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2lffxocib.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2gpvojcnx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2mtkssqhe.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ytoyymnh.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2slbtyyfx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2uoehpkvg.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2zkjfwvik.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2iplpqcmy.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2iceyarqb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hbpkfdju.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2erbrpmja.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dvtanftu.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zkpuuayo.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2rypbmfee.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2ifnozmxf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2eaeeqldv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2bkzuizqn.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2ffooijip.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2rjfxeqgq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pzhgidnf.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2dcccfhbo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2pdhbcqgm.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2hgablkeg.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2kmfelied.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2mouqbvyh.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2tkcsoipc.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2hrbwqrva.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2cwgsfqaa.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2yzsxgfkz.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jzfryzjm.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2wkvwohwc.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2wyuggaik.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2nqqgrihi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2qtxpfdvb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2rvvmjwne.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2xfcququj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2lkssajlf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2kgardiej.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2frqojcqa.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2hsbzmrqe.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2zrguxxte.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ltraxabm.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2bzmysdlb.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2zyblryhe.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2rbvbpnni.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2uuybihfn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2nsdljpbo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xpdwmqcr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2hnbikqaw.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2qzznrkik.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ltqqooxm.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ivjhgzpl.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2qiffbnfr.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2osurecdn.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2mohufjiy.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2kygngvuu.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2yjtujytt.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2glidvqfm.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2mhqjwmwc.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qijzztbt.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2yfdpikdp.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2gkkraqqk.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2rvwfrdaz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2mjmiphuy.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2sqkbzepj.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2catdhdfa.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2rtnvpsjo.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2eekohjge.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2zwqtdbte.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2knpclxmg.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2dsvsufoe.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ustwgbrr.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wlzlodzs.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2xqplqkoc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2ldbcfdae.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2tuxjtqfm.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2wdnrxdmp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2aundptey.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pnxrgaem.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2uonkpinq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fotscptm.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2bugchqrs.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2hzodrauq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2dtelylph.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2frhebyhq.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2ananzzms.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fqlvttsz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gbvispdz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2udnxspcp.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2ehakvlcn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2esgjewau.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2upoyxzqz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2gjaglbfo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wqtdwgfa.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2xyjzanfn.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2lksargmt.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2fgftebgh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2fyldtdsu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2uxovumgg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ngrzyusu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2txdhsvxk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2pfqhjlpw.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2vozbqzyy.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2xndhuaqh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2vjoybhzr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2golufvtp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2diktcgra.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ctrsvajq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kooxlzfp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2nksxgopj.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2sxrxzqya.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2zhoveltk.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2xbbahzrc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2pjujbnkj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2virhjzvc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2yntsbwry.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2yfspbrof.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2zjbigmur.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2sonihhyy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2auqftwht.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2ujwwqqyy.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2hshiahtj.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2vfjytjwf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2jvnlrenm.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2kntjzedf.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2bdsorlsq.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2zptdtsdj.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2stisgbtl.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2giukmqwp.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2eznaalrp.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2fwhxewwk.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2dwjqsvvx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2wwlicauw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2llalpuif.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2uaiatjhd.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2pukbnsop.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2qlehjods.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2hpgmcefe.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uwxahkgh.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2ivdvwxtt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2chcohikh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2qsiligss.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qawznrja.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mxqgibzp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yrmcbxtx.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2tobzttqk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dllgftdq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kearamxo.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2wyenfhls.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dqxvofbz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2fxqlfsbe.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2pnxbophc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2uoboimos.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2qdbytjyp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2dvskgcov.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2nvncalzm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2edsacmvf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lqjgaksy.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2baivpwvt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dddhlulp.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2cnnpefpe.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2jwrtehmi.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cedjzvof.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2rlmcitnk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2wacxvqrb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2pgdfenvp.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2gtfmchbf.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aclqhrej.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gzswwqab.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2urlloytc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2hysjnsja.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkzrgnvi.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2bngsmqll.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fsmymwhf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2akckdfct.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2gkxlahdw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2pszmaztm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ksmepuih.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2mxzqzscu.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2wdqmvpde.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2vnqepubq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2erqcdskt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2awqfirqz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2rmsobtks.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2jgqsafcc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2kvzruvpy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2cuhlzfgv.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2hwgtzikb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2twnqgjmn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2cfadfwgc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2tvsbjvqm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2gwhjtapp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2ezpibsdd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2jzdivggd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2vvangvce.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ekxdbmpg.html


<!-- 参考信息 -->