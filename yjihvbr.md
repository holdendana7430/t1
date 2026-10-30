代发 wailian999

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://m.share.hesvh.cn/Article/details/ggvcokond.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.hesvh.cn/Article/details/gmmqnsknq.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://3g.hesvh.cn/Article/details/gkqarqltf.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://blog.fehbvm.com/Article/details/gackvhusl.sHtML

[E06] 替换子串
来源：http://read.share.hesvh.cn/Article/details/gljtsprru.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://m.share.hesvh.cn/Article/details/gkdkepxkk.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://mobile.hesvh.cn/Article/details/grxudoewn.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://baike.hesvh.cn/Article/details/gposvcwsl.sHtML

TS:   s.replaceAll("a", "b")
来源：http://www.blog.fehbvm.com/Article/details/gxuobzhvg.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fehbvm.com/Article/details/goebdadxi.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.share.zdbjq.cn/Article/details/gahxcynia.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://m.share.hesvh.cn/Article/details/gpkpxbxqn.sHtML

C#:   s.Replace("a", "b")
来源：http://www.share.zdbjq.cn/Article/details/gbxzpzwui.sHtML

[E07] 按分隔符拆分
来源：http://read.share.hesvh.cn/Article/details/gbwamolzj.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://3g.hesvh.cn/Article/details/gwimfjjdd.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fehbvm.com/Article/details/glnyjhmuy.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://mobile.zdbjq.cn/Article/details/gmzctrvnw.sHtML

TS:   s.split(",")
来源：http://read.share.fehbvm.com/Article/details/gtruvqqna.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://wap.fehbvm.com/Article/details/guivkmvqm.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.hesvh.cn/Article/details/guyzfdlhq.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fehbvm.com/Article/details/garsrqvpp.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://wap.fehbvm.com/Article/details/gfbiyojvh.sHtML

[E08] 数组按分隔符合并
来源：http://read.share.hesvh.cn/Article/details/gelqrvjaq.sHtML

Py:   ",".join(items)
来源：http://wap.zdbjq.cn/Article/details/gedaorwki.sHtML

PHP:  implode(",", $items);
来源：http://m.share.fehbvm.com/Article/details/gobyvavds.sHtML

JS:   items.join(",")
来源：http://baike.hesvh.cn/Article/details/gdvbfnoli.sHtML

TS:   items.join(",")
来源：http://blog.zdbjq.cn/Article/details/gepwfpamg.sHtML

Java: String.join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gkxbxffsc.sHtML

Go:   strings.Join(items, ",")
来源：http://baike.zdbjq.cn/Article/details/gzfbkpfux.sHtML

Ruby: items.join(",")
来源：http://www.share.fehbvm.com/Article/details/gypczghtn.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fehbvm.com/Article/details/gzakptflc.sHtML

[E09] 去除所有空白字符
来源：http://baike.zdbjq.cn/Article/details/gnbzabpra.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.m.share.fehbvm.com/Article/details/gvcdbavsm.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.zdbjq.cn/Article/details/guozzkdlf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://wap.hesvh.cn/Article/details/glzhejaxe.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.blog.hesvh.cn/Article/details/gpwzpiqfr.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://wap.zdbjq.cn/Article/details/godmpkgzj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://3g.fehbvm.com/Article/details/ghmuusily.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://read.share.fehbvm.com/Article/details/gtqbabqql.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fehbvm.com/Article/details/glrptbamz.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.zdbjq.cn/Article/details/gzioqiffq.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://3g.fehbvm.com/Article/details/gbaesnkza.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fehbvm.com/Article/details/garhlfynt.sHtML

JS:   "7".padStart(3, "0")
来源：http://3g.zdbjq.cn/Article/details/gcoamniuw.sHtML

TS:   "7".padStart(3, "0")
来源：http://3g.hesvh.cn/Article/details/gyxbvsxmh.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.hesvh.cn/Article/details/gqkwvcwgq.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.blog.zdbjq.cn/Article/details/gkcbytvzp.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.fehbvm.com/Article/details/gygapotpa.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://mobile.zdbjq.cn/Article/details/gkvgdzhit.sHtML

[E11] 反转字符串
来源：http://blog.zdbjq.cn/Article/details/grpyrxbtv.sHtML

Py:   s[::-1]
来源：http://wap.hesvh.cn/Article/details/gxwqueecn.sHtML

PHP:  strrev($s);
来源：http://m.share.fehbvm.com/Article/details/gdobalarl.sHtML

JS:   [...s].reverse().join("")
来源：http://m.share.fehbvm.com/Article/details/ghzamywsx.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.zdbjq.cn/Article/details/gylnytpaj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.zdbjq.cn/Article/details/gqzfzmgli.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://m.share.hesvh.cn/Article/details/gnshfskyn.sHtML

