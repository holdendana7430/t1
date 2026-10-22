代发 wailian999

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2hovuauhy.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2oxiqicbq.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2tlsdzwsg.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2ijxinwsr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2azuqeikx.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2cawjtliv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wbkcfybd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2zxyjiwqq.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rmxdzzxl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2ztguzesw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ekurbxly.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vjfmicfx.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2dhhjcnlu.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2eprjxodx.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2isykaxph.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dwpksxlr.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ulqrxskm.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qskrvxsm.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ykhvdgmm.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2udzaheah.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2nfjinddd.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2tasbyxva.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2bjbgoaqu.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2eywbxcxn.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2yfuasrpd.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2aebahqrz.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2uutvmebm.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mcmjsomq.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2vpnlflry.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2eopxdhir.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2hdsuzber.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2pqppooja.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2ywkpzgvl.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2fjknoyfh.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2wyfxuefp.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2iocbfowv.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2qfgvglda.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wckgxdsr.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ohzqfbiz.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2aafijxgb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2yxtwelqu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2aziiwugk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2ckotxazi.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2qwcijbcy.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2xszawjmv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2wyhmgqri.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2yqrlmogk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2tslowsdl.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2pgtcrlja.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2hxwdwhpq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2uqqgishq.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2sraxxgiz.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2romuhshi.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2mgokngrp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2okzegrjj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vsjezrdh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2josdavlc.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2gfutevjo.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2nelxhflt.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2huxohxrp.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zvagbcrs.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wxspptbz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2bqgwswdm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2uodkhcdj.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2aupvkegr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2gwtsbpbk.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2gbmlamvf.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2vqkeftec.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2hymoyzov.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ivwbjonw.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ofovikzf.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2hnnpzopr.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2cydsnina.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2lavrcwiu.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2pvwpdlfj.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2gujminzw.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2uoiddtjc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2rkyumpbo.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2lwhhelrb.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ugjnajoq.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vyogdzik.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wcbglwuf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2eawimudo.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2brfoftdh.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2kfmthvhi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2jdllwand.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2yqplcoju.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2kfyarles.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2vckdygnf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2iwgpgbdt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2eesaczgt.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2rqfphkkr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2vcneivhc.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2puunlpkc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2gqvroisf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2zeahbfvo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2vqvhqtug.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2bvjmdzvo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2opmpiffd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2sjzujguv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jxurkfkx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dldvombx.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2gofxktpt.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2pashesur.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2svshosyn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2qjprjyus.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2emytkqeu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2hjqgbsuz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2dmdblvao.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2xsxjqhvp.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2otmkmsia.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2oedoryph.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2bsrscyqk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2srduspqm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2srygywfy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2jkyicxqx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sxsepxpk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2nxhdeuwf.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2derqkqvu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2ibsuupdn.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2vsvzqkby.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2dxedghlu.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2gwrjexhl.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ggyqmcps.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2dzyteopq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rzznnfnb.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jkpqvicy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2xnxieria.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2bpgahovj.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2eiuoheer.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2cuntvnbd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2xoqdnmzn.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ltlybxeu.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2ajjaytju.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2debqvagd.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2zsqtuyan.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2gvwrnaca.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2vmzxhhaf.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2fmurymbe.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2ufyhkxlh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2knuwsxrd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ucsusgxo.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2sekxkyaf.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2focddiiy.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2zcywamqy.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2iltnskln.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2msmwkvrj.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2yrmpreri.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2jlznynux.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2jslcsdvs.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2uenxwwex.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wvbffutm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2yyzctxcw.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2gyjxzmgs.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2dwpzynyi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zfiqprrk.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2iypapyud.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lrqpxqov.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rubjacyl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ywuaybxg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fdtjrejy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2fofbsvso.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2sswdcfuq.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2qezoaqam.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2svkuneqv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hqtfhqmu.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2udlwwoas.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mewzpvrn.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2ieefupgh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2hrbyyfte.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zdafswve.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2qsoarzrs.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2zatmurki.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xbbaochz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2cfqauwpw.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pvcrkylf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2njpmlfvu.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2dgjwvfjs.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2ckxmtdyq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2nztxobei.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2kapnonve.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qiicutah.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2wkauztzh.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2xhwvkixf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2bexdrulq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2goejvrkk.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2tcuydksq.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2iwxukgak.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ohwtjcsy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2zrluhxmo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2iwbwxinq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ghebcjbo.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2dobozttb.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2hnyyytye.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2irvrvwsb.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2namsnwml.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dhjcypxe.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2imdnixir.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2jhhejjko.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ipjxapiq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2jsnjiyie.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tucqdxhb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2dnjoipdr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2nktlzokd.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2lptmmpjj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2iebsywet.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2gvrgkxnk.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aipiatsx.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qlhnovdd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ilslfuhg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2mfveqgdk.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yfjiabfy.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hdbmcilu.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2bixgjzkq.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dcpthfyl.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2glyxempl.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wsdqafjz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mxxddjak.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2iggopaiy.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iduukpkj.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lxvxdibv.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nnboacrj.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2wykjgohp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2ckcamwql.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2duhqkqcg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2lfxjmaeo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2tocgoyyt.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2gayeeenk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2tppzctor.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2jfframyg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2xwszllnd.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2wvbcuocz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2qndilsjn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2xkwoqqsx.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2yguttltd.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2zapdamrp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ayiqhfqb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2nmolbtcq.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2eifcooba.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2oalsrvbv.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2hgqfowwm.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gvekdudf.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qjuqayvu.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2umfnkije.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2athnwomo.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2pmhpiprs.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2udhpkyhm.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ksspvrar.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2qwfrzkdl.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2eygegprv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2abfwsqbw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ocatvrvo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2faomwlep.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hualeqap.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2szqmfrcg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hpumdvpd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hzcbfyhy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nzjrctuc.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2trravoac.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2maibvdlp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bxnrezdt.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2pnuyskxs.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2nyjffneh.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2yipbvbtt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2yeoordvq.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dehdaypg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2wtksjyoh.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2ynugldmk.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2boyyqndm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2qajmsnro.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2fbhpzwns.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2tmvcetay.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2hidwsoih.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2hkycztgd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2zkaqydnl.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2cszudzgx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mmrfajwp.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2zuueeouz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dluqzrtj.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2jwcujwkc.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2wrlrsbum.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2hfzpjnwk.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2aweulald.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2zwbfnsxc.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2bwlydnvp.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2ghamtchd.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2auggsoxb.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ehspjfgw.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2wnzmynuo.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2xlvkdrxk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2duybsupn.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghsfjgkm.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2zvqrgisk.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qvzdqrqd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2wzkmgnkn.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2flwcwyww.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ggspiwnc.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2uikbwqot.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2bwpeyshj.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2mhlnsjxt.html


<!-- 参考信息 -->