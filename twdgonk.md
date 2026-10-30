代发 wailian999

Java: new ArrayList<>(list);
来源：http://3g.hesvh.cn/Article/details/ghanshnls.sHtML

Go:   copied := append([]int(nil), arr...)
来源：http://blog.zdbjq.cn/Article/details/gkewiuwvn.sHtML

Ruby: arr.dup;  arr.clone
来源：http://3g.zdbjq.cn/Article/details/gkwyezgyk.sHtML

C#:   new List<int>(list);
来源：http://wap.fehbvm.com/Article/details/gicpuxuvw.sHtML

[D23] reduce 累积计算
来源：http://read.share.zdbjq.cn/Article/details/gnqdhrirb.sHtML

Py:   functools.reduce(lambda a, b: a + b, arr, 0)
来源：http://mobile.hesvh.cn/Article/details/gsfogvrhu.sHtML

PHP:  array_reduce($arr, fn($carry, $x) => $carry + $x, 0);
来源：http://www.m.share.fehbvm.com/Article/details/gjaggauaf.sHtML

JS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://blog.fehbvm.com/Article/details/ggfgnmbks.sHtML

TS:   arr.reduce((acc, x) => acc + x, 0)
来源：http://mobile.zdbjq.cn/Article/details/gutgitviw.sHtML

Java: list.stream().reduce(0, Integer::sum)
来源：http://www.blog.fehbvm.com/Article/details/gkmsyyorg.sHtML

Go:   // 手写循环
来源：http://www.blog.hesvh.cn/Article/details/gfpovrkrh.sHtML

Ruby: arr.reduce(0) { |acc, x| acc + x };  arr.sum
来源：http://www.blog.zdbjq.cn/Article/details/gfqiffgvj.sHtML

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://www.blog.zdbjq.cn/Article/details/gffxpmxdn.sHtML

[D24] 字典 / Map 基本操作
来源：http://m.share.fehbvm.com/Article/details/ghcuqqkwj.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://read.share.hesvh.cn/Article/details/gaqzmpspt.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://mobile.fehbvm.com/Article/details/gmpqmccxc.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://wap.fehbvm.com/Article/details/gdfarutfs.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://mobile.fehbvm.com/Article/details/gexpnbmqn.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://www.blog.zdbjq.cn/Article/details/gclkvoikn.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://read.share.fehbvm.com/Article/details/gkbgpksny.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.fehbvm.com/Article/details/gfkjraxed.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://blog.zdbjq.cn/Article/details/ghexipdlb.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/gkusarkch.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.fehbvm.com/Article/details/gxpioamcl.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://3g.hesvh.cn/Article/details/gxmxdnuqv.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/genjoxuzf.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://read.share.fehbvm.com/Article/details/gxhqbhrha.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gysakspvg.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.hesvh.cn/Article/details/gywtfuqvf.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://wap.hesvh.cn/Article/details/groizndnc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.share.fehbvm.com/Article/details/gxdbgspnd.sHtML

[D26] 数组转字符串
来源：http://www.blog.hesvh.cn/Article/details/gmshhgarl.sHtML

Py:   ", ".join(map(str, arr))
来源：http://read.share.fehbvm.com/Article/details/gdhonxjwq.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.fehbvm.com/Article/details/gluixqnyk.sHtML

JS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gjvtshbyu.sHtML

TS:   arr.join(", ")
来源：http://www.blog.zdbjq.cn/Article/details/gljdrlakr.sHtML

Java: String.join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/goepqqxax.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.hesvh.cn/Article/details/ghvzvbwfh.sHtML

Ruby: arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gsgqofjtx.sHtML

C#:   string.Join(", ", list)
来源：http://wap.fehbvm.com/Article/details/goadbfwlp.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/giydxomcy.sHtML

E. 字符串处理
来源：http://3g.fehbvm.com/Article/details/ggwylgihr.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gvqspbxyw.sHtML

[E01] 拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gmvsuxpjy.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.blog.fehbvm.com/Article/details/gzpquywhj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://wap.hesvh.cn/Article/details/gpxzowzcp.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.fehbvm.com/Article/details/glksbslsr.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://m.share.hesvh.cn/Article/details/gyyertcvo.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fehbvm.com/Article/details/gccvzixmt.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.blog.hesvh.cn/Article/details/gesrfghrg.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.m.share.hesvh.cn/Article/details/ghrsbyzkl.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gwxuedohh.sHtML

