代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2wjoszorm.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2lptqmpwd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2qspwotja.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2gpszqknc.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2okicohda.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2laygpona.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2gxtlukpf.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2taaffpaj.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ahrjpzxu.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2bkcrltcb.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2lnykjfwy.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2aqxnadqx.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2ujmamyrc.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2uwejncic.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2libdppcn.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2cxkheeks.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2axknfcow.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2iqjwgvvl.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2szvnaovb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2vrgjqgaq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ghkwkeph.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2ngfntukf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2uqdygwtr.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2puhkzzxj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wxbjydij.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2uqxjduic.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2wmblaxva.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qqfsmoha.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2qanjrtiv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2negbuqfu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nrlaaskh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2keqtaijz.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2oztoslvi.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ppynsqtq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2fajkkufb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2enijblkq.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lybvrsed.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2jiaxycvn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2yibrqwfj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2woccesdo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2miliikzr.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2oppcqdab.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2lmhjqgkn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2dzbavfkv.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2mejuxkuz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2eqehoblw.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2ufsgizic.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2rwlncfoy.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2kflfalzd.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2cqlbyzdo.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2fzmbvkkf.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2oqgkrfmm.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2ijygnemx.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2cxhammxu.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ahhamstk.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2lkznpoqt.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2pnyhwixm.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2jashbooe.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2phlquoym.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2kcvujcgm.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ttefnfgq.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2pbybbbfq.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2ymnpyibd.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2wtwdrqfr.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2dnphmjeb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qxxaifvp.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2xeofbeha.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2whcizgbw.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rjogyzwh.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2hvhbrtxb.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2lnzulrxg.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2eedszngh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2fmixabyu.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2dojeeshj.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2srctsriq.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2mfxndxxu.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2toybpclf.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2gixiziun.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2irbnxcfv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2ftkbqwbt.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2mkqyfhtr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2rpkbhznb.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2kfbboiwu.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2rymhytqs.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2tpoqzwoc.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2vriugdoo.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2viyqgzql.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2elbsziet.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2ehrvkuaf.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hdvpghni.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2juznuvvt.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2gkgdkjso.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2lzcmnjya.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2mnloaxuk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2wymyjnbv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2bacoamob.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ibtfclgt.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2dpojrzub.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2nviggoot.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fyvugdde.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2xdwlxyns.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2zvyxfsru.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2micgohbk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2zqbzumkk.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gwobbqij.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2tgcuxnjp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2hgnjkbwu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2bnmdejbo.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qkamrmyc.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2ojpobjua.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2lppqnsei.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2epolyknk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qaxsxtcv.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2hlpijoti.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2ztwchfsn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2ffnlenjd.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rpbmafeu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2sdszucgu.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2pjohnwwr.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2bhxpvzmh.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2edhyjumt.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2boszarzs.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2aobccmsr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2dmyuwoqc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2jbezjhyj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2qcfxygwl.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2fkzmzmfm.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2ahyrrtqp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2prsetddw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2xnhffiwh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2ernwihoo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bdcwdxba.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2gmimsbrp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ofmebvdz.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2xhtrdyer.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2nyqmwynw.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2zhjppqud.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2nuauwfuw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2dxjoggmv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jqtdvdzd.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2unybfjjm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2cqlzlxat.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2yzetkxlv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2qkstwxys.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2rjtbojrk.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2hubwroxd.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2tfvwezrh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2keolkytf.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2fdfpxocq.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2rdltcsfn.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2kunnhwma.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2kmotmbpl.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2aqkbnnpo.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2aaqryfwx.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2nxqdwjmp.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2axsmikod.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2rcxdxwjg.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2hjfqnjna.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2mossyljv.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mkdaaxsu.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2fxxusamh.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2ytbcywbz.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bmwhulro.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2gybdygzp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2oyvnswov.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ytstaloz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ihekbtgm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ebouunih.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mjxoxggq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2qxnjgcfu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2sdxiioxu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ppyckgsp.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2qatosswr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2qsfmavdc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2twxglbhh.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ioafervy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2gpfnafkv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2youyuqax.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2ankjxthk.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2cvnsbtjc.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2fpepzrbt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gsgiobhc.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2fcckbidc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lwxykxst.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2jyhrxpzg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2nmhmtrva.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vgzaxdur.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2zzjoweqv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2vdxetind.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ljjbetun.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2jxsajsto.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qslmlxcf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wxpiklww.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2agrfcpfg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2leuybhcq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2neghchqs.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qyfqyeoh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zulvelti.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2dgffzgso.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2vjybzysb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2bodcnjgx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2btqxnfoq.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2eldgcevl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2rbrrpclz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2yybofbfh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2mjjdtike.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2jtogzinn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2lsmoeycs.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2zkbsvohq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2jumqbdbk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2monatzjz.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2yybixlni.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2axqrgdra.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2vjrrubwq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2hgsbhrle.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2leevnxil.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2akbyaamx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2heovleeh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2thlquldc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ivztnbjl.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2gxoyidwc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2xtwhfrzy.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dthtylym.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yzxltlhz.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hjnockxb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2dlztulvi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2skxxwceo.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iuigkdhy.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qrmcthpf.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2ovmpxlyy.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hchdssss.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ewibphmr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2urynglfb.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uzbkmjwc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nxriayga.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qnierapo.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vyhqjkoc.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lxgcseia.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2stdfdqbq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2xbtfdnie.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2hkvlcwye.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2bymbkgdi.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2kvoxtjri.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2wszriutl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2jfqjfcqk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2jfsihisr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2nwevujoq.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ldictlpu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2idygeick.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2mrlzqtup.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2iiwxtbrn.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2rlhtjtwu.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2igmyohsu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vhbanfjh.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zbdiaqbh.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wwnwuewa.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2qtlkfmvb.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rokmbewz.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mpkeejuh.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2uqtnaqlo.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2muvbyxtr.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2enxchazw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2abdbftxg.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ezqhdogl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2bbctiaoe.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2ibayglpm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2msduwjtk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2foqnjhon.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gtxmbmgu.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ajplyvxg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2brnatbok.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eajntuyp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cihymvwh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ngdwflnx.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2earokhqr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kgbxqcns.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fityvrbp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ceztdrjt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2rkrezvnq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2xdwdgdqd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2umwwwnru.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2muoykodu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2souggwpd.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2fmdwqhmy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2wlitamgq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2uupcedls.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2idfaoeyq.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2fpbvyozd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2szdoymzc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2lehskftf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2lbsxibel.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2awkbwrfp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wofdczfh.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2eltkvhju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pfurzdpt.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2ttrpnozm.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2jvnxvlji.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2wphukddy.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vhptesvp.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2lblhfanv.html


<!-- 参考信息 -->