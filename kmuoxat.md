代发 wailian999

[E06] 替换子串
来源：http://m.share.hesvh.cn/Article/details/gxcwtqgyg.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.m.share.hesvh.cn/Article/details/geuunwimf.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://m.share.hesvh.cn/Article/details/gdzoqphzp.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://mobile.zdbjq.cn/Article/details/gnahafsdl.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gzysxiwjx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://read.share.fehbvm.com/Article/details/gnatwtvua.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fehbvm.com/Article/details/gbauwxqbg.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://wap.zdbjq.cn/Article/details/gjyzradmk.sHtML

C#:   s.Replace("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gzbzcmknp.sHtML

[E07] 按分隔符拆分
来源：http://m.share.fehbvm.com/Article/details/gozkzhnxi.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://blog.fehbvm.com/Article/details/gbceodnik.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.hesvh.cn/Article/details/ghszgiznl.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.zdbjq.cn/Article/details/grqckwyhq.sHtML

TS:   s.split(",")
来源：http://read.share.fehbvm.com/Article/details/gwdicqitj.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://baike.fehbvm.com/Article/details/grvivzphm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://m.share.zdbjq.cn/Article/details/gfgxsntua.sHtML

Ruby: s.split(",");  s.split
来源：http://www.m.share.zdbjq.cn/Article/details/gnfrrnoxp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://3g.fehbvm.com/Article/details/gzdmzjpke.sHtML

[E08] 数组按分隔符合并
来源：http://www.blog.hesvh.cn/Article/details/gowtnjrkd.sHtML

Py:   ",".join(items)
来源：http://www.share.zdbjq.cn/Article/details/glwdifhpo.sHtML

PHP:  implode(",", $items);
来源：http://wap.fehbvm.com/Article/details/gydehtatc.sHtML

JS:   items.join(",")
来源：http://blog.hesvh.cn/Article/details/glwvgvwwt.sHtML

TS:   items.join(",")
来源：http://baike.fehbvm.com/Article/details/grepohfto.sHtML

Java: String.join(",", items)
来源：http://www.m.share.hesvh.cn/Article/details/gxfmzmyhi.sHtML

Go:   strings.Join(items, ",")
来源：http://www.blog.hesvh.cn/Article/details/gvvjuskno.sHtML

Ruby: items.join(",")
来源：http://3g.fehbvm.com/Article/details/gylwjthmn.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gshahdvrf.sHtML

[E09] 去除所有空白字符
来源：http://www.m.share.hesvh.cn/Article/details/gpzmxjfzr.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/ghrllrxjw.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fehbvm.com/Article/details/gpangpifa.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.hesvh.cn/Article/details/grcxvuqvx.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gokvfevhs.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://3g.fehbvm.com/Article/details/gebbgrvzj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://blog.fehbvm.com/Article/details/gfmjegyso.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.zdbjq.cn/Article/details/gyfnogcgu.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.fehbvm.com/Article/details/gjunjpkie.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.hesvh.cn/Article/details/ghimehorv.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.zdbjq.cn/Article/details/gcahokjkp.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.m.share.fehbvm.com/Article/details/gpcdsbhad.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gtghuizof.sHtML

TS:   "7".padStart(3, "0")
来源：http://mobile.zdbjq.cn/Article/details/goowzzcri.sHtML

Java: String.format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gumgmzqwo.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.share.zdbjq.cn/Article/details/gcxiocjng.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.zdbjq.cn/Article/details/gyxdlcasy.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.zdbjq.cn/Article/details/gscabujil.sHtML

[E11] 反转字符串
来源：http://www.share.fehbvm.com/Article/details/glmpvjjjx.sHtML

Py:   s[::-1]
来源：http://wap.zdbjq.cn/Article/details/gzllziszu.sHtML

PHP:  strrev($s);
来源：http://m.share.hesvh.cn/Article/details/gqmmlzrqy.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.hesvh.cn/Article/details/ghxfxrlyz.sHtML

TS:   [...s].reverse().join("")
来源：http://blog.fehbvm.com/Article/details/gyozdbvel.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.hesvh.cn/Article/details/gpsnhcbpc.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://wap.zdbjq.cn/Article/details/grkydzjdm.sHtML

Ruby: s.reverse
来源：http://read.share.hesvh.cn/Article/details/givehiftv.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fehbvm.com/Article/details/guqivkrwh.sHtML

[E12] 统计某字符出现次数
来源：http://www.blog.zdbjq.cn/Article/details/giwsbakul.sHtML

