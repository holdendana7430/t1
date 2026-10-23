代发 wailian999

Py:   arr.copy();  arr[:];  list(arr)
来源：http://www.52xcode.cn/Article/details/gt3chonjjzm.html

PHP:  $copy = $arr;        // 数组是值类型，赋值即复制
来源：http://www.52xcode.cn/Article/details/gt3eftkbxpf.html

JS:   [...arr];  arr.slice();  structuredClone(arr)
来源：http://www.ydjk.org.cn/Article/details/gt3axkuzmjv.html

TS:   [...arr];
来源：http://www.ydjk.org.cn/Article/details/gt3czuydsxd.html

Java: new ArrayList<>(list);
来源：http://www.52xcode.cn/Article/details/gt3ahbijara.html

Go:   copied := append([]int(nil), arr...)
来源：http://www.52xcode.cn/Article/details/gt3eilcbwwa.html

Ruby: arr.dup;  arr.clone
来源：http://www.ydjk.org.cn/Article/details/gt3svkpchup.html

C#:   new List<int>(list);
来源：http://www.ydjk.org.cn/Article/details/gt3rbhwwnhk.html

[D23] reduce 累积计算
来源：http://www.52xcode.cn/Article/details/gt3ygbqkadd.html

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://www.52xcode.cn/Article/details/gt3tlzjiuch.html

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.52xcode.cn/Article/details/gt3osdxbjrv.html

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3evtxchdu.html

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://www.ydjk.org.cn/Article/details/gt3mpiwljmj.html

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.ydjk.org.cn/Article/details/gt3dgeqyqni.html

Go:   // 手写循环
来源：http://www.ydjk.org.cn/Article/details/gt3oppbgfau.html

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.52xcode.cn/Article/details/gt3aibxwyld.html

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.52xcode.cn/Article/details/gt3lvaenjpl.html

[D24] 字典 / Map 基本操作
来源：http://www.ydjk.org.cn/Article/details/gt3hqqbxpgu.html

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.ydjk.org.cn/Article/details/gt3ehpnyrci.html

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://www.ydjk.org.cn/Article/details/gt3gzzobxem.html

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://www.52xcode.cn/Article/details/gt3pdxdzaga.html

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3hhtsvvck.html

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.52xcode.cn/Article/details/gt3lhsalhlf.html

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.52xcode.cn/Article/details/gt3rvrqfagv.html

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.ydjk.org.cn/Article/details/gt3lreywbvk.html

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.ydjk.org.cn/Article/details/gt3ntmhoopt.html

[D25] Set 集合去重与交并差
来源：http://www.ydjk.org.cn/Article/details/gt3bnbledwd.html

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.52xcode.cn/Article/details/gt3yuwjsuqy.html

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.52xcode.cn/Article/details/gt3pkqngsll.html

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.52xcode.cn/Article/details/gt3lddifacs.html

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.ydjk.org.cn/Article/details/gt3eheaksxi.html

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xdqujcff.html

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.52xcode.cn/Article/details/gt3mjwatsuv.html

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.52xcode.cn/Article/details/gt3nmywpdex.html

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.ydjk.org.cn/Article/details/gt3pdactooq.html

[D26] 数组转字符串
来源：http://www.52xcode.cn/Article/details/gt3vjudvufa.html

Py:   ", ".join(map(str, arr))
来源：http://www.ydjk.org.cn/Article/details/gt3mfhrrunm.html

PHP:  implode(", ", $arr);
来源：http://www.ydjk.org.cn/Article/details/gt3fcxvnaur.html

JS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3vnjsuafd.html

TS:   arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3etaabwrn.html

Java: String.join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3meicondj.html

Go:   strings.Join(strs, ", ")
来源：http://www.52xcode.cn/Article/details/gt3oszwsewq.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3lbtciqvp.html

