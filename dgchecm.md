代发 wailian999

JS:   obj.k = 1;  "k" in obj;  delete obj.k;  new Map().set("k", 1)
来源：http://mobile.hesvh.cn/Article/details/gwnrbpwor.sHtML

TS:   const d: Record<string, number> = {};  d["k"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gmgnwueer.sHtML

Java: map.put("k", 1);  map.get("k");  map.containsKey("k");  map.remove("k")
来源：http://blog.fehbvm.com/Article/details/gohmiaugm.sHtML

Go:   m := map[string]int{};  m["k"] = 1;  v, ok := m["k"];  delete(m, "k")
来源：http://3g.zdbjq.cn/Article/details/gujmtwzfg.sHtML

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://www.blog.zdbjq.cn/Article/details/gqcmzdzlx.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://read.share.zdbjq.cn/Article/details/grhlribyg.sHtML

[D25] Set 集合去重与交并差
来源：http://blog.fehbvm.com/Article/details/gpqzcpwkx.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://m.share.zdbjq.cn/Article/details/gklmdtpsi.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://baike.hesvh.cn/Article/details/gpnzliwac.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://www.m.share.hesvh.cn/Article/details/gdjwbahyt.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://blog.zdbjq.cn/Article/details/gswpyzylb.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://m.share.fehbvm.com/Article/details/gpyjjplmw.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://3g.fehbvm.com/Article/details/gajvkokzu.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://www.share.zdbjq.cn/Article/details/gtyvyxfdo.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/grohmpmkh.sHtML

[D26] 数组转字符串
来源：http://www.share.zdbjq.cn/Article/details/gbtuxzvzk.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/gtjnickpp.sHtML

PHP:  implode(", ", $arr);
来源：http://www.share.hesvh.cn/Article/details/gjefxtupe.sHtML

JS:   arr.join(", ")
来源：http://3g.fehbvm.com/Article/details/gfrqozrdv.sHtML

TS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gubillogx.sHtML

Java: String.join(", ", list)
来源：http://read.share.fehbvm.com/Article/details/gzplgtirh.sHtML

Go:   strings.Join(strs, ", ")
来源：http://read.share.zdbjq.cn/Article/details/gzckufaql.sHtML

Ruby: arr.join(", ")
来源：http://read.share.fehbvm.com/Article/details/gofmvoyxg.sHtML

C#:   string.Join(", ", list)
来源：http://blog.fehbvm.com/Article/details/gcltwgwzh.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/ghcbzwthh.sHtML

E. 字符串处理
来源：http://www.blog.hesvh.cn/Article/details/gnrcadcms.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwlfmjiqn.sHtML

[E01] 拼接字符串
来源：http://wap.fehbvm.com/Article/details/gopvyfoal.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.zdbjq.cn/Article/details/ggfexpmat.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://read.share.hesvh.cn/Article/details/gnhjtqefi.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.fehbvm.com/Article/details/gcwhjghuh.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.blog.hesvh.cn/Article/details/gfeookguu.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://m.share.fehbvm.com/Article/details/ggkaswgdz.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/gjxaadqpf.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.hesvh.cn/Article/details/gcuosrqjw.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gdbfdlile.sHtML

[E02] 重复字符串
来源：http://blog.zdbjq.cn/Article/details/gvzrfpnsv.sHtML

Py:   "ab" * 3
来源：http://3g.zdbjq.cn/Article/details/ghzqmaede.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.m.share.hesvh.cn/Article/details/ghnzprffl.sHtML

JS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/gawkvwicp.sHtML

TS:   "ab".repeat(3)
来源：http://wap.hesvh.cn/Article/details/geqpyrszr.sHtML

Java: "ab".repeat(3)
来源：http://baike.fehbvm.com/Article/details/gbntzejai.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.hesvh.cn/Article/details/glzlonzkg.sHtML

Ruby: "ab" * 3
来源：http://read.share.zdbjq.cn/Article/details/gqbqlbgud.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.blog.fehbvm.com/Article/details/gkmnlbqcu.sHtML

[E03] 截取子串
来源：http://m.share.hesvh.cn/Article/details/gltebbtcg.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://3g.hesvh.cn/Article/details/gfowiumig.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://mobile.fehbvm.com/Article/details/gshjlezvg.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://blog.hesvh.cn/Article/details/gfibvqcqm.sHtML

TS:   s.slice(1, 4)
来源：http://www.share.fehbvm.com/Article/details/gszbgyyca.sHtML

Java: s.substring(1, 4)
来源：http://mobile.fehbvm.com/Article/details/gdemzmxou.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://m.share.zdbjq.cn/Article/details/grmbnpjpq.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.hesvh.cn/Article/details/gfhjzxrzh.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.fehbvm.com/Article/details/ghxrrcrad.sHtML

[E04] 查找子串位置
来源：http://blog.zdbjq.cn/Article/details/gaqwpkhmm.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/ggkibsvqb.sHtML

PHP:  strpos($s, "x");
来源：http://www.m.share.zdbjq.cn/Article/details/gbfockknz.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://m.share.fehbvm.com/Article/details/giraghyyf.sHtML

TS:   s.indexOf("x")
来源：http://baike.fehbvm.com/Article/details/gkusbbwfr.sHtML

Java: s.indexOf("x")
来源：http://blog.fehbvm.com/Article/details/gyupffpxs.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.hesvh.cn/Article/details/gwrdebysh.sHtML

Ruby: s.index("x")
来源：http://wap.hesvh.cn/Article/details/gbdhuzccw.sHtML

C#:   s.IndexOf("x")
来源：http://baike.zdbjq.cn/Article/details/glterepkv.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.blog.hesvh.cn/Article/details/gtabqhfum.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.hesvh.cn/Article/details/ghhvddefm.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.fehbvm.com/Article/details/gzdepiriv.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://blog.hesvh.cn/Article/details/gfvitqihc.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.m.share.zdbjq.cn/Article/details/guazodqlv.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.fehbvm.com/Article/details/goranmyth.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.blog.fehbvm.com/Article/details/gsfbpsxqi.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.hesvh.cn/Article/details/grzoixpym.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://m.share.zdbjq.cn/Article/details/gzdeyucru.sHtML

[E06] 替换子串
来源：http://wap.hesvh.cn/Article/details/gtbrzywxb.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gdtmkbqcw.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://www.share.hesvh.cn/Article/details/gstkevtkf.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.hesvh.cn/Article/details/ggcwqzrdh.sHtML

TS:   s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gacdyhacr.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/ggermjzmf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.blog.fehbvm.com/Article/details/gxrficmhc.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gwwxkgjji.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gknqqkupx.sHtML

[E07] 按分隔符拆分
来源：http://wap.fehbvm.com/Article/details/gxyacmafz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fehbvm.com/Article/details/gbrqeadjd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.m.share.zdbjq.cn/Article/details/glmycrrew.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.fehbvm.com/Article/details/gqpxjzjqc.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/gzatgrsjd.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.zdbjq.cn/Article/details/glsicpeke.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.blog.zdbjq.cn/Article/details/gmktqzoqj.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.zdbjq.cn/Article/details/gfensndob.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fehbvm.com/Article/details/ghnwebbbx.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fehbvm.com/Article/details/gltvjuzco.sHtML

Py:   ",".join(items)
来源：http://read.share.hesvh.cn/Article/details/gukfqtqhv.sHtML

PHP:  implode(",", $items);
来源：http://baike.hesvh.cn/Article/details/gqfxbvhtf.sHtML

JS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/goncqsgvg.sHtML

TS:   items.join(",")
来源：http://read.share.fehbvm.com/Article/details/gmwomjwil.sHtML

Java: String.join(",", items)
来源：http://www.blog.zdbjq.cn/Article/details/gxhcvglba.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.hesvh.cn/Article/details/gzimnffxn.sHtML

Ruby: items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/ggeysqsdt.sHtML

C#:   string.Join(",", items)
来源：http://m.share.hesvh.cn/Article/details/gkgvnngmi.sHtML

[E09] 去除所有空白字符
来源：http://baike.hesvh.cn/Article/details/gjqbywtmc.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.fehbvm.com/Article/details/gjkocacsn.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.fehbvm.com/Article/details/gaejbqigi.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/glahhesqy.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gizebxrgj.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.m.share.zdbjq.cn/Article/details/gwrqtkqit.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.share.fehbvm.com/Article/details/grbpvmiwj.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://mobile.hesvh.cn/Article/details/gqfmkfwmh.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.hesvh.cn/Article/details/grlelsghb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.m.share.zdbjq.cn/Article/details/gbafbtugr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.hesvh.cn/Article/details/goghztvrr.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.hesvh.cn/Article/details/gzzxrbyuk.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.share.fehbvm.com/Article/details/grfopazgs.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.hesvh.cn/Article/details/gwimubnge.sHtML

Java: String.format("%03d", 7)
来源：http://3g.hesvh.cn/Article/details/grghednia.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://m.share.hesvh.cn/Article/details/gttacqzdb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gzcbmrrmt.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://baike.fehbvm.com/Article/details/geohnnvvp.sHtML

[E11] 反转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gjhduscbk.sHtML

Py:   s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gybcoeaas.sHtML

PHP:  strrev($s);
来源：http://blog.fehbvm.com/Article/details/gvtcysteq.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.fehbvm.com/Article/details/gvigbszwo.sHtML

TS:   [...s].reverse().join("")
来源：http://3g.fehbvm.com/Article/details/gigvgksel.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.fehbvm.com/Article/details/glwshyizq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.fehbvm.com/Article/details/gjjadvnkz.sHtML

Ruby: s.reverse
来源：http://3g.fehbvm.com/Article/details/ghhtuqobd.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.share.hesvh.cn/Article/details/gejgxsqmi.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.hesvh.cn/Article/details/grgqmltqb.sHtML

Py:   s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gcwimraox.sHtML

PHP:  substr_count($s, "a");
来源：http://blog.hesvh.cn/Article/details/gspeakacu.sHtML

JS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/goraprgee.sHtML

TS:   s.split("a").length - 1
来源：http://www.share.zdbjq.cn/Article/details/gcnweklxj.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.zdbjq.cn/Article/details/gtadcmtre.sHtML

Go:   strings.Count(s, "a")
来源：http://blog.zdbjq.cn/Article/details/grzstovft.sHtML

Ruby: s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gjpvxnawk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.zdbjq.cn/Article/details/gxckhbmby.sHtML

[E13] 逐字符遍历
来源：http://www.m.share.zdbjq.cn/Article/details/givhjdocs.sHtML

Py:   for ch in s: print(ch)
来源：http://read.share.hesvh.cn/Article/details/gtizbokqv.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.hesvh.cn/Article/details/grjubmego.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.hesvh.cn/Article/details/gwptilquo.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.zdbjq.cn/Article/details/gdtbhjsvp.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gfdlghras.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fehbvm.com/Article/details/gkpfwddmk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://wap.fehbvm.com/Article/details/gmzvhkblb.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://wap.hesvh.cn/Article/details/gkaowlctt.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.hesvh.cn/Article/details/gvesvvmtv.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.hesvh.cn/Article/details/gtvdpkcnd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.zdbjq.cn/Article/details/goztecbvv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://read.share.fehbvm.com/Article/details/galdcyiot.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://3g.hesvh.cn/Article/details/gnfbimopa.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.hesvh.cn/Article/details/gfcxllykk.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.blog.zdbjq.cn/Article/details/gewqhthih.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://blog.zdbjq.cn/Article/details/gzqizryqd.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://m.share.hesvh.cn/Article/details/gpzyabnuv.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.hesvh.cn/Article/details/gjmaksamt.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.zdbjq.cn/Article/details/goskgsuqv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.hesvh.cn/Article/details/ghnxiqbbm.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.hesvh.cn/Article/details/gkcbrnrcg.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.fehbvm.com/Article/details/gowzbmydl.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.blog.zdbjq.cn/Article/details/gqkecvulq.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://baike.zdbjq.cn/Article/details/gnzqdoblf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fehbvm.com/Article/details/gutvxagbc.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.share.fehbvm.com/Article/details/gotahhkmi.sHtML

[E16] 数字千分位
来源：http://www.share.hesvh.cn/Article/details/gvqqkmzfh.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/gittcjocz.sHtML

PHP:  number_format(1234567);
来源：http://www.m.share.fehbvm.com/Article/details/gjisrexmv.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gbxzpkzyf.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.hesvh.cn/Article/details/gwdfyawaa.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://3g.hesvh.cn/Article/details/ggffkjhkh.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.hesvh.cn/Article/details/glextecqr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.zdbjq.cn/Article/details/gxqpcejod.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.fehbvm.com/Article/details/gjmmcincg.sHtML

[E17] 首字母大写
来源：http://www.blog.fehbvm.com/Article/details/gofyfjsoi.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.hesvh.cn/Article/details/gnaodxglc.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://baike.fehbvm.com/Article/details/gmohrggdz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.hesvh.cn/Article/details/ghbdpmazu.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.fehbvm.com/Article/details/gbrvbedkc.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.zdbjq.cn/Article/details/gutcfblpb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.hesvh.cn/Article/details/gwknevxig.sHtML

Ruby: s.capitalize
来源：http://www.share.fehbvm.com/Article/details/gprrcgflm.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.fehbvm.com/Article/details/gqqgbsdtk.sHtML

[E18] 模板占位符替换
来源：http://wap.fehbvm.com/Article/details/gqwqgvbig.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.hesvh.cn/Article/details/gogoxhfwo.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/glpesbjfr.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.share.hesvh.cn/Article/details/gznbgfifd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.m.share.hesvh.cn/Article/details/gwznylypc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.fehbvm.com/Article/details/grfklcicp.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gsmwykmfj.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.blog.zdbjq.cn/Article/details/gqvrheiht.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.zdbjq.cn/Article/details/gfmaeadqc.sHtML

[E19] 多行文本按行拆分
来源：http://www.blog.zdbjq.cn/Article/details/gekfwdzbt.sHtML

Py:   s.splitlines()
来源：http://baike.fehbvm.com/Article/details/gmccgmouw.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.zdbjq.cn/Article/details/gzmukvzii.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gdakiphvx.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gmlwsmcja.sHtML

Java: s.lines().toList()
来源：http://read.share.zdbjq.cn/Article/details/gzvrncprl.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.fehbvm.com/Article/details/gammooqiq.sHtML

Ruby: s.lines
来源：http://3g.zdbjq.cn/Article/details/gnxduclwh.sHtML

C#:   s.Split('\n')
来源：http://read.share.zdbjq.cn/Article/details/gcfpvtulj.sHtML

[E20] 判断字符串是否为空
来源：http://www.share.zdbjq.cn/Article/details/gkboxfqae.sHtML

Py:   if not s:
来源：http://mobile.zdbjq.cn/Article/details/gfboahmkf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://wap.fehbvm.com/Article/details/gfkgdxxgc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.hesvh.cn/Article/details/ggmcactnz.sHtML

TS:   if (s === "") {}
来源：http://baike.fehbvm.com/Article/details/gdbmtupdt.sHtML

Java: if (s.isEmpty()) {}
来源：http://wap.hesvh.cn/Article/details/gdzyagrgo.sHtML

Go:   if s == "" {}
来源：http://blog.hesvh.cn/Article/details/guphuzfxy.sHtML

Ruby: if s.empty?
来源：http://3g.fehbvm.com/Article/details/gxsuvutmf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://3g.hesvh.cn/Article/details/gaskqzxbv.sHtML

[E21] 超长截断加省略号
来源：http://mobile.hesvh.cn/Article/details/giluhcibx.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.fehbvm.com/Article/details/gkiynsyep.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gijuhkclv.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/goxgbkeyn.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://baike.hesvh.cn/Article/details/gnpuhjxld.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gltvucmnc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.hesvh.cn/Article/details/gtoghdpew.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://3g.hesvh.cn/Article/details/ghogehkkq.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://m.share.zdbjq.cn/Article/details/gunlwnwbm.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.zdbjq.cn/Article/details/ghysxjuyz.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.fehbvm.com/Article/details/gjzjiuizg.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://3g.fehbvm.com/Article/details/givoaglgp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gdycjgbwy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gdwowpnnf.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.m.share.fehbvm.com/Article/details/gbnvpnkdg.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fehbvm.com/Article/details/gyboardkw.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.hesvh.cn/Article/details/goslfdmeh.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.m.share.hesvh.cn/Article/details/gigxhucww.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvdaeqmbb.sHtML

F. 文件与目录
来源：http://baike.hesvh.cn/Article/details/gfpklzkpl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/glemqckid.sHtML

[F01] 读取整个文件
来源：http://www.m.share.fehbvm.com/Article/details/glstwmqxk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.hesvh.cn/Article/details/gxibswlln.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.share.fehbvm.com/Article/details/gyzmspcpn.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://mobile.zdbjq.cn/Article/details/gxzkzuokl.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gbkbvfwlo.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.zdbjq.cn/Article/details/gyhtzixgf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.hesvh.cn/Article/details/gncxkzubt.sHtML

Ruby: File.read("a.txt")
来源：http://blog.zdbjq.cn/Article/details/ghwzxctik.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fehbvm.com/Article/details/gequkdlqa.sHtML

[F02] 逐行读取文件
来源：http://www.share.zdbjq.cn/Article/details/gclulbvsk.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.zdbjq.cn/Article/details/golkpujzb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fehbvm.com/Article/details/ggwyzctqi.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.hesvh.cn/Article/details/ggrnzhzjk.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.hesvh.cn/Article/details/gowufngdo.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gbihygrms.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fehbvm.com/Article/details/gbetfpvhk.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fehbvm.com/Article/details/gwvqaregx.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://baike.fehbvm.com/Article/details/gdwgjjiqe.sHtML

[F03] 写入文件（覆盖）
来源：http://wap.hesvh.cn/Article/details/gorsexpqv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.zdbjq.cn/Article/details/gmhpvnoki.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://read.share.hesvh.cn/Article/details/gsnawcdje.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fehbvm.com/Article/details/gbrmhmzpe.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gsbhlmqwn.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.zdbjq.cn/Article/details/gvfrwngda.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fehbvm.com/Article/details/gvujcywlt.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fehbvm.com/Article/details/givlkjdst.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.blog.fehbvm.com/Article/details/glmfzovbc.sHtML

[F04] 追加写入文件
来源：http://www.m.share.zdbjq.cn/Article/details/gccfbtwbc.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.hesvh.cn/Article/details/gdfabwwsp.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.zdbjq.cn/Article/details/ggjttugvg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.zdbjq.cn/Article/details/gtgxyxevc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.hesvh.cn/Article/details/gwkgkbogn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.zdbjq.cn/Article/details/ghmdkyqvs.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.zdbjq.cn/Article/details/gwgoucpwn.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://read.share.zdbjq.cn/Article/details/ghhkietey.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.zdbjq.cn/Article/details/ghjyrsmuo.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.blog.hesvh.cn/Article/details/gmninymtn.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/gqszgjzlq.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/guqctqyxx.sHtML

JS:   fs.existsSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gejrcjsma.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gnskodwtf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gswciocjc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://m.share.fehbvm.com/Article/details/gpafhpwsy.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gixcqgoer.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gakivhaan.sHtML

[F06] 删除文件
来源：http://m.share.fehbvm.com/Article/details/gltwdusmp.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/gewuwpqey.sHtML

PHP:  unlink("a.txt");
来源：http://blog.hesvh.cn/Article/details/gdnchgklz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gcaxspzai.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/ggeyywgvj.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://wap.fehbvm.com/Article/details/gzepeqply.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gkligioqp.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gwlwsugyy.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.zdbjq.cn/Article/details/ggwlxevkr.sHtML

[F07] 创建目录（含多级）
来源：http://wap.hesvh.cn/Article/details/gxugdjlqe.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.share.hesvh.cn/Article/details/gyfsfkaar.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.fehbvm.com/Article/details/gyczwrsja.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.zdbjq.cn/Article/details/gqqdhfymf.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gsfmlvrgn.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.hesvh.cn/Article/details/giikdhozm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.zdbjq.cn/Article/details/gbhavldog.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.fehbvm.com/Article/details/gaiytsdoo.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fehbvm.com/Article/details/gaorlfdrg.sHtML

[F08] 遍历目录
来源：http://www.m.share.zdbjq.cn/Article/details/glccilzho.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fehbvm.com/Article/details/gvydwxjqr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.zdbjq.cn/Article/details/glxbxkfsq.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.hesvh.cn/Article/details/gnlchrqfx.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/gpuuefrek.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.hesvh.cn/Article/details/gqhktndmq.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.hesvh.cn/Article/details/gtrypqsen.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/gjgizqqol.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/gbfjzfeiu.sHtML


<!-- 参考信息 -->