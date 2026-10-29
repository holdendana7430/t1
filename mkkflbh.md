代发 wailian999

Ruby: h["k"] = 1;  h["k"];  h.key?("k");  h.delete("k")
来源：http://read.share.zdbjq.cn/Article/details/gvbruxnjk.sHtML

C#:   dict["k"] = 1;  dict.TryGetValue("k", out var v);  dict.Remove("k");
来源：http://www.blog.zdbjq.cn/Article/details/gdkvbfyiz.sHtML

[D25] Set 集合去重与交并差
来源：http://www.share.fehbvm.com/Article/details/gfwxkgngo.sHtML

Py:   s = {1, 2, 3};  s | {3, 4};  s & {2};  s - {1}
来源：http://www.blog.zdbjq.cn/Article/details/goovhjgag.sHtML

PHP:  // 无原生 Set：用数组键或 SplObjectStorage 变通
来源：http://mobile.zdbjq.cn/Article/details/gvyoppbqn.sHtML

JS:   const s = new Set([1, 2, 3]);  s.add(4);  s.has(1);  s.delete(1)
来源：http://3g.hesvh.cn/Article/details/gmmpistwq.sHtML

TS:   const s = new Set<number>([1, 2, 3]);
来源：http://m.share.zdbjq.cn/Article/details/gatbzbfxn.sHtML

Java: var s = new HashSet<>(List.of(1, 2, 3));  s.add(4);  s.contains(1)
来源：http://www.m.share.zdbjq.cn/Article/details/ggwklgkxi.sHtML

Go:   // 无原生 Set：用 map[int]struct{}
来源：http://baike.fehbvm.com/Article/details/gmpbckuwi.sHtML

Ruby: s = Set[1, 2, 3];  s.add(4);  s.include?(1)
来源：http://m.share.fehbvm.com/Article/details/gvewmvmin.sHtML

C#:   var s = new HashSet<int> { 1, 2, 3 };  s.Add(4);  s.Contains(1)
来源：http://mobile.hesvh.cn/Article/details/geiznmwvj.sHtML

[D26] 数组转字符串
来源：http://www.blog.hesvh.cn/Article/details/glojmcyqg.sHtML

Py:   ", ".join(map(str, arr))
来源：http://wap.zdbjq.cn/Article/details/gnwpuztkw.sHtML

PHP:  implode(", ", $arr);
来源：http://m.share.hesvh.cn/Article/details/ggobhadbp.sHtML

JS:   arr.join(", ")
来源：http://blog.hesvh.cn/Article/details/gufgdmfim.sHtML

TS:   arr.join(", ")
来源：http://wap.hesvh.cn/Article/details/gftjwfizk.sHtML

Java: String.join(", ", list)
来源：http://www.m.share.fehbvm.com/Article/details/gcbcfmqtr.sHtML

Go:   strings.Join(strs, ", ")
来源：http://wap.hesvh.cn/Article/details/gdrupqytp.sHtML

Ruby: arr.join(", ")
来源：http://3g.hesvh.cn/Article/details/gnperselb.sHtML

C#:   string.Join(", ", list)
来源：http://mobile.zdbjq.cn/Article/details/gaxrpytdq.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/goxrvpodr.sHtML

E. 字符串处理
来源：http://3g.hesvh.cn/Article/details/gowkhwleg.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqfexwxup.sHtML

[E01] 拼接字符串
来源：http://www.share.zdbjq.cn/Article/details/gxlybwtql.sHtML

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://blog.zdbjq.cn/Article/details/gjigrfvjq.sHtML

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.blog.zdbjq.cn/Article/details/grhzulxts.sHtML

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gwvulzkzi.sHtML

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://3g.fehbvm.com/Article/details/gtvubedow.sHtML

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://blog.hesvh.cn/Article/details/gpgvmofwv.sHtML

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.m.share.fehbvm.com/Article/details/gvevjuixa.sHtML

Ruby: "a" + "b";  ["a", "b"].join
来源：http://read.share.zdbjq.cn/Article/details/grtunwody.sHtML

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gxrakfial.sHtML

