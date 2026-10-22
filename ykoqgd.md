代发 wailian999

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2klbpbmbr.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2kjpqyclk.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tdaovewt.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2zhfjlwvu.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2efxisxog.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2lrvdumyf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2soiigyra.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ogmjiqpr.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2qyucgxmr.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2wxgvleoy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2nbaltrqs.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2jrnzojom.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2lsopuriu.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2dfplcbho.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2mtbeubyx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2dzpabqow.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2fuoaukqk.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2vaoqdtam.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2nppffaob.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2deqkiadk.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2btbmyofh.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2bpcdhfor.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2xtwuelqj.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2yndbqijr.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2rgifxtix.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2lfnvhaiu.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2rikbmvek.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2vskcizjo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2fealeszl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2zxwcrfrz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ugzagbmi.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2atxlbeno.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zvbsvpjn.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2ueuilebs.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mmonddvn.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2iqwycekp.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2rdrafywm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ncjozctl.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2cqubzodu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rrijnwtd.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gpetnbqx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zxmojwzb.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2seybppvk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rscebnpw.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2sjbhlose.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2fzntxbfr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2tddewlwb.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vjygdpsv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2tvyoevbf.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2lkjrkhgz.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2tnsenajo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2vsdktiea.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2yzdqqozw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2spmusqjt.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2lssbjqvm.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2rvuuudkh.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2vtfcjjxb.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2soqmsooo.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2uhxkkffl.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2eduuowro.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2xmmikyek.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2afykhcpd.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2cyoelhtv.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2ryxzdkfc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2jbtgxhol.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2nhpevzbs.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2zixzzzfw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tbifzdmy.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2xwldamdg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2gjxzrrvn.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2dcnmrtdv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ahtyuypl.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2fejszoac.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jalpeduf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2mxqqbutk.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2unrewecb.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zjatrszv.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2cuthapby.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ifgsfwxh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2yolozljr.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2nehfkrvx.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ezcgvxzz.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2zaewttzz.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2yqtwzkms.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2fukzzloo.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hslntrzv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2mbjgoxdl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2oqqtqszr.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2pcpgazmm.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ncfarznx.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2wkjlkfbs.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zkvndoyx.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2cvjjcvei.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ylkzhbnx.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2qlcqirqn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2wnkuevjt.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2eztmgpio.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2okvrcrvu.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2cqjooqmg.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zsgiasit.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2afmpcgvu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2izfxslos.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ynshtgtr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zenslnif.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2jrlvenuy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2dbfmimts.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2ncjaihmg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2nmlpfluc.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2kieytzyd.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2lxubfsxs.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2teaxymch.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2ytqeskvq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2lqaxjeld.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2txgwfwgw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2mrisqhho.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2tziwdohr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2uvxejzuw.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2wtktunez.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ulywywui.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lhxydcjw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2ammnhqzw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xrbmoyoc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2fgvwosdi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2oswtzzpw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bxikkwgh.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qpujvlfv.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2acxzidfe.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2wvvkhcvm.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2tkdldzlm.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2owtrfygl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ybbhaivm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2ocinehyp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2ladopkyc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2llihzwyf.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2dzxcrdsx.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2taeinvms.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2bogldtir.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2tkhzqtlc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2htpgsirq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2apnjpzuk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vlnnqvzv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2wpfvckix.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2mvgqemzi.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2qckdpgfi.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2knxzplff.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2xdsknppo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2plrezvia.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2nyztpoxe.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2nbuswkxi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vdelxqej.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2tpdvlpgq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2pkaxoibl.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ogvbmmsy.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ffforzfh.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2sptrgyfx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vsvonoxs.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2xbkjztuq.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2txbvhwge.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tbiqyioj.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kvfbelum.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2qhwdawcz.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2qgsbaoag.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2drtvjqqb.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2xhictgnj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2gikrcshi.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2qkpgatkf.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2bxbuhdsv.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2hxqpqjkt.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2lufukurn.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2waatyuax.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2diexmypw.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2kfeoqhbf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2njhktwew.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2phrtpdup.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dqblhsgi.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dsgfyzwl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ucmztjwt.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2hzeuyvsf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vkbwddte.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ybixxsim.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2pucsqfxk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2cukpffzl.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2tblsepki.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2uhvztrdy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wzakbare.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2rysiitbm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2rxtocscu.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2vgbnrvhu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2sgmcelhw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qrwhjddm.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2osxrmycx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pkyofkai.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2bpkxvrxh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2xnhqxopw.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nhvluesb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2icoxyghx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2yntfnbmg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2qwivvwrw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2azevkcgu.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ofjbhvmy.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2sgtrhjsu.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2zsmkywar.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2jmfnxgha.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2dbgamqya.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ytrgpfwl.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ccqolipv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2soswsibb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2vrihkvja.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2efctvnkg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2lkjjasct.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2kyqcfsen.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2rmlyrvkj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ldcjutzk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lkgataqj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2wsegczcx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2nyltxeon.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2rqvovbpq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2pdmvapeo.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2agpcxayy.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2uhjxwpst.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2hojqwzhv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2ptlzmudn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2qyxsqbpc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2nefrmajo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2yxqltrpr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2eksmcahq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2skbslogn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ojmwrftc.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2nagtxpxp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2lgzvtmee.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fnaypzhs.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gbdmflwb.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cgoeqbdy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fjxrgflx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2qgirmsen.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2txcxzdxd.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hfddgygw.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2plefeeym.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2exugpzbc.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lrmjuzoj.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jxjzosme.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bhcdqmcq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2tuvmgvga.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tqyqcvox.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jvxrekcc.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pxenmktg.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2algmgksz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2uuauafrt.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2tptmrqdi.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2speducuv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2gnmqgjpi.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2gdhruylc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2vmelseuv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2mvuhpspb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2dkrttiin.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2hywaetwj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2hndyfixm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2jevleaij.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2sdocxddk.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2blwaysdx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ncoupvzs.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2sdktxvrb.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wcsnalkl.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ltjfhtwn.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2wgsxbhoq.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2llzaritz.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ogfssigu.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2vpegdcod.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ophjkxtr.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2jtndqwyj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2yzwbadib.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2begwoobf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2rsrcqmrt.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2yowynjwz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eagyxtwa.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cmmxizhr.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qshyehhd.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gilikyyx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2vwagkygc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nbhkubdp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xkjrawea.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ldqpuvhz.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2leumdhnb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nhudwpcg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dhtwxdnf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2wafwoaya.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dslbnfik.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2goxwvdrq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2xdkzrjbz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xmxballp.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2qyneirai.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2ruddlgcu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2smgwpngd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2igztdknb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2mhbfkbdm.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2zuvzledt.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2pyjlgibo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2flaakcgh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2yblaxkyd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2urtezoaw.html


<!-- 参考信息 -->