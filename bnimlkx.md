代发 wailian999

Java: new ArrayList<>(list);
来源：http://3g.fehbvm.com/Article/details/gkfogknxn.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://baike.zdbjq.cn/Article/details/gyyhaomtz.sHtML

Ruby: arr.dup;  arr.clone
来源：http://mobile.fehbvm.com/Article/details/glojhmjaf.sHtML

C#:   new List<int>(list);
来源：http://www.share.hesvh.cn/Article/details/gcpraarzr.sHtML

[D23] reduce 累积计算
来源：http://m.share.fehbvm.com/Article/details/gulaqmwdi.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://3g.fehbvm.com/Article/details/gnkyzrove.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://3g.hesvh.cn/Article/details/gbdokklqy.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://baike.fehbvm.com/Article/details/gejxvqvgo.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://3g.zdbjq.cn/Article/details/grxitvpqf.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://mobile.zdbjq.cn/Article/details/geqnoombt.sHtML

Go:   // 手写循环
来源：http://www.share.hesvh.cn/Article/details/gwxebbcdb.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://mobile.hesvh.cn/Article/details/gaciaibkd.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://read.share.hesvh.cn/Article/details/gmklnijbl.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.share.fehbvm.com/Article/details/gpuwsidgn.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://mobile.zdbjq.cn/Article/details/giozlpvae.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.zdbjq.cn/Article/details/gsotcgago.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://blog.hesvh.cn/Article/details/gxzuiqvaq.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://read.share.fehbvm.com/Article/details/gzdixiptr.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.hesvh.cn/Article/details/gjvwiremp.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://www.m.share.zdbjq.cn/Article/details/grklkfqrg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://wap.fehbvm.com/Article/details/gvwtaaxnh.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://wap.hesvh.cn/Article/details/gocrwbvwn.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/gxsajouzl.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://blog.fehbvm.com/Article/details/gyoparvxd.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://www.m.share.hesvh.cn/Article/details/gwjjdrsff.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.fehbvm.com/Article/details/gelfrrcte.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.blog.zdbjq.cn/Article/details/gzsxfrdry.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gwwlnucby.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://www.share.fehbvm.com/Article/details/gnhxaeqff.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://read.share.zdbjq.cn/Article/details/gmhbmcrix.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.blog.hesvh.cn/Article/details/gocjcysan.sHtML

[D26] 数组转字符串
来源：http://baike.fehbvm.com/Article/details/gctezvkyz.sHtML

Py:   ", ".join(map(str, arr))
来源：http://m.share.hesvh.cn/Article/details/gjmrrzzji.sHtML

PHP:  implode(", ", $arr);
来源：http://www.m.share.fehbvm.com/Article/details/gsqiamsmu.sHtML

JS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gxbglpvxb.sHtML

TS:   arr.join(", ")
来源：http://mobile.hesvh.cn/Article/details/gdvdifpwj.sHtML

Java: String.join(", ", list)
来源：http://www.share.hesvh.cn/Article/details/gboavnfao.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.fehbvm.com/Article/details/ganzlpblc.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/grhkxlsly.sHtML

C#:   string.Join(", ", list)
来源：http://3g.fehbvm.com/Article/details/gmtotirrp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwzietecc.sHtML

E. 字符串处理
来源：http://wap.fehbvm.com/Article/details/ggnmxnjwz.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gxviwcyqh.sHtML

[E01] 拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gocqlqwuu.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.m.share.fehbvm.com/Article/details/govkyjjnf.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.hesvh.cn/Article/details/gnsfniqup.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.m.share.fehbvm.com/Article/details/ghekvhsrw.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gmgfsjynu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://read.share.hesvh.cn/Article/details/gzavqmpwb.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://wap.fehbvm.com/Article/details/gehjbklkr.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://wap.zdbjq.cn/Article/details/gtseakatf.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gfswextzi.sHtML

[E02] 重复字符串
来源：http://m.share.fehbvm.com/Article/details/ggjjrhgio.sHtML

