代发 wailian999

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nqxjzmcl.html

E. 字符串处理
来源：http://www.ydjk.org.cn/Article/details/gt3dthitnzt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vmttdywq.html

[E01] 拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3krsebcaj.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3mreptqvx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.52xcode.cn/Article/details/gt3azqzlcwn.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3dfsbpbzb.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jjrumjjs.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.52xcode.cn/Article/details/gt3vrngjqof.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vxwecrzh.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3nakpgdyy.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3msmxkxfm.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3edffmcmu.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3hmwkwgox.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt3pegrolue.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ybglecyx.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3aukilyre.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3yphixatb.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3clhbcxle.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3zlhfpqqg.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3nujrbeot.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3bvrpkvjh.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3bcnztard.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jtqacuam.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dtktjjdd.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3yjqghabh.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3hvpslexr.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3vraacjpz.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3oemzotso.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3apyglgpd.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3hbyvmpfo.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xpywcttl.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3fzadvldo.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3uqplzpyi.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3qonnosuj.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3knnkmchq.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3jnwukrcp.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3kksijxju.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3umhlswso.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3xdeetgqp.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ivjfldoe.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3sjoecisn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3wvtidrxn.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3cqfzwmqd.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3owwgotcp.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3fkgpwruq.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3ckzumgas.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vnvviwfi.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3eqheiijx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3nyknaigv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3vdbrueom.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hubzceca.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3asuivgeq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pmsozbbi.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zgeprijx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3bwovstdb.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xsvkdsza.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3cndoqzub.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3dhyeqqcm.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bmgecuyc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3qenrpfro.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3yeudggxe.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3pzkkyozt.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3ihvzcxhi.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3tcydqzqi.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3qdgjlmht.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3qzawvpsu.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3gsnymjof.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3mjhzqjex.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3urhcxksn.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3xmtbtdqw.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3lvcrbsbo.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3rjiqzcqm.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bfffgjxu.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3lwbvfrdj.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3grdrteno.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3quemcfhi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3jrntbnrs.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3igiyjgkk.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3qpeurkbl.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3cqofzgis.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3klaqhdkv.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3walklolb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3kjstmxfn.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3qujntrpb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ikaiifav.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3pdhsddia.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ngnkqidz.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3jtsbdrwo.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3euswxrwy.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3oufjakzr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3pbpmdifh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3wepffxxp.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3dblmvffs.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3bgtynqlu.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3axgvdwvx.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3afnqffla.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3kjwumhct.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3ghxikffe.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3vuwiomkc.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3qmjhpnnf.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3thvmeqgb.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3vcfdvhit.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xqhqyuoo.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3rzskycdu.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3kkinbmkh.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3xelkyxru.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3qllbdwtu.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3mlvlmfgv.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xzceufqu.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3fxfvmffc.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3uuaxvubf.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3bukpauvx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3vwsdlxfa.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3uixoijnn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ejdjetcf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jjttclyr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3uxbvqjlo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3scrlhewu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3tzhenmkm.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3iurvqvbh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ixacvdkx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3fghkpcra.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3bfgcqviu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3otipsbzf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3xokgafxh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3ywbpmrqz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3ptgcrsug.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3fvstxqcl.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3pnvpbpmk.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3wytpyyrg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3shniyuiw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aasfgnoa.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3mxookggf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3thqfiokg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vsjfahgs.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3nqcxvxrc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xcwkzydg.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3etnksunb.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3zgjjxkck.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3tlhkyrnz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3bupmrpge.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3zbddtxoi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3layeejux.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3bqdfdbql.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3koejfltj.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3ctghcpwx.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3lxzwdekn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3qdetvelh.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3okcukerv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dhnrcsdj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3lqenaqpa.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3orufbbze.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3uxyxkgpb.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3gkwossbc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3rnggibqj.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3jlzlbgoz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3hpyucgjq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3gnhocwyk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3htukukpg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ukynwpck.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3uancpqci.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3lwddsmyj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3gxdjafac.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3bwzidizi.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ycudyyef.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3mvsyhosd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xrehyapc.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3ofwayxcx.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3jchgevxw.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3odnyrmbf.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3cacwineq.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3wzbuyubp.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3mscjmgex.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3metkgrqp.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3idxjzpge.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3mwvdxpza.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ithaaakm.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3bgxfekla.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3xmryxazg.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3zufnohcu.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3hhblavks.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3duuauxce.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3iukkmpxo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3rxhtgesa.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3qvrwaabp.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3pvdheczn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bzqwrhwj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3bgkprgmi.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3jejashmt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dzdyyvij.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3emrruyus.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3nofepyct.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3hgzecjvg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3tmynjlth.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3teajidyq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3eclocffd.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ihkrlgod.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3betsgrlb.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3jpvouugj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ikmekukr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oxnpklth.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3cjokkjsg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ekqtcfod.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3zliedawb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3oxcpobwi.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fgkmgphb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3csmbvxft.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3xwpieglb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rlpdmjfg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3aghwczlu.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3awgcrfqv.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ygzvxmjs.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3olsyylvp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3jpfflugb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3kagvsjyk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vybnahcl.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qvipxymp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3mrbzvwsn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3erhqrhyt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3rxzneaxd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3olazboft.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3xonywrdo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3kycnwiex.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3mypfxzoy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3lzrzkysd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ujjiydhu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3wuxlmehz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3fydgqtyi.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3gezdqgti.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3giogextz.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3ozpuzzod.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3jdoguqcb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3osrhrjxs.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3egljonnj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zkkzzwtu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3odgclqri.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3eiljxigl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3wgtyvcvn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3nazybuvn.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3psytoygx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3xuomgpzl.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3txkwyoim.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ozlwcspn.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wvemxwkm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ffpymbza.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3vpupkhzv.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mwtaaijf.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vzszxvst.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3hzgwjnaj.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3paweoydq.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3stgzhkad.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xmrphhvg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lsnfmscu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kheqwwsl.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ceckoyaw.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ckwbiqgy.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ypvjloze.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3cqapgnkg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3hpecmzvb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3fecnewuv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3lztyyfkp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3crhqbeql.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3jebqaoyo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3owreavpm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3szivravw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3bhivsayf.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3jnysgiwp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3qndfuibf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3phparfpt.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3qfkdwcvr.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ylxtppyl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ctwxjjwc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fvleybiy.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3jvcpgiyb.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3nbeauntx.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3xtehlwvg.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zzbnhlsk.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3khqbsdnc.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3cogekjxp.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ueyczuxy.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xmrpbtuo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3ijnozkwj.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ipyalulb.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3zrhqowlp.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3sgtlvowz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3flvxivdi.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3orbeohmw.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xgefggor.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3irjbztrn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3xrtrhiio.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lfhpcapn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jhyrqdoo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xvvjtien.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3gqtmxnhf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hhthyera.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tyuaujed.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3udncrpma.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qhqgxhbr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3zcxygziu.html


<!-- 参考信息 -->