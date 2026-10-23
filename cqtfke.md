代发 wailian999

JS:   arr.reduce((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3nkyolfhr.html

TS:   arr.reduce<Record<string, number>>((m, x) => (m[x] = (m[x] || 0) + 1, m), {})
来源：http://www.52xcode.cn/Article/details/gt3sbfdkwre.html

Java: list.stream().collect(Collectors.groupingBy(x -> x, Collectors.counting()))
来源：http://www.ydjk.org.cn/Article/details/gt3baztbnug.html

Go:   // 手写 map[T]int
来源：http://www.52xcode.cn/Article/details/gt3iqyibiix.html

Ruby: arr.tally
来源：http://www.52xcode.cn/Article/details/gt3rxpfgnlk.html

C#:   list.GroupBy(x => x).ToDictionary(g => g.Key, g => g.Count())
来源：http://www.ydjk.org.cn/Article/details/gt3qfwrbgkk.html

[D21] 判断是否包含某元素
来源：http://www.ydjk.org.cn/Article/details/gt3quwuzsnj.html

Py:   x in arr
来源：http://www.52xcode.cn/Article/details/gt3swewbmtb.html

PHP:  in_array($x, $arr, true);
来源：http://www.52xcode.cn/Article/details/gt3shhqwtez.html

JS:   arr.includes(x)
来源：http://www.52xcode.cn/Article/details/gt3uvzqmrvf.html

TS:   arr.includes(x)
来源：http://www.ydjk.org.cn/Article/details/gt3lxsbejpn.html

Java: list.contains(x)
来源：http://www.52xcode.cn/Article/details/gt3hnjpkuur.html

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt3rdqmanxu.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt3jdjqfxyj.html

C#:   list.Contains(x)
来源：http://www.ydjk.org.cn/Article/details/gt3ztalputx.html

[D22] 复制数组（避免共享引用）
来源：http://www.ydjk.org.cn/Article/details/gt3cfpfmyyq.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3ennsrryi.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3zviaixoc.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt3gxdaauze.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3mkqfiszo.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3bsjrbwlv.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt3hjrsqbpw.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3cgmkfiqn.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3xumxyqam.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3iyapyufr.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3fjvabvap.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt3onraxlhu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3woaradyo.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt3jmxtspdw.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3obzxeazv.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt3hhdagklm.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3xwaaafyp.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3sjpimepi.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt3pelspbgw.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.52xcode.cn/Article/details/gt3onprinnt.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.52xcode.cn/Article/details/gt3ckcoezwc.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3hepgmwnj.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3arvagjbp.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3ezbyfpif.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3vsgqqrsf.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.52xcode.cn/Article/details/gt3rqpnbtjm.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3ynofvewx.html

[D25] Set 集合去重与交并差
来源：http://www.52xcode.cn/Article/details/gt3bziqcftg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.ydjk.org.cn/Article/details/gt3cdmuiwkf.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3pmtweagp.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jmyuiqbq.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3wxnefgmm.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.52xcode.cn/Article/details/gt3dnyartve.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.ydjk.org.cn/Article/details/gt3lmpehyvq.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3locxczzf.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt3hbvlmyce.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3brjlfwsc.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3ivatgkox.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3imntoopv.html

JS:   arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3mappbfgd.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3dcxcnuin.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3ktxrqcvp.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3cbppbbfx.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt3avhrimrm.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3gpybhbxn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3izvttxet.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3nwiusjfi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3twxddexj.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3vohfqubz.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3tmqofwgr.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3udqmyhpx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3moomxmcl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3wfwhvheq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3vkdhiftp.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3crvveema.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3yrbnlebz.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wsvgukht.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3hbujgeoc.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3oxrbbkwh.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3hqpcrclj.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3bsiqeeix.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xtookyqj.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xfhnozvc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xvnrdjyb.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3hqwhknwt.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3stgkcoao.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3udwkjdbw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3hhcxesgu.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wuflklei.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3upyvcofs.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3fqfynxhg.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3usbzepxh.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3ihszjjwj.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3ldvkstoq.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3kixxogoc.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3tlxdonac.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3sjvvwzev.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3kvnrcpzp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3dctsdreq.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3eebhqqxl.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jigrpmhy.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3auvcwntf.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ozlzhzra.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3jcneeefs.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3qlczxyto.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mjknhisw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3mpvouvgc.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ymevaerw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3erjxvkpf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3crnibgtw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3srmsljnx.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rtwuehyr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3maqiqgjq.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3fgprtuhu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lntaohbt.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lgljdilt.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kwtdxcaw.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ndpvpykq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3fghggiej.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3jrspbqeq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jumyhuby.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ewhccntr.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3eviubwyg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3nzitffcy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3vlavmcpp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3jghzstpu.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3zbjquphe.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3yvhsqmhl.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gknpasqp.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3fwclevsg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3nmahpfua.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3wmsmtjyt.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3ituuictg.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3udwbwgkf.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3nrrbwdra.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3gxyrdidm.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ouogcple.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3ysnmnthy.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3pmizunoe.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3hmeavxmc.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3vnuiqtoz.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3sizwnoka.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3eenvjtdh.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3disxlvjk.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3umzjapyb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3fypgwbwi.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3nxtkdxwg.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3kkbnupnk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3oeaxkzwe.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3dppmzgtq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ounkhqph.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3vrubmbtm.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ctijngia.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hsjakpat.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3hzfcivmk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3epuklytf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3gaqkswyp.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3wiusfxyp.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ugjtluvb.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3gnbmdpdm.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3grzjqkjj.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3zpcrydcd.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3etbqaogj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3xreumtge.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3xrvbqada.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3pdhabujv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3kviesdiz.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3uotfkxnu.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vgkmmsgx.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3zuaazlxm.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3fsxybnds.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3wrttuplb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3vqjjlrdb.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3ydnebzcn.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3nkwrexhq.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3btlrkdfc.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rsqtaqpj.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3fisiibsz.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ymjiuolr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ftmfmgby.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3suppucku.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3tgvqzeox.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3zjawwpxx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3iwyiopvc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nnmusnro.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3zpcuupim.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3uwiqjuel.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3osjbftpt.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3eoektvpp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aviexewe.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3yxxewtdk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3nxlivgwi.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3ycwuziyu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3tsjlfzml.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3zlojhyfn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3mmsuaver.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qmitfzov.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dukwgubv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pcyliidc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3thyezqlp.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3itqrgsgs.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3blrxcsyp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3vnqyppeg.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3huiaspct.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3tiwxowjc.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3ntixlhkv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3sdwcuoru.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3mkzysodg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3nzutaxwg.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3utldkohb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3uipahctx.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3noubemmo.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3uaoehipf.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ufswnfrk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3aetjfhsk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3bxfjghot.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3pgfgcoow.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3gzgcsvpo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3wdodwcly.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3qnrfcccg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3wextqhbm.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3fxnymkqs.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3ifgkztqd.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3sckyowbz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3psrafdgc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ofnmgnex.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3tfwskihx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3jhkhwydd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3agzpufot.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3ywsneyji.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3miwfkqxb.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3zphthcuh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3zzamojyu.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3zmchneax.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3yafktgse.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3hwkbgoec.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3dgbkevre.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3ucvpeclb.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3tkkvmikb.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3ddbdfcfq.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3pppqxibn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3frgkfawc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3qzxsonfu.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3dohhmmpv.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3yhpuomif.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3jlzdokev.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3aoxmqaef.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3enlwyscc.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3nylpydna.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3zmtjwunp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3qlmeahnr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3oexuleao.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kwoyodvo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3aqfwpmdo.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3nxoqqtbr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hmdwlxoo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qiwnpfup.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3oxflirns.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3rwsxciwn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3yvadpsnz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ckvyyhcd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3gpmbqwon.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3qghojsdl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3muewvegi.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ckfvwbra.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3yyascpkm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ijccfoxd.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3ibljneqb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kkndquis.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3nbrrbjny.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3dnobheri.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ocsljzok.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3iygdgvrj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3efzemaug.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jloemeab.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3fhuxfjxy.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qmfdpkyv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3uzlwwlad.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3xftdowvi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3hfdoupxi.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3mnvjbiho.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3sgghtedx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ilbkoojg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3tvynoczy.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3ubeslwxv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3zybactwh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3svisvgef.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3hxaifsqn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3jhujvhgl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3lkocdzbl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3mjifziaj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3fzrjfmuh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3gjlzniyi.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3yzbzinhw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3pqhdiibc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3kvnccekq.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3ldcidzby.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3nplvzdtu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3buojhyxn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3iusmeyud.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3opqmrlem.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3crkjihpi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3xpafomxz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3zrckaqpf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3plgkvbrm.html


<!-- 参考信息 -->