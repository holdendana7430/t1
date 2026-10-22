代发 wailian999

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2yyrihouv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2mmlinoja.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2vnzcstyo.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2bwhmyprt.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2aywwznri.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2zqjmwrxk.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fncsagwd.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2pjfccvud.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2silwuxbt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2izhvicwg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2kidlzhub.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2osaexszm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cbcccimy.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2pyekdqej.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wnwynggd.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2axixwfxn.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2zginiuyk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2hmadlttw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2rrunhgmp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cihgmgzr.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ugakvlxq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2qpbgcflu.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2ugnyyrhr.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kjmaeden.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2yehkbcdm.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2pvptjgru.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2nqrssiit.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2lfosujmu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2abltrmqm.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2kugctyyf.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2qduughrc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tmmygtab.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ltghtbuh.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2ycwqabfx.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2ufsbgeyr.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2gvursicr.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2hcawqgen.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2wivmysfr.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2dqjqkftb.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2udsovstz.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2hublqoks.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ovbajati.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2moelqgsy.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2kirzvunb.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2yxowtent.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mtrtyhbu.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2iebupxko.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2jqxadczu.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2qtubeycm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2vzkrtmbj.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2duxohmin.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2zcmsllty.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2nzbhzgev.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2jbrktxrv.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2wjlqkqik.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rqtlbpxk.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2oxainccy.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2kuadfhqe.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2tawysyxk.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ocbserjm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2qcabntcg.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2niquzczu.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2qrmuanho.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jmyzlfxl.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mzuqystq.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xhoegrlp.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2gkwkzion.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2oqachwmf.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2qbnhwswp.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2dhwdmwrw.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2uhbodmdq.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2wsxcxudt.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2rhzdfece.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2imldbple.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2pzgrwkdu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2hdisrkmh.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2gujowahb.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2rrzvyioi.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2gpwzhhqw.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2aaszsimm.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2upeplike.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2jarprljb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ikhtjjpc.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2cqmmduzh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fumaneep.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2mrfcplxj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2gdpnsvrm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zxpvripi.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2cerjmdpw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2tiewjwik.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2recovcio.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2tdjwqexy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2mhmvtkdz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2oixzvvjt.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2zfdhfkpi.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2xpskkkui.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2waohikwz.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2pzkflsfd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2cusfuxam.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ztbgzvce.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xkyvovod.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2akcgceqn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2gltnxyrd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2azqmixif.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2ralbcbom.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2qbzgswjw.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2rdujypia.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2ugoybsyd.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2xipxvdki.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2xawnjdji.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2afuvpfhx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2pdawxtde.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2iigjnhjk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2pdgqthzj.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2lrqbjzqc.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2hkpcmoch.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2ibbzdqac.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2xwwxqgex.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zoajesco.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2pkkgugat.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2ulxvtjwi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2vqlojfwd.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2vyoxfmza.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2gibpogar.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2bfgspxqc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2buihpnko.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2twtxlzxm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2hxklaqgq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rxmxkhfw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2jivegoqx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2omqoevla.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2ygubhocy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2tpbcepny.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2hnoxybvm.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2wmhmfhcd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2udlazcxb.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2nuqbhevd.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2bvlkfany.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2tiulywtx.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2logzvhnv.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2dxuygxrx.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2xvqhkjel.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2ewzmwahd.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2wiyvcrmn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2zrfbrlfo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tsmnuhdk.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2abmuwqkf.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2xpkhnrrd.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2utkgckkr.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2rjdxvdms.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2mrrrbibn.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2uihhmqvq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2wqqhlkla.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2txjrqrrr.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ilzyxnwk.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2rhbmmnsx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2uvrravdf.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2vqthlwbw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2myvtjucy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2slcdqrxo.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2hpjhhrfr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ngkdnqva.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2niexltgc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2qbnnvnrf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2dmdunywe.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2diklcaxk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2bcvstrto.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2vzfvazgt.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2fwwbutsq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kqnctarh.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2matqtrkq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pugnqffo.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2zibbeojj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2yjsumbfs.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2zkkdshsv.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2agpusufc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2oywfmvjd.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ockxfbeb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2iblvfosa.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yrowlhyw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mfszjchg.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2plfyjfqo.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2uyrxcmce.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2bmnqwodx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xaimtujx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mcgtssmc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2pforwhqc.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2meracdbu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2turhjeva.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2nerabtom.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2qbviofvp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2igpjpmqn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2oolneiad.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2fwbgtixi.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2hjtpplma.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ukbgvmmb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2jdvonprr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2uyhhkwos.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2exmrutrt.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2dmhevuzi.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bajtubah.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2jzwqyhuq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wqeyytlo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2mvlyznnp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2rnzqayvn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2omivkgma.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2soxcauxg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2anygvjax.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2svfojtgr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2euafmknz.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bddabdqy.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fmwwquzw.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lqoktgdy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jygwwkno.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2uodhaese.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2veqdtndd.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yxtczqrx.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2opcffpjt.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dbhqldfj.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ftofuwfx.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ialblmrt.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2olwkiiym.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wcxqbabh.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fylhulmg.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hblhctxh.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2egqioubq.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2dqkqdaof.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2hkezfzls.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2hzforftn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2fapuralh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2rgfjmwgq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2obfboigm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2vjqxzewy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2ynnzyvyz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2jgqzowig.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ftmmsnfg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2geuntwku.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2redyrvwa.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2hjaremrq.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ioojrqbe.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2akwfjvsi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2bwqtmdjp.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2gxdecluq.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2rskedikm.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2nsniisqr.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nzwznfla.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ktwoipgl.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2aszlgcew.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2lbnllwha.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2gsqfitxy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2esvjqxuy.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cqlictus.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2eopwpljv.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2sunnmyda.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ckyuajup.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gmltzxwb.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bgmeabjl.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wotxqoas.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2jorugiqn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lszynspa.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2khunxjxj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nwtyiljs.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2kblsqdlj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jisslhcb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2usfoyvhh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qimpudsp.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bjsdview.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2qwrlppud.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2jurfxiim.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ntwlywnw.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2bbmjalpf.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2qupvwjdc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2donlzpkr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2ktpxdkrh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2rtlsumqt.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2asendklj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2yqmdbdkq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2iigoiccw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2xmkqeszr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2utpuuhjn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bpychwjc.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2apmxblpg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fyejmplk.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2wvnnwvuc.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2mocvdyoy.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2euntxdhn.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2pxcjazgg.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2jasmprnq.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ldnwvouw.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2rrbilhzh.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2dvgbhfaw.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ocfeuxgo.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2azlrqcfa.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2okcxafcg.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2ieqlvgja.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2dhvrduqh.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2upmplwuz.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2kfdohtwt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2shiegswa.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2aqimpunj.html


<!-- 参考信息 -->