[E02] 重复字符串
来源：http://blog.fehbvm.com/Article/details/gkhfecxrw.sHtML

Py:   "ab" * 3
来源：http://read.share.hesvh.cn/Article/details/gxlubuglf.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.zdbjq.cn/Article/details/glmipdqgx.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.hesvh.cn/Article/details/gdrdoprad.sHtML

TS:   "ab".repeat(3)
来源：http://mobile.hesvh.cn/Article/details/gmjriecjf.sHtML

Java: "ab".repeat(3)
来源：http://www.share.hesvh.cn/Article/details/goghwnikm.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://read.share.hesvh.cn/Article/details/gtimetyaf.sHtML

Ruby: "ab" * 3
来源：http://blog.hesvh.cn/Article/details/gorffnlni.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.zdbjq.cn/Article/details/gqvrxueny.sHtML

[E03] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gnqfeimye.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.m.share.hesvh.cn/Article/details/gvdjzvgev.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://read.share.fehbvm.com/Article/details/ghoagkyoe.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://mobile.hesvh.cn/Article/details/garbbtcox.sHtML

TS:   s.slice(1, 4)
来源：http://baike.fehbvm.com/Article/details/gxtseavtt.sHtML

Java: s.substring(1, 4)
来源：http://baike.fehbvm.com/Article/details/glqbxfrey.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://mobile.hesvh.cn/Article/details/gyexuscbq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://mobile.fehbvm.com/Article/details/gtskqfyqq.sHtML

C#:   s.Substring(1, 3)
来源：http://www.blog.zdbjq.cn/Article/details/givqsrita.sHtML

[E04] 查找子串位置
来源：http://read.share.zdbjq.cn/Article/details/gxohahtdk.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.fehbvm.com/Article/details/glqtivstk.sHtML

PHP:  strpos($s, "x");
来源：http://www.share.fehbvm.com/Article/details/gcszoxlln.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.hesvh.cn/Article/details/gvwxflnjr.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gxokkrukc.sHtML

Java: s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gihtaiuzz.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.fehbvm.com/Article/details/gqwctjffq.sHtML

Ruby: s.index("x")
来源：http://3g.hesvh.cn/Article/details/ghxpnhmfj.sHtML

C#:   s.IndexOf("x")
来源：http://blog.fehbvm.com/Article/details/gbsbzbmgd.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://wap.fehbvm.com/Article/details/gcjwspxkt.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.zdbjq.cn/Article/details/gvhjtssas.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.share.hesvh.cn/Article/details/gfobfpqex.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.m.share.fehbvm.com/Article/details/gbiglvnbj.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.zdbjq.cn/Article/details/gzqshtjti.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gurfwegid.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://wap.zdbjq.cn/Article/details/ghzxwbmjf.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fehbvm.com/Article/details/girndlvhu.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.zdbjq.cn/Article/details/ghlzavmnd.sHtML

[E06] 替换子串
来源：http://blog.hesvh.cn/Article/details/gpkotfpju.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gczaznbox.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.hesvh.cn/Article/details/gtgpdhxim.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/grkqmbrka.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gbzntphwy.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gbkqqduyf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.zdbjq.cn/Article/details/gzlibpwas.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.fehbvm.com/Article/details/gxwnjomrq.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gfaobijzm.sHtML

[E07] 按分隔符拆分
来源：http://baike.zdbjq.cn/Article/details/gppauepfr.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.fehbvm.com/Article/details/gigiugpsb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.share.fehbvm.com/Article/details/ghdknhqap.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.zdbjq.cn/Article/details/gnfodkgos.sHtML

TS:   s.split(",")
来源：http://baike.zdbjq.cn/Article/details/gfswcerpx.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.zdbjq.cn/Article/details/gxhcsjkef.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fehbvm.com/Article/details/gwgeqoeje.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.hesvh.cn/Article/details/gdfibhbhu.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.zdbjq.cn/Article/details/gqcuyfmqa.sHtML

[E08] 数组按分隔符合并
来源：http://mobile.hesvh.cn/Article/details/gyqgxhltp.sHtML

