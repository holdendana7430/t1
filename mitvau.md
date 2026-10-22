代发 wailian999

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2bwmzfjfy.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2tyczpzib.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2wfgsqjww.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2upazawuv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tqmrbnnu.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2czlirvvh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2gxdpjcgt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2kbedzubw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2rsoxgqyl.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2nefnxohm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2tgomujzm.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pokujqxq.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2sxthgfzk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2kgdajmve.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2falorxhb.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2uwxfczyq.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fwbzeghl.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2nzcpzutg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2plvuisdt.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rvkhbebw.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2svkxktuz.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2oitgxbvj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2fwpqxmdy.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vunnemjd.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2yvrchxzh.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2uwwcdcrr.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2levgnowj.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mstsjztj.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2knflpkbv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2upqrybdj.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2cwepdfqu.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2zrwzjgvi.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2vnhrfbrl.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2hknalrsg.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qmiwqzbo.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2cjytfbsh.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2wesdgoqb.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2wdtxrisc.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2prcnzwta.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2aszdzgdv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2ccvjkzcg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ietpqsaw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2uuyvwbfw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2zlfzfldq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2kcokgdle.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2mskdtopg.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2cstfztgf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2mzkhxcfp.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2rpftkmvo.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2weendepu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2zvoabolr.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qqtbpolz.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2iimxhbia.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2efqnzdyv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ckvdoonu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2adizjwzj.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2kvkngngm.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2xbntrekw.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2jcepityb.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rmlzlcjl.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ahaptjna.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2wwhwhasq.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2xjilrnzo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2scdxxadh.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2csagrdnx.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2crzcwiix.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2hbxrddfy.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2trzsabgo.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2smhslyjp.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2wpwahmax.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2gswrasqd.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2yzemgoyi.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2rvddllwr.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2gtoxgnga.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2cjxxxsmz.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2jwfirigz.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2cignnvwl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2hpizqjdd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ejzdvqim.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2crwagawe.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2bwyssxbb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xanymopk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2xaaiixgf.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2gbycpskf.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2uhstibpa.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2acibnish.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lakctktf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2vihyioek.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lhnwmubg.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2wuvajlqk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2rhvcosav.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2mxyalula.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2drklpfvz.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2bcgsfeiu.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iwhxldwg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zjkddcdt.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qvsscovg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jbkrggxk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2jkxehqxd.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2evxllegy.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2ekyvgtes.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2guzfroep.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2kpvybhqh.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2yskqxydf.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2nriukwsg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2mjciyeyy.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2xjgmkntd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2coyglzso.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2tcbbdhmd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2acjhruhd.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2slazmtfx.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2jxvvngmb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2fjfexbfn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xbztddyf.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vrmjvpme.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2lvbgbnye.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2oawnxfze.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2iddszkru.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2zgezjgqu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2prtzjrnb.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2vcscmztn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2khzdfoyo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2fdnlmxwu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2hgpyfmmm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jgafcnbg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2xvubctbx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jzwxpqfd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2hgebyjul.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2jggeevfr.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2zsxrylhv.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2shrefztk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2bvnsrcwu.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2bazihpjd.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2xhiglqrq.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2rcdnekea.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2btevimjx.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2pizenazx.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2vcuqqgqm.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2enkmbbpr.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2tfhojrmk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2kywqdttr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zmcadhhr.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2psydgeov.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wibnrivf.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2acoxieea.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2uskzmagw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2asmzshgw.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2htkdbsgo.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2xctrqhjs.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2gipedgyv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ggpssogz.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2uhnxvyrv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2xfgzqhfk.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2rjxgfdde.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mjilfkrb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jzdoffui.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ggixsbkz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qsmopzme.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ozaixzlg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2mqavzxtw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wcdrolgp.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2fplnuhuz.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2vdyvmsgy.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2oqlvjbty.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2jlqtmhap.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yilkcrgm.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2ysregwkf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hegmmtmh.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2obzasrnq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2wcwyjsiz.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xcoomtry.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2odgizpmh.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2reahhcpr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2glpvsfvx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2ksqcdkla.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zekjuhpc.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fmefkpip.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2nrliguru.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2kfstlhzc.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2ifbxlviq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2sxunyzcd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mvxuzybg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2gjqmgtbt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2jogpvvbf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2yqpyugdw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2thkmkfxv.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2cxqtsayz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2mxsthxee.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2wicolcxx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2mgwxjjzk.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2sxtukayl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2zxcgkbnt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ojbkysad.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2hzeqttuu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hibfkmvn.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2eruypbew.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2cybmrhdk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2qidstpxq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2douaejpm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ykwsmtkw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2dlfxebta.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2yfgrbntm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2whhwmhow.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2wctzhqrn.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jcugdniw.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2eulrnkcg.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xlrhgpul.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2foizredz.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2peofizvb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2awusvagj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2lpshtord.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2itkhabef.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zyrjuxxw.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2xdlxsdej.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fjskzagd.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hwnpnura.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vtmtommq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mumuluvm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ddxkehzc.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hbflfxdi.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ctyunssp.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vltojfyq.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2zkglukeb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2cshmcmct.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2ouznakcl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2kgkilelk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2mlgssqqp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2mtlpkhoy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2vxpjodqy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2bhtimnau.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2wfmrewzt.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2dbttoljp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2veashpjj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2jveitfwa.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2zicmskek.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2yjnhixuz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2hvwivuhx.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ooqpxpfe.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ycvbfjlk.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2puipobvk.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2vghujfif.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eaisrepa.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lgddgyhh.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2dfzkiakv.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2mpkiupus.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ebxtgndt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2uhggreft.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cxafzsea.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2glhrddth.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2oobxzuyd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2prxlwcuw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qmtdmcsy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vrhpkfup.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fymyvpoe.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2pduwcrtr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ymwbhgbm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lxcmjngj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tposstua.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ezgekfem.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bkhvpysu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2hkznireh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nnfmmlsv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2wzphbawt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2zugorcry.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2qwyggfgx.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ovatukez.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2uwstauzg.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2fkvvszyo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2qrcibxzc.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2fraorjli.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2lyqryifa.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2hashyzwq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2dbfrurwk.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2icrrspvn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2ahvwxcuq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2uzzewvoq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jodwuogm.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2csbmwizc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2edoimvdx.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2ackyuhma.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2rjssneix.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pbgnjujj.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2ckpclsah.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2zrubcyou.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2axgevrib.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2vaubkizg.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2satanbfh.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dtqitoza.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2shrmuxnj.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2wwwgogtq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2uesgiyrz.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2tcprlyjb.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2mtjhidqu.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2dlwlwskz.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2hypxecak.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2piaqvgmf.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2mzbegufh.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2ragsvizg.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2ijuzlhgo.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2fodxrwjx.html


<!-- 参考信息 -->