C#:   string.Join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3wxibcims.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aidzpfnh.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3txinovtb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mpitentz.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zjtiswkq.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3xhdwznwp.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3zceqpdme.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uxawighm.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3quztyjgs.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3atkyupyn.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.52xcode.cn/Article/details/gt3fqtotqki.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3zadlrlun.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tjzvrqtm.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3bufclieu.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3djudelmq.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3kfprvdmi.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3rozlljft.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3usqvmaqy.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3dczjrelc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rywffjwt.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3mntubnug.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ysuipdol.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3fckbvxrw.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3bbdmstiq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3flihdtpf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3riadcpke.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3wxfkwtay.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3fpmosqgn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3worpspsv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3sarsydsh.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jjldrqoo.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3gqdjvfzg.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ieumkdsw.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3lawtwfzp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3jdlvqflr.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fgwqmgal.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xbqtelvd.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3mmipgeio.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3qdptbfil.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3beyveqsi.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3rjvogxcz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3toskqova.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3yryrweun.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bskhepqp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3mdhbbmpx.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3bebsorzm.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3dljltjag.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3bhfpkfjq.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3imxyizet.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3lzgbfsss.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3bblulrpc.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3yuphqseg.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xveuxntj.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jyrgtuwg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ckustyjw.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3udmwtcum.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rekaixtr.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3tjmjjhft.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3tmenhzpn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3gkwhfynt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3qggdhazx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3zbefbzwy.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3duxgnuka.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3eponoqev.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3myylndnb.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3lrunsurl.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3yxxpiguf.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3irswbpci.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3xyftqzit.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3tkkqdlgm.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3vsuyjkhj.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3rvnqkfkg.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3zohvdwes.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3rsiejipf.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ltpglkrd.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3hljghcjb.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3qjeologd.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3ncrgttnb.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xiyuxkbd.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3kqhwyvof.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3lntjzfux.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3cfyhyqnf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3zgwedugb.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3zxynkhcp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3fmknybrp.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3szuebsax.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3cbzflaaz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3pnwotrrt.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3rbobydsz.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3xlvjyede.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3vhuoiutz.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3otbgzhed.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xqeytzfh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ksdyshvg.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3oxdxnlyj.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3tsxnurqz.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3foqzfdoy.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3jbivwqdw.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ynzboafq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rlivfgul.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3bsjwhgqx.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3cbadlgrs.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3adsyreei.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3dkdvtglv.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3cwbpsuda.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3cqmypcvr.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3yvrlqdvl.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3lgpdsyvg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3jkvdyzcv.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3cdwskuhq.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gczpdzje.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3hjewvfli.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3ljspmvac.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3rcgzpjir.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3dlwfagqf.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3izwlqqej.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3csyxfetw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3wouzjdsy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3crhtjljx.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3zctvxljl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qujogcdq.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3ehulljpb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3tldmrwuq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cohnvvrz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3cdnqknhd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mrhywwtc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3psjzowes.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3uikehnfm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3xsuucgoh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3khaotcez.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3gleijvjo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3suegkpjo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3iaakxxud.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mrklgzxe.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3fensuwpz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3nwmrdwad.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3knffcafw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3szctzccy.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jscxkntd.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3jxcynbrx.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3xgywnzmt.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3kpdzvncc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3dzjzunfi.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3rdyszhml.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3sacauipc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3oubfzown.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3guzjqxof.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3vymhpdyx.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3pbgvzver.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3kuapvulo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3mhbkxqvn.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3agxdqtup.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3hshukgcu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3yaydtzxr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3cajoobgd.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3tlqldewz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3izhtywbc.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3wcmsaopi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3mzyshiyq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3tcefvtnj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qlrskfbi.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3woxdeywn.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mpvnzfrg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3rurnlxzy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3dqmlmnoi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3kixgwkhq.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3nzdyvmdy.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3duososeb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3cbrsmhrd.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3qphazkfp.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3dtwgmgkk.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3ejxrhwxm.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3gkgqvjid.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3ruediocf.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3efirsvel.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3wiatilwx.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3bieciqbh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3nrenejjh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3zfzqzicx.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3netbbazy.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3dszlwvyl.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3cyemgaaw.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3nnhgsaad.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3louuvruc.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3qhxnubfq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3deytpsqm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3lrqrvosl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xhkavjqm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hkxutmqk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bqvoppyd.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3zbeuhdtj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3qhxiivmh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3wvmhenaf.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3dksekvqr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3swajkspq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rxfzwybw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ihohpaxf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3iisjzplh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3fjhugshn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3yyepgpnn.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3uozhwocq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3hkpnwuie.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rkunfuvk.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3aggbhnxg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lykhrxke.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3sjaadxdu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3whwjfiwx.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3pyxoplkx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3dzopcupg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ihkwwckp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wffnjgmh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3ycnahzxt.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wrlmlbgh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zuozqkqk.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3nnwpgazw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3kpwzrygu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3dcnnpwvw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3wcfukjhz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cuzouugq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3cihotxqx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3lzxpuddw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3iagjzqrh.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3gxxiubpx.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3abvgmylk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3zcgyvufm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ugrroxpd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ycortoio.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3tkgghsvy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3macwweid.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3hyphcjzo.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3bxazqwld.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3azisfltx.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ebhuycjn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3hrfhconb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3uchmessy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zsoreyod.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3shjnmkhm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3ifkqwjyg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hjpnfqlc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3zacowsxf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3vkvjgzoi.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3eyjmnstd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3xqthdhoq.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ylkieenk.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qprgeqlp.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vxiyljza.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3dvrqlczv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3mxwhioep.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vnddjqsx.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uwdabouu.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3krjaqocn.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uwyorymw.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3wsvuaqly.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qtnrrtam.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wmqreuea.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wplmriwx.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xcmibhpa.html


<!-- 参考信息 -->