Py:   ",".join(items)
来源：http://read.share.fehbvm.com/Article/details/gwchdxpom.sHtML

PHP:  implode(",", $items);
来源：http://www.blog.zdbjq.cn/Article/details/gliyvkbue.sHtML

JS:   items.join(",")
来源：http://www.blog.fehbvm.com/Article/details/gckrhcvlf.sHtML

TS:   items.join(",")
来源：http://baike.zdbjq.cn/Article/details/giakrtzrc.sHtML

Java: String.join(",", items)
来源：http://wap.zdbjq.cn/Article/details/ggvtsfwse.sHtML

Go:   strings.Join(items, ",")
来源：http://blog.zdbjq.cn/Article/details/gbmjmicbf.sHtML

Ruby: items.join(",")
来源：http://3g.hesvh.cn/Article/details/gzmryhiup.sHtML

C#:   string.Join(",", items)
来源：http://3g.hesvh.cn/Article/details/gsytamvve.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.fehbvm.com/Article/details/gakgpezaa.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.hesvh.cn/Article/details/gtgnducxr.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.zdbjq.cn/Article/details/grktxhncl.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gaviyhdsn.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fehbvm.com/Article/details/gmhwtfpmk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.blog.zdbjq.cn/Article/details/gsjreheqw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.zdbjq.cn/Article/details/ggzukyqli.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.zdbjq.cn/Article/details/gdftzxrqy.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.hesvh.cn/Article/details/gpasryujr.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.hesvh.cn/Article/details/gyuspzhex.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.fehbvm.com/Article/details/gtoivehbv.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.zdbjq.cn/Article/details/gdcmrfabh.sHtML

JS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gvxbregvi.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/ghztobfxg.sHtML

Java: String.format("%03d", 7)
来源：http://wap.hesvh.cn/Article/details/gbxowtczi.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gxfryubtr.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.fehbvm.com/Article/details/gmdcfctjn.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/gnabxferk.sHtML

[E11] 反转字符串
来源：http://baike.fehbvm.com/Article/details/gnoehxejm.sHtML

Py:   s[::-1]
来源：http://blog.zdbjq.cn/Article/details/gmcyeqfcx.sHtML

PHP:  strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gdkxzvqas.sHtML

JS:   [...s].reverse().join("")
来源：http://baike.fehbvm.com/Article/details/giolimdwa.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gjobqwmsk.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://read.share.zdbjq.cn/Article/details/ggclrbeqb.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.m.share.hesvh.cn/Article/details/gyhbdbncv.sHtML

Ruby: s.reverse
来源：http://www.share.zdbjq.cn/Article/details/ginmocrtm.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/guahsypde.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.hesvh.cn/Article/details/gqimiakgl.sHtML

Py:   s.count("a")
来源：http://3g.zdbjq.cn/Article/details/galkhmjvx.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.hesvh.cn/Article/details/gtneaqqvi.sHtML

JS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gebwvcawl.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/gymxfewse.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.hesvh.cn/Article/details/gkjplfpbf.sHtML

Go:   strings.Count(s, "a")
来源：http://m.share.hesvh.cn/Article/details/gmnvxnspx.sHtML

Ruby: s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gbqwtiyju.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.zdbjq.cn/Article/details/gujyiekwz.sHtML

[E13] 逐字符遍历
来源：http://m.share.zdbjq.cn/Article/details/glmhsvznq.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.fehbvm.com/Article/details/gatucwaik.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.zdbjq.cn/Article/details/gczkbeddf.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://mobile.hesvh.cn/Article/details/gnrqknrla.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/glzxnipdy.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gylriickj.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.hesvh.cn/Article/details/ghhygslih.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.hesvh.cn/Article/details/gzsspdfxh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gdkmplyam.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fehbvm.com/Article/details/gcxxbebbx.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fehbvm.com/Article/details/gqbitqoqm.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.hesvh.cn/Article/details/gfrnahvav.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.hesvh.cn/Article/details/gbdtxrrej.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/gsjeiycef.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://3g.hesvh.cn/Article/details/ggnwvrnzp.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.zdbjq.cn/Article/details/gcogmtprv.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.zdbjq.cn/Article/details/gssubfuxc.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.fehbvm.com/Article/details/goazteenp.sHtML

