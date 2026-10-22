代发 wailian999

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2zbotqmlm.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2xpgimnfp.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hmxmloav.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jwifwtrq.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tllgyqhd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gcmkdwae.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2kaxramtv.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2hvizzwmd.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yscoizsg.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2rgyrqpqq.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2ebtuhrvn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2chrnvggz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2ommcyqmi.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2glekunvw.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2aqmindjk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2egcofaoq.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2egouuqfs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2guhnqhpa.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2fgpssiat.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2rpkqqjku.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2gvrjpyjy.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2zidhdsai.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2vvrftlsr.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2qvndgomy.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2miufugso.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2idyjiqfo.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2okwdxxpa.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2ijuwgeuh.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2fmgxmfgo.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2lzduuiym.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2izvuadqv.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2kccvmhtx.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2pxxdgdge.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2gioqsezf.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2kzqnryuw.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2bmlmvrbk.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2zgthtiwm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rnwtqqov.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2uhmthruo.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2dvqlnvhk.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xhedkict.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2rjnqgypw.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2khmwriic.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2gunzocfm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2ehecmatc.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2gjfwpupd.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2cszrnqyq.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ypezwblh.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2vjysajcu.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bmtgrcnt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2hekpxoxd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2geyoecjc.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2smsydhrq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2inwurzzc.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2pctvjspg.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fqjscfzv.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2dosukuhc.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2yyqtemvx.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2sdsnqemo.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2lxpuovcb.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2tffpvfnk.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2mcvjlxpq.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2micxiehw.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2skbtvaxa.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2hqkkdhyl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2exyhwtyb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2cagtkois.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rgyojwhl.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qmocackq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2rqsfjpen.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2bbvxaidk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2epbgzeyd.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2kdtkmavi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2ddifvayj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2eozwhpyl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2sasnokek.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dgyppbtr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2bgeyptds.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2lanzzxuz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2ipetmhzy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2cvmoudys.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2nwzrzvlf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2rojopjku.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2hovgmljx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2lrpodghb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2jttrqcuz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2iuxwbxzl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2jaslejiv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2noppbcqv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qlivblpl.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ikgiibll.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2fqaywraf.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2vobdvikj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ibpcqudr.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2iruraner.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2mbjwmdza.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2rfrlodiq.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2yelajgnn.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2gcdxzfrb.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2xddvzqnz.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2pqtwxoab.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2qvcqswul.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2yzciywbq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2stxewctm.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2ipkzluus.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2stxipfsw.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2jmdaxxni.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2vkffjoim.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2aoobeliw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2vcebtvcx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2dtwrwsbe.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jeyxmuhe.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ogtyejsv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gbltncjc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2ppqndokk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2bkjfyuzm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2dnlbancg.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2yyeprpal.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2yjljsnob.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kvkobglr.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ybsuxpmd.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2nquyhhzk.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2wkdnrkna.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2mdaelzjx.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2oyfxsrux.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2ndvkodyb.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2wfeglvhm.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2hbwzwmtd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2ibnwbhfu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2capecjmf.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2hqwkylsr.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2tuskuorg.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2nagsanxn.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2hxdcchru.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2nhvwsnph.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2umneevcl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2lkodyxuq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2lymfsjao.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2vmzlwtib.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2tgvxedpj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vbuumgwi.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2xqwpdapl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2uyegymbi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2roqrazbc.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2ftakhsvq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2amxqnouc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2wyyjokpv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dkfpjajg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2hphafycv.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2gabejecx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2dguznylx.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2dcuvnxsz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ointxxmn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yoajtuzj.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2nopokrsm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ylyhgjyb.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ywubhbod.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2eqwkzmsx.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gerqnfeh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2mwgkiugg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2gbcjdjvt.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ngloysvo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2esnclnrq.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2refqaafp.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pcuividk.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2tjruesrp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2gxaipaff.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2cmikqeoe.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2lgwtkreq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ffbpjfbh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ycsybujo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2mznpzzba.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2typgojsg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2ibxnsrst.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2yidhdcjj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2kdvvqzew.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2aatjzwlx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2gqsklmhb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ahdxmhrn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2jegaoqrc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2cgncbznh.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2dvshtevk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2bmyvlwwc.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2gjgptuka.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2qknzxcpc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2gzadyctf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2nuroimeu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pjtprijx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2njzhxnzr.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2alcnlakb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2nkqquued.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ediqvmiy.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2nrcmpros.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2ziepyjiw.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vtrsmmlv.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mqcxoszs.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gxryfcld.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2nmfmvqxp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2vinfbtko.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dbvyifxz.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mvozfarg.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2wpctarkc.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2erdfsddd.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2heoajbir.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ilyifwik.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eqoadtjn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fgbcxvon.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jqwetvoj.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kipdcvny.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ktehmpmd.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2mkluijcu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2meixaevi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2oucwakbh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2yybhnmlc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2fsnsaung.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2abqfmwqh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2oyhsifok.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2igiouhgm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2cfwcdacs.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2cbsfehha.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2gmlnqxwl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2jufwfewv.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2worwucdm.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2xbgxfxxk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2qfbrqkqa.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2nyhdrznz.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2uqeuelbu.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wwydhclo.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2ioiyqkxj.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tlignges.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vhbqrufx.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2sebkhbxr.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2asymxzby.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2omflcvop.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2pieqxlxo.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jwntqipl.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2bklpmpps.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2vohrswco.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2stjdonch.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wiajsgei.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rdbaxodr.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vsojmqqv.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2eeqlbkax.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tnluzkgx.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2myxxyotj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mmejvcyx.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2abzshlgs.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ggvjumnl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2szrtfmef.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2sdavrbcj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2yzkgdgnl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2mkavxsij.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2vkusyakk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bskylhuh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2jxpuesxz.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2twpgryml.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2ykdquggj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2iusilmnz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2gjpohxph.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2gjmbftqy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2qvdeacfc.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2gijvliit.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2thbwcghy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2vdslsgpq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2egzqqnlx.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2ozowxvxj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bwkwdlbj.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2qcevvtvc.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2qquaeyew.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2sfhtpcur.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2cbdpidio.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2tnjacwib.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ilbjoabj.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2klhyxmez.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2tyejytte.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2cmoupxto.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2pdlqjmap.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2nrlbadky.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2pkhuojch.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2sojqeqnw.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2djqcdvox.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tkuycukr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2spswpzvm.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2mosrjacu.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2wuhcirwv.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2aonggvnq.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2kufbeauq.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2hxrnyijv.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2fpjjsaei.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2kebjpdmy.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2sawhdamd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2vabtrjrd.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2hvhprpau.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2qtqljmab.html

[G04] 定义方法
来源：http://www.ydjk.org.cn/Article/details/gt2trmrbydd.html

Py:   def greet(self): return self.name
来源：http://www.52xcode.cn/Article/details/gt2gledgwov.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2vqilbrhe.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2mwzcwwgh.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt2duzafhpq.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt2hazagxvp.html


<!-- 参考信息 -->