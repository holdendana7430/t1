代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2vzwcpllk.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt2javkjgom.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.52xcode.cn/Article/details/gt2boolckrd.html

Go:   // 手写 map[T]int
来源：http://www.ydjk.org.cn/Article/details/gt2mjotmvxo.html

Ruby: arr.tally
来源：http://www.ydjk.org.cn/Article/details/gt2cnptgigw.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt2zpjyjjrx.html

[D21] 判断是否包含某元素
来源：http://www.52xcode.cn/Article/details/gt2bzqcudfr.html

Py:   x in arr
来源：http://www.ydjk.org.cn/Article/details/gt2lijltfca.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt2skutbvdo.html

JS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2cccqqbsb.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt2baswazdo.html

Java: list.contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2vxswydtk.html

Go:   slices.Contains(arr, x)
来源：http://www.ydjk.org.cn/Article/details/gt2dywopgkl.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2bvdvuugj.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt2svicymuw.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2krohuduh.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt2jcpxcfpx.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.ydjk.org.cn/Article/details/gt2tspzcidq.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2ruyfsfyd.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2sfatjqjb.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2uyfedtxn.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2uttjuxji.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2vjarquea.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2efostthb.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2qfomvdls.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2kulhbylk.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt2nkmprbas.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2hshjprvu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2iyarlidn.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2gsfkuzek.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2avnqfbpt.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2zfqsjpke.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2ziomxdsf.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2qltsxlji.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2wlpexitm.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2uxonpnzx.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2ytalaavm.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2fvzrzisw.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2wurjglra.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt2lqzoemrm.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2unoynkgw.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2nlbbpyly.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2hfnhjxte.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt2djjneodv.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2xqxzieti.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt2flulldec.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2kmdfeewz.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2myiekzmq.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt2adziobyq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.ydjk.org.cn/Article/details/gt2iupenqtp.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2jgsoqitc.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fkrftyub.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2fabkpqmm.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2wahascue.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2narhbuxj.html

TS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2jdqkvtcj.html

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2fwezvhjm.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2zgjxjybz.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2vmddlnog.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2eouvsneo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yxmunjot.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2xtambiho.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2agyfbkhb.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2honglqhi.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2eoojrxdt.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2axqnqcvc.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2dbfpzkmm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dpcjrxzl.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2ppsmanly.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2utevoiuc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt2svxjijcj.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yujjvmdj.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2luvsqufc.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2zbjpopeq.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2geblagzp.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2cehwvoui.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bqfftqre.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ahqxorus.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2iknletni.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ynlyamvz.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2mwwrczrh.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2poteycmv.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2dtnvwoly.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lnfnbwvu.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2fdbwgvug.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2sdwcubbq.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2riusqmoh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ekywbfoc.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2bbtlmjup.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2mippjzmb.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2fsbzqoxk.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2mmezqzta.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2abfbbzjp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2lkcuggbi.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2dznlawiz.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2awmigjyi.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2vippxjzt.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2cpvgqqdh.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2jqexbzcu.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2geugpqov.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2rnjgpmgd.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2agsyiamn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2lqqovhzy.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2dawbpzjo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2lgllyrgm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2qacjejtt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2rjaouizx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2iegsgbzb.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2edqsfzdc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2oxphewdn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2iidfxrvf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nuibxtro.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2evkftnrk.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ffuudcjf.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2actgfzon.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2goaotuik.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cvjnidcn.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2xddliuha.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2xvsfudjx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kprldtwa.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2ithqbeha.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2mcevpvee.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ukrrzvve.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2fscubgtr.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2ftlnpeyi.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2waykhrih.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2qzjgbzfw.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2pirecbej.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2riromxmz.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2htcdejlf.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2lxogrzxd.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2cykdditl.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2tsvsxdqv.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ntwsxbty.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2wcdyskeo.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2poapujfn.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2wsshpvjc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2wnolmnhk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2vqszoelp.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qywqkkow.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2avwgnsqi.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2nyukxxfa.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2isztbwir.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2aqfwsevh.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2gymuysun.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ihxpzbxh.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2ipsnbuuc.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2pfmizbty.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2awzeufrq.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ttnakiyt.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2aedtumpl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2dbvkrart.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2vlhfocdw.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2eywwrhvq.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2wfsqsmfk.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2liuurkcl.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2luayboej.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ztwfkspa.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2kwpuynqp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2vxstrkxe.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2lltedlvj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2eakysxlr.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2feihjrvv.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ncjswrvg.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2xackqlrx.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2pxgbvpbm.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2mufavumz.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2jmsutlzs.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2utcwioju.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2nicvtvqf.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2llnfyiox.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2ryezhoih.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2azjpcjxt.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2refkeckn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qwugjwbp.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mdzcqupa.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vanztrxb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2siedgflg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2tcazxyrc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2shsxrmmn.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2rminykie.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2bliagtay.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2kgnncqdz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2ndwdrdtg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2ujdhlpai.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ugzqpacp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2svnabovn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2uleihdvr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2vwlhunjy.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2ufentleu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2wntpbwtv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2pmdlunhz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2nacdlmal.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2reqklaol.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2jxxpnjww.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2iespcrzm.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ahtxrhfh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2llqyvukd.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2vtdktbem.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2mkynxifw.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2jjgnfsxr.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2olmhpplw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2dfietjfs.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2hleatgka.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2bbchaxkd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2oyhgtrux.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2euyrczhs.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2pamrlqrb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2bjumhskp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xztbwwvc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2xwvjccrf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gkgnboau.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2jaaujpbw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2mbbbwwrp.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2cljshtia.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2iupftevt.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2ixywzsxm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2mtdlikir.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2aiirmzng.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vzglrlhh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ljzpcpyd.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2comyxcjt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wwwptdsw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2ipgsebze.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ananttvy.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2owpivpga.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2drsttvdf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2oorsnwzm.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2tcywcalb.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2zysjphzg.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2muvfezsb.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2icoaryzz.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2xprtkdig.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2nvkygnqw.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2utpoerrb.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2yhocnnjm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2pfdisncu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2xpnszwvh.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2nxboqqly.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2zxaggdfr.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2mkvntyje.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2zazhewzn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2lpikovem.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2lwbipvea.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2qnihgevw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xpelurfn.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2fdfcjfmf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ziqcybcg.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wumogcbc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2wdgxgpna.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mzcjzddo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mgwqghqg.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ztghmtbe.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2sdoumwat.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2aabbpmpk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2loiauipq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2sigbbzns.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2lgykaxyq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2oqalnidj.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2vcqvedia.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ebvwehga.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2itphlrva.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2qcmhxapp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ypaibckv.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2cwzayqyb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2mmtsmljx.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qtohxzsl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2vaxutuln.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2tpbnagwb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mscfieos.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2dzjdqcdy.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gwjkajkp.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lixsfohs.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2gtdowkfk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2ijuptxwj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2szvsygux.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2rcwmjlox.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mjjlcvmt.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2xngloooe.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2lzvqlwne.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2ebheijmu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2wqmtskwc.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2oanksmza.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2mjnalogy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ggdwzank.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2oajodlei.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2miniqppp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2gwlmbgvv.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2nmpsckgp.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2fdnxkttm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2wtyrafgs.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2suzxhjal.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2utuysogu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2empqfmph.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2gtkhuiny.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ldrbhkjs.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2vuumzodj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2plcevtph.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2wjowrekz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2obzfzoyt.html


<!-- 参考信息 -->