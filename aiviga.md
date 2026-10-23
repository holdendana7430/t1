代发 wailian999

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zijerqql.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3xkkdushl.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3lsumabau.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zblvyaql.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ljdmkggx.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3qyiqwoqg.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3hmlrtjwd.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3zdyrtlhc.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3njdyfszq.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3dkhuulij.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3oyofxnva.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bwomeved.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3lwlpdmhp.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3aiivcmfm.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3uqjyauct.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3xmnuzgfe.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3buhywscy.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3cmtksmph.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3pikmcspu.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3toryvvte.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3vheumbmp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3hdgdiegh.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3vnpzvfmh.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3gxhmjwjo.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3kkioowfl.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3qhjlwgdh.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3uahbklbl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3mcyitwuf.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3opoxssgx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3kayvrdhf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ftbddehw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3aeuvzymw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3tmdhsrui.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3zwoudvpp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3rbhnzgws.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3vkvconoi.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3qvkhihgl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ixlerchr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3vfuhetpr.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zznnnxkk.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qtgsaaqx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3owshzlqi.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3tocpbgyw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kxgwzskq.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qhucecvk.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3yizdbrys.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3yaqfcgxq.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3pusnbsmm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3fcwluvrw.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3gnyqxevw.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3nkuzetcj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3wtyrtzyx.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3thpecijx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3ksnxjxop.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3vwafpniv.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3dqtmztfv.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3cocjodcd.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3oopddsct.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3swjyvulk.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3nypqybfp.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3xnmhtllh.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3eeebhrei.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3kmjzdooj.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3spqpqcki.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3qxdezcoo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3yaviucqa.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xvbvvipv.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3usulspft.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3hmbmtemr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3mxjxwusq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3ingskjde.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3hrrmkpuu.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3xxbdxflx.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3budimriu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3qaehdwwh.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3rgsmetzt.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3febsuwdq.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3eiculssk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xyyfnyyo.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3lilmgkiv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3nqslrlbj.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3peyibfen.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3busiqlsd.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ocbupthx.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ucijkgly.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3wqtiuogh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3kabaxtqa.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3sgkfeper.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ysweqhte.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3xuqajifx.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3jaaxjkjk.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3kdeloazn.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3bkeuvcqv.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3rcqanncf.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3drwtneui.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3ajewxolx.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3wshgtoka.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3dsftzgqn.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3gegfctib.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3yghepsoj.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3mkuufbat.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3omqixqwz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3swunzkvh.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3embfytti.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3hpvlnyms.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rnasmdjc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3wtvmibhz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3hvuftreb.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3jffmacux.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3dnerkzrh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3jxhtzbhm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3iopwssdq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aqrkpihr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3mbpvdjkp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3uobzkpjd.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3qudchbni.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3sjmpvigh.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3fdanjqvh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3efzveulq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3vhrdldix.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3ptiaotfa.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3snvhkyfk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3bkrdypls.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3cfqxkyaf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qirmjwiu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3udscbelh.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3bfidqhup.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3cqcgmfps.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3eigukagp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3xaxgbkhe.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ntbphnta.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3qinmttxn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3laazrfoc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3jxfrokrz.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3yncctpqa.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3jbciwdda.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3usiieeus.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lisklckz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3gbluhmtv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vceiwdkk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3juxzajzr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3zsrlmqad.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3fdhcfbvg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3hckwzczu.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3qhedsqam.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3bzdhdtuy.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3pyzmwydd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3oorligep.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3yaqsouja.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qrmdzukj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3szbnjxpq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3bvfjqtlf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3xwnwykur.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3lajokmhz.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3qmviwehu.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ihetbkbt.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3nkqfdjdf.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3lpahwnrg.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3xmlxiihf.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3bloozpeu.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3idjwzvap.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3scinppkr.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3njadqgkp.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3luulhlei.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3nemlkuyy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nxhgkkrx.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3wnqtzqkj.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pnkgyttb.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3noqqnvbe.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3zvuffcrz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3odoxcqcy.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3slopqieq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3oxumlcle.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vwjdysqz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3fbwsyuzl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3posupbsw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3bmzdurqt.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3jmzscqyh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3kqfuxxjs.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dlpvojiu.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3fwrqfawk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3bhbhelnk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jwctllzl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3cvsqqbcc.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vwyvrgnj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3pjbcthzd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3sxucfsns.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3aanyqsyi.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3jkpwbqjb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vznunbzs.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3hbiibggp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fddmebwd.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3urwwlahs.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3lpvqbglr.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hjvnnkog.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3vknjmydx.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3mqcpoyjt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3uiyomktx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3oindlkyy.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ugaulaax.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3plohsycr.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3kqlwdahy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3ouymilym.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3shqjtkxy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ytxctvxk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3xjkrrldl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3rsmwywsu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3wjfamouf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3wypskbag.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3esmvogxg.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3jcsjetes.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3jbvbparh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3eosuykhr.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3odbykiar.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3xqubqhsu.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3wpdpayeq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3jaawqdmf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3eklmspfv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3knihweut.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3orerzmyt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zzebgvyj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3uyxhpwfo.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3fzpsvuph.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3qqmxiexe.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3foylrxqb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3uqhqdfmo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3inrlwfgh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3sjxvcgwv.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3pryzhvjy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3eouwbflx.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dtzigxgw.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zrodgszs.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3acszykmj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3bjcvrrgv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3xsfankoc.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kenyibqx.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sroiawwe.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3irvfwbjx.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iwzowytl.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rbgdcfgq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lpsmhqat.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jynkjnyu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3srpzbzfh.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qwcdthvj.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dwyydpbh.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kmxacnva.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3thifyxmv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3rrvwbjwq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3tnmwinia.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3begthjbe.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3zddohsil.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3ciyrdyzk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3cqauswjn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3sndfinkk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3vtsyuwsl.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3mxsmadui.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3vnzgiaqd.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3kwiuggxc.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nmwgjitq.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3iftoawak.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3kgwnpthc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3jwtivhne.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3ryeskvgi.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3ybuafswb.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3graythfl.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3towfbbly.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dzjercto.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3fwtfzitw.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3qubvjygq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qykeljjq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3vxckpyxg.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3onoiaotb.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3hujwzlqi.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3tqesqnnr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ujsldqrd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ccsqzuph.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hrnttian.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ltkjcfeh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3pgzuvrpy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nqggllri.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uoaibvow.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qpuqfjxm.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3qwjjvrsf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3wfxlsnwd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bawfxfst.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vhufikgx.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3juetxkhs.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3rrbajnvl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3yqoxmemb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lnzwoktl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3zrdcocbq.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3zgdwfmoi.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3mlqplges.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3bkudvfdi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3vsztdsyg.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3qxpkfjmh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3sclphjny.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3vvruewhp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3pldapwha.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3mzfqzmpg.html


<!-- 参考信息 -->