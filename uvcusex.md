代发 wailian999

C#:   list.Aggregate(0, (acc, x) => acc + x)
来源：http://wap.hesvh.cn/Article/details/gvimxhaqm.sHtML

[D24] 字典 / Map 基本操作
来源：http://www.m.share.zdbjq.cn/Article/details/gpplazrde.sHtML

Py:   d["k"] = 1;  d.get("k");  "k" in d;  d.pop("k")
来源：http://www.share.hesvh.cn/Article/details/gdaummvkx.sHtML

PHP:  $d["k"] = 1;  $d["k"] ?? null;  isset($d["k"]);  unset($d["k"]);
来源：http://3g.zdbjq.cn/Article/details/gerldinbd.sHtML

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://m.share.hesvh.cn/Article/details/gkqzjkgia.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gmbubrycd.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://wap.fehbvm.com/Article/details/gwreusdqa.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://baike.fehbvm.com/Article/details/gjgwvhrus.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.share.hesvh.cn/Article/details/giefkotwm.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://3g.zdbjq.cn/Article/details/gklqonfpt.sHtML

[D25] Set 集合去重与交并差
来源：http://3g.hesvh.cn/Article/details/gftwolhpf.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.share.zdbjq.cn/Article/details/ghudpbgzt.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://wap.fehbvm.com/Article/details/gkrojfjyk.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://mobile.zdbjq.cn/Article/details/gqwezomey.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://3g.hesvh.cn/Article/details/gsbrhmgrv.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://read.share.fehbvm.com/Article/details/gfdyuxutz.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/geeiyglct.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.zdbjq.cn/Article/details/ggasvkdch.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://baike.fehbvm.com/Article/details/gkcutyvrs.sHtML

[D26] 数组转字符串
来源：http://read.share.zdbjq.cn/Article/details/gerogpeks.sHtML

Py:   ", ".join(map(str, arr))
来源：http://www.blog.zdbjq.cn/Article/details/gnmllkuof.sHtML

PHP:  implode(", ", $arr);
来源：http://www.blog.hesvh.cn/Article/details/gdjkwjfmo.sHtML

JS:   arr.join(", ")
来源：http://www.blog.hesvh.cn/Article/details/gfdmwnpdi.sHtML

TS:   arr.join(", ")
来源：http://www.share.zdbjq.cn/Article/details/gqmwatnrz.sHtML

Java: String.join(", ", list)
来源：http://wap.fehbvm.com/Article/details/gjfgzidfc.sHtML

Go:   strings.Join(strs, ", ")
来源：http://www.blog.fehbvm.com/Article/details/gqaxnqxmh.sHtML

Ruby: arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gbbhznkap.sHtML

C#:   string.Join(", ", list)
来源：http://baike.hesvh.cn/Article/details/gdtqvyzxr.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gdjiqckzl.sHtML

E. 字符串处理
来源：http://www.share.fehbvm.com/Article/details/gfhkffwvc.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gbzbxmjwk.sHtML

[E01] 拼接字符串
来源：http://baike.hesvh.cn/Article/details/gbybpbhyc.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.zdbjq.cn/Article/details/givekwsyj.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.fehbvm.com/Article/details/gwmwpqekk.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gnpdsioef.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://wap.fehbvm.com/Article/details/gktufyrkj.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://wap.zdbjq.cn/Article/details/gcsnitxij.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://mobile.fehbvm.com/Article/details/gzlslvkmu.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://baike.fehbvm.com/Article/details/gprljryru.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fehbvm.com/Article/details/glfhyvkog.sHtML

[E02] 重复字符串
来源：http://baike.fehbvm.com/Article/details/gjrwzitap.sHtML

Py:   "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/gfynzzgxr.sHtML

PHP:  str_repeat("ab", 3);
来源：http://mobile.fehbvm.com/Article/details/gzpdaumsh.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.fehbvm.com/Article/details/griuofvyg.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.zdbjq.cn/Article/details/gxodecpgy.sHtML

Java: "ab".repeat(3)
来源：http://m.share.hesvh.cn/Article/details/gzbtnramj.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://mobile.zdbjq.cn/Article/details/glmhcwljz.sHtML

