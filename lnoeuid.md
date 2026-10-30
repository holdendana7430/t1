代发 wailian999

PHP:  implode(",", $items);
来源：http://baike.fanxiaobao.xyz/Article/details/gxrwrjmmn.sHtML

JS:   items.join(",")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbdwdpsbb.sHtML

TS:   items.join(",")
来源：http://m.share.fanxiaobao.xyz/Article/details/gifpgvieh.sHtML

Java: String.join(",", items)
来源：http://baike.fanxiaobao.xyz/Article/details/gdnvbijux.sHtML

Go:   strings.Join(items, ",")
来源：http://www.share.fanxiaobao.xyz/Article/details/gshgoogmn.sHtML

Ruby: items.join(",")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gomtskadb.sHtML

C#:   string.Join(",", items)
来源：http://wap.fanxiaobao.xyz/Article/details/ggcqiplol.sHtML

[E09] 去除所有空白字符
来源：http://baike.fanxiaobao.xyz/Article/details/gioqhuxob.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://blog.fanxiaobao.xyz/Article/details/gzzsolnuy.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://blog.fanxiaobao.xyz/Article/details/ghfbpvgai.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://baike.fanxiaobao.xyz/Article/details/gcjvapevj.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://mobile.fanxiaobao.xyz/Article/details/gufivdbxx.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqidtlmxz.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fanxiaobao.xyz/Article/details/geduwhddf.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmfaoccfn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://baike.fanxiaobao.xyz/Article/details/gqwabahgb.sHtML

[E10] 左侧补零 / 定长填充
来源：http://baike.fanxiaobao.xyz/Article/details/gicjdygjk.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://wap.fanxiaobao.xyz/Article/details/gfdhyynun.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqxhxsyf.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwfeiqyby.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.share.fanxiaobao.xyz/Article/details/gefboijny.sHtML

Java: String.format("%03d", 7)
来源：http://3g.fanxiaobao.xyz/Article/details/gqlvtocux.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://3g.fanxiaobao.xyz/Article/details/ggjrvgynf.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqjkepyy.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkuymsawy.sHtML

[E11] 反转字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gvpebvytw.sHtML

Py:   s[::-1]
来源：http://m.share.fanxiaobao.xyz/Article/details/ggleaueqy.sHtML

PHP:  strrev($s);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkiyhnhvr.sHtML

JS:   [...s].reverse().join("")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnyarflbo.sHtML

TS:   [...s].reverse().join("")
来源：http://wap.fanxiaobao.xyz/Article/details/gtrgsdnie.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fanxiaobao.xyz/Article/details/gywmezjbk.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvhicdfg.sHtML

Ruby: s.reverse
来源：http://wap.fanxiaobao.xyz/Article/details/gytmmxtzf.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://read.share.fanxiaobao.xyz/Article/details/ggkqqcyvf.sHtML

[E12] 统计某字符出现次数
来源：http://mobile.fanxiaobao.xyz/Article/details/gnhdlaojc.sHtML

Py:   s.count("a")
来源：http://blog.fanxiaobao.xyz/Article/details/gwwxqsimv.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fanxiaobao.xyz/Article/details/gkngwkvyq.sHtML

JS:   s.split("a").length - 1
来源：http://baike.fanxiaobao.xyz/Article/details/goxyxiktz.sHtML

TS:   s.split("a").length - 1
来源：http://m.share.fanxiaobao.xyz/Article/details/ghxlqqmsw.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.share.fanxiaobao.xyz/Article/details/ghzeiteqo.sHtML

Go:   strings.Count(s, "a")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtmedvbh.sHtML

Ruby: s.count("a")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpfqugdyt.sHtML

C#:   s.Count(c => c == 'a')
来源：http://blog.fanxiaobao.xyz/Article/details/gycjagcao.sHtML

[E13] 逐字符遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/godujuypj.sHtML

Py:   for ch in s: print(ch)
来源：http://blog.fanxiaobao.xyz/Article/details/gaxwskdrp.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.share.fanxiaobao.xyz/Article/details/goonhoyih.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwpnuoeql.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://3g.fanxiaobao.xyz/Article/details/gfcxmiuty.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://3g.fanxiaobao.xyz/Article/details/grygxydws.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvocvnwk.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsfrfquir.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcghdyskt.sHtML

