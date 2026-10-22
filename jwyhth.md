代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2ahaivonf.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2vbuicoph.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2xbkghklt.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ugzgctkn.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2poknyqdd.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2sfbwxhwh.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ievrovfq.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2hvtorvqh.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2zqqkkrnr.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2msjonkbs.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2btsqqtsk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2ousxdoqs.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2lxwteqqn.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2pqitchtt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2xxrxrcje.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2rteoltyc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2yfxzipdv.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2vosrqkat.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2xjmlnhkk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ipptuxcf.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2ahjkznzc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2nrznhbvr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2wncyrzup.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pqitozap.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jnwamuhu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lbxaybci.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2klxkkrdl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fuiltjwq.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ydwsmowq.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ncupscli.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2nnegjwzt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ufvxohqz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2oygonats.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2issehdqh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2hkocvujc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2clevixws.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2hmcbyqft.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2ncepmsfw.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2rvzpkrwe.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2nqjpzctu.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2adobtuwn.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qmqlrcer.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ggomsibu.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2cphknjsu.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2zcqafein.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2hktmkumh.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2epbqkowx.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2bdndsuia.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2uiphkxjk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2pshdhjiq.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2whpclfui.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2epzsrdua.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2gvdotuyc.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2hrgkntdh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2mkdgkqpw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ucubzvrt.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2zmdosdoz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2mzfhwryt.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2nptmlxvm.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2djiiioff.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2ogiazqti.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xlnnhcte.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2dwoxtala.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vobgygui.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2qpyqamrh.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2vsjruuss.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ilveqctl.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lnvwqtxn.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ositnlyn.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2uzidjyqm.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2vsezcqcr.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2zivlaymh.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2klbxeavi.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2gqwxdtkd.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2laabqdjx.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2imokzcwx.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2xmfmmeif.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2vbfrswto.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2awwxdcvw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2btcmoeme.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2kvfhzgfa.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2jqoewzui.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2ierlyrnr.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2qzggzslu.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2vqfmnxfm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxfwuwfe.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2zhrcswcj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jnqqdbmk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2htljqbuf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pwrxigxw.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2pszdfihy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ermxuxjv.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2ptaqmcno.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2xpmkqmav.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jgspnxjk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2nxgpsxgh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2xiwqikgg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2lubjhizr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2qpthxjfe.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2qtpjiiox.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2tdyeukbr.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2uvlaebpf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2vkhlxhzc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2zrprmccw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qrynkvtb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2eqibcwss.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2buntovxl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2bqcshspe.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2zmjyyowx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ilkhttpa.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2nmctutmn.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2odtxqbxo.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2nvsapshp.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2rnmvlfty.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2swcnlrhk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2trthnmff.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2wujodvtb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2ggwusvtk.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2gcxpekzt.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2lumnxwsv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2xxquqsox.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nwbcmilj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2cvxicasu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2gpogexrw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2nbgpigln.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2wplpwppt.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2gginzauj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2kbeenzio.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2pgfujxbc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2iitsryds.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2qjpsmmka.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2nzjxjeyi.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2lfwrdayc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gcznjztn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2dgsjedzu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2vxbbkunb.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2wjcqmnky.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2sqsqgouf.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2wjlovqkl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2tulylmvl.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2dnugoknl.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2rgtxlfdi.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2cvtewkua.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nycinrwi.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2vgkenynw.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2krjqkjmk.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2unidjlmg.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2fhcipsed.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2ljcofnlk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2qcmncxdx.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2uliebbvn.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ctngwkik.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2wqibggjr.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2erkpohdw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2waeuoxrc.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2taitscyi.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2qzyffxhk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2mqgulggo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2skvdiqhn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2losuhgml.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2gvnptplc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2ggsshlpw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qemnszpu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vfuczbvk.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2gutgqhft.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aknoioxu.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2iagmlhvk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wurxrlia.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2qfxqalhl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ewapmhmx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2srotlasi.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2eymoxvni.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2wvbnvsjc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rwbswvsm.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2wxvvwlnr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ykfcmrdq.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2ltjgxiux.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2uecvpbzf.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pnngfhox.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2zfyanzni.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2kucododo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2lmbntpdn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2knhwzzwl.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nhlfocfm.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2alhfapwa.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2rcklaong.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2dzqpjwfl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2anzewcly.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2snhntzlq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2hsmddntg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2vslladln.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2aysqybgd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2jjftadpp.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2gamfddmn.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2ekagbzpo.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2kzbysrog.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2qrntaedj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2pclqxoct.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ochemspg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2vijyjpob.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2kboppwlm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2cgmzagct.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2nulduzot.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2bwsfszfb.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2mrpheamm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2cvcbqwvd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2hdhpelza.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2gdgfmmvn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2vjrcqjnv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2xndndlsu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2ojpybgla.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2hvvsotjs.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jixspsuh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2omevevxo.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2eksycing.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dkpwjqca.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lutyplva.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2cxdevihy.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2uxjmiosj.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2erlbllfy.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lwpkswpx.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2ihjzdezr.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qakjpebp.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tjdsaphj.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zsnbhgxa.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ytvmoxrh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2lbfvcoji.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vdpyynvo.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wmspftpp.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2efguoftn.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2pdowdbgk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2goqjhofa.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2njxamvdc.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2wktkkqpv.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2imhfrpwp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2fvjscbdt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2ahpmnmoa.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2glyptrbm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2tsldzxxd.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2shtkpskw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2kiooygqt.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2sjocbpko.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2dbtbgnwu.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2lolmbkce.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2zrpjamyi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2hvrsrure.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2yafggyxd.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2eangznsc.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2wjcylueg.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2alpgfrev.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pktpmpov.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2pwyweimu.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2bbjftnok.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2grvyocuh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2gqdxkwov.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dnnkdyav.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2lvhauzdq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2hvxkbmln.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mhhpeewo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bgjrljly.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rtuikgxc.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yiccvmrw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2opnuoeaq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uzhrjoro.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cucgbklc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pmfuyutj.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2tmxaydxv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kahrbscp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lcgbnxjc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dwzfabuq.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gvtrwjyi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2obfzehoa.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2aobdvhqn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hlkstkkk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2bclwrunt.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2haiglrlb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2vjtavnyj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2wybxbcrt.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2jxulkvrk.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2mdumhcna.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2xfjlstrz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2hpdclsvb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2lvetdswm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2bjironjk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lzbouape.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2xtotkigu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fjcphspk.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2ximqkwun.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2qkcpasfn.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2slvckern.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lqhghfdu.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2krrbenwn.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2umanpouq.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2mojenhrm.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2okbskonz.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2mrqueujy.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2znsglmzx.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2svptzawf.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2ggfxqytz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cruwqxsw.html


<!-- 参考信息 -->