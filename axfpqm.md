代发 wailian999

Go:   slices.Contains(arr, x)
来源：http://www.52xcode.cn/Article/details/gt2tgacyenw.html

Ruby: arr.include?(x)
来源：http://www.ydjk.org.cn/Article/details/gt2ohrwqtgg.html

C#:   list.Contains(x)
来源：http://www.52xcode.cn/Article/details/gt2rqmorbkd.html

[D22] 复制数组（避免共享引用）
来源：http://www.52xcode.cn/Article/details/gt2blthtpnv.html

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.ydjk.org.cn/Article/details/gt2aliebzbd.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt2liqazsaa.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.52xcode.cn/Article/details/gt2abmzsegk.html

TS:   [...arr];
来源：http://www.52xcode.cn/Article/details/gt2uppzbqra.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt2fynwykvb.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.ydjk.org.cn/Article/details/gt2yxgsxryh.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt2dvefekce.html

C#:   new List<int>(list);
来源：http://www.52xcode.cn/Article/details/gt2bytrclzp.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt2uikfobux.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt2mqujbygo.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.ydjk.org.cn/Article/details/gt2ggqddpmu.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.52xcode.cn/Article/details/gt2caofxnxr.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt2zuzyzulg.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.52xcode.cn/Article/details/gt2cnkmgkmq.html

Go:   // 手写循环
来源：http://www.52xcode.cn/Article/details/gt2mjdybdan.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.ydjk.org.cn/Article/details/gt2apswpsgj.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.ydjk.org.cn/Article/details/gt2tucomkzn.html

[D24] 字典 / Map 基本操作
来源：http://www.52xcode.cn/Article/details/gt2nqzsmquy.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt2yrvjctgh.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt2uiurswhm.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2flstnmls.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2clrojzzj.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.ydjk.org.cn/Article/details/gt2iodvchyn.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.ydjk.org.cn/Article/details/gt2forlzmjq.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt2stqzifvl.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt2xkynjcdx.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt2fgsqqsqg.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt2nfuxhcwb.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt2jacojfbd.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt2qtflsbft.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt2ynrbpqam.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zyazzfwx.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt2zhafxbov.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt2lspmkhef.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.52xcode.cn/Article/details/gt2mxgglnqv.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt2fzcokssq.html

Py:   ", ".join(map(str, arr))
来源：http://www.52xcode.cn/Article/details/gt2pusffjzj.html

PHP:  implode(", ", $arr);
来源：http://www.52xcode.cn/Article/details/gt2jjywqipo.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2cxrhghoi.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt2uzzvvgex.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt2bfeqfcaq.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt2ocsmsgjw.html