[E15] HTML 转义 / 反转义
来源：http://mobile.hesvh.cn/Article/details/gqyepvjwr.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.zdbjq.cn/Article/details/gtmmwonsq.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://mobile.zdbjq.cn/Article/details/grbdqaclz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://read.share.zdbjq.cn/Article/details/gsftxzxqe.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fehbvm.com/Article/details/gqjnvwicx.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.hesvh.cn/Article/details/ghmkaabaw.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.zdbjq.cn/Article/details/gjvwsturk.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.zdbjq.cn/Article/details/gzerfowte.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.hesvh.cn/Article/details/gidekirvq.sHtML

[E16] 数字千分位
来源：http://m.share.zdbjq.cn/Article/details/gyfugqwhh.sHtML

Py:   f"{1234567:,}"
来源：http://3g.hesvh.cn/Article/details/gyscwueax.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.zdbjq.cn/Article/details/gmsmxbnwx.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://blog.zdbjq.cn/Article/details/gmzdfmctb.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/gnjbiaobl.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.hesvh.cn/Article/details/gtjrazcrs.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.zdbjq.cn/Article/details/gisskwosx.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://mobile.zdbjq.cn/Article/details/gsapdrqjv.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.zdbjq.cn/Article/details/gbeozfmmu.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/gfvsngvkl.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.hesvh.cn/Article/details/guybdofxl.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.zdbjq.cn/Article/details/gajvqbbvi.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/gxmhxqcbr.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/geazonvyd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.zdbjq.cn/Article/details/gzvvlfepd.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.zdbjq.cn/Article/details/ghefkhkpz.sHtML

Ruby: s.capitalize
来源：http://m.share.zdbjq.cn/Article/details/gotqzposo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://baike.hesvh.cn/Article/details/gwkfxsiwd.sHtML

[E18] 模板占位符替换
来源：http://baike.fehbvm.com/Article/details/gijgvmekc.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.zdbjq.cn/Article/details/gstgntwrf.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://3g.fehbvm.com/Article/details/gsnnwiqgf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gcpnflojh.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gyrhjjwsf.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.fehbvm.com/Article/details/gfusfdgyi.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gilazjsbk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.zdbjq.cn/Article/details/gkfwitlvn.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.hesvh.cn/Article/details/gltbiupwc.sHtML

[E19] 多行文本按行拆分
来源：http://wap.hesvh.cn/Article/details/gvuhubkrd.sHtML

Py:   s.splitlines()
来源：http://read.share.fehbvm.com/Article/details/gpueqssbw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.hesvh.cn/Article/details/guilfxwfe.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fehbvm.com/Article/details/gbomifjqi.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/ghwvvtwmn.sHtML

Java: s.lines().toList()
来源：http://www.blog.zdbjq.cn/Article/details/gcwvazqnu.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.hesvh.cn/Article/details/gxcjefqdm.sHtML

Ruby: s.lines
来源：http://www.blog.zdbjq.cn/Article/details/gtdtaxwuv.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/gvdquobpm.sHtML

[E20] 判断字符串是否为空
来源：http://www.blog.hesvh.cn/Article/details/gsigqvfag.sHtML

Py:   if not s:
来源：http://baike.zdbjq.cn/Article/details/gqkosnwkr.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.zdbjq.cn/Article/details/gohjvmlxq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.share.fehbvm.com/Article/details/guvnfkvek.sHtML

TS:   if (s === "") {}
来源：http://www.blog.fehbvm.com/Article/details/gmnqbaaqh.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gcwmauicn.sHtML

Go:   if s == "" {}
来源：http://www.share.fehbvm.com/Article/details/gtgbndglu.sHtML

Ruby: if s.empty?
来源：http://baike.hesvh.cn/Article/details/guopdetjn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.hesvh.cn/Article/details/gcspapcxi.sHtML

[E21] 超长截断加省略号
来源：http://m.share.zdbjq.cn/Article/details/gjqfemfyx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.share.fehbvm.com/Article/details/ghkkmkvac.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gcvdizgcl.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gqpekgvkz.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gcweljvms.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gicguvkfw.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.fehbvm.com/Article/details/gvlasxhvh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gtucijlfu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.fehbvm.com/Article/details/gfecbctyu.sHtML

