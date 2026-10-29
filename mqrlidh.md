代发 wailian999

Ruby: s.split(",");  s.split
来源：http://read.share.zdbjq.cn/Article/details/gvmqcoejn.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://read.share.fehbvm.com/Article/details/ggbbzlruz.sHtML

[E08] 数组按分隔符合并
来源：http://www.m.share.fehbvm.com/Article/details/gkgepzjdd.sHtML

Py:   ",".join(items)
来源：http://baike.hesvh.cn/Article/details/gpfttutgg.sHtML

PHP:  implode(",", $items);
来源：http://read.share.hesvh.cn/Article/details/gacjslqgl.sHtML

JS:   items.join(",")
来源：http://www.share.hesvh.cn/Article/details/gxozhszxn.sHtML

TS:   items.join(",")
来源：http://mobile.fehbvm.com/Article/details/glauyzzgw.sHtML

Java: String.join(",", items)
来源：http://blog.fehbvm.com/Article/details/gusszknzm.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.hesvh.cn/Article/details/gcjmhzbzx.sHtML

Ruby: items.join(",")
来源：http://baike.fehbvm.com/Article/details/gyqeayzfd.sHtML

C#:   string.Join(",", items)
来源：http://3g.fehbvm.com/Article/details/ggsxnmytl.sHtML

[E09] 去除所有空白字符
来源：http://3g.hesvh.cn/Article/details/grpijpvuf.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.hesvh.cn/Article/details/griawwjmb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.share.fehbvm.com/Article/details/guyksiqxf.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.hesvh.cn/Article/details/geyzqdauz.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.zdbjq.cn/Article/details/gcvumhgwk.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://m.share.hesvh.cn/Article/details/gxpzqswnj.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://mobile.zdbjq.cn/Article/details/gpmlqqrux.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.blog.fehbvm.com/Article/details/gmnfdubpl.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fehbvm.com/Article/details/geybidfdp.sHtML

[E10] 左侧补零 / 定长填充
来源：http://read.share.hesvh.cn/Article/details/gkblpvldo.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.hesvh.cn/Article/details/gmtmrkipi.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://3g.fehbvm.com/Article/details/gybwuaxvb.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.zdbjq.cn/Article/details/gipxysdlr.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.blog.zdbjq.cn/Article/details/gkwiieeda.sHtML

Java: String.format("%03d", 7)
来源：http://mobile.hesvh.cn/Article/details/gzjzxksdr.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://read.share.fehbvm.com/Article/details/ghjurjfcj.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.m.share.hesvh.cn/Article/details/grcazfteo.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://blog.zdbjq.cn/Article/details/gblfaulft.sHtML

[E11] 反转字符串
来源：http://3g.fehbvm.com/Article/details/gvqgcvcpn.sHtML

Py:   s[::-1]
来源：http://baike.fehbvm.com/Article/details/gwfndkudl.sHtML

PHP:  strrev($s);
来源：http://mobile.fehbvm.com/Article/details/gtqsamjeb.sHtML

JS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/goqkbxhvm.sHtML

TS:   [...s].reverse().join("")
来源：http://www.share.zdbjq.cn/Article/details/gflzqpaqa.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fehbvm.com/Article/details/gaaviqibv.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://baike.hesvh.cn/Article/details/gqaehdkeg.sHtML

Ruby: s.reverse
来源：http://blog.zdbjq.cn/Article/details/gdptsagkt.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://baike.zdbjq.cn/Article/details/gkxitzrsu.sHtML

[E12] 统计某字符出现次数
来源：http://www.share.zdbjq.cn/Article/details/gcnxhfihk.sHtML

Py:   s.count("a")
来源：http://mobile.zdbjq.cn/Article/details/gowdttbac.sHtML

PHP:  substr_count($s, "a");
来源：http://read.share.zdbjq.cn/Article/details/gphijkisi.sHtML

JS:   s.split("a").length - 1
来源：http://mobile.zdbjq.cn/Article/details/gsoujweni.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fehbvm.com/Article/details/gcuccgqju.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.hesvh.cn/Article/details/gvtzgusut.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.hesvh.cn/Article/details/gdzyvyfhw.sHtML

Ruby: s.count("a")
来源：http://read.share.zdbjq.cn/Article/details/gadkajmnk.sHtML

