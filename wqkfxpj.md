代发 wailian999

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.blog.zdbjq.cn/Article/details/gfcyrgieb.sHtML

TS:   s.split(",")
来源：http://read.share.hesvh.cn/Article/details/gbxiwkcxy.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.fehbvm.com/Article/details/ggeowmcut.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fehbvm.com/Article/details/gbgqzkuaa.sHtML

Ruby: s.split(",");  s.split
来源：http://wap.hesvh.cn/Article/details/gjqhnkvyl.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.m.share.zdbjq.cn/Article/details/gvqrkhkcu.sHtML

[E08] 数组按分隔符合并
来源：http://www.share.hesvh.cn/Article/details/gnsqpuzru.sHtML

Py:   ",".join(items)
来源：http://www.share.hesvh.cn/Article/details/gnixkprxx.sHtML

PHP:  implode(",", $items);
来源：http://wap.zdbjq.cn/Article/details/gmgqqpxxs.sHtML

JS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gsodjzimm.sHtML

TS:   items.join(",")
来源：http://www.blog.hesvh.cn/Article/details/gfcriodbb.sHtML

Java: String.join(",", items)
来源：http://www.share.hesvh.cn/Article/details/gxvfbyqph.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.zdbjq.cn/Article/details/gibawbozu.sHtML

Ruby: items.join(",")
来源：http://3g.zdbjq.cn/Article/details/guchpfsaw.sHtML

C#:   string.Join(",", items)
来源：http://www.blog.fehbvm.com/Article/details/gqoaoxwov.sHtML

[E09] 去除所有空白字符
来源：http://baike.zdbjq.cn/Article/details/gphclawcl.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://m.share.hesvh.cn/Article/details/gssezdxpb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://wap.hesvh.cn/Article/details/gnzjqbltx.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/ggrookpdi.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://baike.fehbvm.com/Article/details/ghugkfmob.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.hesvh.cn/Article/details/gkdigyhbw.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.zdbjq.cn/Article/details/gackxeoga.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.zdbjq.cn/Article/details/glaijfbui.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.zdbjq.cn/Article/details/gkvjcisbk.sHtML

[E10] 左侧补零 / 定长填充
来源：http://3g.zdbjq.cn/Article/details/gqtewnlhr.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://baike.zdbjq.cn/Article/details/gckgwseip.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.share.hesvh.cn/Article/details/gmslrxrcr.sHtML

JS:   "7".padStart(3, "0")
来源：http://blog.fehbvm.com/Article/details/gvvrmaimk.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/ghxzmbzkn.sHtML

Java: String.format("%03d", 7)
来源：http://baike.fehbvm.com/Article/details/gjvtswvxk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.zdbjq.cn/Article/details/gurhddgfl.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://baike.hesvh.cn/Article/details/gndyydsug.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.fehbvm.com/Article/details/gzigzurgf.sHtML

[E11] 反转字符串
来源：http://m.share.fehbvm.com/Article/details/gcpeztthy.sHtML

Py:   s[::-1]
来源：http://www.share.zdbjq.cn/Article/details/ghygngsof.sHtML

PHP:  strrev($s);
来源：http://www.blog.hesvh.cn/Article/details/guweltmhx.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/gjhzgnxkh.sHtML

TS:   [...s].reverse().join("")
来源：http://www.blog.zdbjq.cn/Article/details/gvlvxwyom.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://m.share.zdbjq.cn/Article/details/grdlmiwbh.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://blog.hesvh.cn/Article/details/glmcbcjek.sHtML

Ruby: s.reverse
来源：http://3g.hesvh.cn/Article/details/giubevnpn.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://wap.fehbvm.com/Article/details/gerbvfvrv.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.fehbvm.com/Article/details/guphcxune.sHtML

Py:   s.count("a")
来源：http://wap.zdbjq.cn/Article/details/gqglrjuqh.sHtML

PHP:  substr_count($s, "a");
来源：http://www.share.hesvh.cn/Article/details/gkyqymjdh.sHtML

JS:   s.split("a").length - 1
来源：http://www.share.hesvh.cn/Article/details/gjszjzdtk.sHtML

TS:   s.split("a").length - 1
来源：http://www.blog.fehbvm.com/Article/details/gwtljpvlq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.fehbvm.com/Article/details/gbevldtun.sHtML

Go:   strings.Count(s, "a")
来源：http://www.share.hesvh.cn/Article/details/gwnklivxc.sHtML

Ruby: s.count("a")
来源：http://m.share.fehbvm.com/Article/details/gzlnphegn.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/gybbpsglr.sHtML