Ruby: "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gwkjniehp.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.m.share.hesvh.cn/Article/details/gyqadkhvr.sHtML

[E03] 截取子串
来源：http://blog.fehbvm.com/Article/details/gstauhstc.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.hesvh.cn/Article/details/gnhornqiw.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/gftkmnxmr.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://m.share.zdbjq.cn/Article/details/gnpyzxrbu.sHtML

TS:   s.slice(1, 4)
来源：http://wap.hesvh.cn/Article/details/gmltktmae.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gcydgmfgj.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://3g.hesvh.cn/Article/details/gjslxvqrx.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://baike.hesvh.cn/Article/details/gjzpwmuzs.sHtML

C#:   s.Substring(1, 3)
来源：http://3g.hesvh.cn/Article/details/gtqkoipit.sHtML

[E04] 查找子串位置
来源：http://mobile.fehbvm.com/Article/details/gumumbivn.sHtML

Py:   s.find("x");  s.index("x")
来源：http://blog.hesvh.cn/Article/details/gxyyryxxp.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.hesvh.cn/Article/details/glmbnbmmr.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.share.zdbjq.cn/Article/details/ggddqruds.sHtML

TS:   s.indexOf("x")
来源：http://www.m.share.fehbvm.com/Article/details/gjlpcnhrc.sHtML

Java: s.indexOf("x")
来源：http://www.blog.hesvh.cn/Article/details/gxytqeetz.sHtML

Go:   strings.Index(s, "x")
来源：http://baike.hesvh.cn/Article/details/ggwlmnkyd.sHtML

Ruby: s.index("x")
来源：http://read.share.fehbvm.com/Article/details/gcbhothvz.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gmymqdqsb.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://blog.hesvh.cn/Article/details/gdqrpmmjm.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://mobile.hesvh.cn/Article/details/gjjunbzoq.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.hesvh.cn/Article/details/gfazsglzw.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://3g.zdbjq.cn/Article/details/gmmqukejg.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.fehbvm.com/Article/details/gjddlugdu.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/gsyzwbxfh.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fehbvm.com/Article/details/gweshmpli.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.blog.hesvh.cn/Article/details/gsdtehcmp.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.zdbjq.cn/Article/details/gprhhcyld.sHtML

[E06] 替换子串
来源：http://www.m.share.fehbvm.com/Article/details/gnxzvnafx.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/guepmqbns.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.fehbvm.com/Article/details/gzyuzzhzc.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.hesvh.cn/Article/details/gayivlpqx.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gxmvpelef.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.hesvh.cn/Article/details/gmtzbogji.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://mobile.zdbjq.cn/Article/details/gppedwodq.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gcblkepyw.sHtML

C#:   s.Replace("a", "b")
来源：http://www.m.share.zdbjq.cn/Article/details/gwmzevuge.sHtML

[E07] 按分隔符拆分
来源：http://mobile.fehbvm.com/Article/details/gwbmcezxg.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.hesvh.cn/Article/details/gbqgcugnx.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://blog.hesvh.cn/Article/details/gwgjxhyol.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.share.fehbvm.com/Article/details/gjmosljpz.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/gkmpgxuej.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://read.share.fehbvm.com/Article/details/gdzqonqbx.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://baike.zdbjq.cn/Article/details/grphilboz.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.zdbjq.cn/Article/details/gbwnmroik.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.blog.zdbjq.cn/Article/details/gaowxlipm.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.hesvh.cn/Article/details/gnebreaeg.sHtML

Py:   ",".join(items)
来源：http://wap.hesvh.cn/Article/details/grqvnnyxb.sHtML

PHP:  implode(",", $items);
来源：http://m.share.zdbjq.cn/Article/details/gxdvjtxte.sHtML

JS:   items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gecdhxtwb.sHtML

TS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gbbmptdlr.sHtML

Java: String.join(",", items)
来源：http://www.m.share.fehbvm.com/Article/details/gygqqpalm.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.fehbvm.com/Article/details/gviotkfvy.sHtML

Ruby: items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gxbkwcaxj.sHtML