Py:   s.count("a")
来源：http://baike.zdbjq.cn/Article/details/gnajyjmhp.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fehbvm.com/Article/details/ggllifmxj.sHtML

JS:   s.split("a").length - 1
来源：http://www.blog.zdbjq.cn/Article/details/gptcvpyiy.sHtML

TS:   s.split("a").length - 1
来源：http://blog.fehbvm.com/Article/details/gvpsrzqca.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.blog.zdbjq.cn/Article/details/grpfqbzoo.sHtML

Go:   strings.Count(s, "a")
来源：http://wap.fehbvm.com/Article/details/gitytlonv.sHtML

Ruby: s.count("a")
来源：http://mobile.fehbvm.com/Article/details/ggdfxfutv.sHtML

C#:   s.Count(c => c == 'a')
来源：http://wap.zdbjq.cn/Article/details/ggvglvwfu.sHtML

[E13] 逐字符遍历
来源：http://www.blog.fehbvm.com/Article/details/gypipthzp.sHtML

Py:   for ch in s: print(ch)
来源：http://baike.hesvh.cn/Article/details/giakydlyu.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.zdbjq.cn/Article/details/gqhfmedeb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.hesvh.cn/Article/details/gblhweldg.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gwgfmzitk.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.blog.fehbvm.com/Article/details/gqqpqhblv.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.hesvh.cn/Article/details/glgxfpkni.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.hesvh.cn/Article/details/gfnygbcdm.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gpvlzdztj.sHtML

[E14] URL 编码与 Base64
来源：http://baike.fehbvm.com/Article/details/gmycrvsmo.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fehbvm.com/Article/details/gqyewvyxp.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://mobile.fehbvm.com/Article/details/gaalznkqj.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.zdbjq.cn/Article/details/grajhxjic.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://read.share.fehbvm.com/Article/details/gftwdfqak.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://m.share.fehbvm.com/Article/details/gdzztfqar.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.zdbjq.cn/Article/details/gigxdhisf.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.zdbjq.cn/Article/details/gmhbplbef.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.blog.fehbvm.com/Article/details/gtpjluhgt.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/gxuiewqst.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://baike.hesvh.cn/Article/details/gmbaxqfdu.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.hesvh.cn/Article/details/gowfjtjct.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://wap.hesvh.cn/Article/details/grmmvlchj.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://3g.fehbvm.com/Article/details/gdfxuuwqi.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.zdbjq.cn/Article/details/goamyjmfm.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.hesvh.cn/Article/details/gcvxfpemq.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.hesvh.cn/Article/details/grsfevvht.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.m.share.hesvh.cn/Article/details/gqltxqsho.sHtML

[E16] 数字千分位
来源：http://blog.hesvh.cn/Article/details/gyjnvcwuh.sHtML

Py:   f"{1234567:,}"
来源：http://wap.fehbvm.com/Article/details/gwkpjtfkk.sHtML

PHP:  number_format(1234567);
来源：http://m.share.hesvh.cn/Article/details/gewlxetex.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/ghnkrebbk.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://m.share.zdbjq.cn/Article/details/gwjmgfyre.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.share.zdbjq.cn/Article/details/gcpigrsuz.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.share.fehbvm.com/Article/details/gdqbilcgy.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://read.share.hesvh.cn/Article/details/gecedvfks.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fehbvm.com/Article/details/gzsuvzopi.sHtML

[E17] 首字母大写
来源：http://www.m.share.fehbvm.com/Article/details/gipsnants.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.blog.hesvh.cn/Article/details/gexotbunb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://read.share.zdbjq.cn/Article/details/gudyaitri.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fehbvm.com/Article/details/gsionsuux.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://blog.hesvh.cn/Article/details/grziojofg.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://baike.hesvh.cn/Article/details/guoizceua.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://read.share.zdbjq.cn/Article/details/gigbmhndk.sHtML

Ruby: s.capitalize
来源：http://read.share.hesvh.cn/Article/details/gxqhdshjo.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://blog.zdbjq.cn/Article/details/ggcivglxq.sHtML

[E18] 模板占位符替换
来源：http://3g.zdbjq.cn/Article/details/gfiliaxae.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.fehbvm.com/Article/details/gxptnofci.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/gniaubvcb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://wap.hesvh.cn/Article/details/gilpdkrpf.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.zdbjq.cn/Article/details/gwzkwdjaw.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://3g.zdbjq.cn/Article/details/gavrsqucu.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://wap.zdbjq.cn/Article/details/gnfobmywp.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.fehbvm.com/Article/details/gnvmgabrx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.blog.fehbvm.com/Article/details/ghbukxhkl.sHtML