[E14] URL 编码与 Base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbaahwbu.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqarsmiv.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggbryflkq.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://3g.fanxiaobao.xyz/Article/details/ghbpkyusy.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://baike.fanxiaobao.xyz/Article/details/gdptzqohv.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://baike.fanxiaobao.xyz/Article/details/gegojgxiz.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://baike.fanxiaobao.xyz/Article/details/gvzpswcap.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://m.share.fanxiaobao.xyz/Article/details/gbreujvdk.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://read.share.fanxiaobao.xyz/Article/details/gajdecvzz.sHtML

[E15] HTML 转义 / 反转义
来源：http://www.share.fanxiaobao.xyz/Article/details/gymszmtqu.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gahdiwypy.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://blog.fanxiaobao.xyz/Article/details/gcgpkrggk.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxutlsgz.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/guqjfplqt.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmjuadvl.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwkzhcxy.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftothugd.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gzcxpefrh.sHtML

[E16] 数字千分位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqojobqa.sHtML

Py:   f"{1234567:,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gqjaqnzom.sHtML

PHP:  number_format(1234567);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwunohrz.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://www.share.fanxiaobao.xyz/Article/details/gaeqtvshq.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://baike.fanxiaobao.xyz/Article/details/gxdtvpqym.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://read.share.fanxiaobao.xyz/Article/details/gukyvfdju.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fanxiaobao.xyz/Article/details/gevvpixnj.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtapybvp.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fanxiaobao.xyz/Article/details/glfcskokk.sHtML

[E17] 首字母大写
来源：http://m.share.fanxiaobao.xyz/Article/details/gpieiearm.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://mobile.fanxiaobao.xyz/Article/details/gllmxcyul.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gerxblwbw.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfuklskis.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gbzqarant.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/ghwknokts.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmzfizuf.sHtML

Ruby: s.capitalize
来源：http://mobile.fanxiaobao.xyz/Article/details/gmtzsjsii.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fanxiaobao.xyz/Article/details/gpottqgtp.sHtML

[E18] 模板占位符替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/guhqbskoh.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://3g.fanxiaobao.xyz/Article/details/gjwmdcbxd.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://baike.fanxiaobao.xyz/Article/details/gefdsfety.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fanxiaobao.xyz/Article/details/gmpvuyuwu.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://mobile.fanxiaobao.xyz/Article/details/gazzigikn.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcbfdvpc.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://m.share.fanxiaobao.xyz/Article/details/glqjrcnvd.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gheurddcx.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://baike.fanxiaobao.xyz/Article/details/gkguwrafg.sHtML

[E19] 多行文本按行拆分
来源：http://baike.fanxiaobao.xyz/Article/details/gzwultmko.sHtML

Py:   s.splitlines()
来源：http://blog.fanxiaobao.xyz/Article/details/gasfmcefc.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://3g.fanxiaobao.xyz/Article/details/ggbdgnodz.sHtML

JS:   s.split(/\r?\n/)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgbperpf.sHtML

TS:   s.split(/\r?\n/)
来源：http://3g.fanxiaobao.xyz/Article/details/gfqsfthht.sHtML

Java: s.lines().toList()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwadtfmuk.sHtML

Go:   strings.Split(s, "\n")
来源：http://wap.fanxiaobao.xyz/Article/details/gmpvknhnf.sHtML

Ruby: s.lines
来源：http://baike.fanxiaobao.xyz/Article/details/gruhahdnr.sHtML

C#:   s.Split('\n')
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhfugvac.sHtML

[E20] 判断字符串是否为空
来源：http://baike.fanxiaobao.xyz/Article/details/gcjwdhqgh.sHtML

Py:   if not s:
来源：http://m.share.fanxiaobao.xyz/Article/details/gmrnaafsk.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://mobile.fanxiaobao.xyz/Article/details/grxsfynqm.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusbqvhma.sHtML