Ruby: s.reverse
来源：http://3g.zdbjq.cn/Article/details/gvhhpewmu.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://blog.fehbvm.com/Article/details/gchwmfnkd.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.hesvh.cn/Article/details/gjhkytzcr.sHtML

Py:   s.count("a")
来源：http://3g.fehbvm.com/Article/details/gwtzteggj.sHtML

PHP:  substr_count($s, "a");
来源：http://www.m.share.hesvh.cn/Article/details/gmjvazptk.sHtML

JS:   s.split("a").length - 1
来源：http://wap.hesvh.cn/Article/details/gmtpayfyh.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fehbvm.com/Article/details/grplkjhcc.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://baike.fehbvm.com/Article/details/ghvqcmwuz.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.zdbjq.cn/Article/details/gflnchgkp.sHtML

Ruby: s.count("a")
来源：http://baike.fehbvm.com/Article/details/gyshukbgh.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fehbvm.com/Article/details/gpwlcbauo.sHtML

[E13] 逐字符遍历
来源：http://baike.hesvh.cn/Article/details/grtwbyxuc.sHtML

Py:   for ch in s: print(ch)
来源：http://3g.zdbjq.cn/Article/details/godbwfanl.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://read.share.hesvh.cn/Article/details/gzgbljufi.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://wap.zdbjq.cn/Article/details/gayasamlw.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.hesvh.cn/Article/details/gtvlbpywl.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://blog.hesvh.cn/Article/details/gbzagiyjz.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://blog.hesvh.cn/Article/details/gqykncquj.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.zdbjq.cn/Article/details/gadafzibh.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://blog.fehbvm.com/Article/details/gscyjizjv.sHtML

[E14] URL 编码与 Base64
来源：http://baike.zdbjq.cn/Article/details/gpdyhmzoo.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://blog.fehbvm.com/Article/details/gvuhdwzzd.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fehbvm.com/Article/details/gfapuunmh.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://m.share.zdbjq.cn/Article/details/gcphmhxqr.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.blog.zdbjq.cn/Article/details/gngmustqh.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.zdbjq.cn/Article/details/gigthavpq.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.zdbjq.cn/Article/details/gqdflkxbi.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://read.share.fehbvm.com/Article/details/glxeiatat.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.hesvh.cn/Article/details/gntbmxxgi.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.m.share.fehbvm.com/Article/details/gxztfsxwk.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.zdbjq.cn/Article/details/gsvvszzqj.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://3g.zdbjq.cn/Article/details/gosaqjhan.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.hesvh.cn/Article/details/gmksixwvo.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://blog.zdbjq.cn/Article/details/gjhenlwfa.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://wap.zdbjq.cn/Article/details/gligjprdl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.share.fehbvm.com/Article/details/grpjyovmf.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.zdbjq.cn/Article/details/ggsxhuzcb.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://3g.hesvh.cn/Article/details/gijgeiwcy.sHtML

[E16] 数字千分位
来源：http://www.share.fehbvm.com/Article/details/ghpebsnda.sHtML

Py:   f"{1234567:,}"
来源：http://3g.zdbjq.cn/Article/details/gkswididv.sHtML

PHP:  number_format(1234567);
来源：http://blog.zdbjq.cn/Article/details/ghzxhjeoe.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.m.share.fehbvm.com/Article/details/ghejorrjy.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://wap.zdbjq.cn/Article/details/gwtktakfi.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.zdbjq.cn/Article/details/gfwiiqypu.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.m.share.hesvh.cn/Article/details/ghotpfmwg.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fehbvm.com/Article/details/gpcfkwegx.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.hesvh.cn/Article/details/ganfcfywj.sHtML

[E17] 首字母大写
来源：http://baike.fehbvm.com/Article/details/gmjyzsbqa.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://baike.fehbvm.com/Article/details/gmfkbzwey.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://mobile.fehbvm.com/Article/details/ggkbqpnfk.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://3g.zdbjq.cn/Article/details/gnwayiodp.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.zdbjq.cn/Article/details/grichdikd.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.hesvh.cn/Article/details/gcmkvraca.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.hesvh.cn/Article/details/ghugustrs.sHtML

Ruby: s.capitalize
来源：http://baike.hesvh.cn/Article/details/gqzaenore.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.m.share.hesvh.cn/Article/details/gfwjzgegu.sHtML

