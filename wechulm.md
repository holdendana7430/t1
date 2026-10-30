代发 wailian999

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.fehbvm.com/Article/details/grvzzplob.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://blog.zdbjq.cn/Article/details/gsuejkbko.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://www.share.fehbvm.com/Article/details/gnwyyfmtp.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://mobile.zdbjq.cn/Article/details/gbardnhzs.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://read.share.hesvh.cn/Article/details/ggzpydjvs.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://baike.hesvh.cn/Article/details/gwyewpzpc.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://m.share.fehbvm.com/Article/details/goqamoeob.sHtML

[D26] 数组转字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gieahggcr.sHtML

Py:   ", ".join(map(str, arr))
来源：http://baike.zdbjq.cn/Article/details/gpsosezwx.sHtML

PHP:  implode(", ", $arr);
来源：http://read.share.hesvh.cn/Article/details/gvezgfqug.sHtML

JS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gxkztmola.sHtML

TS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gqhymwfyk.sHtML

Java: String.join(", ", list)
来源：http://baike.fehbvm.com/Article/details/gviymtpvi.sHtML

Go:   strings.Join(strs, ", ")
来源：http://blog.hesvh.cn/Article/details/gbwpirmti.sHtML

Ruby: arr.join(", ")
来源：http://www.blog.fehbvm.com/Article/details/gcifjhydm.sHtML

C#:   string.Join(", ", list)
来源：http://wap.zdbjq.cn/Article/details/gmvvosixj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gmyjfrzab.sHtML

E. 字符串处理
来源：http://m.share.hesvh.cn/Article/details/gvthumqcn.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/ghiortpwr.sHtML

[E01] 拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gtmulldrw.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://m.share.hesvh.cn/Article/details/gseejcrpy.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://baike.zdbjq.cn/Article/details/gtcmzfqgj.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://read.share.hesvh.cn/Article/details/guaqhboju.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://blog.zdbjq.cn/Article/details/gdvvvpcbb.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://baike.zdbjq.cn/Article/details/guimvlynw.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://blog.hesvh.cn/Article/details/gudjnoiop.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.share.hesvh.cn/Article/details/gmxuepcsc.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://baike.hesvh.cn/Article/details/ggwcvvpkg.sHtML

[E02] 重复字符串
来源：http://www.m.share.fehbvm.com/Article/details/gxurntjfv.sHtML

Py:   "ab" * 3
来源：http://3g.fehbvm.com/Article/details/gwmxqatqo.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.fehbvm.com/Article/details/gnhllqfkr.sHtML

JS:   "ab".repeat(3)
来源：http://blog.fehbvm.com/Article/details/glrcuaarf.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.zdbjq.cn/Article/details/grachrsua.sHtML

Java: "ab".repeat(3)
来源：http://baike.zdbjq.cn/Article/details/gjjouxppa.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.m.share.zdbjq.cn/Article/details/gglqsnghu.sHtML

Ruby: "ab" * 3
来源：http://mobile.fehbvm.com/Article/details/ggrsofreg.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.fehbvm.com/Article/details/gwtufwzux.sHtML

[E03] 截取子串
来源：http://wap.fehbvm.com/Article/details/gknwfwvpj.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://blog.hesvh.cn/Article/details/gwoivrczh.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gtlkfgppl.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.zdbjq.cn/Article/details/gqhtgljol.sHtML