[E13] 逐字符遍历
来源：http://read.share.zdbjq.cn/Article/details/godgyipit.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/gqlhrwoez.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://m.share.zdbjq.cn/Article/details/gpunoptym.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.hesvh.cn/Article/details/gekjrbeuj.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.zdbjq.cn/Article/details/gpwhlljmu.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.share.hesvh.cn/Article/details/gulnucdle.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gsukvrhlu.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://3g.fehbvm.com/Article/details/gpuvwzxdm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fehbvm.com/Article/details/gdzvfrcir.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fehbvm.com/Article/details/gysenymuf.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/gvcqmhzha.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fehbvm.com/Article/details/gypqscyem.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.zdbjq.cn/Article/details/gftdcbhab.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.zdbjq.cn/Article/details/gjyftunww.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://mobile.hesvh.cn/Article/details/gevgcyifu.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://wap.hesvh.cn/Article/details/ghisujxgd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fehbvm.com/Article/details/ghqvrwqoy.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fehbvm.com/Article/details/gawiuunxn.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.zdbjq.cn/Article/details/gpwtxhuvk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fehbvm.com/Article/details/gkxmbvvzd.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://baike.zdbjq.cn/Article/details/gfywjjnfk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.zdbjq.cn/Article/details/ghbwoptqf.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.blog.fehbvm.com/Article/details/gvbfcdqhd.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://mobile.hesvh.cn/Article/details/glymxzwqa.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.zdbjq.cn/Article/details/guneusxsq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://blog.fehbvm.com/Article/details/glhcvoeis.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.zdbjq.cn/Article/details/gsjaowcgt.sHtML

[E16] 数字千分位
来源：http://www.m.share.fehbvm.com/Article/details/gommnllwo.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.zdbjq.cn/Article/details/gasqoivnh.sHtML

PHP:  number_format(1234567);
来源：http://wap.fehbvm.com/Article/details/gnojbuzpt.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.hesvh.cn/Article/details/ghzctrkfc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.fehbvm.com/Article/details/gjcctxggu.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.fehbvm.com/Article/details/gdoupuchg.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.zdbjq.cn/Article/details/ggdhpefjp.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.blog.hesvh.cn/Article/details/gekzizybn.sHtML

C#:   1234567.ToString("N0")
来源：http://baike.zdbjq.cn/Article/details/guziuofjb.sHtML

[E17] 首字母大写
来源：http://www.m.share.fehbvm.com/Article/details/ggaloeyaw.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://m.share.fehbvm.com/Article/details/gnpqatiif.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.zdbjq.cn/Article/details/glkbllldh.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/grundxpko.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.zdbjq.cn/Article/details/gykkhpxsj.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.share.zdbjq.cn/Article/details/guogcddap.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.blog.fehbvm.com/Article/details/geotssehp.sHtML

Ruby: s.capitalize
来源：http://m.share.fehbvm.com/Article/details/guqzfxzsv.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.zdbjq.cn/Article/details/gkcfqgjur.sHtML

[E18] 模板占位符替换
来源：http://baike.hesvh.cn/Article/details/gcqllgavp.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.fehbvm.com/Article/details/gysrhsvty.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://read.share.zdbjq.cn/Article/details/gesmysxpj.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fehbvm.com/Article/details/gxfmxzqhu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/gqmsjrfcc.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.hesvh.cn/Article/details/gstnmlepf.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gsbqstdwl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://blog.fehbvm.com/Article/details/gatuljdtx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://3g.zdbjq.cn/Article/details/gmehfgxzw.sHtML

[E19] 多行文本按行拆分
来源：http://baike.hesvh.cn/Article/details/gwerxztit.sHtML

Py:   s.splitlines()
来源：http://blog.fehbvm.com/Article/details/grxyfukkc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fehbvm.com/Article/details/gqregwjzt.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gxwtddfrw.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.blog.zdbjq.cn/Article/details/glsudjljj.sHtML

Java: s.lines().toList()
来源：http://mobile.zdbjq.cn/Article/details/glrvlcgxp.sHtML

Go:   strings.Split(s, "\n")
来源：http://mobile.hesvh.cn/Article/details/giboqmpxz.sHtML

Ruby: s.lines
来源：http://blog.fehbvm.com/Article/details/gnrijneav.sHtML

C#:   s.Split('\n')
来源：http://m.share.hesvh.cn/Article/details/ghzvdrfdi.sHtML

[E20] 判断字符串是否为空
来源：http://3g.hesvh.cn/Article/details/gfbevoujo.sHtML