C#:   s.Count(c => c == 'a')
来源：http://www.m.share.hesvh.cn/Article/details/gyrbantek.sHtML

[E13] 逐字符遍历
来源：http://www.blog.hesvh.cn/Article/details/gdeeehrbo.sHtML

Py:   for ch in s: print(ch)
来源：http://wap.zdbjq.cn/Article/details/glzvwegod.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.zdbjq.cn/Article/details/gykfuzbrb.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://read.share.fehbvm.com/Article/details/gicxyldrq.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://wap.fehbvm.com/Article/details/gsbtrekgf.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.zdbjq.cn/Article/details/gdkbycwvu.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://m.share.fehbvm.com/Article/details/ggospeazr.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fehbvm.com/Article/details/gqkbqgzkz.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://read.share.zdbjq.cn/Article/details/gadsynjwa.sHtML

[E14] URL 编码与 Base64
来源：http://www.m.share.hesvh.cn/Article/details/gqnjlkcqg.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.m.share.fehbvm.com/Article/details/gtmrjitfl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://blog.fehbvm.com/Article/details/gfhxlbpok.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://mobile.zdbjq.cn/Article/details/gkaahrepd.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://blog.zdbjq.cn/Article/details/gitkfozkg.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.zdbjq.cn/Article/details/gywbsgntv.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://mobile.hesvh.cn/Article/details/gfelltefi.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.blog.hesvh.cn/Article/details/gviclkuka.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://3g.zdbjq.cn/Article/details/grwmkxact.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.blog.hesvh.cn/Article/details/gtsvblkju.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://mobile.hesvh.cn/Article/details/gnbebqggc.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://read.share.fehbvm.com/Article/details/gdrtmzeob.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://baike.zdbjq.cn/Article/details/gguzgbtmv.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.m.share.fehbvm.com/Article/details/gkjoleayh.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.m.share.hesvh.cn/Article/details/gprwwqyng.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://m.share.fehbvm.com/Article/details/gcrfysspx.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://3g.fehbvm.com/Article/details/gmtbueoer.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://blog.hesvh.cn/Article/details/gibmqfevw.sHtML

[E16] 数字千分位
来源：http://3g.zdbjq.cn/Article/details/gwgsirjsf.sHtML

Py:   f"{1234567:,}"
来源：http://read.share.fehbvm.com/Article/details/gibohlefr.sHtML

PHP:  number_format(1234567);
来源：http://mobile.zdbjq.cn/Article/details/gcdmppczd.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.hesvh.cn/Article/details/gubmcrblg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://www.blog.fehbvm.com/Article/details/gdbdoenlg.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://m.share.zdbjq.cn/Article/details/gjlgdsgye.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://m.share.hesvh.cn/Article/details/gpdlwysbz.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fehbvm.com/Article/details/gtkvcykmq.sHtML

C#:   1234567.ToString("N0")
来源：http://read.share.hesvh.cn/Article/details/gayderyyp.sHtML

[E17] 首字母大写
来源：http://blog.fehbvm.com/Article/details/gznhgfjam.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.m.share.zdbjq.cn/Article/details/giujrhpqs.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.share.fehbvm.com/Article/details/ggderwfeg.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://mobile.fehbvm.com/Article/details/ggktdlxbq.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.m.share.hesvh.cn/Article/details/gnkzeaksp.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://read.share.hesvh.cn/Article/details/ggfuquuka.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://wap.zdbjq.cn/Article/details/gdzzfohfc.sHtML

Ruby: s.capitalize
来源：http://baike.zdbjq.cn/Article/details/gcvvjjbnq.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://mobile.zdbjq.cn/Article/details/ggyunbmen.sHtML

[E18] 模板占位符替换
来源：http://blog.hesvh.cn/Article/details/gxxwbmdzd.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.m.share.zdbjq.cn/Article/details/ghhjdftir.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.m.share.zdbjq.cn/Article/details/gyrgorpyn.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://m.share.fehbvm.com/Article/details/gjryryavd.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://www.blog.hesvh.cn/Article/details/gfoaqamti.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.m.share.fehbvm.com/Article/details/gitkwuxfs.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://baike.zdbjq.cn/Article/details/gyauzytrl.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fehbvm.com/Article/details/gyvruibca.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.hesvh.cn/Article/details/gharknrra.sHtML