TS:   s.slice(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gvavargjg.sHtML

Java: s.substring(1, 4)
来源：http://blog.fehbvm.com/Article/details/gnpulmxmt.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.blog.hesvh.cn/Article/details/gopzhejot.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://3g.hesvh.cn/Article/details/ggrzumzgd.sHtML

C#:   s.Substring(1, 3)
来源：http://wap.hesvh.cn/Article/details/gaegacszz.sHtML

[E04] 查找子串位置
来源：http://www.blog.zdbjq.cn/Article/details/gcnjbxujr.sHtML

Py:   s.find("x");  s.index("x")
来源：http://wap.zdbjq.cn/Article/details/gmfsexogi.sHtML

PHP:  strpos($s, "x");
来源：http://www.blog.fehbvm.com/Article/details/gwbmdbyys.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://blog.fehbvm.com/Article/details/gxlkwgila.sHtML

TS:   s.indexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/garzvibmj.sHtML

Java: s.indexOf("x")
来源：http://read.share.fehbvm.com/Article/details/gabpowmlu.sHtML

Go:   strings.Index(s, "x")
来源：http://www.blog.fehbvm.com/Article/details/gwxyclqqg.sHtML

Ruby: s.index("x")
来源：http://www.share.hesvh.cn/Article/details/gcxirzldb.sHtML

C#:   s.IndexOf("x")
来源：http://blog.hesvh.cn/Article/details/gzifydydg.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.share.zdbjq.cn/Article/details/gvzhgurnr.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.share.hesvh.cn/Article/details/gmslhnufd.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://baike.zdbjq.cn/Article/details/gzvvwqjkn.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.zdbjq.cn/Article/details/gsjjpznvo.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.share.zdbjq.cn/Article/details/gfvcqpfal.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.hesvh.cn/Article/details/gzrqfmzac.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://m.share.zdbjq.cn/Article/details/gyijhdcvo.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://m.share.zdbjq.cn/Article/details/glgbevqow.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://read.share.hesvh.cn/Article/details/glaimnsaw.sHtML

[E06] 替换子串
来源：http://www.blog.fehbvm.com/Article/details/gprstcpyo.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://wap.fehbvm.com/Article/details/gtphvowzi.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.zdbjq.cn/Article/details/girgjxpar.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.fehbvm.com/Article/details/glyirjoii.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gezxnexxg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gosqdguwh.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gioayoteg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gvunezlhr.sHtML

C#:   s.Replace("a", "b")
来源：http://baike.fehbvm.com/Article/details/gqclpzrky.sHtML

[E07] 按分隔符拆分
来源：http://www.blog.hesvh.cn/Article/details/ggrfqmtmv.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.share.zdbjq.cn/Article/details/glfjxlmbb.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://wap.hesvh.cn/Article/details/ggfwqbxed.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.zdbjq.cn/Article/details/gglzobqas.sHtML

TS:   s.split(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gbgbhhgze.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.hesvh.cn/Article/details/gmmlyompf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fehbvm.com/Article/details/gejfyrfus.sHtML

Ruby: s.split(",");  s.split
来源：http://read.share.zdbjq.cn/Article/details/gjbgsxprb.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.fehbvm.com/Article/details/gcvknaerr.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.hesvh.cn/Article/details/gibpsmuhv.sHtML

Py:   ",".join(items)
来源：http://www.blog.fehbvm.com/Article/details/gwbkieiqd.sHtML

PHP:  implode(",", $items);
来源：http://www.m.share.hesvh.cn/Article/details/gitbkghqg.sHtML

JS:   items.join(",")
来源：http://3g.hesvh.cn/Article/details/gudxaorgo.sHtML

TS:   items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gipmewtum.sHtML

Java: String.join(",", items)
来源：http://m.share.zdbjq.cn/Article/details/ggkfnruoo.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.zdbjq.cn/Article/details/gvpdnjnlv.sHtML

Ruby: items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gsrwxipcl.sHtML

C#:   string.Join(",", items)
来源：http://mobile.hesvh.cn/Article/details/gxfswhres.sHtML

[E09] 去除所有空白字符
来源：http://m.share.fehbvm.com/Article/details/gslptjyra.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://wap.fehbvm.com/Article/details/gjqcasqjm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://3g.hesvh.cn/Article/details/gipngkzhk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/grouvoeot.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://3g.hesvh.cn/Article/details/gkwlhhvuh.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fehbvm.com/Article/details/gznezkdgo.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fehbvm.com/Article/details/gcmlxnrhi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.hesvh.cn/Article/details/gghqvvvnk.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/gdzusmmws.sHtML

[E10] 左侧补零 / 定长填充
来源：http://wap.zdbjq.cn/Article/details/gaittwtzs.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fehbvm.com/Article/details/gbfjfvelz.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.fehbvm.com/Article/details/gptznegqa.sHtML

JS:   "7".padStart(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gicnzmsss.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.fehbvm.com/Article/details/gdramqadg.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/gbisswckj.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/geglrrfyp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fehbvm.com/Article/details/gknleifsw.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/gvaxbsjiz.sHtML

[E11] 反转字符串
来源：http://wap.hesvh.cn/Article/details/ggxpaervp.sHtML

Py:   s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gyhhycfvc.sHtML

PHP:  strrev($s);
来源：http://www.blog.fehbvm.com/Article/details/gmibuwycr.sHtML

JS:   [...s].reverse().join("")
来源：http://wap.zdbjq.cn/Article/details/gahvcdrsj.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.hesvh.cn/Article/details/gsqyqtoki.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.hesvh.cn/Article/details/gcegrhqfl.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.hesvh.cn/Article/details/gmarokozk.sHtML

Ruby: s.reverse
来源：http://read.share.fehbvm.com/Article/details/gxrodhfcu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gpkukwyru.sHtML

[E12] 统计某字符出现次数
来源：http://baike.zdbjq.cn/Article/details/gwoalrtre.sHtML

Py:   s.count("a")
来源：http://mobile.hesvh.cn/Article/details/gzwpnzhwp.sHtML

PHP:  substr_count($s, "a");
来源：http://baike.zdbjq.cn/Article/details/gwmkllsyr.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.fehbvm.com/Article/details/giyufqckh.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/gxanewqqg.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://blog.hesvh.cn/Article/details/ganarocsc.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.hesvh.cn/Article/details/gkihbnsjl.sHtML

Ruby: s.count("a")
来源：http://baike.zdbjq.cn/Article/details/giugrianl.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.fehbvm.com/Article/details/glmevcfbs.sHtML

[E13] 逐字符遍历
来源：http://3g.hesvh.cn/Article/details/gaotfldmc.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fehbvm.com/Article/details/guueakzmr.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://blog.fehbvm.com/Article/details/gvmpatcwa.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.fehbvm.com/Article/details/gktvcnlug.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/ghnnaoezb.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.hesvh.cn/Article/details/gjbugzoma.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.zdbjq.cn/Article/details/ggxrkpfao.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.fehbvm.com/Article/details/gdttivazq.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://mobile.zdbjq.cn/Article/details/gkpdmwbed.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.fehbvm.com/Article/details/gdydromra.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fehbvm.com/Article/details/gulahtysr.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fehbvm.com/Article/details/gfiovcnmr.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://blog.fehbvm.com/Article/details/gvbewfsvb.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://m.share.hesvh.cn/Article/details/gpnhckbrc.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.hesvh.cn/Article/details/gkiocgarj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.zdbjq.cn/Article/details/gfjmlxfyl.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://wap.zdbjq.cn/Article/details/gqemtlwij.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.zdbjq.cn/Article/details/gqjjpsyzm.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.zdbjq.cn/Article/details/grpvwwtgj.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.blog.zdbjq.cn/Article/details/gcymylavy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.blog.hesvh.cn/Article/details/gtpahkpgz.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.zdbjq.cn/Article/details/gvqkcqmdf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.hesvh.cn/Article/details/gibohwvrv.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.fehbvm.com/Article/details/gmdkdzptu.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://blog.fehbvm.com/Article/details/gmlpaqywy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://read.share.hesvh.cn/Article/details/gwvjstacj.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://mobile.fehbvm.com/Article/details/gezrpguzc.sHtML

[E16] 数字千分位
来源：http://baike.hesvh.cn/Article/details/gaqkmnrsm.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/gkouflegn.sHtML

PHP:  number_format(1234567);
来源：http://wap.zdbjq.cn/Article/details/gasamdhgl.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/goviybzld.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/glzudyfea.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://baike.zdbjq.cn/Article/details/gyljkgzgu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.blog.fehbvm.com/Article/details/gvrlflkbi.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://baike.hesvh.cn/Article/details/gsplfzlsj.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.zdbjq.cn/Article/details/gfnqktlui.sHtML

[E17] 首字母大写
来源：http://wap.zdbjq.cn/Article/details/gstupukdr.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://blog.zdbjq.cn/Article/details/gywklrpxe.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.m.share.fehbvm.com/Article/details/gxfojrmcv.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/giiregddm.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/grzrcgwkh.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.hesvh.cn/Article/details/gxcznqnaz.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://baike.zdbjq.cn/Article/details/ggkwdzccz.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gwjxgypqr.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.share.fehbvm.com/Article/details/gbxncomwg.sHtML

[E18] 模板占位符替换
来源：http://www.blog.zdbjq.cn/Article/details/gbpapmkyv.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://m.share.hesvh.cn/Article/details/gynwomfys.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.share.fehbvm.com/Article/details/gvljhkuyg.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gvrhaqdcb.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gnuqjdhig.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gxadfakpx.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.share.fehbvm.com/Article/details/gkzbbfgzg.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://m.share.zdbjq.cn/Article/details/gltbmqycy.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.zdbjq.cn/Article/details/gnsxdairq.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.fehbvm.com/Article/details/gwajvfnwv.sHtML

Py:   s.splitlines()
来源：http://blog.hesvh.cn/Article/details/gdjmkvdea.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.zdbjq.cn/Article/details/godrrrflx.sHtML

JS:   s.split(/\r?\n/)
来源：http://read.share.fehbvm.com/Article/details/gxqqvelcz.sHtML

TS:   s.split(/\r?\n/)
来源：http://mobile.zdbjq.cn/Article/details/gfvbppxsv.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fehbvm.com/Article/details/gknronxcl.sHtML

Go:   strings.Split(s, "\n")
来源：http://blog.hesvh.cn/Article/details/gyqshcfjw.sHtML

Ruby: s.lines
来源：http://mobile.fehbvm.com/Article/details/gkgaxrigr.sHtML

C#:   s.Split('\n')
来源：http://read.share.fehbvm.com/Article/details/gpggxaabn.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.fehbvm.com/Article/details/gyrcszjjb.sHtML

Py:   if not s:
来源：http://m.share.zdbjq.cn/Article/details/gkjvzfoal.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.share.zdbjq.cn/Article/details/gcffykfpw.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.hesvh.cn/Article/details/gabycgqsm.sHtML

TS:   if (s === "") {}
来源：http://read.share.zdbjq.cn/Article/details/ghvapexpm.sHtML

Java: if (s.isEmpty()) {}
来源：http://m.share.hesvh.cn/Article/details/gxucwrezg.sHtML

Go:   if s == "" {}
来源：http://3g.zdbjq.cn/Article/details/gqnuhvjoq.sHtML

Ruby: if s.empty?
来源：http://baike.hesvh.cn/Article/details/gfqeeooyu.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.fehbvm.com/Article/details/gbcuyzpec.sHtML

[E21] 超长截断加省略号
来源：http://baike.fehbvm.com/Article/details/geykjmizg.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://read.share.zdbjq.cn/Article/details/gvnzxsdmf.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.fehbvm.com/Article/details/ghkwrvulq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://wap.zdbjq.cn/Article/details/ghrpnczpv.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fehbvm.com/Article/details/gpjfucxwr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/givsnmmue.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.fehbvm.com/Article/details/gocbpzmzv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gtmmtzatb.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://baike.zdbjq.cn/Article/details/gedmpnlvk.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/gwiictizm.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.fehbvm.com/Article/details/gxflcazif.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://mobile.zdbjq.cn/Article/details/gzsykomxe.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gzuiglhwy.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gtgdklovo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://baike.zdbjq.cn/Article/details/gpzgcfqlu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://mobile.zdbjq.cn/Article/details/gpyrzchnt.sHtML

Ruby: s.bytesize;  s.length
来源：http://m.share.hesvh.cn/Article/details/gjpabgjor.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.share.fehbvm.com/Article/details/gojtkbwli.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gjnolzjgg.sHtML

F. 文件与目录
来源：http://www.blog.zdbjq.cn/Article/details/gnjflojse.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/glxgxkptp.sHtML

[F01] 读取整个文件
来源：http://www.blog.hesvh.cn/Article/details/gamqoygpy.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fehbvm.com/Article/details/gqaihuypv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://3g.fehbvm.com/Article/details/gqesgjegd.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://wap.zdbjq.cn/Article/details/gvlhuwker.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.hesvh.cn/Article/details/ghsaiwizg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://mobile.hesvh.cn/Article/details/gaocayysv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.fehbvm.com/Article/details/gjtusneqe.sHtML

Ruby: File.read("a.txt")
来源：http://wap.hesvh.cn/Article/details/gbhnrvepk.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://baike.fehbvm.com/Article/details/gpkaudoly.sHtML

[F02] 逐行读取文件
来源：http://blog.fehbvm.com/Article/details/gbaoymoly.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.blog.fehbvm.com/Article/details/gwhczrqpu.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.zdbjq.cn/Article/details/gtwzuwnvj.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gxcklauci.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.zdbjq.cn/Article/details/gayjeazrm.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gctdoaswe.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.zdbjq.cn/Article/details/gfnryenbd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/gwlaphhfz.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.blog.fehbvm.com/Article/details/gniutgodw.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.fehbvm.com/Article/details/gmturdpvj.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.hesvh.cn/Article/details/gryzggudf.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gbjdqnccg.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gwezousfd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gsgsgzbaz.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.blog.fehbvm.com/Article/details/guywcmqpt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.zdbjq.cn/Article/details/gquqypzzu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.zdbjq.cn/Article/details/gfxtbofug.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.m.share.fehbvm.com/Article/details/glfueokgg.sHtML

[F04] 追加写入文件
来源：http://mobile.fehbvm.com/Article/details/glkzdlpix.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.m.share.fehbvm.com/Article/details/greekrklh.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fehbvm.com/Article/details/ggzpjqdei.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/ggfsapngb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gnxbfejxi.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.m.share.hesvh.cn/Article/details/glfgchotr.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://wap.fehbvm.com/Article/details/ghbntxpfp.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.zdbjq.cn/Article/details/gihjlnswz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.hesvh.cn/Article/details/gejuzymab.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.zdbjq.cn/Article/details/gdrprregt.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.hesvh.cn/Article/details/gyytxnxfe.sHtML

PHP:  file_exists("a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/guiegazsj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/guvlrplin.sHtML

TS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gffoddbpc.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gftbnhego.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.zdbjq.cn/Article/details/gziijoezp.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gswxjhyua.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gadqxmwlh.sHtML

[F06] 删除文件
来源：http://read.share.fehbvm.com/Article/details/gmhigczyn.sHtML

Py:   os.remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/glktvnmly.sHtML

PHP:  unlink("a.txt");
来源：http://baike.fehbvm.com/Article/details/gwhtzfrbp.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gmgphsjyt.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://wap.hesvh.cn/Article/details/gemlxuqza.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gugldoald.sHtML

Go:   os.Remove("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gwolwssla.sHtML

Ruby: File.delete("a.txt")
来源：http://baike.hesvh.cn/Article/details/grmtglfxn.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.hesvh.cn/Article/details/gciwlnrcp.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fehbvm.com/Article/details/glkjkjsda.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/gcvnyhrai.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://wap.hesvh.cn/Article/details/ggdhhkcqp.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.hesvh.cn/Article/details/ggkybuxyx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.zdbjq.cn/Article/details/gidqyiodz.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.hesvh.cn/Article/details/gxeuaaybx.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fehbvm.com/Article/details/gaipslloq.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.share.hesvh.cn/Article/details/gdimcfsjg.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.hesvh.cn/Article/details/gtsypmdxo.sHtML

[F08] 遍历目录
来源：http://www.blog.hesvh.cn/Article/details/guincnowb.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.zdbjq.cn/Article/details/gtacuwvhq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fehbvm.com/Article/details/gvskoxelh.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.fehbvm.com/Article/details/gppvzhcgq.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fehbvm.com/Article/details/gsmyueyko.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/glyblhyof.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.m.share.hesvh.cn/Article/details/gsozymbyq.sHtML

Ruby: Dir.children("dir")
来源：http://read.share.fehbvm.com/Article/details/gwoatoaof.sHtML

C#:   Directory.GetFiles("dir")
来源：http://blog.fehbvm.com/Article/details/gxcgvzrbr.sHtML

[F09] 获取文件大小
来源：http://blog.hesvh.cn/Article/details/gtszrsuty.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gpqvrdnst.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fehbvm.com/Article/details/glgisaxgz.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.zdbjq.cn/Article/details/gqnqyrlzq.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.share.fehbvm.com/Article/details/gpxrumijm.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gerxdhswi.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.hesvh.cn/Article/details/gmpauiphf.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gduqwbhut.sHtML


<!-- 参考信息 -->