[E18] 模板占位符替换
来源：http://wap.hesvh.cn/Article/details/gavgklnvz.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://baike.hesvh.cn/Article/details/gebtcitlr.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fehbvm.com/Article/details/gitfjottb.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/ghrfolrcv.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://3g.fehbvm.com/Article/details/gfamezskx.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://blog.zdbjq.cn/Article/details/ggcthztcm.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://read.share.fehbvm.com/Article/details/gbhgyjqmk.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://mobile.zdbjq.cn/Article/details/gtnqaomon.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://read.share.zdbjq.cn/Article/details/gurdyvaok.sHtML

[E19] 多行文本按行拆分
来源：http://wap.zdbjq.cn/Article/details/gtekjgnyg.sHtML

Py:   s.splitlines()
来源：http://www.share.zdbjq.cn/Article/details/gsdoborpm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://baike.fehbvm.com/Article/details/gnlisuqqg.sHtML

JS:   s.split(/\r?\n/)
来源：http://blog.fehbvm.com/Article/details/glhrjkqmp.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.fehbvm.com/Article/details/gsdxwxkcj.sHtML

Java: s.lines().toList()
来源：http://m.share.zdbjq.cn/Article/details/ghgrpefbl.sHtML

Go:   strings.Split(s, "\n")
来源：http://3g.fehbvm.com/Article/details/gecdpsoyt.sHtML

Ruby: s.lines
来源：http://baike.fehbvm.com/Article/details/gdfbxxmfh.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/gcucscksd.sHtML

[E20] 判断字符串是否为空
来源：http://3g.fehbvm.com/Article/details/gotwbkwfh.sHtML

Py:   if not s:
来源：http://www.share.fehbvm.com/Article/details/gkivmovhm.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.fehbvm.com/Article/details/gklnviooq.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://blog.hesvh.cn/Article/details/gvwbewmtg.sHtML

TS:   if (s === "") {}
来源：http://m.share.hesvh.cn/Article/details/ghlbcitma.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fehbvm.com/Article/details/guhrmkfqv.sHtML

Go:   if s == "" {}
来源：http://m.share.fehbvm.com/Article/details/ghgtcebwc.sHtML

Ruby: if s.empty?
来源：http://mobile.hesvh.cn/Article/details/grzwxegho.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://mobile.fehbvm.com/Article/details/gxfgtqhap.sHtML

[E21] 超长截断加省略号
来源：http://3g.fehbvm.com/Article/details/gesuzcmrp.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.hesvh.cn/Article/details/gpkmghwuc.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://wap.fehbvm.com/Article/details/grmjnsvlq.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fehbvm.com/Article/details/gopodmddb.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://mobile.hesvh.cn/Article/details/gdevibwcl.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://3g.fehbvm.com/Article/details/glbmfmaqd.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://m.share.fehbvm.com/Article/details/gebstabgn.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://wap.hesvh.cn/Article/details/gcpmhkvzh.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.hesvh.cn/Article/details/gmkgqmkmr.sHtML

[E22] 字节长度与字符长度
来源：http://3g.hesvh.cn/Article/details/gmezdjfvj.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.blog.zdbjq.cn/Article/details/gycxyokaj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.m.share.fehbvm.com/Article/details/glfacwgql.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://3g.hesvh.cn/Article/details/gjsiebhky.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/glncetdxz.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://wap.hesvh.cn/Article/details/gdankieuc.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.blog.zdbjq.cn/Article/details/gmngjfuwz.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.m.share.zdbjq.cn/Article/details/gswdcoirb.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://baike.hesvh.cn/Article/details/gmnlpusth.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gnivbgjiu.sHtML

F. 文件与目录
来源：http://wap.hesvh.cn/Article/details/guxghmslw.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gawnuxemp.sHtML

[F01] 读取整个文件
来源：http://read.share.fehbvm.com/Article/details/ggxslhwbk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://read.share.fehbvm.com/Article/details/glqgtwbfg.sHtML

PHP:  file_get_contents("a.txt");
来源：http://blog.hesvh.cn/Article/details/gwfqpghpt.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.zdbjq.cn/Article/details/gqtlubyfv.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://blog.hesvh.cn/Article/details/gpmsimyrk.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gizpexikf.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fehbvm.com/Article/details/gyhvtpqqd.sHtML