[E19] 多行文本按行拆分
来源：http://baike.hesvh.cn/Article/details/gdkvzfeub.sHtML

Py:   s.splitlines()
来源：http://wap.fehbvm.com/Article/details/ghhtdqwsl.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.zdbjq.cn/Article/details/goecgzvaz.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.zdbjq.cn/Article/details/gfnbhukil.sHtML

TS:   s.split(/\r?\n/)
来源：http://www.share.zdbjq.cn/Article/details/gubpltqst.sHtML

Java: s.lines().toList()
来源：http://wap.fehbvm.com/Article/details/glibnvmtv.sHtML

Go:   strings.Split(s, "\n")
来源：http://m.share.fehbvm.com/Article/details/gkpckevql.sHtML

Ruby: s.lines
来源：http://m.share.fehbvm.com/Article/details/gqrafpiai.sHtML

C#:   s.Split('\n')
来源：http://m.share.zdbjq.cn/Article/details/geuhxipll.sHtML

[E20] 判断字符串是否为空
来源：http://blog.fehbvm.com/Article/details/gucdrsrba.sHtML

Py:   if not s:
来源：http://3g.fehbvm.com/Article/details/gieoqpawg.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.blog.zdbjq.cn/Article/details/gjjyzbvzt.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://mobile.zdbjq.cn/Article/details/gzcovczbr.sHtML

TS:   if (s === "") {}
来源：http://www.blog.hesvh.cn/Article/details/gcqdfntdc.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.zdbjq.cn/Article/details/gcldylvmv.sHtML

Go:   if s == "" {}
来源：http://www.share.zdbjq.cn/Article/details/giacezbgs.sHtML

Ruby: if s.empty?
来源：http://baike.fehbvm.com/Article/details/gmurhoost.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.blog.fehbvm.com/Article/details/gpcpfaaug.sHtML

[E21] 超长截断加省略号
来源：http://baike.fehbvm.com/Article/details/goikmiakq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://3g.zdbjq.cn/Article/details/gywkyuxtl.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.blog.fehbvm.com/Article/details/gqztofoom.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://read.share.fehbvm.com/Article/details/gutorpjnq.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.zdbjq.cn/Article/details/gqkbybcrc.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.hesvh.cn/Article/details/ggrfbdfti.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.hesvh.cn/Article/details/gfsqwtopv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://m.share.hesvh.cn/Article/details/gxemeuztf.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.share.zdbjq.cn/Article/details/gwzrqqhxj.sHtML

[E22] 字节长度与字符长度
来源：http://3g.zdbjq.cn/Article/details/gaqrqeyhq.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.hesvh.cn/Article/details/gbwlaahhj.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://baike.fehbvm.com/Article/details/gmhwqyjhq.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://m.share.zdbjq.cn/Article/details/geccfzlfi.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://read.share.hesvh.cn/Article/details/gkkeykftv.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.blog.hesvh.cn/Article/details/gqljfwlez.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.hesvh.cn/Article/details/gmpgxmrrs.sHtML

Ruby: s.bytesize;  s.length
来源：http://wap.fehbvm.com/Article/details/gsrlsauku.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.zdbjq.cn/Article/details/grfdiwmgh.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/grrjetcro.sHtML

F. 文件与目录
来源：http://www.m.share.fehbvm.com/Article/details/gqncbmkhb.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gniqhwmps.sHtML

[F01] 读取整个文件
来源：http://www.m.share.hesvh.cn/Article/details/gwtihbehi.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.hesvh.cn/Article/details/gebsfvqyp.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.hesvh.cn/Article/details/grafgssbp.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://m.share.zdbjq.cn/Article/details/gtxjxibzs.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://read.share.zdbjq.cn/Article/details/gkmstphfg.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://3g.fehbvm.com/Article/details/gciedvwnz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fehbvm.com/Article/details/gumbckvyj.sHtML