[E02] 重复字符串
来源：http://baike.zdbjq.cn/Article/details/gzbwwbjfj.sHtML

Py:   "ab" * 3
来源：http://m.share.fehbvm.com/Article/details/glqvlxvug.sHtML

PHP:  str_repeat("ab", 3);
来源：http://www.blog.hesvh.cn/Article/details/ggnxpjtyi.sHtML

JS:   "ab".repeat(3)
来源：http://www.share.zdbjq.cn/Article/details/gfzzcvvex.sHtML

TS:   "ab".repeat(3)
来源：http://read.share.fehbvm.com/Article/details/gdqpensbq.sHtML

Java: "ab".repeat(3)
来源：http://blog.zdbjq.cn/Article/details/gzfblxmgi.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://baike.hesvh.cn/Article/details/gufsnztrz.sHtML

Ruby: "ab" * 3
来源：http://read.share.fehbvm.com/Article/details/ghlruqhju.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://read.share.zdbjq.cn/Article/details/gkjzvwwzo.sHtML

[E03] 截取子串
来源：http://m.share.fehbvm.com/Article/details/glvvsxypn.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://wap.fehbvm.com/Article/details/gtlbwwnlo.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.blog.hesvh.cn/Article/details/gkvlbuftx.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://baike.zdbjq.cn/Article/details/gmdpyjbra.sHtML

TS:   s.slice(1, 4)
来源：http://read.share.hesvh.cn/Article/details/gclfsffgv.sHtML

Java: s.substring(1, 4)
来源：http://3g.fehbvm.com/Article/details/ghxxgcknm.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://blog.hesvh.cn/Article/details/gnwrvmwar.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://read.share.zdbjq.cn/Article/details/gixzfijur.sHtML

C#:   s.Substring(1, 3)
来源：http://www.share.hesvh.cn/Article/details/gevntzlut.sHtML

[E04] 查找子串位置
来源：http://wap.fehbvm.com/Article/details/gklfaltfw.sHtML

Py:   s.find("x");  s.index("x")
来源：http://mobile.zdbjq.cn/Article/details/gkhxtvewz.sHtML

PHP:  strpos($s, "x");
来源：http://mobile.hesvh.cn/Article/details/gsxojlsux.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://baike.fehbvm.com/Article/details/gpagjoyst.sHtML

TS:   s.indexOf("x")
来源：http://blog.zdbjq.cn/Article/details/gnytbevqs.sHtML

Java: s.indexOf("x")
来源：http://www.share.zdbjq.cn/Article/details/gyvjqlowk.sHtML

Go:   strings.Index(s, "x")
来源：http://mobile.hesvh.cn/Article/details/gawevkjco.sHtML

Ruby: s.index("x")
来源：http://baike.hesvh.cn/Article/details/gfyywrwum.sHtML

C#:   s.IndexOf("x")
来源：http://www.blog.fehbvm.com/Article/details/gevzhnabr.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://mobile.fehbvm.com/Article/details/gcjnmzgup.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.blog.fehbvm.com/Article/details/gleycoihy.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://m.share.fehbvm.com/Article/details/gnhavvsgl.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.share.zdbjq.cn/Article/details/gpsrcckog.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://3g.fehbvm.com/Article/details/ggxpuvtqd.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://baike.fehbvm.com/Article/details/gegcrvyxv.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://blog.fehbvm.com/Article/details/gjkxxecyp.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://blog.fehbvm.com/Article/details/gzrlplxrw.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.share.fehbvm.com/Article/details/ghcibvmpr.sHtML

[E06] 替换子串
来源：http://read.share.fehbvm.com/Article/details/gmijbirag.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gvocwvmfs.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.fehbvm.com/Article/details/gwmtlmqxb.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://3g.zdbjq.cn/Article/details/gzcvdiqah.sHtML

TS:   s.replaceAll("a", "b")
来源：http://wap.hesvh.cn/Article/details/goaderujb.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.fehbvm.com/Article/details/gnrlvzfhd.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://baike.hesvh.cn/Article/details/gelcihcpe.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gopgyqjhw.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.fehbvm.com/Article/details/gojnoisgo.sHtML

