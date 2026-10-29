代发 wailian999

[E06] 替换子串
来源：http://blog.fehbvm.com/Article/details/glvjythfu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.hesvh.cn/Article/details/gdczixjds.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://3g.hesvh.cn/Article/details/geywhwpuy.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://blog.zdbjq.cn/Article/details/gbnrvgoct.sHtML

TS:   s.replaceAll("a", "b")
来源：http://blog.fehbvm.com/Article/details/gquzolbnd.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://m.share.fehbvm.com/Article/details/gqalcgkyf.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://m.share.zdbjq.cn/Article/details/gwepnwuvt.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://blog.hesvh.cn/Article/details/gxjzkgjvf.sHtML

C#:   s.Replace("a", "b")
来源：http://wap.fehbvm.com/Article/details/gqmiqvham.sHtML

[E07] 按分隔符拆分
来源：http://3g.zdbjq.cn/Article/details/gbvgqpour.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.blog.fehbvm.com/Article/details/glrlrjehi.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://3g.zdbjq.cn/Article/details/goutihfep.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://read.share.zdbjq.cn/Article/details/gsumorqok.sHtML

TS:   s.split(",")
来源：http://m.share.hesvh.cn/Article/details/gbhlxyrjt.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://www.blog.zdbjq.cn/Article/details/gtdgemmiv.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://blog.fehbvm.com/Article/details/gcmbsywvt.sHtML

Ruby: s.split(",");  s.split
来源：http://mobile.fehbvm.com/Article/details/gsrdmlbiz.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://baike.zdbjq.cn/Article/details/geigwxywr.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fehbvm.com/Article/details/gitvqjavu.sHtML

Py:   ",".join(items)
来源：http://baike.zdbjq.cn/Article/details/gyimfzucn.sHtML

PHP:  implode(",", $items);
来源：http://m.share.hesvh.cn/Article/details/gpbvhuvzb.sHtML

JS:   items.join(",")
来源：http://m.share.zdbjq.cn/Article/details/gkgddkwid.sHtML

TS:   items.join(",")
来源：http://m.share.fehbvm.com/Article/details/grfotxacq.sHtML

Java: String.join(",", items)
来源：http://baike.fehbvm.com/Article/details/gsyuvdppu.sHtML

Go:   strings.Join(items, ",")
来源：http://m.share.fehbvm.com/Article/details/gktacssoj.sHtML

Ruby: items.join(",")
来源：http://mobile.fehbvm.com/Article/details/gutayyfsx.sHtML

C#:   string.Join(",", items)
来源：http://mobile.fehbvm.com/Article/details/grrqnsstz.sHtML

[E09] 去除所有空白字符
来源：http://wap.zdbjq.cn/Article/details/gtmckrlrk.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://read.share.zdbjq.cn/Article/details/gmrjjsazs.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://read.share.fehbvm.com/Article/details/graxswcwq.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/gosxiihjg.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://blog.zdbjq.cn/Article/details/ggxuyqtvw.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://www.share.zdbjq.cn/Article/details/ggvkjwrvh.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.m.share.zdbjq.cn/Article/details/gjiamccoi.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.hesvh.cn/Article/details/gwawtahed.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://mobile.zdbjq.cn/Article/details/gxfshyotj.sHtML

[E10] 左侧补零 / 定长填充
来源：http://blog.zdbjq.cn/Article/details/gsyhicdef.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.blog.hesvh.cn/Article/details/gjdvwwfui.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://read.share.hesvh.cn/Article/details/gciipdjcb.sHtML

JS:   "7".padStart(3, "0")
来源：http://baike.hesvh.cn/Article/details/getkfeuiu.sHtML

TS:   "7".padStart(3, "0")
来源：http://wap.fehbvm.com/Article/details/gglnkamgw.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.zdbjq.cn/Article/details/ghwykxbvk.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://blog.hesvh.cn/Article/details/getnfugbu.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.zdbjq.cn/Article/details/gstquvwrb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.zdbjq.cn/Article/details/gbfektipu.sHtML

[E11] 反转字符串
来源：http://blog.hesvh.cn/Article/details/gpgyjyqrk.sHtML