Ruby: File.read("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/glzskpagj.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.hesvh.cn/Article/details/glolrcrcg.sHtML

[F02] 逐行读取文件
来源：http://mobile.zdbjq.cn/Article/details/gqpyqgzff.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.fehbvm.com/Article/details/ghxtxrhdk.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://read.share.fehbvm.com/Article/details/grmbixurm.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gwjcsbxap.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://read.share.hesvh.cn/Article/details/gvadsysex.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/gwnjdjziu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.blog.fehbvm.com/Article/details/gsmiyjshd.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fehbvm.com/Article/details/gacggyswj.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fehbvm.com/Article/details/gtrkkxwrf.sHtML

[F03] 写入文件（覆盖）
来源：http://3g.fehbvm.com/Article/details/gjqbxaiuv.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://3g.zdbjq.cn/Article/details/gkccovavy.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://mobile.zdbjq.cn/Article/details/gubsxbxpv.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://baike.hesvh.cn/Article/details/gyfpvehbi.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.zdbjq.cn/Article/details/gfmkltmhf.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.share.zdbjq.cn/Article/details/gmrietqly.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.zdbjq.cn/Article/details/gaycvnczi.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://blog.hesvh.cn/Article/details/ggreztioo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://m.share.hesvh.cn/Article/details/goqkoikcp.sHtML

[F04] 追加写入文件
来源：http://3g.hesvh.cn/Article/details/ggmzxxttm.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.hesvh.cn/Article/details/gaqxuoaje.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://blog.zdbjq.cn/Article/details/giiqavlza.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fehbvm.com/Article/details/gcdqudlvb.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.hesvh.cn/Article/details/gvbdwgpng.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://read.share.fehbvm.com/Article/details/gmxnsivyg.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fehbvm.com/Article/details/gyqxnpywl.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.m.share.fehbvm.com/Article/details/gzerdotqc.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.hesvh.cn/Article/details/geaewymlc.sHtML

[F05] 判断文件或目录是否存在
来源：http://3g.hesvh.cn/Article/details/ghqfnbojr.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/gepbkilyl.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gdoucdcpr.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.zdbjq.cn/Article/details/gfpwezihx.sHtML

TS:   fs.existsSync("a.txt")
来源：http://baike.hesvh.cn/Article/details/gldbycjps.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://read.share.hesvh.cn/Article/details/gnpykeexw.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://blog.fehbvm.com/Article/details/gkhkcwzry.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gbrereajy.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gboivxwsd.sHtML

[F06] 删除文件
来源：http://wap.hesvh.cn/Article/details/ggmwkjsfe.sHtML

Py:   os.remove("a.txt")
来源：http://read.share.fehbvm.com/Article/details/gnvrlhcxg.sHtML

PHP:  unlink("a.txt");
来源：http://baike.hesvh.cn/Article/details/gjnvjorjn.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://read.share.fehbvm.com/Article/details/glvimlngs.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/glwzbhsrv.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gugopyomi.sHtML

Go:   os.Remove("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gntnmsasa.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gguvkvapo.sHtML

C#:   File.Delete("a.txt");
来源：http://3g.zdbjq.cn/Article/details/gbjgsokkk.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/gjrfergfh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fehbvm.com/Article/details/gkydinxbr.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.m.share.zdbjq.cn/Article/details/gahkupbem.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://blog.fehbvm.com/Article/details/gjpxhrtsa.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fehbvm.com/Article/details/gjbvsskiq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://baike.zdbjq.cn/Article/details/gfgoqjnjq.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://read.share.fehbvm.com/Article/details/gzhmhphzx.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.zdbjq.cn/Article/details/ghopoxdwp.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://blog.fehbvm.com/Article/details/gqeknvwvl.sHtML

[F08] 遍历目录
来源：http://baike.fehbvm.com/Article/details/gwijgajux.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.zdbjq.cn/Article/details/gyoltsqpl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://m.share.fehbvm.com/Article/details/gmnvhmgnb.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gfxamikct.sHtML

TS:   fs.readdirSync("dir")
来源：http://www.blog.zdbjq.cn/Article/details/gtvsnkqst.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://mobile.hesvh.cn/Article/details/gbahlzebh.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/gdpftymkb.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.hesvh.cn/Article/details/goazupezf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://3g.zdbjq.cn/Article/details/gsaegsysm.sHtML

[F09] 获取文件大小
来源：http://m.share.hesvh.cn/Article/details/gditzgcwg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gsbiepmdm.sHtML

PHP:  filesize("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gpkulfavu.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.hesvh.cn/Article/details/gudpqzaqg.sHtML

TS:   fs.statSync("a.txt").size
来源：http://baike.hesvh.cn/Article/details/gaaspvhsz.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://m.share.fehbvm.com/Article/details/gwttzdpjw.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://baike.fehbvm.com/Article/details/gyqbuyulc.sHtML

Ruby: File.size("a.txt")
来源：http://read.share.zdbjq.cn/Article/details/gcsfvyidj.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://blog.hesvh.cn/Article/details/gpskobwgb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://mobile.hesvh.cn/Article/details/gwlhdcztz.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gftctgzms.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.hesvh.cn/Article/details/gamejkkkg.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gmqmpthpc.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gjnzngdbr.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/gsgujoenw.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://read.share.fehbvm.com/Article/details/gdraoyybn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://wap.fehbvm.com/Article/details/gsilxlawd.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/grlyireac.sHtML

[F11] 复制与移动文件
来源：http://baike.hesvh.cn/Article/details/gulqoizoc.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://wap.zdbjq.cn/Article/details/gjlcknvfs.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gtdjgynks.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://baike.hesvh.cn/Article/details/gwivvgjid.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://blog.fehbvm.com/Article/details/gclgqftua.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.hesvh.cn/Article/details/gnbcvtgqj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://baike.fehbvm.com/Article/details/gamsphtdi.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://blog.zdbjq.cn/Article/details/gdtuzcefy.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.blog.zdbjq.cn/Article/details/gdeqxdefj.sHtML

[F12] CSV 读写
来源：http://3g.zdbjq.cn/Article/details/gjryhlfgd.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://3g.hesvh.cn/Article/details/gugzniojv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fehbvm.com/Article/details/geljguxpj.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://wap.fehbvm.com/Article/details/grxvlatnq.sHtML

TS:   // 同上
来源：http://www.m.share.fehbvm.com/Article/details/gemknywzj.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://blog.zdbjq.cn/Article/details/gwbrvwlro.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.hesvh.cn/Article/details/gcpnrdnwy.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.share.fehbvm.com/Article/details/gsxztuqko.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://m.share.fehbvm.com/Article/details/ggnrfrmir.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gmtqlbxqv.sHtML

G. 面向对象
来源：http://blog.hesvh.cn/Article/details/gtcfhnkkj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gkvfuqenw.sHtML

[G01] 定义类
来源：http://blog.zdbjq.cn/Article/details/gyfclwdtj.sHtML

Py:   class User: pass
来源：http://www.m.share.hesvh.cn/Article/details/gzwudigit.sHtML

PHP:  class User {}
来源：http://blog.zdbjq.cn/Article/details/grzrdlzbm.sHtML

JS:   class User {}
来源：http://baike.hesvh.cn/Article/details/gskmwikvh.sHtML

TS:   class User { name: string = ""; }
来源：http://3g.zdbjq.cn/Article/details/gtzvrvevi.sHtML

Java: class User {}
来源：http://blog.hesvh.cn/Article/details/gdzdlkzaj.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fehbvm.com/Article/details/gvfmjbxkm.sHtML

Ruby: class User; end
来源：http://baike.zdbjq.cn/Article/details/ghnhwtodf.sHtML

C#:   class User {}
来源：http://www.blog.fehbvm.com/Article/details/gtzjetueb.sHtML

[G02] 构造函数
来源：http://baike.fehbvm.com/Article/details/gexmxzbrr.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://m.share.hesvh.cn/Article/details/gfqlmfcsl.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.hesvh.cn/Article/details/gjxgforus.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.zdbjq.cn/Article/details/gbjddxfbv.sHtML

TS:   constructor(public name: string) {}
来源：http://read.share.fehbvm.com/Article/details/gdsutyark.sHtML

Java: User(String name) { this.name = name; }
来源：http://3g.zdbjq.cn/Article/details/gkglqkbaz.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://read.share.hesvh.cn/Article/details/glisfdiiw.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://read.share.hesvh.cn/Article/details/galaenrvr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gnaxndchm.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/gkqkqcheh.sHtML

Py:   self.name = "x"
来源：http://blog.zdbjq.cn/Article/details/gspkcsapz.sHtML

PHP:  public string $name = "x";
来源：http://m.share.fehbvm.com/Article/details/gvpkfwrlr.sHtML

JS:   this.name = "x";
来源：http://wap.hesvh.cn/Article/details/glrbaaupc.sHtML

TS:   name: string = "x";
来源：http://blog.fehbvm.com/Article/details/geushpwra.sHtML

Java: private String name;
来源：http://3g.hesvh.cn/Article/details/gwgdrhibs.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://wap.fehbvm.com/Article/details/gvwdnxszs.sHtML

Ruby: @name = "x"
来源：http://blog.zdbjq.cn/Article/details/gftaocztm.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://www.blog.fehbvm.com/Article/details/gqwozffps.sHtML

[G04] 定义方法
来源：http://mobile.zdbjq.cn/Article/details/gmyabfukw.sHtML

Py:   def greet(self): return self.name
来源：http://www.m.share.hesvh.cn/Article/details/gohpxgsmc.sHtML


<!-- 参考信息 -->