[E07] 按分隔符拆分
来源：http://wap.fehbvm.com/Article/details/ghhzcvlza.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.fehbvm.com/Article/details/gdnextemu.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.hesvh.cn/Article/details/gsnfweczi.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.m.share.hesvh.cn/Article/details/gtjihkrms.sHtML

TS:   s.split(",")
来源：http://mobile.zdbjq.cn/Article/details/gnontoqvg.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.share.hesvh.cn/Article/details/gaqefkedf.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.fehbvm.com/Article/details/gmquzxdis.sHtML

Ruby: s.split(",");  s.split
来源：http://www.share.fehbvm.com/Article/details/gzwhzrrqc.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.zdbjq.cn/Article/details/glelpyrxk.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fehbvm.com/Article/details/gvhbfvwhc.sHtML

Py:   ",".join(items)
来源：http://www.blog.hesvh.cn/Article/details/gwgcnrpax.sHtML

PHP:  implode(",", $items);
来源：http://blog.zdbjq.cn/Article/details/gbvtehwhm.sHtML

JS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/grdunvpye.sHtML

TS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gfxilrxkh.sHtML

Java: String.join(",", items)
来源：http://wap.fehbvm.com/Article/details/grwdgnhtf.sHtML

Go:   strings.Join(items, ",")
来源：http://3g.hesvh.cn/Article/details/gbxtpwmfs.sHtML

Ruby: items.join(",")
来源：http://mobile.fehbvm.com/Article/details/ggdcsvpzz.sHtML

C#:   string.Join(",", items)
来源：http://wap.hesvh.cn/Article/details/ggyprhsoy.sHtML

[E09] 去除所有空白字符
来源：http://m.share.hesvh.cn/Article/details/gyvphfhoe.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.hesvh.cn/Article/details/gqhdvskzw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.m.share.hesvh.cn/Article/details/gevkxofpj.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://www.m.share.hesvh.cn/Article/details/gytfukprj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.zdbjq.cn/Article/details/ghdpvnuss.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://blog.fehbvm.com/Article/details/gsbdfwgpz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.fehbvm.com/Article/details/ginkzkrhh.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://3g.fehbvm.com/Article/details/guoptshtl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://m.share.hesvh.cn/Article/details/ghsrojisd.sHtML

[E10] 左侧补零 / 定长填充
来源：http://www.share.zdbjq.cn/Article/details/gpobjobed.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gkvknqarp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://baike.fehbvm.com/Article/details/gxkcollbg.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/glfkxteha.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.zdbjq.cn/Article/details/gyyzmhjfl.sHtML