Py:   s[::-1]
来源：http://www.blog.fehbvm.com/Article/details/gmbnwxgxf.sHtML

PHP:  strrev($s);
来源：http://3g.hesvh.cn/Article/details/gwrmfvmcp.sHtML

JS:   [...s].reverse().join("")
来源：http://blog.zdbjq.cn/Article/details/gmkjtqoql.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fehbvm.com/Article/details/gdqzwjsmj.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://wap.hesvh.cn/Article/details/gvzvjupmd.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.blog.zdbjq.cn/Article/details/gubzsqdkv.sHtML

Ruby: s.reverse
来源：http://3g.fehbvm.com/Article/details/ggojxqtno.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.blog.zdbjq.cn/Article/details/ggtgjvauy.sHtML

[E12] 统计某字符出现次数
来源：http://baike.zdbjq.cn/Article/details/gnvtzxucm.sHtML

Py:   s.count("a")
来源：http://www.m.share.hesvh.cn/Article/details/gaitssyvx.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.hesvh.cn/Article/details/gtvqyoiua.sHtML

JS:   s.split("a").length - 1
来源：http://3g.hesvh.cn/Article/details/gshbdbfsx.sHtML

TS:   s.split("a").length - 1
来源：http://www.m.share.fehbvm.com/Article/details/gvbsfmheh.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://3g.hesvh.cn/Article/details/gitfmlclg.sHtML

Go:   strings.Count(s, "a")
来源：http://www.blog.zdbjq.cn/Article/details/gzgaosiye.sHtML

Ruby: s.count("a")
来源：http://www.blog.zdbjq.cn/Article/details/gumstltfs.sHtML

C#:   s.Count(c => c == 'a')
来源：http://read.share.hesvh.cn/Article/details/ggnsndcqj.sHtML

[E13] 逐字符遍历
来源：http://baike.hesvh.cn/Article/details/gcdjjmmvt.sHtML

Py:   for ch in s: print(ch)
来源：http://m.share.fehbvm.com/Article/details/gmqcxbmuw.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://3g.hesvh.cn/Article/details/ginzovjoy.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.blog.zdbjq.cn/Article/details/guybypphq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gkzaplvfl.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fehbvm.com/Article/details/gzebaezuc.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.m.share.zdbjq.cn/Article/details/guqlhszyg.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://blog.hesvh.cn/Article/details/gpirqvkye.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://m.share.zdbjq.cn/Article/details/gesdcqiox.sHtML

[E14] URL 编码与 Base64
来源：http://mobile.fehbvm.com/Article/details/glkchmvce.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://wap.hesvh.cn/Article/details/gfzrwdtcb.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://wap.fehbvm.com/Article/details/grkvntwkf.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.zdbjq.cn/Article/details/gzcodmfgz.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.zdbjq.cn/Article/details/gthagxvjw.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.share.hesvh.cn/Article/details/gdkivtbdg.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://m.share.zdbjq.cn/Article/details/gsyowubdd.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://baike.fehbvm.com/Article/details/goqmrcgdt.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.hesvh.cn/Article/details/gfrgszbhz.sHtML

[E15] HTML 转义 / 反转义
来源：http://read.share.hesvh.cn/Article/details/gyiidnifx.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://m.share.fehbvm.com/Article/details/glmycjsts.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://wap.hesvh.cn/Article/details/ggbiffwsu.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.m.share.fehbvm.com/Article/details/gnwshiovm.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://mobile.hesvh.cn/Article/details/gzpimpwfu.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fehbvm.com/Article/details/goqeysnwy.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fehbvm.com/Article/details/gdsuqcjuc.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://baike.fehbvm.com/Article/details/gepslyqck.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.zdbjq.cn/Article/details/gcatjinwu.sHtML

[E16] 数字千分位
来源：http://3g.hesvh.cn/Article/details/gvjfsnmge.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/gkrqpzzut.sHtML

