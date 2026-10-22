代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2nlakwcxc.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2wwyxickw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ozhwanmd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2dwqisiyu.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gtqajepx.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2ypcoutvd.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2piuahrxi.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2nflhgamu.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2nhkrfehd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2bqcxlbcd.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bvclgyyo.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yoteltkw.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2sghbaebr.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fyivcwmv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2edlpcykq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2aiaglwtp.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bejhgpik.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2xdotortv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2ararncke.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2urgecdsv.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2onhqjbhk.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2yfymdqhz.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2pmuybwjk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2otqbesid.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2cymslejc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2mtrltpkc.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2xakpwbzi.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2oevrxjfu.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2ikutfxqm.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2gehrasnl.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2sgndvddk.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2wqlpyxlr.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2fkibwdeh.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2flyiutxa.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2auugaxtx.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2omznepfs.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2ufnawipg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vhkswkdl.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2wgdchfoh.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2nqhtfvpg.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2ieoyzfex.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2yzhumqmw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2emrppolb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2hixoathl.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2vqmqfwdn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2tuttlays.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2vdjyckld.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2uljlgmwv.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2upkyqqkz.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2pjiqunhf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2tkkfxclm.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2thplpizw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2ouuulkjc.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2tsaajfex.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2mgayafkh.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2urtyrhcf.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ypmrcvcy.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2jfobdgun.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2irtubyir.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2qjnimjco.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2plcvxzbg.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2gznedktn.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2vnprzuzg.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2uzeljqko.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2kfgtqulk.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2sbwepysn.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2tktfsvcr.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2wxdlnnmi.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2arnnsffq.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2zjfdmdzw.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2swncybei.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2qsemcmts.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2szcblivs.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2uryqzjzz.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fhbdcjls.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xceuqbvw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2wdcwkavt.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2oreewdzj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2eokobsjv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2klkmavnt.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2rgsfwiir.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2tsamkpro.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2hugvpinj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2qxyiptmq.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2rvathbpk.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2ydwoqwiw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2gptpxjbz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2schsdtff.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2adzjnxrc.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2nfzjgzpp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aumkeudb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2nctuzajd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2uuyvyjlc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2ojfyrvep.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2dxkquqpt.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2kxemevlf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2usgrpfni.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2wbxijdeh.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2sajgcsjy.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2oaujpldp.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2gqlxinfh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2bgkughki.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2qumxhfyi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2duysjrim.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2xggkawpk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2jwcuujpz.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2hggemjfb.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2oxvmgook.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2wezkkfsf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2ejpbymik.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2dhoxqefo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kyztgldp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2ieaemkwm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2dudypjkt.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2bprczwmi.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ddrimsmr.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2rwcgmsin.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2inkewkzj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2uihnopxi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2irxgylkg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2klhqulde.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wpsxwrkz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2uhwdbxsx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2jkrhzobf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2khytpoqk.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2svpqwvaw.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2vwvmfetb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2suithcyo.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2armwxbyz.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2reraujks.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2vdufzzev.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2qbmeosrw.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2zsnbubxd.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2dnvmfhpt.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2xsmtgyym.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2cvzjagqd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2ykmlnsyh.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jndtteot.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2xoxplcel.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2ubmahadu.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2etqikodd.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2avnkjqjx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2xyfvjdsm.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2joanssaz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2reyimqkq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2yqowzkhj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2spwuxlgc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2idkxovck.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ehsruucz.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2otrwuazo.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ijcfwlui.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2rzeycusi.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2wfybakmb.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2ofgoitkm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2wvoltnwf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2hvhfrbgr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2oecrewqk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2klaccgbm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2vlnkcfsb.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2mkndjssa.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2qgchqtpr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fyyfggix.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2novtyypv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2owmysznn.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2wifzpyic.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2uillgcyk.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2pthvfevc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2jdrycodi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2qcztbphu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2dscjtsae.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2pyiulrfb.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zjlzvznq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nwtsuzsj.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2ganrcwqt.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2bbmtaxbn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2mzbdmbey.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2gldgifbu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jbusifnz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2qvxgqrpn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2fpwongay.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2agoswdqv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2eldudotl.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2bjagggjk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ljzkwmtz.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ezebkzut.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2xewcgcsg.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2lqdtzukv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ovnrotil.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2naetwkrp.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2ybsnkteq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2qtaafuwf.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2ufomneac.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2bpwgicrz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2tzdmyhyl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pgfgpnem.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2zgcmlmcs.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2voxurrix.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2yxqvutai.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2fdyagiyr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2ajcaqdhl.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2hpthhfzi.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2esximout.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2abnoergw.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aijskqid.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2axwinbbb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fdyjgyud.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2cedqboec.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vgbskhqs.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2paahqkbs.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2fgioribc.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2aksxkffh.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dqgecmlz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mpplnecc.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rmffgxht.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2baiempxr.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tjsquhoa.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zzdorott.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2brkmltvh.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2yovmbejl.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2xsffudyl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vunhmayq.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2yqxknrqn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2flzwebxp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2yrywzxql.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2irrmcimy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2dflsnkid.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2zbcusqur.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2dmvqqeqw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2axqhqynb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2qkxhpemx.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2gavpzqph.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2uslowycl.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2pqpasbax.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2urdlvnxi.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2awcrnwqo.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2wqpmwrth.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2xthebwmn.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ofbffwfx.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2uxghdtwt.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2bipmciri.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ymsfgjhw.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2rvodcbkw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2uexrlujp.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nzacdesm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2gzixnjkj.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2yteweigz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pendlpcp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2iewnfybg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zfpwciuk.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wyeyufvn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2uxcihlnw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zocwayht.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lfmfcafw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yfbxdqou.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2nmmvbflk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iayjftep.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2tshgwdxl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qolfmhxb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hfoipjdl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2sjjjkqfd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2iqvhnihz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kttjqhbn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2sisrtdkp.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2iwkoqoti.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2hcpastmr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2pknzerpn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2cciclwqa.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2feghupfw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2rgjyvftp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2rawdesjv.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2ayiffleg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2xdtscitj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pzigbzno.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2tpbjjets.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qmvnlkdl.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2gkxzgrye.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2ulxmtkvw.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2unyhscaj.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2mfkkkezn.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2lymvqjcw.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2yuextrok.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2ukdnrjct.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2sgqavvhb.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2lxdxipzm.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2imhzletw.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2bhpuezxj.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jjriegxa.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjikgjpp.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2hjtcblri.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2laxqdxdy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2jultvgec.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2pbrfaqlg.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2okzipehi.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2gcqhdcna.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2savanifi.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2xhyjwddu.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2tmtucqmh.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2xqfcwmcr.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2oxndjieo.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2jfyebuhh.html


<!-- 参考信息 -->