Py:   "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/gxsugiumg.sHtML

PHP:  str_repeat("ab", 3);
来源：http://m.share.hesvh.cn/Article/details/gbdsxofju.sHtML

JS:   "ab".repeat(3)
来源：http://read.share.hesvh.cn/Article/details/ghqxiauik.sHtML

TS:   "ab".repeat(3)
来源：http://wap.fehbvm.com/Article/details/gnlicdyib.sHtML

Java: "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gzxggdflf.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.fehbvm.com/Article/details/glbqiabtp.sHtML

Ruby: "ab" * 3
来源：http://www.blog.hesvh.cn/Article/details/gxefijvba.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://mobile.zdbjq.cn/Article/details/gvgjphcls.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/gypcgrhrw.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.share.hesvh.cn/Article/details/glvbnbcab.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.share.hesvh.cn/Article/details/gmjmilinj.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/geqhxeqmi.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gukivftar.sHtML

Java: s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gbgfomube.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://wap.zdbjq.cn/Article/details/ggtiadvoe.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://wap.zdbjq.cn/Article/details/gxxuxdqlb.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.hesvh.cn/Article/details/ghkcocgqd.sHtML

[E04] 查找子串位置
来源：http://www.blog.zdbjq.cn/Article/details/ggfeypqhb.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.zdbjq.cn/Article/details/gsuvcjtfs.sHtML

PHP:  strpos($s, "x");
来源：http://baike.fehbvm.com/Article/details/gpqfpxwqj.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://wap.fehbvm.com/Article/details/gxdfhtbfq.sHtML

TS:   s.indexOf("x")
来源：http://read.share.zdbjq.cn/Article/details/gpjedbcof.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gjcopalwt.sHtML

Go:   strings.Index(s, "x")
来源：http://www.m.share.zdbjq.cn/Article/details/grpqwgcfl.sHtML

Ruby: s.index("x")
来源：http://mobile.fehbvm.com/Article/details/gsuazhfmi.sHtML

C#:   s.IndexOf("x")
来源：http://m.share.zdbjq.cn/Article/details/gzbrinhtz.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.fehbvm.com/Article/details/gxnifqoth.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.fehbvm.com/Article/details/gpszzoacu.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://read.share.fehbvm.com/Article/details/gmxndphhz.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.fehbvm.com/Article/details/ghrfvclsa.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://read.share.fehbvm.com/Article/details/getxmecda.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.zdbjq.cn/Article/details/gxnadkhxn.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.share.hesvh.cn/Article/details/gzcglfods.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://wap.zdbjq.cn/Article/details/gkzaxeenu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://baike.hesvh.cn/Article/details/gcepuanqu.sHtML

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/gpqbnjlws.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.zdbjq.cn/Article/details/gwgjkagtb.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.zdbjq.cn/Article/details/gbdsmbhlq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gymbgtvou.sHtML

TS:   s.replaceAll("a", "b")
来源：http://3g.hesvh.cn/Article/details/gyizdgbru.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gjamolpmf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gkddrctnm.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/ghyfgsfll.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/gksaqzklr.sHtML

[E07] 按分隔符拆分
来源：http://read.share.hesvh.cn/Article/details/gcqyyoenj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.hesvh.cn/Article/details/gzpgptrye.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.fehbvm.com/Article/details/gucaqtnbw.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gmixwumpv.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/gbjuzlcqu.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.hesvh.cn/Article/details/gajsfwhiz.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gbnaoykbj.sHtML

Ruby: s.split(",");  s.split
来源：http://m.share.fehbvm.com/Article/details/gdcqpejga.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fehbvm.com/Article/details/gizbreyjx.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.zdbjq.cn/Article/details/gtucfekuq.sHtML

Py:   ",".join(items)
来源：http://m.share.zdbjq.cn/Article/details/gftxdtysh.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.fehbvm.com/Article/details/guhnyscmp.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gtaxfuuvw.sHtML

