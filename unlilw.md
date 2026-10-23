代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3dpugocci.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3tythcqxt.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3jeqeeact.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3bdvlavei.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3ygvkxfhs.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ncxrkrtw.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3wgdcbovt.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3bcwgdxxw.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3xtehyqcc.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3iwyncgpp.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3bxbknink.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wpilcczi.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3qikkbyte.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3urtusinx.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ebyqdidf.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3imsnpvmu.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3hxidjgjm.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3cjelhbgu.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3mcsqtkst.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3xlfxxrpi.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3khpedrrc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3mzpnjxdl.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3qxulcvxx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3zdarfayb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3osngtxid.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3mgsivfba.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3fdeowfqu.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3adccpxyy.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3fbwakkkw.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3lpqoqvri.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3qtadjggo.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3dgclqgem.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ldlyemuw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gahkmctd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3iotpcauz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3trswhbkv.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3mnnrrshw.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3oyuyzpoj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3morloqvi.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cliwtfmo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3alqquued.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3stkvbebs.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3djjwezou.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3wohvvpft.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3xwlcdteu.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3dbqlpuso.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3owvbtpoa.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3ihciqgir.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3gzxjreoc.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3qgxjtuqg.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qqebmnxg.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ldxutykv.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3kkgtkddg.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3vhgqxuzr.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ikslzqkx.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3rzqagotl.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3jgpjouir.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3xnnwglfh.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3sykhqmnk.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3bqzqqqvy.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3lzzlniur.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3jkylgmtr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3smerwbek.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3flkzpque.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3abwghpjf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3jgklfcyg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3phtlffja.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dkljvgsu.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3pylvafjf.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3djkvvmwn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3sygwrlku.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ogbugpvs.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3hpgrqkux.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3wdjbrwic.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3bqiqesvx.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ozhnnzwj.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mdzgjhjd.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3oocljebe.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3rjfqgcic.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3hgwlrxpn.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ndgmbbeq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3sjmlztik.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3yhijazdl.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3camgivtm.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3pbzmprto.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3rewtuvyr.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3bjaoztot.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3vledehjc.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3mzivpzdp.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ubzhqidx.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3hwogwhbt.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3egbqjwty.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3rvcbgwhq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3dtvsspda.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3hohdvptz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3iwgleihe.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3zakqcafj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3vfauyzwh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3sabimuaj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mmdmecfb.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3vfkfljpo.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3sztcroog.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3emhzciuo.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3yitvnfnu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3nzwzfcor.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3fjpicksi.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3zstbbpgf.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3gcmujjax.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ouryzlnf.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3nrqhvoji.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3iidplgab.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3syngskab.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3eztbxlvi.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3oakqnyvm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3tsqiyntw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vsdsdjyi.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zieoqimn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hzciwwqa.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3raxgkjki.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3vdajpjjf.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3jvauvknx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3hdsbxjwf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3baaswmgd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3xojiujst.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3ttvyarqq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3ovqhogoo.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3phzyjycm.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3axmilrvp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3rregqaig.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ycnjhsfz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3nbzmvplv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3yindsmku.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3spmsipuh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3mibaknqx.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3mmxxkxud.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3spiwslbi.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3crcxqith.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3yxifyttc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3xzuluidy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3wtakulft.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3copbplxz.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3wgtwyeoq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ejvjnbmp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3uomzyyzt.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3jjznbtmc.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3rvoiwcro.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3nfrbqhvu.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hwstrlbd.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3trkwdkwr.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3urmbsnww.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3zzwdiihh.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3qhzjjyon.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3hqxxteyu.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3wgahfxjz.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3oxfxdvfg.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3nxzzgdeo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3klrmkapb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3tkxrxczy.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3icttsfgy.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3yuryedig.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3vfonqwoi.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3iyedtxdv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ekuvuwgv.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3qupdicvb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3cxesfxld.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rlxqurkc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hyacowgj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rljndfyu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3yjxuqoeu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3kostwyxz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3akmlamda.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3swlzuugr.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3kssfqoiu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3cdxrwsrz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bdzmrxsz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3xlblysvw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3kyddtnmp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3fsgzncor.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3euogshtw.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ekadjeth.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3evcyiutc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mjiysiju.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3vfefoktt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3icyqwkgh.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3njxfwciw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3hebqglrl.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3zcpbcdor.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3yhgtvdmg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3huenurmw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3clvlshef.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3ezhybrfv.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wcspmqnc.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3cfixnpit.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3eoueufgh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3hgqeszzz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3rnzrngyw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zwybafcx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3zjspaxiu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ndbmzcvu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3yvqbucyn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3qcgfrryd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3tuxqhxkw.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3diaqvseg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3hpdnwmvp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3dxbahmea.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3cjxcdspc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3mtroumun.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3sruimucq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3qtaxzxzk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3psijxwrc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3vfkpfaek.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3oetwgwyt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lyvipdtu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ksotklkc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lhphvmxp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ukhcshpi.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3hdqkwytj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ygfxfsrj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3odlaysxj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3dacayhhg.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3gykiugdt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3fmosyafu.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ltxkpzog.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ujphgmip.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zuoqeplz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3yjscvsds.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3qahosqbj.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xzxaflav.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ztegrogk.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3ubewjrna.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hompuemx.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nwvueckn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ondsdbxs.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aebwmlrc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3lctppcxf.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fxwcrizq.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bxumpsio.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3akivbdoj.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3kgwzqngl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3syqsslmd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3cixiylww.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3gjgaprar.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3awhwhdsx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3jzlgnrqk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3olblqkfa.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3wpryjkxg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3cidmpjzs.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3glqbdjmz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3cjrceevg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3rlvpijqi.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3gmzzxcha.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3idbamotu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3xhutqufy.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3djysqprb.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ecefaknv.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3hrwgntep.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3gwnpiglf.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rffyyxqr.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3otixznkb.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ohmtnhti.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3vnewjzxh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wlyfmolm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3mkgbtwwq.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3efrsuhhd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3qpcxcakk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3isfnstir.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3anarlgeq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3pdkglgic.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mtshqodn.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jtdmqjvw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3evefbnch.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rpuctafm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ehwmoqou.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gtwurask.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3qntyivgc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3jmxfkfpo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3wjmfghhf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3custhwsj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pkrphemt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3uvwpduya.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3axpbzyba.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3lycoezmd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3uvwtdtbp.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3icygpwql.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3muevapab.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3tfgjnxyp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3hgwwxoai.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3gseorgdt.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3wmqhdcjz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3asrxbpwj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3nzcmvyys.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3rbajueyp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ziawlvig.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3afxcdjgx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eovugqyy.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3bjkphshr.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3llpvdjvp.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3vrhqcceb.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cjeakqvr.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3kwghxiqg.html


<!-- 参考信息 -->