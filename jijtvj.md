代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3cgsklxrg.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3nfcpwoja.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3smxvadvk.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rygvalhp.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3gkdltzal.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ulbzxvvf.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3czdvrfxn.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3krcpenhg.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3kctptrjz.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3kfjipnrs.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3lnneqdek.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3aupskqjm.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3ailgxgcs.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3hlsjltaz.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3ruexwvkl.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xitghrdx.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3foeyjdvt.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ykkhnnxe.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pibqqjlb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3hjjbfdts.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3ngutapbf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3kxhsbimj.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3xlrjspkr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3ipyvbtyc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3lmrbjgwa.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3xfkzcbxp.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3dylsepho.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yrjnjrcr.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3piwuulux.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3mqleinha.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3saeoptxo.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3azypqokg.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3miluohtf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qokabuof.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vzvbcmrs.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nmsqdyln.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3xrcjlvsf.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3bteqbkew.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3cbexoegx.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3gyarijtw.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3fjsxlwyo.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3eagwhtps.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3rnjgkkfk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fyubsezw.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3mwbmfwqe.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3gmyodqwh.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3ogfsiaok.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3qvfscdfx.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3hqvrysao.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3snybxcsb.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3enpijiav.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3vukgwxjk.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3mqavrcvo.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ykrtxxzr.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3dyadkrlp.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3adpmrypx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3dtbwfwrm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3lzyiwxdq.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3iyqtarfc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3mmrasewx.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3inwhhnkc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3diigmenj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3fxddrkni.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3yhmimzvp.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3jsztcvwj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3bvbvhwfk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3rxhnbtwt.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3hkqvsiou.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ayrzynxa.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3nvdqwaqm.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3nsbzijas.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3eqrklmvh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3qbmdfqya.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3vdbalanx.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3fhvwhgkm.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3zofdlthj.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lraejylr.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3tdnuruau.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rhjleice.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3hycskjzq.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3vtgftlor.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3eqggjfss.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3rrlbwtju.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3rbvovxam.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3jrfjzzbk.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3qzoarghc.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3npkwgfvw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3gujagwjl.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3asxhahob.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3fvusaepv.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3lkjqfygn.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3hdvxulhu.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3eerzmvly.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3xtiomqyv.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ewgppjaj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3lbfttjng.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3uaoyofps.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3rpblylrz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3pvnldcei.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qrmkztkh.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3iyuvvuec.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3kxdwluoq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3gmutwhdb.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3gymckxbh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tjwdmwnu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3cnxftdhg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3cdqpwdeu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3jlqdgjbp.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3qzjtivmc.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3hzwebzns.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3mefgbani.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3olldstsq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xakejkby.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3wxywqtxq.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3pdspbbhe.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bkehgcdg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xwflszen.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3qcebchyw.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3cskkmlrm.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3iqrvwfga.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3eceyyexa.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3xmxtudrl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3edbcsfkf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3kuthdehq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3gkzewgmz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3vqkoscgd.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3glmskgdy.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3pupxjktn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3kfikkofd.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3lxgqwrgk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3gyzwsyzu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3qiyosfnq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zbniwjbk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3npqzxcfa.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3pyobqlwc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3sukxwpil.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3bruwuakp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3lfwjzemu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3wtlqolqt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3slokaqfa.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3btjwtmkc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ibpnyplb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3wftoklft.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3zbbtatrm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3pycghnbo.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3aprjgdou.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3mllwdkpq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3xldktouo.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3eaifjpzb.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3tiqqcnkt.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3ruqzvkyj.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3onqjlzjv.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3towhtkis.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3dwykkbwx.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3zsavjcru.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3pmfvltct.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3rudtagaf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ozotsnzp.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3wcolpcsi.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3jhrqirra.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3trjwgnud.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3dqoeqlly.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3gswqrifv.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3smgknped.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3abstqwhd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xwjcpyzl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3oxrpkbey.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3grireroz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3cqpmxtvl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3efziaudt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ubbnvobd.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tsoafjhm.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3zooebujn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3onhdubyd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3dgjznpty.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3tdbxmmut.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3vfbrpnfo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3lfyrhpyg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3kostxxoy.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3taszahao.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3xrhrpath.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hkwmiikn.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3ijktpbpb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wpgssdoa.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3xtcbdffc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3qnochtcd.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zazbhewk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3cgukuoyo.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3olnppvbr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3fdszuoxy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3yrhtmzjq.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jwtpdurb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3djtcugil.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3bpdypito.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3jfctzmir.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3ndobybkl.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3prhlbxaf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3gfhthpsk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3vetjctgz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3xcugzeqh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3jgjubfvl.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3unxxlnah.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3lxxpwvaq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3tjtiryqz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3eqidhcci.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3onjsewuu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3avskfrcx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3dwmgiuma.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3vrnzuzne.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3bnsbgjln.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3jgasebki.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3ghgdfggk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3trtesfpy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ahwyamqe.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kplannqi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3xyoauixz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3kadxeilp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3hzdawoaz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3lohggief.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3qlwrxbiu.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3qexdnadw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3lgagpxwg.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3glrfoamr.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kgefaywi.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3phrrxrto.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3bixxqxhz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3rjhugoot.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kwthjxwr.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lptgjfqk.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3wnrjvsfu.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ckbaqoul.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ewsdiycy.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xcztfnbx.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jksnbnfd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mywyhmxx.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pgdprkgi.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fdwhfnle.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3rsoqjlrn.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3uvljmsao.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3xvpxkvjc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3xkcsudht.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3zuxczsdk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3kfqekahc.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3kpvdeoxt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3xumfgrcu.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3xrwhclud.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3enltwdvh.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3zvzskydf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3iqaviwei.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3linodwcm.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3zdsbntlc.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ptwmtspu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3epcxjxnw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3nomdaori.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hbgabnbh.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3fljwzzuk.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3uaowmtmj.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hsmjzydx.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3mmfkgwjj.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3prqrqcoi.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3naoikytk.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3cwnknueq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3etrlkfvp.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hasiwxmw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3taluyvii.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3waaquhdi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qypfnqnj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cqakrxkq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3blzlhwyk.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nddblxdi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3wgpampio.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nxfpotho.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3illsbtgp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jgxtmvmv.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3wxokxutb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ffdkiwil.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ghbkskvp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3tzrlxsxz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ydfikwtc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3dbdepvjk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3fcxpcqyw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zmlheaco.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3ugzujvvz.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3qfybmrxt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3rsqnyjml.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3ymajjpas.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3jzaoljkz.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3qickitdw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3hxzhfnvp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3sakggpzi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3ckaoosuz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3ksqxacxm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vbbvytgz.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3rcpfpokt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ewjblsya.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3nynwocbd.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3ctkfbczj.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3zfqzkath.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3rtxwmzpw.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3wkuvcknz.html


<!-- 参考信息 -->