TS:   if (s === "") {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfxnzfvy.sHtML

Java: if (s.isEmpty()) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gacayxgvr.sHtML

Go:   if s == "" {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gjkawtjmo.sHtML

Ruby: if s.empty?
来源：http://wap.fanxiaobao.xyz/Article/details/grovssrjn.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghpcpxffs.sHtML

[E21] 超长截断加省略号
来源：http://read.share.fanxiaobao.xyz/Article/details/gcisfgyqq.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://wap.fanxiaobao.xyz/Article/details/gpudfocdb.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://read.share.fanxiaobao.xyz/Article/details/gfexpcmsb.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grkfltosk.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://m.share.fanxiaobao.xyz/Article/details/gmysnnfqs.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsywojaj.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxenusyv.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxvjbwcuc.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://3g.fanxiaobao.xyz/Article/details/gtgnutugv.sHtML

[E22] 字节长度与字符长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxoeptra.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxpdyvjz.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fanxiaobao.xyz/Article/details/gsthcmxab.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://baike.fanxiaobao.xyz/Article/details/gtnmvxbft.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://wap.fanxiaobao.xyz/Article/details/gfeymmruk.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://blog.fanxiaobao.xyz/Article/details/gtanoyurp.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fanxiaobao.xyz/Article/details/garsozupv.sHtML

Ruby: s.bytesize;  s.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gnshqvvwr.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrpdkjrr.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhqqsctl.sHtML

F. 文件与目录
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxinixfqx.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gibftjhil.sHtML

[F01] 读取整个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbavztzpk.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://baike.fanxiaobao.xyz/Article/details/gurzpwqlu.sHtML

PHP:  file_get_contents("a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqmizckm.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxkrvgeu.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgnuzzgi.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gtulpnrjz.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnzspqegk.sHtML

Ruby: File.read("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gthqqwldu.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvmlqdzd.sHtML

[F02] 逐行读取文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/garyuddio.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkzxbbjb.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://blog.fanxiaobao.xyz/Article/details/gssyahmjw.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gmppiakwm.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://wap.fanxiaobao.xyz/Article/details/gokgpiwdd.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://blog.fanxiaobao.xyz/Article/details/gjkirbxkl.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtdunkgq.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvhfpuabr.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://blog.fanxiaobao.xyz/Article/details/gorujoqdp.sHtML

[F03] 写入文件（覆盖）
来源：http://baike.fanxiaobao.xyz/Article/details/gseufyowf.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.share.fanxiaobao.xyz/Article/details/geuynzeiz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gunelfrfn.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.share.fanxiaobao.xyz/Article/details/gtabiagtk.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvyjlemmq.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://wap.fanxiaobao.xyz/Article/details/giesxbnxe.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhraahjn.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://baike.fanxiaobao.xyz/Article/details/ggaiubdvo.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://3g.fanxiaobao.xyz/Article/details/gwhyubyhm.sHtML

[F04] 追加写入文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwcrpmnu.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqrpzlnyj.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwsmdvwv.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fanxiaobao.xyz/Article/details/gwhcfnmog.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://wap.fanxiaobao.xyz/Article/details/grmfvglhg.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.share.fanxiaobao.xyz/Article/details/gsggmedqc.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://blog.fanxiaobao.xyz/Article/details/ghseroyuv.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gudiqjtdb.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fanxiaobao.xyz/Article/details/gcajnxnqm.sHtML

[F05] 判断文件或目录是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gmiwuwgpi.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwgqzhvim.sHtML

PHP:  file_exists("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrtumnkj.sHtML

JS:   fs.existsSync("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gnudufsjq.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gpqzyliah.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://blog.fanxiaobao.xyz/Article/details/gzrizwfjc.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtanuudx.sHtML

Ruby: File.exist?("a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/grnrympsm.sHtML

C#:   File.Exists("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gvklhnwid.sHtML

[F06] 删除文件
来源：http://mobile.fanxiaobao.xyz/Article/details/geygnmwuc.sHtML

Py:   os.remove("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gerlyuqcn.sHtML

PHP:  unlink("a.txt");
来源：http://blog.fanxiaobao.xyz/Article/details/gknaviaks.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/gvlzafczn.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giixumcpo.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmshnkaa.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvzybucj.sHtML

Ruby: File.delete("a.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjsvseoi.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/grtrgsdqt.sHtML

[F07] 创建目录（含多级）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtqjctpa.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://3g.fanxiaobao.xyz/Article/details/gutckjeei.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://mobile.fanxiaobao.xyz/Article/details/glqnbyach.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://mobile.fanxiaobao.xyz/Article/details/gkzdjrlxv.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fanxiaobao.xyz/Article/details/gxhzpffbv.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://3g.fanxiaobao.xyz/Article/details/gikvslysi.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fanxiaobao.xyz/Article/details/gjxiwjbay.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjoettcb.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://wap.fanxiaobao.xyz/Article/details/gcrifgqup.sHtML

[F08] 遍历目录
来源：http://read.share.fanxiaobao.xyz/Article/details/guvsxzjss.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://read.share.fanxiaobao.xyz/Article/details/gatpprveg.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsqklzqnx.sHtML

JS:   fs.readdirSync("dir")
来源：http://blog.fanxiaobao.xyz/Article/details/gmspvizsc.sHtML

TS:   fs.readdirSync("dir")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggbdnbuwo.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfejfmpjm.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://3g.fanxiaobao.xyz/Article/details/grbjdysmg.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnljpjeau.sHtML

C#:   Directory.GetFiles("dir")
来源：http://baike.fanxiaobao.xyz/Article/details/gijywdpks.sHtML

[F09] 获取文件大小
来源：http://wap.fanxiaobao.xyz/Article/details/ghqiscyuh.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gevolzzsm.sHtML

PHP:  filesize("a.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gubnkjtir.sHtML

JS:   fs.statSync("a.txt").size
来源：http://baike.fanxiaobao.xyz/Article/details/grdpzdglf.sHtML

TS:   fs.statSync("a.txt").size
来源：http://m.share.fanxiaobao.xyz/Article/details/gpajiiaud.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fanxiaobao.xyz/Article/details/gdrhenvwn.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://m.share.fanxiaobao.xyz/Article/details/gpszpeosm.sHtML

Ruby: File.size("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqkuurly.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://baike.fanxiaobao.xyz/Article/details/gbrrwfcbk.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://m.share.fanxiaobao.xyz/Article/details/gtbxcxcwk.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsatutlt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdzkuljzc.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmmfhzsk.sHtML

TS:   path.extname("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/grrmpcvtf.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://baike.fanxiaobao.xyz/Article/details/guxcndhos.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gqurdlweu.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/goymznbvo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/guhgkluzv.sHtML

[F11] 复制与移动文件
来源：http://blog.fanxiaobao.xyz/Article/details/gssqokoxq.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://m.share.fanxiaobao.xyz/Article/details/gofktcwny.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gpzkqdthg.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gbesckwqo.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gyymbkcap.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.share.fanxiaobao.xyz/Article/details/gghpnfvin.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://mobile.fanxiaobao.xyz/Article/details/gthaufdqp.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gotenyero.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://mobile.fanxiaobao.xyz/Article/details/gujdwnfpe.sHtML

[F12] CSV 读写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gliurislf.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://baike.fanxiaobao.xyz/Article/details/gmnbgewbt.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://read.share.fanxiaobao.xyz/Article/details/ghefmcrca.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://3g.fanxiaobao.xyz/Article/details/gcvgpgzqq.sHtML

TS:   // 同上
来源：http://read.share.fanxiaobao.xyz/Article/details/gtjupcnux.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzwhvmeif.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://3g.fanxiaobao.xyz/Article/details/ggphxgbyp.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvnwyecuc.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gorktqsme.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gauedtppb.sHtML

G. 面向对象
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqaywekm.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gtyhpsjum.sHtML

[G01] 定义类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnpmdnga.sHtML

Py:   class User: pass
来源：http://3g.fanxiaobao.xyz/Article/details/gawtmowjt.sHtML

PHP:  class User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gwvgifcvt.sHtML

JS:   class User {}
来源：http://mobile.fanxiaobao.xyz/Article/details/gxfclfjwz.sHtML

TS:   class User { name: string = ""; }
来源：http://wap.fanxiaobao.xyz/Article/details/gnhobjkpg.sHtML

Java: class User {}
来源：http://baike.fanxiaobao.xyz/Article/details/gzrdyvmgk.sHtML

Go:   type User struct { Name string }
来源：http://mobile.fanxiaobao.xyz/Article/details/gkaoxrmax.sHtML

Ruby: class User; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gsypghgkw.sHtML

C#:   class User {}
来源：http://wap.fanxiaobao.xyz/Article/details/gozslfkoe.sHtML

[G02] 构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmxlbflz.sHtML

Py:   def __init__(self, name): self.name = name
来源：http://wap.fanxiaobao.xyz/Article/details/ghcmifwta.sHtML

PHP:  public function __construct(public string $name) {}
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyrddsbc.sHtML

JS:   constructor(name) { this.name = name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrnxvpro.sHtML

TS:   constructor(public name: string) {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gcmbagtql.sHtML

Java: User(String name) { this.name = name; }
来源：http://blog.fanxiaobao.xyz/Article/details/ggjubgjol.sHtML

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://blog.fanxiaobao.xyz/Article/details/gkmflmhwj.sHtML

Ruby: def initialize(name); @name = name; end
来源：http://blog.fanxiaobao.xyz/Article/details/gwcnqexqr.sHtML

C#:   public User(string name) { Name = name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrejglrt.sHtML

[G03] 实例属性
来源：http://wap.fanxiaobao.xyz/Article/details/gbjdcbona.sHtML

Py:   self.name = "x"
来源：http://blog.fanxiaobao.xyz/Article/details/gejmcllzw.sHtML

PHP:  public string $name = "x";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlbpgyhu.sHtML

JS:   this.name = "x";
来源：http://3g.fanxiaobao.xyz/Article/details/gzqqxacgo.sHtML

TS:   name: string = "x";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnrnjbovy.sHtML

Java: private String name;
来源：http://baike.fanxiaobao.xyz/Article/details/gmdjmchwl.sHtML

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://baike.fanxiaobao.xyz/Article/details/gfhhgbmdw.sHtML

Ruby: @name = "x"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdrvgpul.sHtML

C#:   public string Name { get; set; } = "x";
来源：http://blog.fanxiaobao.xyz/Article/details/gxiydzirn.sHtML

[G04] 定义方法
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdbvxkad.sHtML

Py:   def greet(self): return self.name
来源：http://wap.fanxiaobao.xyz/Article/details/gqvyfbqwe.sHtML

PHP:  public function greet(): string { return $this->name; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzqmnbur.sHtML

JS:   greet() { return this.name; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghukjnfpt.sHtML

TS:   greet(): string { return this.name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gnizstoef.sHtML

Java: String greet() { return name; }
来源：http://3g.fanxiaobao.xyz/Article/details/gonadxvrb.sHtML

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpocyrfij.sHtML

Ruby: def greet; @name; end
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwrboxqz.sHtML

C#:   public string Greet() => Name;
来源：http://wap.fanxiaobao.xyz/Article/details/gkwfvdkgp.sHtML

[G05] 继承
来源：http://wap.fanxiaobao.xyz/Article/details/guoepjshd.sHtML

Py:   class Admin(User): pass
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkdqfdjvi.sHtML

PHP:  class Admin extends User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gfyppgtzi.sHtML

JS:   class Admin extends User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gommjkveo.sHtML

TS:   class Admin extends User {}
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmdqonmx.sHtML

Java: class Admin extends User {}
来源：http://read.share.fanxiaobao.xyz/Article/details/gcybimscf.sHtML

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://3g.fanxiaobao.xyz/Article/details/gzeloooyi.sHtML

Ruby: class Admin < User; end
来源：http://read.share.fanxiaobao.xyz/Article/details/ghevgzauz.sHtML

C#:   class Admin : User {}
来源：http://3g.fanxiaobao.xyz/Article/details/gjswydxfg.sHtML

[G06] 重写方法
来源：http://www.share.fanxiaobao.xyz/Article/details/gsfymepqp.sHtML

Py:   def greet(self): return "admin"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvipmlxbm.sHtML

PHP:  public function greet(): string { return "admin"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqkgxpdn.sHtML

JS:   greet() { return "admin"; }
来源：http://3g.fanxiaobao.xyz/Article/details/ghjscnqrq.sHtML

TS:   greet(): string { return "admin"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gdcturhfr.sHtML

Java: @Override String greet() { return "admin"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gureeqnnr.sHtML

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://blog.fanxiaobao.xyz/Article/details/gvfyzyfsz.sHtML

Ruby: def greet; "admin"; end
来源：http://mobile.fanxiaobao.xyz/Article/details/gtpwyzmzj.sHtML


<!-- 参考信息 -->