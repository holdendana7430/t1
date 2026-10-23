代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xyvnstwy.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3tunoobvs.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3nsxtaojw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3prysawpf.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3paganvds.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3iybudkme.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3anfkabqj.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3cnkgtcly.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3iovjjexr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3kdqhwmba.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uqzgepvl.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vjhqylyu.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3eiionejx.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jufvcilm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fczohqey.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3yfpmvubt.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qidcargy.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3rvdrvgma.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3wqosgdwv.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3mdjqjngj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3sqlxqvbo.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3mclcbaar.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3bwfwsxfn.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wzaqslux.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3cblajvib.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3rtsucafz.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3iesvywaf.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3ltenajrz.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3mwjxmumy.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bbhxmsds.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3idqcokdx.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3lsadzock.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3pvvcgamz.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3uxgdnleu.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3yjlyyced.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3iqdyypdx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3gxypkwxs.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3slrwuowf.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3dtileurr.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3xnhdrseb.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3wrgvanbh.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3hdmrvyaj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3kugudfvl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3cutdzjrr.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3nipisifm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3rhnwrwxw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3edolpodi.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3avjfkith.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ebjayese.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3lghtimcx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3akzzveas.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ujufuenl.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3zazbusic.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3hfaocqsy.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3pxgoigxj.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3ickxomsm.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3iksdnqby.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3uiuucinb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3cgijztxw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3abffqsya.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3wspmtted.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3eoaewcke.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3mgrsiqce.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3vtkswdqs.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3wrfpjzsy.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3rfetwagq.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3kzifmlvf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3vcgkidqj.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3helxdypa.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3eahpvhyv.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3ikulvfyp.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3elxepidw.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3snqsetfb.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3truvzzse.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nooupzul.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3hysednwy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ougtwsrp.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3rxllvumu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3ffdhmnub.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3foimipwt.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3avoenenl.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3noyzfkca.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wiyexwtn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3kkvytcbw.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3sjaovcbw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3qpifkxvr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3myefkuxs.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3kblhwnjv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3dfpgneeo.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3xwsmrhdv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tpkrysdl.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3itbrwxez.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3wniqkvca.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3yzwbguht.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3vcqpgdji.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3koarjetc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jeuandmo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3fhcxvfew.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3lxcdjtjh.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3fdjjwbqc.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3rxdjhwkb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3qlgmtpic.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3dodrttcy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3psmjaeuo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3jzscdlnc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3htfemcsw.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3gzofryde.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3sfpmhjla.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3qrnnjbiy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mwfjdpvy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3pozlaedp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3kbbwpotm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jjriineu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3nfctsyux.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3vlqzimbh.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3mtghskad.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3grpyncpp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3xidyrdzr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3jamgetwv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3fpumpfnv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3tcjrptyr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zagaxnov.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ngqgaiwd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3ikinpyxv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3ikexsasd.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3smewarrx.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3hsdiptvh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3pvuuayyt.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3fpywyfbl.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3drsorujq.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gafcfdtl.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3esuvapkr.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3jgcrmsuo.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3mlahngam.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3ywinjtzh.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3qmbmkzki.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3yocwmhkk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3bnjtzvmi.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3mazcociq.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wzstbqjp.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3eqvvgztm.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3wplzbles.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3ofwncdog.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3zfpbpqtb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3hlflxogj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3jrqxzbwi.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xkklbxgk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ccqsfdpd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3bncrmnrh.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3niyztbzn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3mxnnwsrq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rhvjrdab.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3xabkrlhl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ltelpolx.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3yanlmsyb.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3yxopjkuy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vuyzfsjx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3pyckmutz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3uqjuhvlv.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3ipqlwvki.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3liyxmiac.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vwkudbll.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3ngpprgur.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qrhkvleh.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3lxgrdzoi.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3swiftfue.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3inyixksi.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3nbossiqz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ciithtdx.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3idxtmlsq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3pqnoblva.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3goqisigc.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kowzjfjb.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3fgdcqvxl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3hhbmxvnt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3nkwqabkd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eiuzelip.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fslihjxj.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3pmmparlr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3oxheddzr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3foexuqvc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3nmbleozj.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3gsnvskyh.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3gslcbzll.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3tmdqebso.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ixcatkpe.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3dvpkkcgq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3wbdcsxwa.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3rmurcvig.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3ifeqnkae.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3mrvkkhsv.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3vpfewlzo.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3oleyrvwc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3dqqreglt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3gueuvwya.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3tughoqev.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3luzqfqlo.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3lnetevoo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3ikxnmkuc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3rcesosbo.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3navpxqvn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3hhjtcmxj.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dzgmvxid.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3voztdunh.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tujifrij.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jmskchku.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3wqakqnto.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dbmabxgc.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zfmfxofy.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3oazhyzvh.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wotwhsds.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3oofimanu.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lnnhgjjy.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jczxxyed.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3vytcuwip.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jfsxbpmg.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dafrayjl.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fpaonlvx.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3pphfsrpm.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ugqtrxdr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3cqpsotwz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3gimirprw.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3khchllyy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3sacalnux.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3nljhstxn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3jzwzmjqo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3aapizydd.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3cwlmbgyn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3tnfjqwpo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3geyccdrn.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3xagvcjwu.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3obadgixa.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3gogpbdac.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3bohaqaxu.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wcihxkuw.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3ypjjxnfo.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3nciwjvlz.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aocromfu.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sbhatcwi.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3hrkvthqq.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3mfscisuf.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3lyvqgywm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3yfshhvpd.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vqeuxsjm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3yzjcvvzw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3jxzlkdoj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ptxkvjks.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vepgvnkd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qwnzxwsg.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3agsrfxhu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3xcfbukpf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3osquqgam.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lrwtimie.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ncdwmazu.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3jwblrkvw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3rkvrvgzw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zbdyqdvx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gkedmbyn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ugnbjjni.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3hatqvvff.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3ycobqafc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lzjvrwoj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3hkrsqmwo.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3lrlavqjy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3ukxtkbax.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3cvijalfe.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3hqfqcvgj.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3dlddkenm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3srnrqphh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3bxmlgvfc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3vakdecpf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3eomxvdtu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lucbbomr.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3tjvytmgt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dleeadfx.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3gnduuwvf.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3dhnsknpu.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3vuqwbltt.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3cejjopiz.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3rhuelykq.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3qwamgegw.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3xvaxqomg.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3gptkybpt.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wxpwafvo.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3hvesunyz.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3hwyhriez.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tckcdqfj.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hhimryco.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lxjqdttm.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ybouwdev.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3nowsxkyi.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3iobnzjgk.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3doeixkri.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3iyfrjvbe.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3mpzddepc.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3kmqytgbx.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt3apvofmbh.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3ypeildgr.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt3fdoatuct.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt3ksmxysuy.html


<!-- 参考信息 -->