C#:   string.Join(",", items)
来源：http://www.share.fehbvm.com/Article/details/gadmlxsad.sHtML

[E09] 去除所有空白字符
来源：http://wap.fehbvm.com/Article/details/gnydxeypo.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/guowzxtft.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fehbvm.com/Article/details/gambcicvd.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.fehbvm.com/Article/details/gjwbjlqqe.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/ggswnvaqx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://read.share.fehbvm.com/Article/details/gwgpgmojj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://wap.zdbjq.cn/Article/details/geamntcbo.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/goyuutgqx.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://read.share.hesvh.cn/Article/details/grueshtei.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.zdbjq.cn/Article/details/gcfpepfpm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gcwovdhkc.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.zdbjq.cn/Article/details/gkqqhlcla.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.zdbjq.cn/Article/details/gsdtlszng.sHtML

TS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gfpyfbodm.sHtML

Java: String.format("%03d", 7)
来源：http://baike.zdbjq.cn/Article/details/gznpzdtux.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.fehbvm.com/Article/details/gbkgvqkzm.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gbvkbmgxj.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.zdbjq.cn/Article/details/gppzwsghd.sHtML

[E11] 反转字符串
来源：http://blog.zdbjq.cn/Article/details/gycfmgomk.sHtML

Py:   s[::-1]
来源：http://baike.zdbjq.cn/Article/details/ggaahpyep.sHtML

PHP:  strrev($s);
来源：http://www.m.share.fehbvm.com/Article/details/ghhmyzxjv.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/ggayapfiq.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.hesvh.cn/Article/details/gbrkkaoke.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://blog.fehbvm.com/Article/details/gjuucyaub.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://mobile.fehbvm.com/Article/details/gpkxrmzeg.sHtML

Ruby: s.reverse
来源：http://www.blog.fehbvm.com/Article/details/guaqcbsxg.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/gkdjwctab.sHtML

[E12] 统计某字符出现次数
来源：http://blog.zdbjq.cn/Article/details/gdadqzjfu.sHtML

Py:   s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gbmsnoecv.sHtML

PHP:  substr_count($s, "a");
来源：http://wap.zdbjq.cn/Article/details/gbcalvhyq.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/glotocxvn.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gdiqcqgoj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.m.share.hesvh.cn/Article/details/gerjoampc.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fehbvm.com/Article/details/gznswcrpb.sHtML

Ruby: s.count("a")
来源：http://www.m.share.fehbvm.com/Article/details/gxifpihsh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.share.zdbjq.cn/Article/details/gdhqlslqw.sHtML

[E13] 逐字符遍历
来源：http://www.share.fehbvm.com/Article/details/gflvrqxdb.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.zdbjq.cn/Article/details/gyzleszpo.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.m.share.hesvh.cn/Article/details/gzyjpkcyp.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.hesvh.cn/Article/details/gwepmsfab.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.hesvh.cn/Article/details/gnnaybgjs.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gjvoafkid.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://read.share.fehbvm.com/Article/details/gqaiqwtya.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.blog.fehbvm.com/Article/details/gvljiagcm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gqncrbfdi.sHtML

[E14] URL 编码与 Base64
来源：http://wap.zdbjq.cn/Article/details/glrzymcpd.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.zdbjq.cn/Article/details/gxrdkhyde.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.zdbjq.cn/Article/details/grpfjcevx.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fehbvm.com/Article/details/gqdpvxpww.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.m.share.hesvh.cn/Article/details/gudaplppc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://blog.fehbvm.com/Article/details/gumylwqvc.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://3g.fehbvm.com/Article/details/ghfiwncxf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.zdbjq.cn/Article/details/gakydzhkd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fehbvm.com/Article/details/gbqndhhxj.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.hesvh.cn/Article/details/gltxwngca.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.hesvh.cn/Article/details/gpjfqvpzv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.hesvh.cn/Article/details/gvipamccc.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.share.zdbjq.cn/Article/details/gilxfzptm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.zdbjq.cn/Article/details/gtrxnoqcd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://3g.zdbjq.cn/Article/details/gcqkokixg.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.hesvh.cn/Article/details/gtcrkbrbt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.hesvh.cn/Article/details/guqeyvdyr.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.hesvh.cn/Article/details/gdgzftvab.sHtML