PHP:  number_format(1234567);
来源：http://read.share.zdbjq.cn/Article/details/gyvfbumco.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://wap.hesvh.cn/Article/details/gnkjbwstc.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://read.share.zdbjq.cn/Article/details/gsycfkaft.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.blog.hesvh.cn/Article/details/gkmfhuyyn.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://mobile.hesvh.cn/Article/details/gifaumxci.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.hesvh.cn/Article/details/guabnupvc.sHtML

C#:   1234567.ToString("N0")
来源：http://www.m.share.hesvh.cn/Article/details/glfjqyfmz.sHtML

[E17] 首字母大写
来源：http://www.m.share.fehbvm.com/Article/details/gktuoohgy.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://read.share.fehbvm.com/Article/details/ggehyaoyr.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.zdbjq.cn/Article/details/goqqhrqde.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://wap.fehbvm.com/Article/details/gwxscjbjo.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/guyjwwjaq.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://wap.fehbvm.com/Article/details/gzudvxejb.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://3g.zdbjq.cn/Article/details/guqcrrewp.sHtML

Ruby: s.capitalize
来源：http://read.share.zdbjq.cn/Article/details/gitkwjegt.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.blog.fehbvm.com/Article/details/gulbewvxq.sHtML

[E18] 模板占位符替换
来源：http://www.blog.hesvh.cn/Article/details/gkccwsfxm.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.share.fehbvm.com/Article/details/geruvofxq.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.hesvh.cn/Article/details/gzmybhsje.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fehbvm.com/Article/details/gsjgemmzq.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://m.share.hesvh.cn/Article/details/gyolchjuj.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://mobile.hesvh.cn/Article/details/gmhfmsmxd.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://3g.fehbvm.com/Article/details/gnscmzvzo.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://3g.zdbjq.cn/Article/details/gxpsmkzuu.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.m.share.zdbjq.cn/Article/details/gtxhgypik.sHtML

[E19] 多行文本按行拆分
来源：http://read.share.fehbvm.com/Article/details/gvbaveqkl.sHtML

Py:   s.splitlines()
来源：http://3g.zdbjq.cn/Article/details/gudnpszsp.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.zdbjq.cn/Article/details/gigctfamn.sHtML

JS:   s.split(/\r?\n/)
来源：http://wap.fehbvm.com/Article/details/gcacqsesc.sHtML

TS:   s.split(/\r?\n/)
来源：http://wap.hesvh.cn/Article/details/gplcertjd.sHtML

Java: s.lines().toList()
来源：http://mobile.zdbjq.cn/Article/details/gxfftnttm.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.m.share.fehbvm.com/Article/details/gevypantm.sHtML

Ruby: s.lines
来源：http://baike.hesvh.cn/Article/details/geztlcyyv.sHtML

C#:   s.Split('\n')
来源：http://www.blog.zdbjq.cn/Article/details/gsqamgonc.sHtML

[E20] 判断字符串是否为空
来源：http://baike.zdbjq.cn/Article/details/gkpjpquvf.sHtML

Py:   if not s:
来源：http://www.m.share.zdbjq.cn/Article/details/ggubpnuvi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://3g.zdbjq.cn/Article/details/gigyurfmr.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://read.share.hesvh.cn/Article/details/grafjfrsq.sHtML

TS:   if (s === "") {}
来源：http://baike.zdbjq.cn/Article/details/gurqyfsyx.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.m.share.fehbvm.com/Article/details/ggrnmmrhd.sHtML

Go:   if s == "" {}
来源：http://blog.zdbjq.cn/Article/details/gpmyemrwg.sHtML

Ruby: if s.empty?
来源：http://baike.hesvh.cn/Article/details/grblcydfa.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://read.share.hesvh.cn/Article/details/gnkirlhdb.sHtML

[E21] 超长截断加省略号
来源：http://mobile.fehbvm.com/Article/details/gncffgfkf.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fehbvm.com/Article/details/gkquaptvt.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.share.zdbjq.cn/Article/details/ghxsxyqpw.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gkzvcnogd.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.hesvh.cn/Article/details/gympmuqri.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.zdbjq.cn/Article/details/gbluqwuay.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://mobile.hesvh.cn/Article/details/gystdiaah.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.hesvh.cn/Article/details/gvfvtiqfn.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.blog.fehbvm.com/Article/details/gethjebva.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.fehbvm.com/Article/details/gmhixkhxa.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://blog.hesvh.cn/Article/details/gzbdcdpdh.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/giybsrxwp.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://mobile.zdbjq.cn/Article/details/geuljmuyh.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fehbvm.com/Article/details/gzoqzzswo.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.hesvh.cn/Article/details/gxuxancnu.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://3g.zdbjq.cn/Article/details/ggqcnssbk.sHtML

