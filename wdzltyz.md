代发 wailian999

[E06] 替换子串
来源：http://www.share.zdbjq.cn/Article/details/gkmxfympk.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.blog.zdbjq.cn/Article/details/gpnipdiqp.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.zdbjq.cn/Article/details/gesquqdlu.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.share.fehbvm.com/Article/details/gjormrohv.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gipzxizsw.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.zdbjq.cn/Article/details/gvymzfzgg.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.m.share.fehbvm.com/Article/details/gmcxxpisa.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fehbvm.com/Article/details/glzinkxan.sHtML

C#:   s.Replace("a", "b")
来源：http://mobile.hesvh.cn/Article/details/gheiggepn.sHtML

[E07] 按分隔符拆分
来源：http://www.share.zdbjq.cn/Article/details/guqwpirez.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://m.share.hesvh.cn/Article/details/gitzngmre.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://baike.hesvh.cn/Article/details/gemdabtzh.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://baike.zdbjq.cn/Article/details/gjuyovzdg.sHtML

TS:   s.split(",")
来源：http://www.blog.hesvh.cn/Article/details/gtvzhcpmm.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://3g.zdbjq.cn/Article/details/gdegwbifj.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://wap.zdbjq.cn/Article/details/gqbvohucf.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.hesvh.cn/Article/details/gqzgyqrlr.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.zdbjq.cn/Article/details/ggggzkfad.sHtML

[E08] 数组按分隔符合并
来源：http://blog.zdbjq.cn/Article/details/gutpmzdrz.sHtML

Py:   ",".join(items)
来源：http://read.share.zdbjq.cn/Article/details/gueyhbsxt.sHtML

PHP:  implode(",", $items);
来源：http://www.share.hesvh.cn/Article/details/graisgtpt.sHtML

JS:   items.join(",")
来源：http://wap.fehbvm.com/Article/details/gpyooxkgf.sHtML

TS:   items.join(",")
来源：http://www.m.share.zdbjq.cn/Article/details/gjizavjpq.sHtML

Java: String.join(",", items)
来源：http://read.share.fehbvm.com/Article/details/gmghgfqkf.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.zdbjq.cn/Article/details/gdgpjlydl.sHtML

Ruby: items.join(",")
来源：http://www.m.share.hesvh.cn/Article/details/gapiissgx.sHtML

C#:   string.Join(",", items)
来源：http://read.share.hesvh.cn/Article/details/gzaazfjao.sHtML

[E09] 去除所有空白字符
来源：http://www.blog.hesvh.cn/Article/details/gwnbkppco.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://baike.hesvh.cn/Article/details/gnwkmejse.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fehbvm.com/Article/details/gogeepjqk.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/gezsevral.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.fehbvm.com/Article/details/ghvffbnkq.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.fehbvm.com/Article/details/gafjsyier.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.fehbvm.com/Article/details/gsjwjetdd.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fehbvm.com/Article/details/goqrhzjwn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://blog.fehbvm.com/Article/details/gswavpkdk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.zdbjq.cn/Article/details/gqomgrvhq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/ggjsnzftu.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://m.share.hesvh.cn/Article/details/gtytscdcb.sHtML

JS:   "7".padStart(3, "0")
来源：http://m.share.fehbvm.com/Article/details/gsupxybxr.sHtML

TS:   "7".padStart(3, "0")
来源：http://baike.fehbvm.com/Article/details/gjahpsvgu.sHtML

Java: String.format("%03d", 7)
来源：http://www.share.hesvh.cn/Article/details/ganhhxmpb.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.hesvh.cn/Article/details/gahstymrb.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/godgsrouc.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://wap.fehbvm.com/Article/details/grmqqpmrl.sHtML

[E11] 反转字符串
来源：http://read.share.zdbjq.cn/Article/details/gtsdamhyl.sHtML

Py:   s[::-1]
来源：http://www.share.fehbvm.com/Article/details/glhajyqpf.sHtML

PHP:  strrev($s);
来源：http://blog.zdbjq.cn/Article/details/glrtltcjn.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gegozhmrw.sHtML

TS:   [...s].reverse().join("")
来源：http://baike.hesvh.cn/Article/details/gxnoqinqr.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://www.m.share.zdbjq.cn/Article/details/glvlftqey.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.zdbjq.cn/Article/details/gcxfsmgpq.sHtML