Ruby: arr.join(", ")
来源：http://www.52xcode.cn/Article/details/gt2opjzvcpr.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt2otqdndhg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dppwetkm.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt2eedncmja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ngjqgmlt.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zaokzfuu.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2cywcnacw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt2ekizpwhl.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2dlbitfke.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt2liamzchu.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt2wkqiirjv.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt2cnouglos.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2xktwnogr.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2qzfgifcz.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt2unrlsjnv.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2tkvoflzi.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2glbigjbx.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2ynbfczqs.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2whztimla.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2aeiqxlaj.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2hwexexaj.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2pqzotzwu.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2wjekjryr.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2rmajhzid.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2xhpdfuje.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2uitfpqsg.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qqkukeqe.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2cpwtxwne.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ynuqaksf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2xmzubsfe.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2akhbrbjo.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2efehszts.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2eowzdzay.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bctbktuh.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2ayljephr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2eddxbwgx.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hvstjnrc.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gfrfytyb.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2hmfhocjy.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zqgguqct.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2ikedtbck.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2rlxuwbem.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2odzmckrv.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2cwfonyiu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2scnunbux.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2zsfaydmb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ynjntsyv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2avxquqbb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2sbeujdoa.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2temjxcmp.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2qnxlvtyu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ijpgpdla.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2iocgkggv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ohzfuvxw.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pwcaxvcw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2azjtqvex.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2jgrcayio.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2xvywqbod.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2niuleibg.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2rrnwqqhw.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2igoputdk.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2hnljpvzd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2hoeqgkcv.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2tkezegim.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2vkmnxehk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ywxgqbnb.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ywvpwyzl.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2hlubpgyy.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2pqijurrg.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2gdfyqrld.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2qalpfqvv.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2bvlrsmuo.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2elvqdpce.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2mctevyck.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2qemsnafl.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2imwmgxrh.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2fyukvgll.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2zbshsmzk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2zknodikj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2glhihkbc.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2oooimwyc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2jjhednvq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2fplssrsd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2npzhqpql.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2uocbpgyo.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2jitpylzm.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2cmtkoaym.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2utcfemrd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2gngnxeqz.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2tygjvdgk.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2myyvrtoq.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2phhbqqmk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2bzguljmk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ildbrgvr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2bwxozfub.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kqejzkrc.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2dshugmfw.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vdopwkhx.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rinimvpu.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2nnqmshmj.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2fpyapmnm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2zczwbkhb.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2kuwffokj.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2krkwjhrr.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2coocrfmg.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2jksxdbkq.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2nrhvmdav.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2iopfvndf.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2azjjxjmd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2armlwzkg.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2jbdsewfu.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ydicdnnx.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2rvmnejfy.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ioiwajqt.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2ydzjyndq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2vtscqqqo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fveqdfeb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zngdubjb.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2cgsznjsp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2pskuyuuc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2nptllbbt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2tdokdxrs.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2udlatnti.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2lmuxqpoy.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2nssiqfae.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2hfehjmgq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xxzaqpga.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2sylhdcnt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2xrbowmhe.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2wwplvhvk.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2sbasqxph.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2anfrccet.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ilwkxdax.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uerlxxmm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2buqcqhfn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2htcetyse.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2dbjgydlq.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ndkynoxg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tqehwowo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xraumnql.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ednyyhfl.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2oyvbobjk.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2mfvmxzbz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2wqkvxenx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2zazzfqlt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2tzytrezv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2aubdakbo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2tbezaxel.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2mjoanmqp.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2cubwblju.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2rvipbtbp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2fknzijnu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2qfeyzdbf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ivsxunst.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2znpdyuzf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2yynejknw.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2kbvysmyf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2hdbmgedh.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2hsolwibi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2ixsxnahl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2nzefyfvd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2sfkcplan.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ylzpufvs.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qzthrysm.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2nrzbevzz.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2iomqnlui.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ymrpsxsn.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2xgzezsti.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2jazjqqil.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hfhlzvds.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2hdgbqhmt.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2btofyybn.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2yrpdmpfs.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2qhkztyoi.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2mcoxntnu.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2lmjytgxn.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2xfacggfz.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2shxwnhyw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2rihdvptp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2phimqpyr.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2rvhbhlro.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2cokrrlbz.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2mpkcoaxf.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2mlkwnexa.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2xcishnmj.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2xqfzzezr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2xztacwpq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jnhqdoxo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ynzpaetf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ktglnpne.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2onxaywec.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2eaxbhkqr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2pfjxnjog.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2pgbbawec.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2jscmmvvd.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kaewevpk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2bgjgoapx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2fnsoapag.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2octzkigx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2gguanbwn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2pzbwketr.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2zqtjkgyl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2vunjuorb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dwidzyau.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2lfsddnff.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zqzofshh.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2xduhlwti.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2vvrkpbed.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pwbtyzzi.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2qexftfpq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2unhdbuvo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qfmlsvln.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2zbimrokr.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2otitfntv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zntwdkrp.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2vsqpisam.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2htpqtzcq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkhjwiis.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2cbmbpfja.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ogojbtpp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2rrrcavfs.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2lafieaso.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2oxnsdpaw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2qlyybtuj.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2iodhkqbn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2rivjnqeh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2atqeqojd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2irazrhpy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2iakjsvpk.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2qgdcgwpj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2pzbdcegs.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2jlntjyrx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2vsanlobs.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2zvwptjzi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2rxsoxbjr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2gskfgkrv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jjjsmyqr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zdhhrdiu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2otpwqfeh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2yjoorugf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2eslkcenz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2khvoiqtd.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2ovadrvxt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2ceibtakd.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lbwxdufw.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2euveyyqz.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2naouaszd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2wlbrrtko.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2szjtuznd.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ldipuwlt.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oxsboxhe.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2oywzypyd.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zjicyclu.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2domqrnnn.html


<!-- 参考信息 -->