Ruby: File.read("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gsrwmsomu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://www.share.zdbjq.cn/Article/details/gdozfjwdb.sHtML

[F02] 逐行读取文件
来源：http://m.share.fehbvm.com/Article/details/gerkzlddg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://mobile.hesvh.cn/Article/details/ggzsavijw.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfrvuglsn.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fehbvm.com/Article/details/gypfjzoco.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://mobile.fehbvm.com/Article/details/gjtdcrtkk.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.hesvh.cn/Article/details/gjsaoovsh.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://mobile.hesvh.cn/Article/details/gbzrywgmj.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://wap.zdbjq.cn/Article/details/gnyhqhebf.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://mobile.hesvh.cn/Article/details/gwppxqkyh.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.zdbjq.cn/Article/details/gsihclqqa.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://baike.zdbjq.cn/Article/details/gyhccpjwp.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gbiwozuim.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.blog.fehbvm.com/Article/details/gfskkhitz.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://read.share.hesvh.cn/Article/details/gpyiqhndv.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://3g.hesvh.cn/Article/details/gziyttuft.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.blog.fehbvm.com/Article/details/gtbeovddr.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://m.share.zdbjq.cn/Article/details/gvavogtuc.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://wap.hesvh.cn/Article/details/gdvjpzwwn.sHtML

[F04] 追加写入文件
来源：http://baike.fehbvm.com/Article/details/gwlwqzpqp.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://read.share.fehbvm.com/Article/details/gcibzhrsf.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://wap.fehbvm.com/Article/details/gedzwatsi.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://baike.zdbjq.cn/Article/details/ggalkktac.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.blog.zdbjq.cn/Article/details/gzkwwnbiy.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://mobile.hesvh.cn/Article/details/giblkmxnd.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.blog.fehbvm.com/Article/details/gknwmkyzd.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://3g.fehbvm.com/Article/details/ggmzxosny.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://3g.hesvh.cn/Article/details/gsebofwzw.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.zdbjq.cn/Article/details/grjfebdve.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://read.share.zdbjq.cn/Article/details/gmaacqpbb.sHtML

PHP:  file_exists("a.txt");
来源：http://www.m.share.zdbjq.cn/Article/details/gimyahiga.sHtML

JS:   fs.existsSync("a.txt")
来源：http://3g.zdbjq.cn/Article/details/gfgeoxdjp.sHtML

TS:   fs.existsSync("a.txt")
来源：http://wap.zdbjq.cn/Article/details/gizxgtraj.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.zdbjq.cn/Article/details/gmxkjzitq.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://read.share.zdbjq.cn/Article/details/gijsztfyz.sHtML

Ruby: File.exist?("a.txt")
来源：http://3g.hesvh.cn/Article/details/gnuhrqpui.sHtML

C#:   File.Exists("a.txt")
来源：http://www.blog.fehbvm.com/Article/details/gfxvoeeph.sHtML

[F06] 删除文件
来源：http://www.share.zdbjq.cn/Article/details/gslgjoybk.sHtML

Py:   os.remove("a.txt")
来源：http://baike.zdbjq.cn/Article/details/gelwcbhrl.sHtML

PHP:  unlink("a.txt");
来源：http://www.m.share.fehbvm.com/Article/details/gruhuygsh.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fehbvm.com/Article/details/gsyszokpr.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.hesvh.cn/Article/details/gkdqkxmze.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://baike.fehbvm.com/Article/details/gtpbpoijj.sHtML

Go:   os.Remove("a.txt")
来源：http://m.share.hesvh.cn/Article/details/gejvenooz.sHtML

Ruby: File.delete("a.txt")
来源：http://mobile.hesvh.cn/Article/details/ghvwtdhos.sHtML

C#:   File.Delete("a.txt");
来源：http://m.share.zdbjq.cn/Article/details/gqqjksfpw.sHtML

[F07] 创建目录（含多级）
来源：http://wap.zdbjq.cn/Article/details/grcyoject.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://blog.hesvh.cn/Article/details/gblpmughf.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.blog.fehbvm.com/Article/details/gtbvbmkpz.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.hesvh.cn/Article/details/gwmqoweeg.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.share.hesvh.cn/Article/details/gyxkaikbm.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://mobile.zdbjq.cn/Article/details/ggrmhtlon.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.zdbjq.cn/Article/details/gbosekllf.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://3g.fehbvm.com/Article/details/gkljlqmyw.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://3g.fehbvm.com/Article/details/gmsrqbwoq.sHtML

[F08] 遍历目录
来源：http://wap.hesvh.cn/Article/details/gqoxhsxlt.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://m.share.hesvh.cn/Article/details/gaimiyumq.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.blog.fehbvm.com/Article/details/gblfpxppz.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fehbvm.com/Article/details/gxwjzzgtr.sHtML

TS:   fs.readdirSync("dir")
来源：http://3g.hesvh.cn/Article/details/ghmxhsefr.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://read.share.fehbvm.com/Article/details/gcttstyxv.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.zdbjq.cn/Article/details/gtbxjyvow.sHtML

Ruby: Dir.children("dir")
来源：http://www.share.zdbjq.cn/Article/details/gkkebbnuc.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.hesvh.cn/Article/details/gsrjcekpx.sHtML

[F09] 获取文件大小
来源：http://wap.hesvh.cn/Article/details/gzzixqldg.sHtML

Py:   os.path.getsize("a.txt")
来源：http://3g.fehbvm.com/Article/details/grjuvznpa.sHtML

PHP:  filesize("a.txt");
来源：http://baike.zdbjq.cn/Article/details/ghaulfskk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://www.share.zdbjq.cn/Article/details/gjvlskbwv.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.m.share.hesvh.cn/Article/details/gxxxnwkst.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://read.share.fehbvm.com/Article/details/gffjfmnzp.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.blog.fehbvm.com/Article/details/gkftetkqq.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.zdbjq.cn/Article/details/gmhixkhel.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://mobile.hesvh.cn/Article/details/gljsombfb.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://wap.hesvh.cn/Article/details/gdwynpcol.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.blog.zdbjq.cn/Article/details/gejmkfzdn.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://baike.hesvh.cn/Article/details/gdyomfcww.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.m.share.fehbvm.com/Article/details/gzercpjjp.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fehbvm.com/Article/details/gdpjkkbfu.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://m.share.fehbvm.com/Article/details/gzsowntse.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fehbvm.com/Article/details/grrvdhbmn.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://m.share.fehbvm.com/Article/details/gvrajnnej.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://mobile.hesvh.cn/Article/details/gecqoshlk.sHtML

[F11] 复制与移动文件
来源：http://www.share.hesvh.cn/Article/details/gplfbsxhe.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.m.share.zdbjq.cn/Article/details/gpxfgvnfy.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://mobile.fehbvm.com/Article/details/gsyqjihhw.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://mobile.hesvh.cn/Article/details/gecrrxpte.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fehbvm.com/Article/details/gyxipfozc.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://blog.hesvh.cn/Article/details/gybpuskch.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://m.share.fehbvm.com/Article/details/gckhbhiin.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://read.share.fehbvm.com/Article/details/gccxvzusf.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://m.share.zdbjq.cn/Article/details/gpvgpbwnp.sHtML

[F12] CSV 读写
来源：http://www.share.hesvh.cn/Article/details/gszfjckdv.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fehbvm.com/Article/details/gglkwiavv.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://wap.fehbvm.com/Article/details/gpbvmbmwl.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.zdbjq.cn/Article/details/gcshinrfe.sHtML

TS:   // 同上
来源：http://mobile.hesvh.cn/Article/details/gepkcdrll.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://wap.zdbjq.cn/Article/details/gvvidmhan.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://m.share.zdbjq.cn/Article/details/gigzamith.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.zdbjq.cn/Article/details/gnchhvpco.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://read.share.hesvh.cn/Article/details/gjezfljjw.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkotjgupz.sHtML

G. 面向对象
来源：http://baike.hesvh.cn/Article/details/gjqkcqaff.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gkvclhrjo.sHtML

[G01] 定义类
来源：http://www.share.fehbvm.com/Article/details/genkjaqkt.sHtML

Py:   class User: pass
来源：http://www.share.zdbjq.cn/Article/details/gsrhxkwda.sHtML

PHP:  class User {}
来源：http://m.share.hesvh.cn/Article/details/gaodwwtrq.sHtML

JS:   class User {}
来源：http://www.share.zdbjq.cn/Article/details/gvwyhzqnw.sHtML

TS:   class User { name: string = ""; }
来源：http://blog.zdbjq.cn/Article/details/goabuvyxg.sHtML

Java: class User {}
来源：http://read.share.fehbvm.com/Article/details/gyucumxhz.sHtML

Go:   type User struct { Name string }
来源：http://m.share.fehbvm.com/Article/details/ggvallmza.sHtML

Ruby: class User; end
来源：http://blog.hesvh.cn/Article/details/gzjqzihlg.sHtML

C#:   class User {}
来源：http://www.share.fehbvm.com/Article/details/gcxqhkrym.sHtML

[G02] 构造函数
来源：http://blog.fehbvm.com/Article/details/gfqokbevi.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://baike.fehbvm.com/Article/details/gafvchvrk.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://mobile.hesvh.cn/Article/details/gilmkwcjq.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.share.fehbvm.com/Article/details/gxfpccgvo.sHtML

TS:   constructor(public name: string) {}
来源：http://www.m.share.hesvh.cn/Article/details/gawoucttx.sHtML

Java: User(String name) { this.name = name; }
来源：http://www.blog.fehbvm.com/Article/details/gtmoncrym.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://baike.hesvh.cn/Article/details/gwhyvyfna.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://baike.zdbjq.cn/Article/details/gctuhcekc.sHtML

C#:   public User(string name) { Name = name; }
来源：http://blog.fehbvm.com/Article/details/gnmouwafh.sHtML

[G03] 实例属性
来源：http://baike.fehbvm.com/Article/details/gnripoteh.sHtML

Py:   self.name = "x"
来源：http://blog.fehbvm.com/Article/details/guvktbreq.sHtML

PHP:  public string $name = "x";
来源：http://blog.fehbvm.com/Article/details/gzptjyatj.sHtML

JS:   this.name = "x";
来源：http://m.share.hesvh.cn/Article/details/gawkuynwp.sHtML

TS:   name: string = "x";
来源：http://baike.zdbjq.cn/Article/details/glwnxlkpi.sHtML

Java: private String name;
来源：http://read.share.fehbvm.com/Article/details/gpoiqpcwm.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.blog.hesvh.cn/Article/details/gohvumfhv.sHtML

Ruby: @name = "x"
来源：http://mobile.hesvh.cn/Article/details/gcyycxotn.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://mobile.zdbjq.cn/Article/details/gzwthdlsn.sHtML

[G04] 定义方法
来源：http://mobile.hesvh.cn/Article/details/gesqpfolq.sHtML

Py:   def greet(self): return self.name
来源：http://baike.fehbvm.com/Article/details/gtneihpef.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://baike.zdbjq.cn/Article/details/gwahgevlg.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fehbvm.com/Article/details/gxbjlpuub.sHtML

TS:   greet(): string { return this.name; }
来源：http://www.share.fehbvm.com/Article/details/gfjhhblis.sHtML

Java: String greet() { return name; }
来源：http://baike.fehbvm.com/Article/details/glaolwrrb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://mobile.fehbvm.com/Article/details/gnknhhkrw.sHtML

Ruby: def greet; @name; end
来源：http://mobile.fehbvm.com/Article/details/gltjdgbte.sHtML

C#:   public string Greet() => Name;
来源：http://wap.zdbjq.cn/Article/details/gacztjfhg.sHtML

[G05] 继承
来源：http://www.m.share.zdbjq.cn/Article/details/gtpoxsxks.sHtML

Py:   class Admin(User): pass
来源：http://www.share.zdbjq.cn/Article/details/glmhwiool.sHtML

PHP:  class Admin extends User {}
来源：http://www.m.share.zdbjq.cn/Article/details/gpxdxtnco.sHtML

JS:   class Admin extends User {}
来源：http://www.m.share.hesvh.cn/Article/details/gwlsigvlu.sHtML

TS:   class Admin extends User {}
来源：http://3g.hesvh.cn/Article/details/ggbgnmaea.sHtML

Java: class Admin extends User {}
来源：http://www.share.hesvh.cn/Article/details/gpwqpfskl.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://www.share.fehbvm.com/Article/details/gnnczifrd.sHtML

Ruby: class Admin < User; end
来源：http://blog.hesvh.cn/Article/details/gwvabbwou.sHtML

C#:   class Admin : User {}
来源：http://www.blog.hesvh.cn/Article/details/gkovihxes.sHtML

[G06] 重写方法
来源：http://www.blog.zdbjq.cn/Article/details/gquccerfb.sHtML

Py:   def greet(self): return "admin"
来源：http://www.m.share.fehbvm.com/Article/details/ggbmxrvco.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://mobile.hesvh.cn/Article/details/gwquccpzj.sHtML

JS:   greet() { return "admin"; }
来源：http://www.share.hesvh.cn/Article/details/gtmfdfqah.sHtML


<!-- 参考信息 -->