Ruby: s.reverse
来源：http://www.blog.fehbvm.com/Article/details/gojpmppqn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.fehbvm.com/Article/details/gfhkjamiz.sHtML

[E12] 统计某字符出现次数
来源：http://baike.hesvh.cn/Article/details/gdvbvxqia.sHtML

Py:   s.count("a")
来源：http://baike.hesvh.cn/Article/details/gojaeboht.sHtML

PHP:  substr_count($s, "a");
来源：http://www.blog.zdbjq.cn/Article/details/gibjhpiax.sHtML

JS:   s.split("a").length - 1
来源：http://www.m.share.zdbjq.cn/Article/details/grvptmidw.sHtML

TS:   s.split("a").length - 1
来源：http://read.share.zdbjq.cn/Article/details/gbmjnufhf.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.zdbjq.cn/Article/details/gtxkohsay.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.hesvh.cn/Article/details/gomqsacab.sHtML

Ruby: s.count("a")
来源：http://3g.zdbjq.cn/Article/details/ghabjzncm.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.blog.zdbjq.cn/Article/details/gnwntensf.sHtML

[E13] 逐字符遍历
来源：http://mobile.hesvh.cn/Article/details/gdhonhopo.sHtML

Py:   for ch in s: print(ch)
来源：http://www.share.hesvh.cn/Article/details/gieigyayn.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://baike.zdbjq.cn/Article/details/gutferitx.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.hesvh.cn/Article/details/gmsfzhynj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fehbvm.com/Article/details/gqxjepyfc.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.hesvh.cn/Article/details/gsqvosbpr.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.zdbjq.cn/Article/details/gqiulzxcq.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://m.share.hesvh.cn/Article/details/gxyuloiym.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://baike.hesvh.cn/Article/details/gcaeqatyf.sHtML

[E14] URL 编码与 Base64
来源：http://baike.hesvh.cn/Article/details/gpompgjmt.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://3g.fehbvm.com/Article/details/gqtiepdqc.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.m.share.zdbjq.cn/Article/details/gynuesqdu.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.share.fehbvm.com/Article/details/gszgsjiaa.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.hesvh.cn/Article/details/gvxyizqyy.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.hesvh.cn/Article/details/gbzwtccoj.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.share.fehbvm.com/Article/details/gcqzzhxoo.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://3g.fehbvm.com/Article/details/gapeynoin.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://mobile.zdbjq.cn/Article/details/gneosrhpj.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fehbvm.com/Article/details/ggckmaiqz.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://wap.fehbvm.com/Article/details/gcrfmzegf.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.zdbjq.cn/Article/details/gudytbldl.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://3g.hesvh.cn/Article/details/gurkqnpdi.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.zdbjq.cn/Article/details/gxgqziwkj.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://baike.fehbvm.com/Article/details/gydwdikrj.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://wap.hesvh.cn/Article/details/gejgtgwvt.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.hesvh.cn/Article/details/glsbrlyrz.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.blog.zdbjq.cn/Article/details/gqakgdvcn.sHtML

[E16] 数字千分位
来源：http://3g.fehbvm.com/Article/details/gpyhkzwha.sHtML

Py:   f"{1234567:,}"
来源：http://baike.zdbjq.cn/Article/details/gpniryuhr.sHtML

PHP:  number_format(1234567);
来源：http://m.share.zdbjq.cn/Article/details/gvirkestb.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gfepuvyiv.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.fehbvm.com/Article/details/geidqvazw.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gkzekfmje.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.zdbjq.cn/Article/details/gujoywayr.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://m.share.zdbjq.cn/Article/details/gxywtqgyy.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.zdbjq.cn/Article/details/gcxbcdvng.sHtML

[E17] 首字母大写
来源：http://mobile.fehbvm.com/Article/details/goqyncpqf.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.zdbjq.cn/Article/details/gmimfsfnd.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.zdbjq.cn/Article/details/giwfxbjgx.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.zdbjq.cn/Article/details/gelafmydg.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gkcojpsvz.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.blog.fehbvm.com/Article/details/gnbjyptjr.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://blog.fehbvm.com/Article/details/ggtrglvxi.sHtML

Ruby: s.capitalize
来源：http://www.blog.fehbvm.com/Article/details/gacocuemq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.hesvh.cn/Article/details/gmuqyabwg.sHtML