Py:   if not s:
来源：http://mobile.hesvh.cn/Article/details/gbltffimf.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://blog.hesvh.cn/Article/details/grpoklduq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.zdbjq.cn/Article/details/guahspdgg.sHtML

TS:   if (s === "") {}
来源：http://blog.hesvh.cn/Article/details/gyniopvih.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.share.hesvh.cn/Article/details/gztgtgzve.sHtML

Go:   if s == "" {}
来源：http://www.m.share.hesvh.cn/Article/details/ggjwxkcdv.sHtML

Ruby: if s.empty?
来源：http://m.share.zdbjq.cn/Article/details/gqefoqjdf.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://baike.hesvh.cn/Article/details/ggdtqscaf.sHtML

[E21] 超长截断加省略号
来源：http://m.share.fehbvm.com/Article/details/gndfzdqqq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.hesvh.cn/Article/details/glglnihxn.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gualmobhi.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gjbpnkmal.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/gbwleynlg.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.hesvh.cn/Article/details/gegwgltqf.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/gochqffwj.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://blog.hesvh.cn/Article/details/gfndvysxm.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gqijnlmqh.sHtML

[E22] 字节长度与字符长度
来源：http://baike.hesvh.cn/Article/details/gastqcska.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://m.share.zdbjq.cn/Article/details/gdrjlahao.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://m.share.hesvh.cn/Article/details/gevitzukn.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fehbvm.com/Article/details/gmlhjfsrn.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.zdbjq.cn/Article/details/gsynaqert.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.fehbvm.com/Article/details/guxbrkpwy.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.hesvh.cn/Article/details/ggotkxrvb.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.hesvh.cn/Article/details/gekkyhwlv.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.fehbvm.com/Article/details/ggsbztzue.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/guxpldeei.sHtML

F. 文件与目录
来源：http://mobile.zdbjq.cn/Article/details/gbukzplbi.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gkzbnmeoq.sHtML

[F01] 读取整个文件
来源：http://wap.fehbvm.com/Article/details/gvdigacwa.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fehbvm.com/Article/details/gluehrfaj.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/gxmadvwgr.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.hesvh.cn/Article/details/gsknfyxdj.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.m.share.zdbjq.cn/Article/details/gihszctxe.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.zdbjq.cn/Article/details/gugkzfysk.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.hesvh.cn/Article/details/gqvpwhnfi.sHtML

Ruby: File.read("a.txt")
来源：http://blog.hesvh.cn/Article/details/gwfgxesne.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.hesvh.cn/Article/details/ganqfdzie.sHtML

[F02] 逐行读取文件
来源：http://www.blog.zdbjq.cn/Article/details/govmuwnzh.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.zdbjq.cn/Article/details/gwmtvxlsw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gkodycuof.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.fehbvm.com/Article/details/gxsujwopq.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fehbvm.com/Article/details/gcbrxftcd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://read.share.zdbjq.cn/Article/details/gogldpkyz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://3g.fehbvm.com/Article/details/gjsyimrfu.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/gvnujyysc.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.hesvh.cn/Article/details/grgimycks.sHtML

[F03] 写入文件（覆盖）
来源：http://www.blog.zdbjq.cn/Article/details/gufcnodvn.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://read.share.hesvh.cn/Article/details/gukkvzhpj.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.fehbvm.com/Article/details/gbocitnsm.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.zdbjq.cn/Article/details/gzbzqazaj.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://blog.zdbjq.cn/Article/details/gvjcpxvyr.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.zdbjq.cn/Article/details/gravqmemz.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://mobile.zdbjq.cn/Article/details/gxqkrgwqi.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.hesvh.cn/Article/details/gzuyesuyq.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.fehbvm.com/Article/details/guxctayjd.sHtML

[F04] 追加写入文件
来源：http://www.blog.fehbvm.com/Article/details/gbtafnknd.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://mobile.zdbjq.cn/Article/details/gxrcjclqy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.hesvh.cn/Article/details/gjespmstv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://blog.hesvh.cn/Article/details/gmalrmgsf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://m.share.zdbjq.cn/Article/details/gzmunvknz.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.zdbjq.cn/Article/details/gpaveoptz.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.fehbvm.com/Article/details/gfytlylbd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.hesvh.cn/Article/details/gfufiumvz.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://mobile.zdbjq.cn/Article/details/guaxzwhtz.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.hesvh.cn/Article/details/gjvrvmikx.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://wap.hesvh.cn/Article/details/grhommqlc.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.fehbvm.com/Article/details/gbbxiuxum.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gbfqkhzwb.sHtML