[E22] 字节长度与字符长度
来源：http://www.share.fehbvm.com/Article/details/gacrzavle.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.hesvh.cn/Article/details/gowylnhqd.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gnlsulrjh.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.zdbjq.cn/Article/details/gxurvfejm.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.hesvh.cn/Article/details/grunzlaju.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.hesvh.cn/Article/details/gorpmsvqq.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.share.fehbvm.com/Article/details/gdhlhrglm.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.hesvh.cn/Article/details/gzffqesyk.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.fehbvm.com/Article/details/gfhxjatjf.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gpxltwznr.sHtML

F. 文件与目录
来源：http://3g.zdbjq.cn/Article/details/gswndbsaz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gsewvdnno.sHtML

[F01] 读取整个文件
来源：http://www.share.hesvh.cn/Article/details/gltzspvcc.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.zdbjq.cn/Article/details/gslrylfsb.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.fehbvm.com/Article/details/gmflhwqng.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://baike.hesvh.cn/Article/details/gtlpefltf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://3g.fehbvm.com/Article/details/gxywlbqjf.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gxdwdbrzq.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://mobile.zdbjq.cn/Article/details/gtexjohms.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gyecqaoyy.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.hesvh.cn/Article/details/gzltltsjr.sHtML

[F02] 逐行读取文件
来源：http://baike.zdbjq.cn/Article/details/ghvikhxqv.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://blog.zdbjq.cn/Article/details/gdvmrpzze.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gutnjitat.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gqadhkppj.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.hesvh.cn/Article/details/gdvunfstd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://3g.hesvh.cn/Article/details/gkqfywfet.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fehbvm.com/Article/details/gedxftauv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.hesvh.cn/Article/details/gwqfahpia.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fehbvm.com/Article/details/gnfqrfgbr.sHtML

[F03] 写入文件（覆盖）
来源：http://mobile.fehbvm.com/Article/details/gqowuepvg.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fehbvm.com/Article/details/gltnkcwbi.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gnowixzfk.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.hesvh.cn/Article/details/ganstmhdp.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gispiotjv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.hesvh.cn/Article/details/gnrpqpkss.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.zdbjq.cn/Article/details/guesllaud.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.zdbjq.cn/Article/details/gistfzufe.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/gdzsnrbum.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/gukgtykho.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.zdbjq.cn/Article/details/gqeoehgrr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.zdbjq.cn/Article/details/gcugoxblz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.hesvh.cn/Article/details/gdhlckmhm.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gykcydgws.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.hesvh.cn/Article/details/gsqqjqguw.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.zdbjq.cn/Article/details/gzzxkdvcq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fehbvm.com/Article/details/gnsotetaq.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/ggycfijbn.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.zdbjq.cn/Article/details/globzwcdb.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://m.share.hesvh.cn/Article/details/gkkcennuy.sHtML

PHP:  file_exists("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gapmgkggu.sHtML

JS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/guhjhccwn.sHtML

TS:   fs.existsSync("a.txt")
来源：http://blog.fehbvm.com/Article/details/gdilwomvp.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://3g.hesvh.cn/Article/details/grbbbzfpe.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.share.zdbjq.cn/Article/details/gdatrlxab.sHtML

Ruby: File.exist?("a.txt")
来源：http://baike.fehbvm.com/Article/details/gtamvydcy.sHtML

C#:   File.Exists("a.txt")
来源：http://baike.fehbvm.com/Article/details/gpxakdqwy.sHtML

[F06] 删除文件
来源：http://read.share.zdbjq.cn/Article/details/grstghofq.sHtML

Py:   os.remove("a.txt")
来源：http://blog.fehbvm.com/Article/details/gnufxandw.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fehbvm.com/Article/details/grexbstaw.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gyownjmvl.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/ggdvvtpnz.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.fehbvm.com/Article/details/gcxvjamxt.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.fehbvm.com/Article/details/gxiofmllb.sHtML

Ruby: File.delete("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gcobiilcx.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gcxhbhnvk.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.zdbjq.cn/Article/details/ggxnyfyhx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.zdbjq.cn/Article/details/ggnkjntzi.sHtML


<!-- 参考信息 -->