[E18] 模板占位符替换
来源：http://mobile.fehbvm.com/Article/details/glhvgskav.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://wap.hesvh.cn/Article/details/gmafqlgcx.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://m.share.hesvh.cn/Article/details/gucgkkxgi.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gokncqocc.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://read.share.hesvh.cn/Article/details/gjbkhkouw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gdvsdklpi.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gihxrstpl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.zdbjq.cn/Article/details/ggebloyes.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.hesvh.cn/Article/details/guckmefeq.sHtML

[E19] 多行文本按行拆分
来源：http://mobile.fehbvm.com/Article/details/ghucumhul.sHtML

Py:   s.splitlines()
来源：http://baike.zdbjq.cn/Article/details/gsfndhzck.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.m.share.fehbvm.com/Article/details/giajujvqa.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.zdbjq.cn/Article/details/gesrdqdbb.sHtML

TS:   s.split(/\r?\n/)
来源：http://m.share.fehbvm.com/Article/details/gmqdmuiad.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/gjvfaodfn.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fehbvm.com/Article/details/grufygpiz.sHtML

Ruby: s.lines
来源：http://wap.zdbjq.cn/Article/details/gqxjpltoh.sHtML

C#:   s.Split('\n')
来源：http://www.share.zdbjq.cn/Article/details/gybmqzlum.sHtML

[E20] 判断字符串是否为空
来源：http://3g.hesvh.cn/Article/details/gjweakvwm.sHtML

Py:   if not s:
来源：http://www.share.hesvh.cn/Article/details/gqkorwmcb.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.zdbjq.cn/Article/details/gebbtcwav.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.zdbjq.cn/Article/details/ghzqchjro.sHtML

TS:   if (s === "") {}
来源：http://wap.zdbjq.cn/Article/details/guadnpipi.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/gxcfllumk.sHtML

Go:   if s == "" {}
来源：http://www.share.fehbvm.com/Article/details/gbmcutrnh.sHtML

Ruby: if s.empty?
来源：http://blog.hesvh.cn/Article/details/gzpszalex.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.fehbvm.com/Article/details/gkjugrngi.sHtML

[E21] 超长截断加省略号
来源：http://read.share.hesvh.cn/Article/details/gabkxjglu.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://blog.fehbvm.com/Article/details/glxwulxqm.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://m.share.zdbjq.cn/Article/details/gnzbvjwib.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.hesvh.cn/Article/details/gnxuqndrc.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://blog.zdbjq.cn/Article/details/gquyotkfg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://blog.fehbvm.com/Article/details/gqgeqojax.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://blog.hesvh.cn/Article/details/gqxfrsrbn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.fehbvm.com/Article/details/gruunxhpd.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gadzufmpv.sHtML

[E22] 字节长度与字符长度
来源：http://m.share.fehbvm.com/Article/details/gufztncyi.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://3g.zdbjq.cn/Article/details/gpdtddidp.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gocueggnb.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.hesvh.cn/Article/details/grbkeaakg.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://blog.fehbvm.com/Article/details/gxmsobljc.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.fehbvm.com/Article/details/gcxkafzel.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://read.share.zdbjq.cn/Article/details/gphzfzrqy.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.zdbjq.cn/Article/details/gmxpcuqzq.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://blog.zdbjq.cn/Article/details/ggwcoanbq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gwqsevnss.sHtML

F. 文件与目录
来源：http://baike.fehbvm.com/Article/details/gspviwukt.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gxhazyxdr.sHtML

[F01] 读取整个文件
来源：http://www.share.fehbvm.com/Article/details/glyzpnhva.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://mobile.hesvh.cn/Article/details/gztugamav.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.hesvh.cn/Article/details/grnutjwjs.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fehbvm.com/Article/details/gzfcjsjwv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.zdbjq.cn/Article/details/gpiyxdgsw.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gyjktjqwa.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://3g.hesvh.cn/Article/details/ginfnerqq.sHtML