[E19] 多行文本按行拆分
来源：http://www.share.hesvh.cn/Article/details/ghnslascn.sHtML

Py:   s.splitlines()
来源：http://3g.zdbjq.cn/Article/details/gpuivytar.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.zdbjq.cn/Article/details/gyoepwwfz.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.zdbjq.cn/Article/details/gcszdvxxv.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.hesvh.cn/Article/details/giittmezy.sHtML

Java: s.lines().toList()
来源：http://baike.zdbjq.cn/Article/details/gkheyrwdw.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.zdbjq.cn/Article/details/gzrddzvrr.sHtML

Ruby: s.lines
来源：http://www.blog.fehbvm.com/Article/details/gdyhyxovp.sHtML

C#:   s.Split('\n')
来源：http://www.share.hesvh.cn/Article/details/gnsqyhtbb.sHtML

[E20] 判断字符串是否为空
来源：http://m.share.zdbjq.cn/Article/details/gdkyxuyii.sHtML

Py:   if not s:
来源：http://3g.fehbvm.com/Article/details/gxykfxvbj.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.hesvh.cn/Article/details/gauivefeq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.zdbjq.cn/Article/details/guokfotkl.sHtML

TS:   if (s === "") {}
来源：http://www.share.hesvh.cn/Article/details/gpxyqhizj.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.hesvh.cn/Article/details/gpmqzowcq.sHtML

Go:   if s == "" {}
来源：http://read.share.fehbvm.com/Article/details/gzfpnkeqj.sHtML

Ruby: if s.empty?
来源：http://blog.zdbjq.cn/Article/details/gbgmmwodx.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://m.share.zdbjq.cn/Article/details/gpznwzsnb.sHtML

[E21] 超长截断加省略号
来源：http://baike.hesvh.cn/Article/details/gfucrugom.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.m.share.hesvh.cn/Article/details/glevdewxv.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fehbvm.com/Article/details/gihwzmqxb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.fehbvm.com/Article/details/gnhwdgter.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.share.hesvh.cn/Article/details/geeoirafu.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gdazxlpxc.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://wap.zdbjq.cn/Article/details/gksvqicwk.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gbcbpieng.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.zdbjq.cn/Article/details/gvxyjnueq.sHtML

[E22] 字节长度与字符长度
来源：http://www.blog.fehbvm.com/Article/details/giskdnoux.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.m.share.zdbjq.cn/Article/details/groakpkms.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://wap.hesvh.cn/Article/details/gnltfzgws.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/gpynjjxab.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.fehbvm.com/Article/details/garwfuvbi.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://m.share.fehbvm.com/Article/details/gepuaukbh.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.m.share.fehbvm.com/Article/details/gofmogftb.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fehbvm.com/Article/details/gfqxideil.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/gqqtoksdm.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gcxftjmub.sHtML

F. 文件与目录
来源：http://wap.zdbjq.cn/Article/details/gdrswfdrl.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfhpprhst.sHtML

[F01] 读取整个文件
来源：http://wap.zdbjq.cn/Article/details/gphggtqut.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://3g.hesvh.cn/Article/details/genqdmdri.sHtML