TS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/ggyftveip.sHtML

Java: String.join(",", items)
来源：http://mobile.zdbjq.cn/Article/details/gelttrdpw.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.hesvh.cn/Article/details/gvqkncxik.sHtML

Ruby: items.join(",")
来源：http://mobile.zdbjq.cn/Article/details/gzxvvqejs.sHtML

C#:   string.Join(",", items)
来源：http://m.share.hesvh.cn/Article/details/grpzjslnz.sHtML

[E09] 去除所有空白字符
来源：http://baike.fehbvm.com/Article/details/grjisgqyo.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.fehbvm.com/Article/details/gewbmscpa.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.zdbjq.cn/Article/details/gehjtttcd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://m.share.hesvh.cn/Article/details/gayicjcjx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.hesvh.cn/Article/details/guykklpkk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gshchvlqe.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.blog.hesvh.cn/Article/details/gzlrspmea.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fehbvm.com/Article/details/gkwavduir.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.zdbjq.cn/Article/details/gjkkqizuo.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.hesvh.cn/Article/details/gbrlaojav.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://m.share.hesvh.cn/Article/details/gcsebhrzk.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fehbvm.com/Article/details/gjqvyokxy.sHtML

JS:   "7".padStart(3, "0")
来源：http://mobile.hesvh.cn/Article/details/gkypjplph.sHtML

TS:   "7".padStart(3, "0")
来源：http://m.share.hesvh.cn/Article/details/geecnoecn.sHtML

