代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2roukbusx.html

Ruby: arr.include?(x)
来源：http://www.52xcode.cn/Article/details/gt2oiypkuby.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2oxomsadk.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt2ztjsloab.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2tojvcghh.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2bqunipsz.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2rpiipjxh.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2rbxskebf.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2jpidbkcm.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt2jclidojy.html

Ruby: arr.dup;  arr.clone
来源：http://www.52xcode.cn/Article/details/gt2cpakclzu.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt2yfoqqcwa.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2kenejqcp.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2sxkjijps.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2afairkuk.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2hneamphd.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2madgllky.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt2wixtbrbv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2fcvzuhuu.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt2wzvfqaxv.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt2wbobbmpu.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt2widpysdm.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2kgcfdran.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2jbhptvch.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt2ikrxtpqf.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vuwdofpd.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2mhvieuhi.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2dfzugviw.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2liqiziwv.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2wdqrjhju.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2zpnioteq.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2eqspzblb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2ddhoxwwy.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2wdbsmwsg.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.52xcode.cn/Article/details/gt2uulmaxnh.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt2rbgoljsk.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2nnopnbgo.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2zrsjvxdh.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jvcjjhku.html

[D26] 数组转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uescgsce.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2ngmqvape.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt2vruewlpf.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2tlbkomzk.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2fpxuiqig.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2gfazsjei.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt2vfxpmtcs.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2xrcqrxgg.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2rvsdjisv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jrtwijtz.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt2galinzqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2azsovarz.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2owdfwbud.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt2gpzqilnj.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nzugqbya.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2vifbwgjo.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2frbtrosn.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2ybwwltpb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2iybktfnn.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2evvzirhz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qcwifjwf.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2zohwnpuk.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2lnufbfuw.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2kibbyzgj.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ruwxyfhw.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ehrrmebj.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2nzylrvdu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2gfraipep.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2uuuhspsa.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2wewtjggl.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2eivqooeo.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2wjxyanvm.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2gdkaqgvk.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2gejhcbvh.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ciedosob.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2vryfubmn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2nohxlofo.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2fxnqhlmc.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2ytglerpj.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2istbwkhp.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ueljdafw.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2cdogmmwe.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ivtjmooj.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2nzktlexm.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ywveuyxp.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2wluiqeub.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2yjuveutq.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2sfsnbxqo.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2holtlqvs.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2utyiyoco.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2cjlgxnxu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2eysnxqhp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2lzeusgpr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kpjbebsy.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2vqznuugr.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zbnmdaar.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2isosfhew.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2wcmpjdrg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2skklpvzj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2npukjmhk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2duxojocv.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xygcwvro.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2lfymoydr.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dfykatfr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fzhsordc.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xdvoibgs.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ypsnowvo.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2aulmfdgy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2uqfrkaho.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2igvbhvhb.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bdodbuzg.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2eeiumlhn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fyuczqja.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2vqgtotpy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2vptnubzl.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2ikacavgc.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2olxpgjmc.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2ymywvqpv.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2vtzsghjm.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ghntqojz.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ofbnyrmg.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2imnyprsw.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qozbjcfp.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2cnkjvljm.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2yyupchxw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ipzszpfz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lrdkxssm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2kafdyquc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2whmbtusj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2nnfbteya.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2msqtbezy.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vsrehkve.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2kecdfgtp.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2llfwytjn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zrnyfqon.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2wbszyzmf.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2qprptubs.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hphszgzi.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2fbvldiii.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2kiuosxmn.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2vltiykao.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2tutphzrh.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2fqfesuhe.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2hzxuwjhj.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2skpmnwkz.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2zdqsygza.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nagwyjfb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2qzqdsvdx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2vlplaqpv.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2dipihkxi.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2zwvufxxd.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2owsnresv.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2mozkdwvh.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2mkytoifz.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2dhwipgim.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2cvafrhdf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2lfntcrax.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2ssjkuiak.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2epeyrjna.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2foewkmlb.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2afzfypnd.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2yvnqwhwg.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2zgylnntm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ojjkmsjc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fjqsxumt.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vwbpeili.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2jtqtgbmq.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2ijgihorv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2dhqmxoih.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2nskejkvt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2keawpvrp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rzzipmjx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2jscjxxtf.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2swhzgbkq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2gzyatjuc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2ctwuzurc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2nnfxfijd.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2vtvypsvo.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2urrypgbx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2thwjqvva.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lbfpykte.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2tyrexlyl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qmqhtwtr.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2qddlbzuv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2yaevlvnp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2idgzfgae.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2lsaoahxj.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2xfngruam.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2xfhhdjwa.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2cofzxgog.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2zhimhmef.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ppnyemgd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2uitoclxg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2nrawrkdd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2yziwtirf.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2xwewtqsv.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2xkdrqbmu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2rbajpyea.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2ojkbjtcx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2dfmxhpbs.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ntooguja.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cinljlnn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2zyzovkjf.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2vqtkaefi.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2kboeceea.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2lmuclwrd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2hxauqqby.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2mocokqod.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lucbhhss.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2nbazyasp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lecvuwqq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ezzgshkv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2poptobvf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2tqyoyrdk.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2cwltybtu.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2vsqziuhm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ogffuemv.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2gkrfpeqz.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2xdmzwxgf.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2cpcqeuze.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2ggxrvhpr.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2wvocjnxm.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2wcgxaioz.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2frtymmjs.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2fmwpryjp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2vqzqdjyw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rsjslhib.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2skifsstz.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2uilxrowi.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2rhgpesou.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2hafyktgk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2paeqghif.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2lbokfzhy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2wcripuyj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2pbcxfmiz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2caingygx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2onulreyx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rflpolqq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2mdqzrawy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mvgzjdmx.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2chiadzeu.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2hxjjonrl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2jqoiduem.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jdsiyhxe.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2tjgrpdfn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2uxhguudh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2mtpsrlea.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2ndxrzcef.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lydqwtls.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ogevkink.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ewrclkys.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2jjqpudld.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nwxkekfl.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2evetvdqf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2gihghsyg.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2blhhxqjw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2foxmtrlo.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2efscyntr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qntcvfnb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2ahcktusd.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bwnjjrvf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2liyespsq.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2mgyzlbqh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2pmcpkfeb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2mbwvnxyl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2lndpirmy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xufciaqm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2yywjrnwy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2ulshugbv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2lnircavi.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2vksqgqra.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2svjjsvdp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2wjykaybp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2chdtgtrc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2kyqzqfme.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2aabsaork.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2qizwklmf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2hjtnflzo.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2vrwtggju.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2cfltfpnq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2gtzxfint.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2vzvsmack.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2xaobxdtd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nuynystq.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2qezzcjsd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2zukungmg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ehyuhzku.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2lxjbilqq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2lujngzni.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2emogxvuc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2rqfomomz.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2udpiohze.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wlpnsbhj.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2scermlkh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xognituz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2zexebenx.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fbmewnnv.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wxtfrkbx.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2dgamfhqn.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iuwsyqdp.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dzyobgnj.html


<!-- 参考信息 -->