Ruby: File.read("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ggofjbydp.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fehbvm.com/Article/details/gfvrcdowv.sHtML

[F02] 逐行读取文件
来源：http://www.m.share.hesvh.cn/Article/details/gipsdjskq.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://baike.hesvh.cn/Article/details/getmzetxf.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.hesvh.cn/Article/details/gjykwwcxs.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.share.hesvh.cn/Article/details/gerydofix.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.zdbjq.cn/Article/details/gakerqvdc.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gidhfzkkx.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://blog.hesvh.cn/Article/details/gvwmwvsgv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://3g.fehbvm.com/Article/details/geztiazrj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.zdbjq.cn/Article/details/gvymerrsz.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.zdbjq.cn/Article/details/gjxreigob.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.m.share.zdbjq.cn/Article/details/ggoioeqee.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.blog.hesvh.cn/Article/details/gxwgtbhmd.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/ggcbtssgl.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://wap.fehbvm.com/Article/details/gwqrvqlqk.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.zdbjq.cn/Article/details/gvnupmjuz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://baike.hesvh.cn/Article/details/gpnegwtmb.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.zdbjq.cn/Article/details/gbcdqbzsd.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/ggnigkeso.sHtML

[F04] 追加写入文件
来源：http://wap.zdbjq.cn/Article/details/gyrsfmnzh.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fehbvm.com/Article/details/grczzkqqd.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://m.share.fehbvm.com/Article/details/gtljgzuso.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fehbvm.com/Article/details/gtftcisrc.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.hesvh.cn/Article/details/gwcxqpjqt.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://3g.hesvh.cn/Article/details/gzpmejpuq.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://mobile.hesvh.cn/Article/details/grcxgjhvi.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://baike.fehbvm.com/Article/details/gslbpvmsn.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://baike.fehbvm.com/Article/details/glaksrlxp.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fehbvm.com/Article/details/gtsedfpkx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.fehbvm.com/Article/details/grbwtswjn.sHtML

PHP:  file_exists("a.txt");
来源：http://read.share.fehbvm.com/Article/details/gulkxavic.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gotptliai.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gydvciqig.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gydxbstxy.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.hesvh.cn/Article/details/gychkooyc.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gclluwhdy.sHtML

C#:   File.Exists("a.txt")
来源：http://blog.fehbvm.com/Article/details/gosikujwq.sHtML

[F06] 删除文件
来源：http://www.share.fehbvm.com/Article/details/gtvpsxijm.sHtML

Py:   os.remove("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/godgmzrwq.sHtML

PHP:  unlink("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gcjnrcamz.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggobudhyf.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gcpyetwje.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gspyzsxlg.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gzirrnvkm.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.hesvh.cn/Article/details/ghvejfeit.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gqwwwtvsq.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.hesvh.cn/Article/details/glzahdbwd.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.m.share.fehbvm.com/Article/details/gkwdxzxhu.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.hesvh.cn/Article/details/gqgcyleli.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://m.share.fehbvm.com/Article/details/gpetydnbr.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.zdbjq.cn/Article/details/gplqcgwkc.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://read.share.hesvh.cn/Article/details/grmbupsgt.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://baike.fehbvm.com/Article/details/gtmiicrvp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fehbvm.com/Article/details/gybkbghau.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://mobile.fehbvm.com/Article/details/gjsxjecwf.sHtML

[F08] 遍历目录
来源：http://read.share.hesvh.cn/Article/details/gtfgfbwhu.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.m.share.hesvh.cn/Article/details/gjowptket.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.hesvh.cn/Article/details/gccjwbzkv.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/ghfeprjra.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gpwanpivj.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://baike.zdbjq.cn/Article/details/gmtyteocg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.fehbvm.com/Article/details/geursdreo.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fehbvm.com/Article/details/goqcluobi.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.zdbjq.cn/Article/details/gkpvduedm.sHtML

[F09] 获取文件大小
来源：http://3g.fehbvm.com/Article/details/gilmgknkf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fehbvm.com/Article/details/glvnsdmco.sHtML

PHP:  filesize("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gyltqkbhs.sHtML

JS:   fs.statSync("a.txt").size
来源：http://wap.hesvh.cn/Article/details/ggloxiffy.sHtML

TS:   fs.statSync("a.txt").size
来源：http://read.share.fehbvm.com/Article/details/guoldfobg.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.share.fehbvm.com/Article/details/gyqgdonac.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.zdbjq.cn/Article/details/gtfgjvmmn.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gpfnphyok.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.zdbjq.cn/Article/details/gqwaaunnh.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.hesvh.cn/Article/details/gpobngqjq.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gpquzzait.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://wap.hesvh.cn/Article/details/grcillvxa.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://blog.hesvh.cn/Article/details/guaerdfuh.sHtML

TS:   path.extname("a.txt")
来源：http://baike.fehbvm.com/Article/details/glgxikluw.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.share.zdbjq.cn/Article/details/goltwnfhh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.fehbvm.com/Article/details/gxbvbkuus.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/ghayascvm.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.hesvh.cn/Article/details/gteltwefa.sHtML

[F11] 复制与移动文件
来源：http://wap.hesvh.cn/Article/details/gqktoeeal.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://mobile.fehbvm.com/Article/details/gecfscbhk.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://m.share.fehbvm.com/Article/details/gvvmnvqnz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gjmnydhon.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.hesvh.cn/Article/details/godopmzdg.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/gifipmmez.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fehbvm.com/Article/details/glomguots.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/grdwugtya.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.hesvh.cn/Article/details/gwtxkwlqi.sHtML

[F12] CSV 读写
来源：http://baike.zdbjq.cn/Article/details/ggwpoddbc.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fehbvm.com/Article/details/gvmuuxsrv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://baike.fehbvm.com/Article/details/gglqjpkfu.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://baike.fehbvm.com/Article/details/gyohltcfo.sHtML

TS:   // 同上
来源：http://www.share.fehbvm.com/Article/details/gphieuerf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.hesvh.cn/Article/details/gpwqguame.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fehbvm.com/Article/details/glhylpsgm.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/gqpfachzr.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.hesvh.cn/Article/details/groeffuhg.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gvewnzzwt.sHtML

G. 面向对象
来源：http://read.share.hesvh.cn/Article/details/gzodzglsi.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gxgcqlkul.sHtML

[G01] 定义类
来源：http://3g.fehbvm.com/Article/details/gayslohge.sHtML

Py:   class User: pass
来源：http://3g.fehbvm.com/Article/details/gtzzexhxt.sHtML

PHP:  class User {}
来源：http://read.share.zdbjq.cn/Article/details/gxcrsfebo.sHtML

JS:   class User {}
来源：http://www.blog.hesvh.cn/Article/details/ggvepvzrw.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fehbvm.com/Article/details/gxvshbuwq.sHtML

Java: class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gkkkrhdzz.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.zdbjq.cn/Article/details/gzkswudls.sHtML

Ruby: class User; end
来源：http://m.share.zdbjq.cn/Article/details/gnknigvlq.sHtML

C#:   class User {}
来源：http://blog.zdbjq.cn/Article/details/gmglrbcpi.sHtML

[G02] 构造函数
来源：http://read.share.fehbvm.com/Article/details/gedswpcpu.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.m.share.fehbvm.com/Article/details/gvvyfbais.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/gnpaxghjs.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gmafwmcio.sHtML

TS:   constructor(public name: string) {}
来源：http://mobile.zdbjq.cn/Article/details/gkpcwtcai.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.zdbjq.cn/Article/details/glbllhmtc.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://wap.hesvh.cn/Article/details/gcotavwgw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.share.zdbjq.cn/Article/details/gneqksdwt.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.zdbjq.cn/Article/details/gncpnldkt.sHtML

[G03] 实例属性
来源：http://3g.zdbjq.cn/Article/details/ggfkuovbl.sHtML

Py:   self.name = "x"
来源：http://m.share.hesvh.cn/Article/details/gybufegyu.sHtML

PHP:  public string $name = "x";
来源：http://blog.zdbjq.cn/Article/details/guwvneovk.sHtML

JS:   this.name = "x";
来源：http://www.share.zdbjq.cn/Article/details/ghtkqlefn.sHtML

TS:   name: string = "x";
来源：http://read.share.hesvh.cn/Article/details/gcjojblzi.sHtML

Java: private String name;
来源：http://www.blog.hesvh.cn/Article/details/gvumbdytx.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.m.share.zdbjq.cn/Article/details/glwjfkdpm.sHtML

Ruby: @name = "x"
来源：http://wap.fehbvm.com/Article/details/gwdmqbvnb.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.zdbjq.cn/Article/details/gbmftesmj.sHtML

[G04] 定义方法
来源：http://m.share.hesvh.cn/Article/details/gmxqfebdw.sHtML

Py:   def greet(self): return self.name
来源：http://blog.hesvh.cn/Article/details/guaxhpltr.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.share.fehbvm.com/Article/details/gtkeegcpe.sHtML

JS:   greet() { return this.name; }
来源：http://blog.fehbvm.com/Article/details/gheubjshc.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.zdbjq.cn/Article/details/gvilskctk.sHtML

Java: String greet() { return name; }
来源：http://mobile.fehbvm.com/Article/details/gfgibubma.sHtML


<!-- 参考信息 -->