Java: String.format("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gtvjrpkxq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://mobile.fehbvm.com/Article/details/gnreaqysz.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gzirqqaue.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://read.share.zdbjq.cn/Article/details/gbntktobw.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gpikbvrwf.sHtML

Py:   s[::-1]
来源：http://www.blog.zdbjq.cn/Article/details/gqoffrvmq.sHtML

PHP:  strrev($s);
来源：http://www.share.hesvh.cn/Article/details/gjhsengio.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.zdbjq.cn/Article/details/gdjwefxrm.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gwassiqgz.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fehbvm.com/Article/details/gajeoyouq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gsurftuis.sHtML

Ruby: s.reverse
来源：http://www.share.fehbvm.com/Article/details/grxdzeytq.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.hesvh.cn/Article/details/gkcbrefjh.sHtML

[E12] 统计某字符出现次数
来源：http://blog.hesvh.cn/Article/details/gpdctbmfa.sHtML

Py:   s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gemrlwiwx.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.hesvh.cn/Article/details/gobpbezpx.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/gkejoflmx.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gvkxvtysg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://wap.zdbjq.cn/Article/details/gxacwwrle.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fehbvm.com/Article/details/gcayyfqxk.sHtML

Ruby: s.count("a")
来源：http://www.share.fehbvm.com/Article/details/gcdgounwr.sHtML

C#:   s.Count(c => c == 'a')
来源：http://m.share.fehbvm.com/Article/details/gltvuxaim.sHtML

[E13] 逐字符遍历
来源：http://blog.hesvh.cn/Article/details/ggfqxodfc.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.hesvh.cn/Article/details/gcibhmfca.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.fehbvm.com/Article/details/gwfalxbyx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fehbvm.com/Article/details/gdnafannt.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gdkintcqg.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://mobile.hesvh.cn/Article/details/gmuijyber.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.zdbjq.cn/Article/details/gnbkcmzpg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.zdbjq.cn/Article/details/grdlhmvwh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gjuyxhhzj.sHtML

[E14] URL 编码与 Base64
来源：http://wap.zdbjq.cn/Article/details/grevrodfl.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.zdbjq.cn/Article/details/gjuxgvyww.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fehbvm.com/Article/details/ghznbpbqr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.hesvh.cn/Article/details/ggllkuhqm.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fehbvm.com/Article/details/gaqiiygil.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.hesvh.cn/Article/details/ggbfjojly.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://read.share.zdbjq.cn/Article/details/gmztagdwc.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.hesvh.cn/Article/details/gqlhrjikf.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.m.share.hesvh.cn/Article/details/glcpucoeh.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.fehbvm.com/Article/details/grtyxdeue.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.zdbjq.cn/Article/details/gezjgqlyv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fehbvm.com/Article/details/gshptzfms.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://blog.zdbjq.cn/Article/details/gryxatdjv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://m.share.hesvh.cn/Article/details/gdmuotpfc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fehbvm.com/Article/details/gkiwxsnmn.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://3g.zdbjq.cn/Article/details/gsavqtctn.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/gfqwevygb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.zdbjq.cn/Article/details/goqehssac.sHtML

[E16] 数字千分位
来源：http://wap.fehbvm.com/Article/details/gfofnrxvc.sHtML

Py:   f"{1234567:,}"
来源：http://www.blog.zdbjq.cn/Article/details/gbllmvmmo.sHtML

PHP:  number_format(1234567);
来源：http://m.share.hesvh.cn/Article/details/gjvxwjrke.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/guumtlwba.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/gqgkouufr.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.hesvh.cn/Article/details/gdvzminda.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.zdbjq.cn/Article/details/gxycdvzxi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://wap.fehbvm.com/Article/details/gytofwlmh.sHtML

C#:   1234567.ToString("N0")
来源：http://mobile.zdbjq.cn/Article/details/gcbkonkpp.sHtML

[E17] 首字母大写
来源：http://www.share.zdbjq.cn/Article/details/gnzniivze.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.zdbjq.cn/Article/details/gmamgqrzp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://wap.zdbjq.cn/Article/details/gsnqhtxft.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.hesvh.cn/Article/details/gxqdjhdyq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gazjwgutx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.zdbjq.cn/Article/details/gmvvoupiz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://m.share.zdbjq.cn/Article/details/gsveohayb.sHtML

Ruby: s.capitalize
来源：http://m.share.hesvh.cn/Article/details/gpdbaqpou.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://3g.zdbjq.cn/Article/details/gogponqrk.sHtML

[E18] 模板占位符替换
来源：http://mobile.hesvh.cn/Article/details/gajxqxtju.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.zdbjq.cn/Article/details/gcihtpoll.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.hesvh.cn/Article/details/gmotpupds.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/grzvybygk.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.hesvh.cn/Article/details/ghwzrslrw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gpgxbcqac.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gflhwwaqy.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.hesvh.cn/Article/details/gwskhiwvh.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://mobile.hesvh.cn/Article/details/gwimhkpqo.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fehbvm.com/Article/details/gaibcpzhr.sHtML

Py:   s.splitlines()
来源：http://baike.hesvh.cn/Article/details/gfwiqnboh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://m.share.hesvh.cn/Article/details/ggaxqwtjp.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/govawlfyb.sHtML

TS:   s.split(/\r?\n/)
来源：http://blog.zdbjq.cn/Article/details/gnqscdabg.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gcgdwtyww.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.zdbjq.cn/Article/details/gytoynvdu.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/gyfgigeqk.sHtML

C#:   s.Split('\n')
来源：http://www.blog.zdbjq.cn/Article/details/gwnzpdytf.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.hesvh.cn/Article/details/ghkbjgmtj.sHtML

Py:   if not s:
来源：http://blog.fehbvm.com/Article/details/gklurkaie.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fehbvm.com/Article/details/gxrmahzyi.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.hesvh.cn/Article/details/gtpjznrtf.sHtML

TS:   if (s === "") {}
来源：http://www.share.hesvh.cn/Article/details/gixdsvhqw.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.fehbvm.com/Article/details/gwllxxmod.sHtML

Go:   if s == "" {}
来源：http://3g.zdbjq.cn/Article/details/gkempsenm.sHtML

Ruby: if s.empty?
来源：http://www.m.share.zdbjq.cn/Article/details/grhvcbsjm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.zdbjq.cn/Article/details/gqwflbvlp.sHtML

[E21] 超长截断加省略号
来源：http://www.share.fehbvm.com/Article/details/gwdwuqeky.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.hesvh.cn/Article/details/gbjozkrmr.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/gvyacbtio.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/glnvkevpz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gyahwxtwn.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/ghdejljct.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/gloiebopr.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gamdoehak.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fehbvm.com/Article/details/ggsfdlslc.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fehbvm.com/Article/details/grgpbrmce.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.zdbjq.cn/Article/details/gwtxlbyuv.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.zdbjq.cn/Article/details/ghvfasiud.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/giokienkf.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.fehbvm.com/Article/details/gtkubejdn.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://read.share.zdbjq.cn/Article/details/gkuojvkix.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fehbvm.com/Article/details/gquyxotpp.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gcrmgjsdo.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gtmepxtau.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gucbfnghi.sHtML

F. 文件与目录
来源：http://mobile.zdbjq.cn/Article/details/gochyzujp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gwyxxiaxt.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gdzbdzcem.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fehbvm.com/Article/details/gmgkaqrwv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.zdbjq.cn/Article/details/garsmjcoz.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.fehbvm.com/Article/details/grekhkeze.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gefirogna.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.fehbvm.com/Article/details/gbfpqpjnm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://baike.zdbjq.cn/Article/details/gmsnpkxvy.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gyijnuqza.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.hesvh.cn/Article/details/gsnnafynm.sHtML

[F02] 逐行读取文件
来源：http://baike.hesvh.cn/Article/details/ghrnzmpnj.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.zdbjq.cn/Article/details/gvxzqgfft.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.zdbjq.cn/Article/details/gjgjntgeh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gymlpimxp.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://3g.fehbvm.com/Article/details/geoabrznj.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://mobile.zdbjq.cn/Article/details/ggvdkbbyh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.zdbjq.cn/Article/details/gnqmzpsvz.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fehbvm.com/Article/details/gsmistrur.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.zdbjq.cn/Article/details/gxytsxeqt.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.fehbvm.com/Article/details/gmzmfmjuw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.hesvh.cn/Article/details/grhnmkmou.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gnamekbyk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gxhmupocr.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.fehbvm.com/Article/details/goxupvomw.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.hesvh.cn/Article/details/gvogoisfk.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.fehbvm.com/Article/details/grtmtowrs.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/gsodgpdbt.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.hesvh.cn/Article/details/gjyoftzhs.sHtML

[F04] 追加写入文件
来源：http://m.share.hesvh.cn/Article/details/gnvevsjki.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.hesvh.cn/Article/details/gsrhqqsdo.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.hesvh.cn/Article/details/givlqiwsg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gyokxvzdl.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.fehbvm.com/Article/details/gdzjynxzq.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://blog.fehbvm.com/Article/details/gpidkbkqr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://read.share.hesvh.cn/Article/details/geobneklr.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/gzrzvjtup.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.zdbjq.cn/Article/details/gupozbdbx.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gfeevmhnl.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/geepurgkb.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.fehbvm.com/Article/details/gmpfkgjxj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gkuxxenxw.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gmwfymjpb.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gvnszvxms.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.zdbjq.cn/Article/details/gbdevyybo.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.fehbvm.com/Article/details/gkknxwbih.sHtML

C#:   File.Exists("a.txt")
来源：http://3g.hesvh.cn/Article/details/gxjroprct.sHtML

[F06] 删除文件
来源：http://blog.fehbvm.com/Article/details/gvkupcxvg.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/galsklmmq.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/gcimztqev.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gwclfpoyn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/ggbjbavqm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gihemddye.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gllftzbps.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gadmbewpg.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.hesvh.cn/Article/details/gscurdpfx.sHtML

[F07] 创建目录（含多级）
来源：http://3g.zdbjq.cn/Article/details/gzmalqadg.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gauiwvelj.sHtML


<!-- 参考信息 -->