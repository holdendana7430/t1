代发 wailian999

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3exsqyixv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3qcqndzfi.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3plpvwwzl.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3sbylpnat.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3emliwqbi.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3hjewdadw.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3loumoeqc.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3yitmgtbt.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3aadtydyi.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3mtknqmie.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3mcqxaduq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3qyaxcwso.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3peqzdnss.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3fvtiycgf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3qjsznkra.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3qtthvgtz.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3pkucvoxk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mhtbyqho.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3garflsds.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tzgvhnyk.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3anospmae.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3rxcyhzvq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qpbduznx.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3uqeouwrm.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vptojclx.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3acowwyvz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3xwypqxsj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ktavksyc.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3uojkxnxn.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ojxoudps.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3mfxntpfx.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3lfigszja.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3eyrbkydu.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3ffyswjlr.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3rpfuudug.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3itufthvv.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3swddrsix.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3hsuuflyd.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3cjfljbgu.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3vssmxlnl.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3yjequxpw.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tekgivvu.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3wqshfjkc.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3hsoxfgns.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3btyduqoz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3smxwebag.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3exvobgck.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vdeiwjsb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3javpyrjm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3ckhwhhzh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3zygpstxc.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3fwpqykby.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3veedvpkb.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3dtcnnvaq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3txdhwzju.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ttxhteuf.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ugsfmnof.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3pxqbrudp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3cdnxwqjf.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3yvwimptl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3pkhzqgyd.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3zsdgadiw.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3tjzugbyf.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3wrhfgbuu.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uizxjije.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ggsamykl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3mpgqkgrl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3mhdwpawk.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3gqlsrmgd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3bcczgnju.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3anewhwxp.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3rgoorejx.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3uqzsqvnz.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3gagfslfx.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ioiwyxbe.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3vmwgrvwq.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3mnlwwhkv.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3olsntxdr.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ybjeuzvn.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3sihlapcs.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3qvtvaust.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3bznlthvn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ttgwucsb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3znagecen.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3qeyyqpnp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3mvsjusln.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3hrowagde.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bbpkcwqz.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3cjhsjfyp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3xpnjvrcu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3vrpfltus.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3ozkvrmbh.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3pzthqkiv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3essurjjw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3inudlxmc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3zbfxmrrs.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3osqgvjvx.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3gauiovah.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3eakdiuup.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3iuwcjsmg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3lutlncwd.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3dettsegy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3abbfxnzu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wnpiokzu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3opuhgoph.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rmtaxcau.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3oxafdayq.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3rbaaofgx.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3dzmewfzq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3xbkhzbli.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ybttquik.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3ecehqxzp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3jjyleuys.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3pkaefiry.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3tbcncudz.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3sppwpbmp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3coobzegl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wfiftdfz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vczybwsu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3abicomla.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3fyhjeuwx.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3jpefrshw.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3bdvupgid.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3feoxmywu.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3qcppchre.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3fqtwufue.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3kfawqjjb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3woxhityc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3oxixcxyx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3gngpyanu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3typsptvq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3xpsynnim.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3axgltxlo.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3jomofyct.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3qsqyrxgv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3dgugxzcm.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3zocyxukg.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3lscwnmao.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3asksdvqj.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3uldbrgba.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3myfpvdrj.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3xzahjvkm.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3jrasxxvs.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3bnskizuw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3widjapze.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3pmjndmea.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3ephpeafe.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3cmwuhqpb.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3ywvnldnr.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3kcwagpmj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3iiwiwzwl.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3utzmfoea.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3fbtkyqxr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3srtimpqd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3lljriqyt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3dlpjwaqb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3imgdysvz.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3mlnbjzjh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ooycibcy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3imhorhkj.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3qblyclow.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3qqgymwrh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3rapppsjj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3sgfbszei.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ddrvfyqx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3myipekyq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3ypdbohlx.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3hrjapvpu.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3evvgzzgi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pngaivrw.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3uhuxjidx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gjiyepdn.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3dtbzekrf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3dfesauqc.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hlyqmdjf.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3vclokkif.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3jmknxehc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3yjaajwua.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3xmykgrln.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rofvtbqo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ewfpxzsm.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3cwyxdaop.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3bjbfflpw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3uwyubhbz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ogxfbuxk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rpbhdhsx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3vrvndctx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3hfcorpiw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3tcwzwwba.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3fqklfdub.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3iqkiwufw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3osfdtbeu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3qgsrlrlw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3yccagfut.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3ximvlcgx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3yekcthrt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3wwdwilwg.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vwysxklg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ejpqzghl.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3kphnbmkv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3nkoebwwv.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3nxkitirv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ztzgvdvs.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3hantlgzx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3npgsyovi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3oitbhgbc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3plrhwxkc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ksfownah.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3zxnorasd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3hxnnfzkh.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qbcuomnr.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3upkfwjqv.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gijphkzo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ftlhljez.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3kfljtins.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3robsdokk.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ncuvprky.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3xevzbcxp.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vlqkirho.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hisbzrqs.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3eilzxugv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fikpflan.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ybfomlix.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ksmwvtzu.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ewnbjcsm.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ciiggmlh.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3zzrjrkxl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3gmudyoql.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3yvizzfnx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3vfrdbbfk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3cxnormzf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3ftzmbpga.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3euotbchj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3rywxuriw.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3jzabmxiv.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3lzgszpjq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3odperyvj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3bvzjgjmp.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3unxfeair.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3tidyuptg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3xkzherqs.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3ubkvpvxu.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xgxoijmt.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3exzqlyxb.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3srefcorb.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vtfqbglh.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kedqbofl.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3fscpbtgl.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3iewnswti.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3pwsuayas.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3spuagkjn.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lxneuhwc.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3yaqbzqbu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3hbnzdafo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ekmdahzw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3exnwebmg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lfitddkt.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tymsknmv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3becmlkxw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ghkpgvdp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uhgnoytr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rfgdjwyy.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3ogetegjw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ptnfmgoa.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3uvyaoyaq.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dbubngwj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pqzhnbff.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3nebkscku.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3kybqynci.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3sidwblqe.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3xgvpoebk.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3gyyprpdf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3hpetdwfk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3yfljzois.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3bckorxaq.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3swqqaror.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3hjgqabtj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3xlfhghoj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3syapxhhs.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3yuvtcxxy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dyeadjun.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3erauhuyc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eadrinez.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3kfbfsxdm.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3urzgfsju.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3jbeofguz.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gripdpau.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3usmafqti.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3zbfyukzr.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3qwxuydgx.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3zthsgnbh.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3hjmxyvph.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3xucowlfp.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3tvajjawy.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3zsieaitk.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3irrmslvy.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yoheitne.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3cqzgraqu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3ziyhdujw.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3yxzfdvfu.html


<!-- 参考信息 -->