PHP:  file_get_contents("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/guzjpgwjc.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/glngjkyfr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gdinkesds.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gkisgrtih.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.zdbjq.cn/Article/details/gsscedbvg.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gvkgduvbh.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gougtjzwb.sHtML

[F02] 逐行读取文件
来源：http://mobile.hesvh.cn/Article/details/glgvflmis.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.hesvh.cn/Article/details/gxmeaewih.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://3g.hesvh.cn/Article/details/gnqkrwkgd.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.zdbjq.cn/Article/details/glgkygcud.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.m.share.hesvh.cn/Article/details/gqnukxwro.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gpqznvsxz.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://wap.hesvh.cn/Article/details/gzrnibuau.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://mobile.fehbvm.com/Article/details/ghudsommp.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.zdbjq.cn/Article/details/gmrbzctbv.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.zdbjq.cn/Article/details/gbauwrezz.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.fehbvm.com/Article/details/gxfussbgl.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://m.share.zdbjq.cn/Article/details/gmlejchbv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gcaobuaff.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://3g.hesvh.cn/Article/details/gayxxoixf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://m.share.hesvh.cn/Article/details/gvxhcqiez.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://3g.fehbvm.com/Article/details/grnzitzly.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://read.share.hesvh.cn/Article/details/gvonmefzz.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/ghkdkrqhm.sHtML

[F04] 追加写入文件
来源：http://blog.fehbvm.com/Article/details/glohfbbrw.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.zdbjq.cn/Article/details/gkatmvfvy.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://baike.fehbvm.com/Article/details/gahklppwg.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fehbvm.com/Article/details/gsecghawi.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.m.share.fehbvm.com/Article/details/ghdaorxce.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fehbvm.com/Article/details/gbmvmwnot.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://m.share.hesvh.cn/Article/details/gsugqawhq.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.zdbjq.cn/Article/details/ggifyherj.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.blog.hesvh.cn/Article/details/gyqgeuzdb.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.hesvh.cn/Article/details/gonuafanj.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.blog.hesvh.cn/Article/details/gakhfetah.sHtML

PHP:  file_exists("a.txt");
来源：http://baike.hesvh.cn/Article/details/gwybovjbg.sHtML

JS:   fs.existsSync("a.txt")
来源：http://m.share.hesvh.cn/Article/details/geiqxxfep.sHtML

TS:   fs.existsSync("a.txt")
来源：http://read.share.hesvh.cn/Article/details/ghidoylbh.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gmssoimar.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.zdbjq.cn/Article/details/govxdlukv.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.fehbvm.com/Article/details/gerdoujfi.sHtML

C#:   File.Exists("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gxojbavpt.sHtML

[F06] 删除文件
来源：http://www.share.zdbjq.cn/Article/details/gzkcpwqrj.sHtML

Py:   os.remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gvzprpbxj.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/gcrcgedfo.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://www.share.hesvh.cn/Article/details/gwnonwdxb.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://baike.zdbjq.cn/Article/details/ghxybuadd.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.zdbjq.cn/Article/details/giztopgln.sHtML

Go:   os.Remove("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gkcofoqhr.sHtML

Ruby: File.delete("a.txt")
来源：http://3g.fehbvm.com/Article/details/gdnnzmyhn.sHtML

C#:   File.Delete("a.txt");
来源：http://wap.fehbvm.com/Article/details/gthkhlogm.sHtML

[F07] 创建目录（含多级）
来源：http://3g.fehbvm.com/Article/details/gqimlmswf.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://mobile.zdbjq.cn/Article/details/grkbewlhv.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.fehbvm.com/Article/details/gqipnkdrj.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://read.share.hesvh.cn/Article/details/glmzmfltv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.zdbjq.cn/Article/details/gkltfprsg.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fehbvm.com/Article/details/gvwpmilnm.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://mobile.zdbjq.cn/Article/details/ghjqsleph.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.blog.hesvh.cn/Article/details/ghslhjdih.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fehbvm.com/Article/details/ghsoabkgy.sHtML

[F08] 遍历目录
来源：http://mobile.hesvh.cn/Article/details/gpzjqagpr.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/gyhfftglb.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://blog.zdbjq.cn/Article/details/gsshcbtkb.sHtML

JS:   fs.readdirSync("dir")
来源：http://wap.zdbjq.cn/Article/details/grwlokggn.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.share.fehbvm.com/Article/details/guvuudmmd.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://m.share.zdbjq.cn/Article/details/gqbpzouhs.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://m.share.zdbjq.cn/Article/details/gezllmbqz.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.fehbvm.com/Article/details/gpqznliqk.sHtML

C#:   Directory.GetFiles("dir")
来源：http://wap.fehbvm.com/Article/details/gvfleirvc.sHtML

[F09] 获取文件大小
来源：http://read.share.fehbvm.com/Article/details/gmsmqlkba.sHtML

Py:   os.path.getsize("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gaojaqbaz.sHtML

PHP:  filesize("a.txt");
来源：http://baike.fehbvm.com/Article/details/gssxmkafx.sHtML

JS:   fs.statSync("a.txt").size
来源：http://m.share.zdbjq.cn/Article/details/giyksoinu.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.zdbjq.cn/Article/details/gkcwtwqwf.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://blog.fehbvm.com/Article/details/gixqpdqjg.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.hesvh.cn/Article/details/gxlqqclym.sHtML

Ruby: File.size("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gcltylthj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.hesvh.cn/Article/details/gpkhgfurw.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.hesvh.cn/Article/details/gbhtejxmz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gkigqkbtg.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gmtxiyfxx.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/gqlgqjmmv.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gifzoxvia.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://mobile.hesvh.cn/Article/details/gjuvuxaum.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gmdamszsk.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gfrgopztr.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://blog.zdbjq.cn/Article/details/gxhyouuoj.sHtML

[F11] 复制与移动文件
来源：http://m.share.hesvh.cn/Article/details/gqifwryax.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gdhfvqxpi.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://blog.hesvh.cn/Article/details/gblslwayc.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/ggashppqu.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.share.hesvh.cn/Article/details/gjbwkccko.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fehbvm.com/Article/details/gpobfwdpl.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fehbvm.com/Article/details/gaupkaycf.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.hesvh.cn/Article/details/geajktuni.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.fehbvm.com/Article/details/gehbuwuxv.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/gamuuoppg.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.fehbvm.com/Article/details/gehjksueh.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.hesvh.cn/Article/details/gqqajurkb.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://m.share.hesvh.cn/Article/details/gftyhiqjk.sHtML

TS:   // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gsdrrzhdo.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://read.share.hesvh.cn/Article/details/gwmolqfen.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.fehbvm.com/Article/details/gvecubctt.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.fehbvm.com/Article/details/gnjpqdvht.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://wap.zdbjq.cn/Article/details/gjhjcwioz.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfjoagwyq.sHtML

G. 面向对象
来源：http://www.share.zdbjq.cn/Article/details/gjgipmori.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gjcevnvkd.sHtML

[G01] 定义类
来源：http://baike.hesvh.cn/Article/details/gnliytndf.sHtML

Py:   class User: pass
来源：http://baike.hesvh.cn/Article/details/gpbhueyhh.sHtML

PHP:  class User {}
来源：http://m.share.fehbvm.com/Article/details/gaxxvudgj.sHtML

JS:   class User {}
来源：http://baike.hesvh.cn/Article/details/gxwpjuwgv.sHtML

TS:   class User { name: string = ""; }
来源：http://mobile.fehbvm.com/Article/details/gskzqcyst.sHtML

Java: class User {}
来源：http://blog.zdbjq.cn/Article/details/gxikxmswz.sHtML

Go:   type User struct { Name string }
来源：http://read.share.zdbjq.cn/Article/details/gvzlvedff.sHtML

Ruby: class User; end
来源：http://3g.hesvh.cn/Article/details/gotkqlqsm.sHtML

C#:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/ggpooqplz.sHtML

[G02] 构造函数
来源：http://blog.zdbjq.cn/Article/details/gbjaaypsr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://read.share.zdbjq.cn/Article/details/gzfsujacl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/ghfsuktmx.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.m.share.fehbvm.com/Article/details/gbrmynpbj.sHtML

TS:   constructor(public name: string) {}
来源：http://baike.hesvh.cn/Article/details/gsfbvgjiw.sHtML

Java: User(String name) { this.name = name; }
来源：http://read.share.hesvh.cn/Article/details/gzosbhwni.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.hesvh.cn/Article/details/gkavsjtre.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.hesvh.cn/Article/details/gkclpbuts.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gglaxxnuk.sHtML

[G03] 实例属性
来源：http://read.share.zdbjq.cn/Article/details/gdmhmveeh.sHtML

Py:   self.name = "x"
来源：http://www.m.share.hesvh.cn/Article/details/gqjxbtapx.sHtML

PHP:  public string $name = "x";
来源：http://read.share.hesvh.cn/Article/details/gjczwefxf.sHtML

JS:   this.name = "x";
来源：http://www.share.fehbvm.com/Article/details/ggbpnobsn.sHtML

TS:   name: string = "x";
来源：http://read.share.fehbvm.com/Article/details/gkygoigmb.sHtML

Java: private String name;
来源：http://read.share.hesvh.cn/Article/details/gutzsdwkg.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://3g.zdbjq.cn/Article/details/gtwwjjonc.sHtML

Ruby: @name = "x"
来源：http://m.share.fehbvm.com/Article/details/glorjmjtg.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.fehbvm.com/Article/details/gejcjvfvp.sHtML

[G04] 定义方法
来源：http://wap.hesvh.cn/Article/details/gepqcahys.sHtML

Py:   def greet(self): return self.name
来源：http://read.share.zdbjq.cn/Article/details/gzlyowpit.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fehbvm.com/Article/details/gwvtrbkba.sHtML

JS:   greet() { return this.name; }
来源：http://blog.hesvh.cn/Article/details/gdkzrmbwy.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gvxqtfkix.sHtML

Java: String greet() { return name; }
来源：http://wap.zdbjq.cn/Article/details/gjningqwa.sHtML


<!-- 参考信息 -->