Ruby: s.bytesize;  s.length
来源：http://mobile.fehbvm.com/Article/details/gammgomfj.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://3g.hesvh.cn/Article/details/ggyazzddh.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/glnzutytc.sHtML

F. 文件与目录
来源：http://www.m.share.zdbjq.cn/Article/details/gsogrhcoo.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxcswfxcf.sHtML

[F01] 读取整个文件
来源：http://m.share.hesvh.cn/Article/details/ganwrxanf.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.share.fehbvm.com/Article/details/gpqcxynbv.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.hesvh.cn/Article/details/ggmuvbbey.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://read.share.fehbvm.com/Article/details/gtjicvbcy.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.share.hesvh.cn/Article/details/gngozyffx.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://baike.hesvh.cn/Article/details/gscwsdbkv.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.m.share.hesvh.cn/Article/details/glcypnezn.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/glttpqweq.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gmdasvyrd.sHtML

[F02] 逐行读取文件
来源：http://mobile.hesvh.cn/Article/details/gapdpetry.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.hesvh.cn/Article/details/gcvbskmav.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.hesvh.cn/Article/details/gxnbmhqtu.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.zdbjq.cn/Article/details/gfojzfovt.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.hesvh.cn/Article/details/goofkepid.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.blog.zdbjq.cn/Article/details/gsidfxhny.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.zdbjq.cn/Article/details/goizsvrav.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.m.share.hesvh.cn/Article/details/giwpsnhfu.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://m.share.fehbvm.com/Article/details/gccthelrq.sHtML

[F03] 写入文件（覆盖）
来源：http://www.m.share.hesvh.cn/Article/details/guzmojees.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.blog.fehbvm.com/Article/details/gbvakxkgk.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.share.hesvh.cn/Article/details/gymgjmkeu.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gleqfjnzk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gecurnpxs.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://blog.hesvh.cn/Article/details/gbstxbvdg.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.hesvh.cn/Article/details/gmqoylhdu.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.m.share.zdbjq.cn/Article/details/gzqhiesii.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://mobile.hesvh.cn/Article/details/gwebursjd.sHtML

[F04] 追加写入文件
来源：http://3g.fehbvm.com/Article/details/gnhwlmiua.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://baike.zdbjq.cn/Article/details/gwrnedyjv.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.share.fehbvm.com/Article/details/gbjvkjobd.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/govjldark.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://mobile.zdbjq.cn/Article/details/gqcvwsefn.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.hesvh.cn/Article/details/gtptunxuj.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.m.share.zdbjq.cn/Article/details/ghvjmuwni.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fehbvm.com/Article/details/gwziohnry.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.share.zdbjq.cn/Article/details/gzkytgbco.sHtML

[F05] 判断文件或目录是否存在
来源：http://mobile.zdbjq.cn/Article/details/glpebcrom.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.share.hesvh.cn/Article/details/gbzoadwqq.sHtML

PHP:  file_exists("a.txt");
来源：http://wap.hesvh.cn/Article/details/guehcirfs.sHtML

JS:   fs.existsSync("a.txt")
来源：http://mobile.hesvh.cn/Article/details/gbxxfzppd.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gqdpiyxob.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.blog.hesvh.cn/Article/details/gjjoprxhf.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.blog.fehbvm.com/Article/details/gylguamfs.sHtML

Ruby: File.exist?("a.txt")
来源：http://m.share.zdbjq.cn/Article/details/ggrtlvnyc.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.hesvh.cn/Article/details/giwtnajal.sHtML

[F06] 删除文件
来源：http://www.m.share.zdbjq.cn/Article/details/gpbhenecy.sHtML