TS:   fs.existsSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gmhecfyaf.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gtmvykwee.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://wap.hesvh.cn/Article/details/gwiprqqeg.sHtML

Ruby: File.exist?("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gggmvbgbv.sHtML

C#:   File.Exists("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gdoovtaxt.sHtML

[F06] 删除文件
来源：http://baike.hesvh.cn/Article/details/gsylqzvwy.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gthlhzyod.sHtML

PHP:  unlink("a.txt");
来源：http://wap.fehbvm.com/Article/details/gkamunpyn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/gpjvmjnlr.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://3g.hesvh.cn/Article/details/gkecrrwly.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://read.share.zdbjq.cn/Article/details/gumtshocr.sHtML

Go:   os.Remove("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gqlkztjrj.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gcfykosdx.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fehbvm.com/Article/details/gmdagrkjx.sHtML

[F07] 创建目录（含多级）
来源：http://mobile.zdbjq.cn/Article/details/giemrbtpu.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.hesvh.cn/Article/details/gcdboxlmz.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://3g.zdbjq.cn/Article/details/glegbquae.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gwfmeganx.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/gtubyhfwh.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.blog.hesvh.cn/Article/details/gmmavkyna.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.blog.fehbvm.com/Article/details/goewreeej.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://m.share.hesvh.cn/Article/details/gokblzpok.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fehbvm.com/Article/details/gbbxtihqi.sHtML

[F08] 遍历目录
来源：http://www.blog.fehbvm.com/Article/details/gffgvjfpm.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/grjrlvbaz.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://read.share.fehbvm.com/Article/details/gepgvjnyw.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.zdbjq.cn/Article/details/gtwuajupj.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.m.share.zdbjq.cn/Article/details/gsnaniqkq.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://3g.fehbvm.com/Article/details/gkqoryili.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://mobile.hesvh.cn/Article/details/gakijzlct.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fehbvm.com/Article/details/gtjrffczp.sHtML

C#:   Directory.GetFiles("dir")
来源：http://read.share.hesvh.cn/Article/details/gdauleftg.sHtML

[F09] 获取文件大小
来源：http://www.share.fehbvm.com/Article/details/gqxeqyzja.sHtML

Py:   os.path.getsize("a.txt")
来源：http://blog.fehbvm.com/Article/details/gofkitpcw.sHtML

PHP:  filesize("a.txt");
来源：http://baike.zdbjq.cn/Article/details/gpchwwgnk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.hesvh.cn/Article/details/glvmasnut.sHtML

TS:   fs.statSync("a.txt").size
来源：http://mobile.fehbvm.com/Article/details/gwawjcgcl.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gkhcjhpbd.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.m.share.fehbvm.com/Article/details/gyhxtfyxr.sHtML

Ruby: File.size("a.txt")
来源：http://3g.hesvh.cn/Article/details/gdniekcdy.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.share.fehbvm.com/Article/details/ggkdrwlpl.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://read.share.hesvh.cn/Article/details/gmcsskobw.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gzkfrgvmu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.zdbjq.cn/Article/details/giyduustg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gczadbmxs.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gkdzlegrq.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.zdbjq.cn/Article/details/gxqvniewh.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gobflxium.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/gbfdackbt.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gyecvzfdx.sHtML

[F11] 复制与移动文件
来源：http://www.blog.fehbvm.com/Article/details/gbemkfvqf.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/glfencuxf.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.zdbjq.cn/Article/details/ggjvkmsmz.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.zdbjq.cn/Article/details/gxgjtollt.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/gqxqnwlpy.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://m.share.zdbjq.cn/Article/details/gyhpvcfiz.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.hesvh.cn/Article/details/gdhkuexis.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://3g.zdbjq.cn/Article/details/goqgejnsm.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://baike.fehbvm.com/Article/details/gowzgfgyo.sHtML

[F12] CSV 读写
来源：http://m.share.hesvh.cn/Article/details/gkzinyktr.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.zdbjq.cn/Article/details/gtjfmbirh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gwkgupsuh.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.hesvh.cn/Article/details/gcloqwdeq.sHtML

TS:   // 同上
来源：http://blog.fehbvm.com/Article/details/gzolabwpu.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.zdbjq.cn/Article/details/gpajsetzl.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.zdbjq.cn/Article/details/ghxkkgqoh.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://blog.hesvh.cn/Article/details/gkqmznjub.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.share.hesvh.cn/Article/details/gfntdwmtj.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxkqutkub.sHtML

G. 面向对象
来源：http://wap.zdbjq.cn/Article/details/goitgbgqm.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gkmkdfnhq.sHtML

[G01] 定义类
来源：http://read.share.fehbvm.com/Article/details/gbenblazi.sHtML

Py:   class User: pass
来源：http://www.share.fehbvm.com/Article/details/gbpjvvdim.sHtML

PHP:  class User {}
来源：http://wap.hesvh.cn/Article/details/gjjlkhsyn.sHtML

JS:   class User {}
来源：http://www.m.share.zdbjq.cn/Article/details/ginldtbgl.sHtML

TS:   class User { name: string = ""; }
来源：http://m.share.fehbvm.com/Article/details/gegmuxbpk.sHtML

Java: class User {}
来源：http://wap.zdbjq.cn/Article/details/gbdtuwvcd.sHtML

Go:   type User struct { Name string }
来源：http://www.blog.hesvh.cn/Article/details/gyrcjrtvr.sHtML

Ruby: class User; end
来源：http://wap.hesvh.cn/Article/details/gnijeswnh.sHtML

C#:   class User {}
来源：http://3g.fehbvm.com/Article/details/gpbdkgdct.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gclqagetm.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.zdbjq.cn/Article/details/geblqqfeq.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/gqrfmuppd.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gkrmljqtu.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.zdbjq.cn/Article/details/gkmzwuqge.sHtML

Java: User(String name) { this.name = name; }
来源：http://m.share.hesvh.cn/Article/details/gwwkzytyg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.fehbvm.com/Article/details/ghtisrkhj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.fehbvm.com/Article/details/gppokrfcw.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gdvkrykrz.sHtML

[G03] 实例属性
来源：http://www.m.share.hesvh.cn/Article/details/glzvzuqmi.sHtML

Py:   self.name = "x"
来源：http://www.blog.zdbjq.cn/Article/details/gstniqmxu.sHtML

PHP:  public string $name = "x";
来源：http://blog.hesvh.cn/Article/details/gllssdbyo.sHtML

JS:   this.name = "x";
来源：http://www.share.hesvh.cn/Article/details/gfxrkrtqw.sHtML

TS:   name: string = "x";
来源：http://mobile.hesvh.cn/Article/details/gszaxusnx.sHtML

Java: private String name;
来源：http://www.m.share.hesvh.cn/Article/details/gbktonolv.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fehbvm.com/Article/details/gfvixywpi.sHtML

Ruby: @name = "x"
来源：http://www.m.share.zdbjq.cn/Article/details/gitdhaypq.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://m.share.hesvh.cn/Article/details/gleavtqya.sHtML

[G04] 定义方法
来源：http://blog.zdbjq.cn/Article/details/gemrnusgh.sHtML

Py:   def greet(self): return self.name
来源：http://3g.hesvh.cn/Article/details/glcvfennf.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gseqckvwm.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.hesvh.cn/Article/details/gwmnqanku.sHtML

TS:   greet(): string { return this.name; }
来源：http://baike.hesvh.cn/Article/details/gohtbuuro.sHtML

Java: String greet() { return name; }
来源：http://blog.zdbjq.cn/Article/details/guzepalhi.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://wap.hesvh.cn/Article/details/gdtdtjjor.sHtML

Ruby: def greet; @name; end
来源：http://wap.zdbjq.cn/Article/details/gsnqroluk.sHtML

C#:   public string Greet() => Name;
来源：http://mobile.zdbjq.cn/Article/details/gimwxgrwa.sHtML

[G05] 继承
来源：http://baike.zdbjq.cn/Article/details/gscfdmvjl.sHtML

Py:   class Admin(User): pass
来源：http://www.share.hesvh.cn/Article/details/gbmnbpkcs.sHtML

PHP:  class Admin extends User {}
来源：http://www.share.zdbjq.cn/Article/details/gufqureoq.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.fehbvm.com/Article/details/guuhyligj.sHtML

TS:   class Admin extends User {}
来源：http://mobile.hesvh.cn/Article/details/gmnfpisdp.sHtML

Java: class Admin extends User {}
来源：http://read.share.fehbvm.com/Article/details/gbpitzkwu.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://m.share.hesvh.cn/Article/details/gjvchtlgg.sHtML

Ruby: class Admin < User; end
来源：http://wap.hesvh.cn/Article/details/gdvmtzifr.sHtML

C#:   class Admin : User {}
来源：http://wap.zdbjq.cn/Article/details/gbayzwloy.sHtML


<!-- 参考信息 -->