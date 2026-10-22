代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2zvsznmgu.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2gwwdlttt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2xpqjxkex.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2drhmhxtt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2tgnoympt.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2jyzhnoqi.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2dmzxwwyt.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2yrxuvpgx.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2pekrliks.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2fgiiadxu.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2wtvnrhel.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2mldpvvug.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2wdpceocy.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2ubgswhwg.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2cmytfwgj.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2rwwxwnyf.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2uvcprisc.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kkgylzyj.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bhoqnppk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2cqzerbco.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bxgfjrft.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2xfyodize.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2tqyzzoyj.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2hbgpcuot.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2aemgrahe.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2xebcabsv.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cczdobty.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2jwcgearj.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2atkzqxdr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jsjinkib.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2ziaqwkgb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kthsorhn.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rcfhzexz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vchtsmcn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2zganabfl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2npibtync.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gsjuurqj.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2xekecygi.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2jwrutsep.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lssenvzy.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2oakmpxdb.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2pugptjhu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2bbemabjo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2rihihsyq.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2srzpquut.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2duzubdjg.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2ecwudaco.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2nrvrufnk.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2uwvkcazx.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2wlualpfu.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ywbpizjt.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2xwhefjyt.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2eosbpqyh.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wzuqbajx.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2knjtxipe.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2jjsicbwp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2sjjhsesr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2szpldewm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2vbjgqlcc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2hjpgdogj.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2reztgcku.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2ldpzredz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2zaiavtra.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2dseuzubw.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2lqjprapv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ddrvzbxt.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2vdgtfusl.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2shbxusbn.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ebuhctfd.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2clhuqwvj.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2otfmllws.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2wlsigcst.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2opalditd.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2gnizmbav.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2gjqyvyqz.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yfhpmjmw.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2nrwwkdup.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2yypkqekl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2qgjiqqul.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2mvkqjleg.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2atgfubiu.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2ljnbnxmu.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2ndvcfagz.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2zrnofitl.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2pqqshqou.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2wclzqpru.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2vlcfmdgf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2jltlakgn.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2fhbqnbyn.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2fsfsquui.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2juavfjyu.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2wmwnnhck.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2fhzcfswo.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2tjlzykwq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wngmpkor.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2uqfjnefj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2wsnboycg.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2ekfwhnng.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2flifvaxr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2adajoxbc.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2pxlyjfry.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2casrfmvh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mtidoqmt.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2hewiynzj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2zavynndy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2tzboggmt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2rtdagbzo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2tlyhxcow.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2yobhklxx.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2yjgzvsoa.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wgeirejg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2dnntkyze.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2yqetpxxs.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dugcmnfe.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2ibbblfyc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2skdhrdat.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bialuapj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2gbtcqsdz.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ervfjicg.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2xanstbui.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2fcclwcuc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2uworrxbj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2cjlbmvav.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2xyyueyfy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2bhyfjsqj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2wlfcfahp.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2nzdkjrxl.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2toxgrmkd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2sbnwwaee.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2jpajczsa.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rzvujieb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2qduohtno.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2mowxslwh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2kfjsiijm.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2mptkrdqm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2potnzdtt.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2yxydgicz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2mvapvzst.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2hmcfrtor.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xnsvbjcx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2umjxhiep.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ctujmdwb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gdrvglnu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2wastxcth.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2mgalgpqq.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2vjiztxtr.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2jkmnehpx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2kjgtzjgy.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2voaxhuzi.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2wgvqwyin.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2moannbcn.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2uujrqbjf.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2ccsnsmza.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2kyzylrcn.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2yoxpswgv.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2rucouelo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2pomqhdjf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2jqolijzd.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2vinpqmko.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2abplngyw.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2yrhonpku.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2avmbfovd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2ldajiclq.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2yqyeuqdg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2yhoovpja.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ostuvkjv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mjuuipgk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kfndgzvb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cvvdngsl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2fmdaemhg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jtsicorv.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dbnkrykp.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2dhdinqyg.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rfxyzzyv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2corufwfr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2zotywcax.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2wvxhztmc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2khoiaxqa.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2yxbyumlw.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2asrvohqd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ybgazyaq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hpoxyhjg.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2qqehnlcm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jwlxroya.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2nnuqzysk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2aroryppo.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cwmfglzh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2gurkqtpk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2gwlwdwzz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2czyrrcgc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2onpyfbif.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vshxouqr.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bizgqweh.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2ctrphyjs.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2hbeeeuhy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2pcujegzh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2nptekeut.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2wetzzouu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2loqbosdc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2zbyhjwtl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2eyygsusx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2nrrkoicw.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2nochqrue.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2wcwqanvb.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2tfzyxaum.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2bccamuip.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xzttgtkj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2gwxvifwk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2njgobinf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2qholrvcg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2nxtrlmnd.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2dkmwnyyl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ggpviiid.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2tzaunvbx.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ivdxnceu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2oremzphi.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2qwzcscjw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2sivodntt.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2jkuyvhnv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2ranhjuht.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2vayyetzj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2olwfhkia.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fuhxedzr.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kdznjmas.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zpwtgwwz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2tignkknm.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2ixqkrrvx.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bgmvwals.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qqhemens.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2ggyrycns.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eaezhrkg.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2hjcmrzww.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tlzkvvdr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jeyldlwj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rhfjobgk.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ahdptquh.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2edqqfcdw.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jadrdibg.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2yycesysc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2cgbkdfld.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2wmoxcykv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2hrueaqgf.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2rhdatztw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2zodikrul.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2htwidjjh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2mhinizcu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2vmintfsk.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2rdbqvxfp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2gbwgmclb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2gwvymjpz.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lzhlvdfz.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2qdvtgxsa.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2isgthlrg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ocmzrtld.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wphzifjy.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2nureyxvn.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2urzgmffh.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ucverzrm.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lxayepvo.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2tzpgkrqg.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2gljmralq.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2nmhckgtu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2unawqlxs.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zmervmgs.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2xoxgstgt.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2uvmstzjg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jzgoesyv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qpvypugu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vxuxknao.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zixbncrx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2kmustfto.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2saikulqt.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2utiypiuh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2knwnvbiq.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2txysgwbu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dlgqnczc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fuqkrkny.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2nemgkxfn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2neqabbfk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2gbsqnwad.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2wtvpcudc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mqujesfx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2fwdfhooh.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2vbzukdcz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2cfpxfdtz.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2nfvohjqj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2qulatdkb.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2quwjtxzb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2qecqiynk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2jmckofdr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ykwqqznz.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2gqsffyei.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nyxnvwlv.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2uaykzkcd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kpbhncsb.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2fikvtiqk.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2xzlnsafp.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2aosvnpue.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2gjpghrzw.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2gzytemke.html


<!-- 参考信息 -->