Java: String.format("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gdrvbqmct.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/gyctfenfi.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://wap.fehbvm.com/Article/details/gsvwfqqpd.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.blog.zdbjq.cn/Article/details/gitfqzffa.sHtML

[E11] 反转字符串
来源：http://www.m.share.hesvh.cn/Article/details/gzkfxekpm.sHtML

Py:   s[::-1]
来源：http://www.m.share.zdbjq.cn/Article/details/gwzsypilg.sHtML

PHP:  strrev($s);
来源：http://3g.fehbvm.com/Article/details/gxfbntpmj.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gidixukho.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.hesvh.cn/Article/details/gdvjmebxa.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.zdbjq.cn/Article/details/gdizdqxob.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.fehbvm.com/Article/details/gtklvrdqh.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/ghqmknbct.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://mobile.zdbjq.cn/Article/details/gdefkmjec.sHtML

[E12] 统计某字符出现次数
来源：http://baike.fehbvm.com/Article/details/ghnnkkbev.sHtML

Py:   s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/ghghgvkdk.sHtML

PHP:  substr_count($s, "a");
来源：http://m.share.fehbvm.com/Article/details/gpknorgkk.sHtML

JS:   s.split("a").length - 1
来源：http://blog.zdbjq.cn/Article/details/gnsiuvuzi.sHtML

TS:   s.split("a").length - 1
来源：http://blog.hesvh.cn/Article/details/gxuxkmnwc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fehbvm.com/Article/details/gaplzkuqx.sHtML

Go:   strings.Count(s, "a")
来源：http://read.share.hesvh.cn/Article/details/grvmkrhty.sHtML

Ruby: s.count("a")
来源：http://blog.zdbjq.cn/Article/details/gpihujcfb.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.hesvh.cn/Article/details/gjapcydez.sHtML

[E13] 逐字符遍历
来源：http://wap.hesvh.cn/Article/details/geophcaqc.sHtML

Py:   for ch in s: print(ch)
来源：http://www.m.share.fehbvm.com/Article/details/gfujgbpbc.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.zdbjq.cn/Article/details/gdljztpmo.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://blog.zdbjq.cn/Article/details/gssmmvkmv.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gmmotbfvh.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://m.share.fehbvm.com/Article/details/grfuegiqb.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.zdbjq.cn/Article/details/giuaagahh.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.hesvh.cn/Article/details/ghlzgzcac.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.fehbvm.com/Article/details/gztehhclc.sHtML

[E14] URL 编码与 Base64
来源：http://www.share.hesvh.cn/Article/details/girvhnddo.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://read.share.fehbvm.com/Article/details/gxsfuaboy.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://m.share.fehbvm.com/Article/details/gvejipexv.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://wap.fehbvm.com/Article/details/gwttkrwma.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fehbvm.com/Article/details/gxfzhdqax.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.hesvh.cn/Article/details/gtdghopcm.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.fehbvm.com/Article/details/ghrxohitt.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/gtstytipx.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.hesvh.cn/Article/details/gywmsdane.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.zdbjq.cn/Article/details/goeldlcvm.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.hesvh.cn/Article/details/gaaebmhgs.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fehbvm.com/Article/details/gqyiocuqu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fehbvm.com/Article/details/gknuiurks.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://baike.hesvh.cn/Article/details/gnobxfpoc.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fehbvm.com/Article/details/gmihyjkex.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.zdbjq.cn/Article/details/gcyqrunur.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://wap.zdbjq.cn/Article/details/gqpqlpbhn.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.zdbjq.cn/Article/details/ggwzqxhar.sHtML

[E16] 数字千分位
来源：http://www.share.fehbvm.com/Article/details/gbagfbnzd.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/gnsywavyj.sHtML

PHP:  number_format(1234567);
来源：http://mobile.zdbjq.cn/Article/details/gvwyvjqnl.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://mobile.fehbvm.com/Article/details/gvhleqjxm.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.share.hesvh.cn/Article/details/gzwsmxprx.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://wap.hesvh.cn/Article/details/gpjysvifw.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://read.share.fehbvm.com/Article/details/gjtdgokjg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.share.hesvh.cn/Article/details/gdnrzvtbb.sHtML

C#:   1234567.ToString("N0")
来源：http://m.share.hesvh.cn/Article/details/gpmekclni.sHtML

[E17] 首字母大写
来源：http://www.m.share.hesvh.cn/Article/details/gzfjwbykq.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.zdbjq.cn/Article/details/gskazgpfp.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.zdbjq.cn/Article/details/ghrrjpsvz.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.share.hesvh.cn/Article/details/gcyakmaxn.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://baike.zdbjq.cn/Article/details/gcfhtglvx.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.m.share.fehbvm.com/Article/details/ggwsjxjfo.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.share.zdbjq.cn/Article/details/gagqakett.sHtML

Ruby: s.capitalize
来源：http://www.blog.zdbjq.cn/Article/details/gqhbboxgz.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/gxxbqtihz.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fehbvm.com/Article/details/gyovemybu.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fehbvm.com/Article/details/gbqmvbvwq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.fehbvm.com/Article/details/guyvwywsf.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.zdbjq.cn/Article/details/gjlugvpvm.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gdegdkloa.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gakqhywvy.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.zdbjq.cn/Article/details/gbmbwdxvl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.zdbjq.cn/Article/details/gllghxbjj.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://m.share.fehbvm.com/Article/details/gnmkwigpx.sHtML

[E19] 多行文本按行拆分
来源：http://3g.hesvh.cn/Article/details/gnqzpghra.sHtML

Py:   s.splitlines()
来源：http://www.blog.zdbjq.cn/Article/details/gbzqjmojh.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.hesvh.cn/Article/details/gukmdmbnw.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.blog.fehbvm.com/Article/details/gxrmyoxju.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fehbvm.com/Article/details/gcgcmrtvf.sHtML

Java: s.lines().toList()
来源：http://read.share.hesvh.cn/Article/details/gxaqnwpcr.sHtML

Go:   strings.Split(s, "\n")
来源：http://baike.hesvh.cn/Article/details/gnfhmflxi.sHtML

Ruby: s.lines
来源：http://www.blog.hesvh.cn/Article/details/gpjspnkid.sHtML

C#:   s.Split('\n')
来源：http://3g.hesvh.cn/Article/details/gibsnuwxv.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fehbvm.com/Article/details/guvjotlll.sHtML

Py:   if not s:
来源：http://www.blog.zdbjq.cn/Article/details/gzirshtpm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.m.share.fehbvm.com/Article/details/gvuoxuujc.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://baike.zdbjq.cn/Article/details/gxfqmxdyz.sHtML

TS:   if (s === "") {}
来源：http://www.share.zdbjq.cn/Article/details/gtkjadfoa.sHtML

Java: if (s.isEmpty()) {}
来源：http://mobile.fehbvm.com/Article/details/gnobdrlfs.sHtML

Go:   if s == "" {}
来源：http://mobile.zdbjq.cn/Article/details/glpxfowxc.sHtML

Ruby: if s.empty?
来源：http://read.share.fehbvm.com/Article/details/gdktdonpi.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.share.zdbjq.cn/Article/details/gymfkecrl.sHtML

[E21] 超长截断加省略号
来源：http://mobile.hesvh.cn/Article/details/guhxzoqhk.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://baike.zdbjq.cn/Article/details/gnturzscs.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/gisnfpyoq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/ggpceelfp.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.fehbvm.com/Article/details/gywertsvr.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/grtttwqhm.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.m.share.zdbjq.cn/Article/details/gmngfohdh.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.blog.zdbjq.cn/Article/details/gkuvedpds.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gdmcwcdnd.sHtML

[E22] 字节长度与字符长度
来源：http://baike.fehbvm.com/Article/details/gcknfmwbf.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.hesvh.cn/Article/details/girngcgth.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.zdbjq.cn/Article/details/gusssnrun.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.zdbjq.cn/Article/details/gckqpjqrb.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/gukjddfne.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://3g.zdbjq.cn/Article/details/gkimhafnk.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://wap.zdbjq.cn/Article/details/gtwjhrcov.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.fehbvm.com/Article/details/gxawkmsmv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fehbvm.com/Article/details/ghqxoxpii.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gmvvpmyul.sHtML

F. 文件与目录
来源：http://baike.hesvh.cn/Article/details/gzaabyjxg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gaxsumeoz.sHtML

[F01] 读取整个文件
来源：http://baike.hesvh.cn/Article/details/gbhtfuoke.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.zdbjq.cn/Article/details/gmybtagyx.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.zdbjq.cn/Article/details/glbaglbjh.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.hesvh.cn/Article/details/gqsqvgzws.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.hesvh.cn/Article/details/gobkszfsj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.zdbjq.cn/Article/details/gpnmpccvm.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/gisypmizb.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gkclbyzwm.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://wap.fehbvm.com/Article/details/gipaamvan.sHtML

[F02] 逐行读取文件
来源：http://m.share.zdbjq.cn/Article/details/gkjonjrup.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://read.share.zdbjq.cn/Article/details/gylprfejl.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fehbvm.com/Article/details/graqqptwh.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gttbcrntv.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.hesvh.cn/Article/details/glypxluyt.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.share.fehbvm.com/Article/details/gmglrzifl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.hesvh.cn/Article/details/gtwahrzmv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://baike.fehbvm.com/Article/details/gehbywbod.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.fehbvm.com/Article/details/gmhhdxtfc.sHtML

[F03] 写入文件（覆盖）
来源：http://m.share.zdbjq.cn/Article/details/gfvzujnla.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://mobile.zdbjq.cn/Article/details/gqcoovwzu.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://blog.fehbvm.com/Article/details/gjdqfavok.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fehbvm.com/Article/details/gsbeextap.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.hesvh.cn/Article/details/gdbmhlfin.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.hesvh.cn/Article/details/gpjyqcyjt.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.zdbjq.cn/Article/details/ghpysmnpu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.hesvh.cn/Article/details/gsaztijwl.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/gmdvcbhsz.sHtML

[F04] 追加写入文件
来源：http://read.share.zdbjq.cn/Article/details/gadpvsnrw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.hesvh.cn/Article/details/gybofetij.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.hesvh.cn/Article/details/gydykxsmz.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://read.share.zdbjq.cn/Article/details/gwcmgufxi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.zdbjq.cn/Article/details/gcgyezcym.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.zdbjq.cn/Article/details/gkskzfcbm.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.hesvh.cn/Article/details/gwfzxjogo.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.hesvh.cn/Article/details/gqzerpnkv.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://blog.hesvh.cn/Article/details/gqyroivhh.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.hesvh.cn/Article/details/gayeidepf.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.fehbvm.com/Article/details/gmhrufnhi.sHtML

PHP:  file_exists("a.txt");
来源：http://blog.hesvh.cn/Article/details/gnufwqtgv.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gjofkkoab.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gzhyqmzig.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/gaownumgf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.hesvh.cn/Article/details/giglvowez.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.share.fehbvm.com/Article/details/gaxwlwfim.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gptnekqtv.sHtML

[F06] 删除文件
来源：http://read.share.fehbvm.com/Article/details/gmbllxrgg.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gkpbyqini.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/ghfeiourn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gkgnwgmkh.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gqexxfnqr.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/giehoqrig.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.hesvh.cn/Article/details/gmsdphgrd.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.hesvh.cn/Article/details/gmiwjlgbc.sHtML

C#:   File.Delete("a.txt");
来源：http://www.share.hesvh.cn/Article/details/gzeuxvvgf.sHtML

[F07] 创建目录（含多级）
来源：http://m.share.fehbvm.com/Article/details/gipbfuijx.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://wap.fehbvm.com/Article/details/geeyzipek.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://baike.fehbvm.com/Article/details/gbkmoeakq.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.blog.zdbjq.cn/Article/details/glzhgrpyr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.fehbvm.com/Article/details/gbcpzmyha.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.fehbvm.com/Article/details/gddujpaml.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.hesvh.cn/Article/details/gbgtabuam.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.hesvh.cn/Article/details/gzaddylxe.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.hesvh.cn/Article/details/grdcmmutr.sHtML

[F08] 遍历目录
来源：http://www.share.zdbjq.cn/Article/details/gdqstkjxy.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://3g.hesvh.cn/Article/details/gxotdwzyr.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.zdbjq.cn/Article/details/glgqyxjhl.sHtML

JS:   fs.readdirSync("dir")
来源：http://m.share.zdbjq.cn/Article/details/gxcstymlx.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.zdbjq.cn/Article/details/ggfwyjxzu.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://wap.zdbjq.cn/Article/details/ghrdkzrpi.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.blog.fehbvm.com/Article/details/gohemnebn.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/gysmkrkbh.sHtML

C#:   Directory.GetFiles("dir")
来源：http://mobile.zdbjq.cn/Article/details/gxkcyrwcc.sHtML

[F09] 获取文件大小
来源：http://3g.hesvh.cn/Article/details/gluphgudv.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/ggumkozxm.sHtML

PHP:  filesize("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/gxyjxpmzw.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.hesvh.cn/Article/details/gtjetxzpn.sHtML


<!-- 参考信息 -->