Py:   os.remove("a.txt")
来源：http://3g.hesvh.cn/Article/details/globseqyg.sHtML

PHP:  unlink("a.txt");
来源：http://3g.hesvh.cn/Article/details/gfnjmfyjr.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gwiwccigj.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gzalqlfvm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.m.share.hesvh.cn/Article/details/gfbinkwrb.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.zdbjq.cn/Article/details/gwxyeamer.sHtML

Ruby: File.delete("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/grnrpqhcp.sHtML

C#:   File.Delete("a.txt");
来源：http://www.blog.fehbvm.com/Article/details/gwywlpnfg.sHtML

[F07] 创建目录（含多级）
来源：http://www.share.fehbvm.com/Article/details/gcgodmhtj.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.fehbvm.com/Article/details/gawaaavkg.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://m.share.fehbvm.com/Article/details/gwprzqugm.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.hesvh.cn/Article/details/gqqbpzean.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.m.share.hesvh.cn/Article/details/gbvypgzyq.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.hesvh.cn/Article/details/gjesuhhxi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.hesvh.cn/Article/details/gkzepnucp.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://mobile.zdbjq.cn/Article/details/gozpnuzpb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://m.share.zdbjq.cn/Article/details/gvxwzwfoh.sHtML

[F08] 遍历目录
来源：http://wap.fehbvm.com/Article/details/gungtpjen.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://baike.hesvh.cn/Article/details/gxtfwgljl.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://mobile.fehbvm.com/Article/details/gthsecdwi.sHtML

JS:   fs.readdirSync("dir")
来源：http://baike.zdbjq.cn/Article/details/gritgpkaf.sHtML

TS:   fs.readdirSync("dir")
来源：http://m.share.fehbvm.com/Article/details/gdtbcckik.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://blog.zdbjq.cn/Article/details/ggxxhmdnt.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://read.share.fehbvm.com/Article/details/gdzaucuou.sHtML

Ruby: Dir.children("dir")
来源：http://baike.hesvh.cn/Article/details/gvnmixgrf.sHtML

C#:   Directory.GetFiles("dir")
来源：http://www.share.hesvh.cn/Article/details/gnwfpuqtt.sHtML

[F09] 获取文件大小
来源：http://www.blog.fehbvm.com/Article/details/ghlovlmcf.sHtML

Py:   os.path.getsize("a.txt")
来源：http://baike.fehbvm.com/Article/details/gomgiqrpg.sHtML

PHP:  filesize("a.txt");
来源：http://read.share.zdbjq.cn/Article/details/gnywlsows.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gccterunb.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gvrkwugem.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://www.m.share.fehbvm.com/Article/details/gmbiwhoha.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://wap.zdbjq.cn/Article/details/gxfdonfbh.sHtML

Ruby: File.size("a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gqmyrnwpg.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://www.blog.fehbvm.com/Article/details/gsrlkotqe.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.zdbjq.cn/Article/details/gxpjobrik.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://m.share.hesvh.cn/Article/details/gzygryxvu.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://blog.hesvh.cn/Article/details/gaifscall.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://3g.hesvh.cn/Article/details/gpcanosde.sHtML

TS:   path.extname("a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gbvvaxpht.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://wap.zdbjq.cn/Article/details/ggjgkjsmt.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.blog.hesvh.cn/Article/details/gazwwfauc.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://baike.zdbjq.cn/Article/details/gyxzbvxrg.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.zdbjq.cn/Article/details/ghqddygiw.sHtML

[F11] 复制与移动文件
来源：http://www.share.zdbjq.cn/Article/details/glfptpffp.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gsrfzmiid.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.blog.fehbvm.com/Article/details/guzufkhxy.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.hesvh.cn/Article/details/gcngjlsce.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://m.share.fehbvm.com/Article/details/gmlnwuqwp.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.hesvh.cn/Article/details/gburnpejc.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.share.fehbvm.com/Article/details/grjdpsbne.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gjllsprct.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.share.hesvh.cn/Article/details/grfqkignm.sHtML

[F12] CSV 读写
来源：http://baike.hesvh.cn/Article/details/gxytkhgie.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.m.share.zdbjq.cn/Article/details/gilnvgzev.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.hesvh.cn/Article/details/gzcjnzoze.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.m.share.fehbvm.com/Article/details/grnbpnqxa.sHtML

TS:   // 同上
来源：http://3g.hesvh.cn/Article/details/gjzezgtyf.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://3g.fehbvm.com/Article/details/gmwhpmtmd.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://wap.hesvh.cn/Article/details/gtxknwwht.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.blog.zdbjq.cn/Article/details/gnpzatogu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.fehbvm.com/Article/details/gezwaksto.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gvoypxysw.sHtML

G. 面向对象
来源：http://www.blog.fehbvm.com/Article/details/gufrgfvpt.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gnucbkzxz.sHtML

[G01] 定义类
来源：http://read.share.zdbjq.cn/Article/details/ggpcxcfkx.sHtML

Py:   class User: pass
来源：http://mobile.fehbvm.com/Article/details/gftylqrap.sHtML

PHP:  class User {}
来源：http://wap.zdbjq.cn/Article/details/gediriisu.sHtML

JS:   class User {}
来源：http://read.share.hesvh.cn/Article/details/gafbfpjnw.sHtML

TS:   class User { name: string = ""; }
来源：http://read.share.hesvh.cn/Article/details/gazyfupog.sHtML

Java: class User {}
来源：http://m.share.fehbvm.com/Article/details/glhxruytq.sHtML

Go:   type User struct { Name string }
来源：http://blog.zdbjq.cn/Article/details/ghkkuwwpn.sHtML

Ruby: class User; end
来源：http://mobile.zdbjq.cn/Article/details/guoyoyhfz.sHtML

C#:   class User {}
来源：http://mobile.zdbjq.cn/Article/details/gpgjuragv.sHtML

[G02] 构造函数
来源：http://wap.hesvh.cn/Article/details/gfzorxkhb.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://www.share.zdbjq.cn/Article/details/gdedtxzkd.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://m.share.zdbjq.cn/Article/details/girzopudf.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gjwlggyaz.sHtML

TS:   constructor(public name: string) {}
来源：http://wap.zdbjq.cn/Article/details/gjyzxrtfu.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.share.zdbjq.cn/Article/details/gqgzkwwdg.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://mobile.hesvh.cn/Article/details/gvqyaogmm.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://www.m.share.hesvh.cn/Article/details/ghyfuhcxc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://3g.hesvh.cn/Article/details/gxforrhpi.sHtML

[G03] 实例属性
来源：http://3g.hesvh.cn/Article/details/gfuhqyvcm.sHtML

Py:   self.name = "x"
来源：http://baike.zdbjq.cn/Article/details/gpfqqrhre.sHtML

PHP:  public string $name = "x";
来源：http://m.share.zdbjq.cn/Article/details/ghhzwlypx.sHtML

JS:   this.name = "x";
来源：http://3g.zdbjq.cn/Article/details/gvyxikkzm.sHtML

TS:   name: string = "x";
来源：http://read.share.zdbjq.cn/Article/details/gmhvwqiua.sHtML

Java: private String name;
来源：http://www.share.fehbvm.com/Article/details/gnrdhquuc.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.hesvh.cn/Article/details/gxtgdktfs.sHtML

Ruby: @name = "x"
来源：http://blog.hesvh.cn/Article/details/gvgykypuy.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://3g.zdbjq.cn/Article/details/gexkyjcnh.sHtML

[G04] 定义方法
来源：http://mobile.hesvh.cn/Article/details/gpckgyfmt.sHtML

Py:   def greet(self): return self.name
来源：http://www.blog.zdbjq.cn/Article/details/gezlqqukj.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://m.share.hesvh.cn/Article/details/gwifxwvph.sHtML

JS:   greet() { return this.name; }
来源：http://www.m.share.hesvh.cn/Article/details/gzxuobiun.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gddapfzxf.sHtML

Java: String greet() { return name; }
来源：http://read.share.fehbvm.com/Article/details/ghqpjsfte.sHtML


<!-- 参考信息 -->