[E16] 数字千分位
来源：http://read.share.hesvh.cn/Article/details/gcshhtgyn.sHtML

Py:   f"{1234567:,}"
来源：http://www.m.share.hesvh.cn/Article/details/gdepepbwx.sHtML

PHP:  number_format(1234567);
来源：http://baike.fehbvm.com/Article/details/gobiffgom.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gzfncqhvc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://3g.zdbjq.cn/Article/details/gpnyvjuya.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.hesvh.cn/Article/details/gbnfllcbz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://wap.hesvh.cn/Article/details/giqzfzvte.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.zdbjq.cn/Article/details/gwaynfmal.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.hesvh.cn/Article/details/gxoxetwxm.sHtML

[E17] 首字母大写
来源：http://www.share.zdbjq.cn/Article/details/gslcubrsp.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fehbvm.com/Article/details/gsnnlilyn.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://blog.hesvh.cn/Article/details/gkslazqms.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.hesvh.cn/Article/details/gcverjdpi.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/ghzeozoso.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.zdbjq.cn/Article/details/goergycqg.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.fehbvm.com/Article/details/gvvvpbzjo.sHtML

Ruby: s.capitalize
来源：http://wap.zdbjq.cn/Article/details/ghpvkzhvw.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://read.share.fehbvm.com/Article/details/ganaukrwm.sHtML

[E18] 模板占位符替换
来源：http://m.share.zdbjq.cn/Article/details/gcydjohwi.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.zdbjq.cn/Article/details/gtzspjjpj.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fehbvm.com/Article/details/gwqfxqddj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.hesvh.cn/Article/details/gtlrtcudr.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.fehbvm.com/Article/details/ghvxieajq.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gdkfnlbpz.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gvawajapd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.zdbjq.cn/Article/details/gldcauaqu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.hesvh.cn/Article/details/gxneqlbes.sHtML

[E19] 多行文本按行拆分
来源：http://blog.zdbjq.cn/Article/details/gvtohhjnt.sHtML

Py:   s.splitlines()
来源：http://baike.zdbjq.cn/Article/details/gkyaoqbdg.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://read.share.zdbjq.cn/Article/details/gbfrboyly.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.hesvh.cn/Article/details/gptizdczr.sHtML

TS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gomanzilu.sHtML

Java: s.lines().toList()
来源：http://www.blog.hesvh.cn/Article/details/gumtvbwgu.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.hesvh.cn/Article/details/gejqmftba.sHtML

Ruby: s.lines
来源：http://www.m.share.fehbvm.com/Article/details/gchbmsiqn.sHtML

C#:   s.Split('\n')
来源：http://baike.hesvh.cn/Article/details/geiojblre.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.fehbvm.com/Article/details/gaskebphv.sHtML

Py:   if not s:
来源：http://wap.zdbjq.cn/Article/details/glweiwyya.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.fehbvm.com/Article/details/gwdltbqng.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fehbvm.com/Article/details/gctgchoqb.sHtML

TS:   if (s === "") {}
来源：http://blog.fehbvm.com/Article/details/gdlltdldk.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.zdbjq.cn/Article/details/gnvqjzrzi.sHtML

Go:   if s == "" {}
来源：http://baike.zdbjq.cn/Article/details/gizrxvwkh.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/gsencuczg.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/gsuzuuqxa.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/grsbvagdr.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.blog.zdbjq.cn/Article/details/glkfyipas.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://3g.zdbjq.cn/Article/details/gfwccpjui.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gchusmpeq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gepvelfzo.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gcxtajuby.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://read.share.zdbjq.cn/Article/details/gixhdixbs.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gweyuwzyr.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gipwtzqct.sHtML

[E22] 字节长度与字符长度
来源：http://wap.hesvh.cn/Article/details/giczyaytg.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fehbvm.com/Article/details/gtelkeimx.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.hesvh.cn/Article/details/gbibvngqj.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.hesvh.cn/Article/details/gzzysxdtt.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.zdbjq.cn/Article/details/gafybvmos.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.zdbjq.cn/Article/details/gnexmhpgy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/guhuteaud.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.fehbvm.com/Article/details/gsfsbnfub.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.zdbjq.cn/Article/details/ggdgtphna.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gxnoufhrj.sHtML

