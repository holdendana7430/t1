代发 wailian999

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2pzkmjvbm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2tzesbyqg.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2cyxblnuq.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kuhqsbng.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2exbwhipr.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2jbogluye.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2qhjxffuc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2psfpfhhz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mmhnhyeq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2flkwxnox.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2prcesoeg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2dqtliqrl.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2xurjwmcx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2zlzxkxkf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2lpddqilj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jzeeghin.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2jbspijtc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2tbaxogaj.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2fgvveeap.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2auuyrlxy.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vpbpauar.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tohxkkli.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bskbpyca.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zvdtczir.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2zxwphwcl.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2uanfowbl.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2wrjsehps.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2cynrsmfu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2vwfeooeu.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2lugdrgmu.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2idrcipam.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2ooebgufe.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2indjwehx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2dcbznosi.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2zlhmstqi.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2ppgdvfcn.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2igyntsis.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gscrkrcz.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2lvrrrnou.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2ontwloyb.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2pdbetszh.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jcoglrxs.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2vtayewmg.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2bubkqguw.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2pcxoollw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2taerzppu.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2tkogvluu.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2rdbqpeia.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2nlupgdtv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2uaoovbbc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ikwghiih.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2iffnryfv.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2cxqlfnla.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2sixnjwzd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2rverdmom.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2vrjswhhe.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2gxlzqbqg.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2leeuwvbn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2cyxupllx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2pwkzmbkl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2mrrgltnp.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2cjwqsoex.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2fjaekbyr.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2hlnwliyg.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2ykzjmivg.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wboxrdao.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2qhlpizei.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ircqmuoc.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2yjdnqqtw.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2qyeoawqu.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2fopsrfuu.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2hsafrfri.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2lfseypnt.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2tjurdhyd.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2tsiaetql.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2afeouele.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2lxsexubl.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2gnlmajzq.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2vkjvqcym.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2myrvxgac.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2wzduejlw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2vayfhsvj.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2oqosfied.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2djecaync.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hyuhzbva.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2ekmbepco.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2fxyarfzl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vapuilux.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2jwtelziw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2lwvlhsdt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2wxrrxrxk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2gehupccx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2nhxiwpjz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2rlobzoup.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2upgkzqdb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2ffkzmoem.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2plmfzkhl.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2yjieckbz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nwbcymwv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2rjqfaqhx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2djrouois.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xyjlqnus.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2szcdkbdk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2klqzhvgo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fnwgvxzm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2jcmmztge.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2crwhaxlk.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2voxaypno.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2jalebvkp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ltnnunlm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2geyjcavb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2hslhvlbh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2lsksjdpu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2sfmlbxrx.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2etvqhsqf.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2xoxhqokk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2qdfoetfj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2wjwnbswc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2izhiassu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2bvjhffmb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jzfeokcp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ukxiewam.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2cxmboill.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2dqhqwjeq.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2zrxwcqie.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2zgskvfav.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2rmiytmqj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rryjzzzr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jrgbfoap.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xynrtwds.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2zuetwput.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2tmkrwrli.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2zdtyvaqi.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2oerclxhw.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2pbzhdrvu.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2pqdnlhwh.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2iyxcaxcl.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2hxyqgmxi.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2nqlhuzdm.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2yqcngqyg.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2yverjyaw.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2tlbdfsju.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2uhajqamx.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2eljlfnkp.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2qysfayyk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fwjloefg.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2pyhiokga.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2yjmlilaf.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2emfxtyhz.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2pyzwvkgb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ywuwzkir.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2yzcgubbd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2cwbkmwsg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2xpoxalgs.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2putzipkr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qkidhjtu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lntnuwdy.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2mauwxoqp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2awgvrokq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wsbwoxhz.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2gkkoxcmm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2eqjhlrsh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2uctkiznk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2euskrjat.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2tafeuzkr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2penwyslb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2wtuneqqu.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2mufxyuyk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ieibqqyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2whqntupq.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2drkjmkko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gedhvyah.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2dovqmmgm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2ckvqvvxd.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tmikzxaa.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2ehgpyynj.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2kwdkbosy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2vpbaduxd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2kamdkeqd.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fknxngap.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2iipwyisu.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2wwzfabsy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2txzpwhnr.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2qknzqvof.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2fevknfat.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2rkxjwwfx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2wcidtsnb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2wxvkwtnf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2niavohvy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2pevajdmj.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2xrbbpbfz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ckzoriuj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2sryszfjp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2fdyxqsuy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2useuxyhw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2njuehbcr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2kcpfwllk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2xmgmncpr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2xpzkpakj.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2qftwujjb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2xqbihqpg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2rsbahtov.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2qezyfvpz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2qxdojlnf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2ofuicyux.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mszlxaws.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2agbozkvb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2dkligpzw.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ttsgmrat.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2lxwygvay.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cdqmjgac.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mnzxcgkj.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2geipplct.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2zcbrcucr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2ygvottej.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nqpelser.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2avjbcbtj.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2fybaaabz.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qnvwaxoa.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2bahiiyrl.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qdteyttg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2djqwhecb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xdtawuqi.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pjzthmpl.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kmxlqnqs.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rsbeupeu.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2jvnxgwss.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2pzgfhcdg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2dgvwdfzu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2testeosr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ggatwavp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2xokdston.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2tofanndz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2hbvhrznv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2txuwibrr.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2lduqsphr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2cxtejlzy.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2jerfbsvp.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2hqofushd.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2eyrtctqv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ikjyfwtq.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2emgalwos.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2tucgcpvv.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2zzjptwti.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2jqsqohlx.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gwmhudlh.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2urqannpr.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2wccggiyt.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2lrdcnrec.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xuhdwjns.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2cqzirrxw.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lbvbzrxo.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2lxrgsmsi.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2qytzqrpk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sxnresir.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zenrcynq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2efjlfvsz.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2urlkfzoi.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2morhlnwg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iceaiofq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2chptsrdk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uveflbkd.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2rskftqtd.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2vvcehntz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2skkbpnzl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2fatuilyp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2isuixnye.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2crpepnmb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2rvqcceyk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2kbqxlqbt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2rqucvbsy.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2lpqsdcnx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2rfyfddli.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2gongdmyi.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2tkzzjodt.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2ueothfta.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2tyraffcy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2rblyqill.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2heyvbsuk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2oujmezke.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vmoujwra.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2beolhmuc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2efcrmkij.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2mzvvdame.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2rfvlinkk.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2uasyvfbr.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2swnfvdts.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2ggwdjevy.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2kmrhzwic.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2lxbpvcri.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2wumnlgrv.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dkltqtec.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2wbjznpgm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2wanxbzfy.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hlxxhjnt.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2aynpxxxy.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2igbmhsdw.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zgsvgjlv.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2oelvuvce.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2huiwsibq.html


<!-- 参考信息 -->