F. 文件与目录
来源：http://www.share.hesvh.cn/Article/details/gdrxzuwln.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gpcfhuzee.sHtML

[F01] 读取整个文件
来源：http://mobile.hesvh.cn/Article/details/gxtxzfdhi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://blog.zdbjq.cn/Article/details/gjxilunwi.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/gyyuimsif.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.hesvh.cn/Article/details/guzwtzymf.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gesgofmba.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/glscbltlv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.hesvh.cn/Article/details/gsgwrduyj.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gpnvnweqk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/gltfjwelx.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/gefsugvwo.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.zdbjq.cn/Article/details/gamsjsvzr.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://mobile.fehbvm.com/Article/details/gbijpqdqi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/guxjhfpbo.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.zdbjq.cn/Article/details/gngemnbhf.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.zdbjq.cn/Article/details/gulluysnz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://baike.hesvh.cn/Article/details/gyenzlwhq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fehbvm.com/Article/details/gxyfyfrbf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.share.fehbvm.com/Article/details/gfaoxbagq.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.hesvh.cn/Article/details/gyomdgyzw.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.zdbjq.cn/Article/details/goytwicoy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/givqyakxu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.fehbvm.com/Article/details/ginaeiqmu.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gcnkbhshm.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.hesvh.cn/Article/details/gjozmvece.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.fehbvm.com/Article/details/gzehrqfrs.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.fehbvm.com/Article/details/gonhmhhwh.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/ghhbmnzcy.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/gklizlbpq.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.fehbvm.com/Article/details/gqdbovnpr.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.m.share.fehbvm.com/Article/details/gttojwdmt.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/guhdysazx.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.fehbvm.com/Article/details/gjctnhnwg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.hesvh.cn/Article/details/gppkdnjiv.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.hesvh.cn/Article/details/gzpusnmgz.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://mobile.hesvh.cn/Article/details/gpdomxxes.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://m.share.hesvh.cn/Article/details/glzrxdlnf.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.zdbjq.cn/Article/details/glbnygumy.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://baike.zdbjq.cn/Article/details/gobxppkxi.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fehbvm.com/Article/details/gpitgctgq.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gsxnxvorg.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gottfzuwi.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gwcmbkwol.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://baike.hesvh.cn/Article/details/gprvmuqlp.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gijhajlao.sHtML

C#:   File.Exists("a.txt")
来源：http://wap.fehbvm.com/Article/details/gdlepsoxn.sHtML

[F06] 删除文件
来源：http://m.share.fehbvm.com/Article/details/gojnfznhb.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gbyokaszc.sHtML

PHP:  unlink("a.txt");
来源：http://mobile.fehbvm.com/Article/details/gvatordzh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gjasrlvya.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.fehbvm.com/Article/details/glhcpvqec.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gzohvifbl.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gdimtgrfd.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gdqxqjogu.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.hesvh.cn/Article/details/gnvnbyjfw.sHtML

[F07] 创建目录（含多级）
来源：http://blog.zdbjq.cn/Article/details/gfvmbzszb.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.zdbjq.cn/Article/details/gzisvryec.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fehbvm.com/Article/details/gwfsbzyai.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/gfseubeph.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gavcspcwm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.m.share.fehbvm.com/Article/details/gnevwyucl.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://m.share.zdbjq.cn/Article/details/ghoetaxpq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.m.share.fehbvm.com/Article/details/glhkjvqiy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.m.share.hesvh.cn/Article/details/glyfbmfyo.sHtML

[F08] 遍历目录
来源：http://blog.hesvh.cn/Article/details/gtbxvwwji.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.share.hesvh.cn/Article/details/guiacnrau.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.share.fehbvm.com/Article/details/gonpsgbjo.sHtML

JS:   fs.readdirSync("dir")
来源：http://www.share.hesvh.cn/Article/details/giabztint.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.hesvh.cn/Article/details/gezmfbbua.sHtML


<!-- 参考信息 -->