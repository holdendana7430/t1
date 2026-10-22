代发 wailian999

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2kqflabfd.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2eycjcyzj.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jaxwjtrr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2mpldpxne.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2ekuiuysn.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2yecfrnyn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2bagzcrnw.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2anfocdvc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2vdlcuhgy.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2snvgbsea.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2mimsijai.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xtwgrmlm.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2jxzubmmi.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2hgxdgcjk.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tzkfuipx.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ojgevnhv.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kdchpxsu.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kxlppofn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2iubzvdxb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kfyrptii.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kasxdzud.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2xunbfgvj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2ydhmyirf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gtxgueoq.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2marssros.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2cmlzvudn.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2jaztjlmg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2ahuvgrgj.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2urdmjiku.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2wsdoqsvq.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2jyxklyex.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2nmfvpudp.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2dyveaagh.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xwwfrfby.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2cystvhwx.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2rhbijhku.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2ruszhplv.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2cintezao.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ermutemd.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2icdafgyk.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2myctoezr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2ybpohjgm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2bpkelznt.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2uxnmkfsr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2iyiocvmr.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2acounmvc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2xzjwiydb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2sgouypzr.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2rjxcrcvg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2aeycgknd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2stkcuwer.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2xebyirjx.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2kyxsnlnm.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2psukujwr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2uwokpkke.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2hmcqwdxn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2kmuiltnj.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2oufufwcj.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2tgbmwqqf.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2lziruwha.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2rtjiirzm.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2tymuhtiz.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2gkhelfou.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2oxqvdwcd.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ohbzkgek.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2hwvallxr.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2bfdsleqi.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2vdcvayca.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2xngvplws.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2xtkkufyj.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ufirrmtg.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2ofjxauvc.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2itrkrpav.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2xpdpzpku.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2cfrmhnaz.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2ofxrjnom.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2mohwjmmq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2ilvlogry.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2cceritjv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2xkspqkyi.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2acxidkyr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hrzhthda.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2byunquer.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2depyytbq.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2uysuqqbe.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2ktwlcnbx.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2gdymeubh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2ljynccrz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qjsraspf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2xrjbtfoo.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2nckmzzvs.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2sfivrdhl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2mhkeetrb.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2mtzfeulz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2urfdzjwp.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2azusmsgj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2abtseoaa.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2najwulhn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2uwwgwlug.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2qnbflwnw.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2koanklnz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2trtuvzkn.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2hlqzjfpe.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2qbrykvkn.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2pvzlpgep.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2dklivpdo.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2wzybytbs.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2tcaxhitt.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2tgfbustb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2soxgajkw.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2lonbzkhr.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2pdxgebxx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2jghlimsz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jiwqgrnd.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gyizglsi.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2djurxzrh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kndrccuh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2pdefkanh.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2qbfloigc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2ivywmhuu.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2ojmudetf.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2cqmiadhv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2yopdjwsf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2enrvdqlh.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bkugkbgj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2zyvfboop.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2iuissobw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2djzdtizd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2umwhhzrn.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2ktusntym.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2hudknfln.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2foovgfdr.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2tduspens.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2mlqamton.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ygjrtylh.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2dtffpuib.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2saigalrh.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2ndbhllua.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2wejsfbvb.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2gvkuzacq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2eotblvpc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bolqnyvv.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2rmfluotp.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2brnfovyc.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2nrymjvwe.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2xqgihzyu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zuxxutnz.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2qebwvibx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2lxzkftus.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2fwbgtgzs.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ywzcqjgi.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2tkkkcrtq.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2kybdqdpl.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2fbkntapx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bdmpuhal.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zjsxpxug.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2uhuuxuee.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2joyigjxn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2gaewgfqt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2pyezrdph.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2jrdpzgmb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2upulkymm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2moucltwj.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2hvwivvvy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2wzsrrzrh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zogdxabj.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2pzcuaten.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aubyoswh.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2dkgkungp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2lupltidz.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yozrykfm.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2wzipaujp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2armzwupn.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2mghqsbec.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2fyagusxq.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zjgfbqyb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fvieqpdk.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2cvdijqgv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2irocgxox.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2hegfnwej.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2fhanrpbk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2zuinjrud.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2qhldcagk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2xjccjdra.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2hruvaamd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2jvuoxgiu.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2clrvcstw.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2fdpzfsst.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2bkbxzsee.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2qcykjool.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2khajrxow.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zmnlxsfo.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2dthyhpar.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2fmrpsqxh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2aqyyzzye.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2szzipwki.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2mcfmbnfn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2ngbtkdyu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2glgytpsn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2ragqnolv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2oyxsxdqw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2tmrxlzdo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2ecnorbuk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2saexgcza.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2ksukvfel.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2mjskdfab.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mzpffqjj.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dediyfyp.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fpjjkspk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2eyeahiru.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2uvsidwan.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mcdbchps.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gbbghici.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2fmwuhrzh.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ytqvzlyg.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jkldklim.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oyripzem.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pnlilixx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2olqaksnc.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2efhtjalu.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sunudqkj.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yhnnrige.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2ujdvvsny.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2sacotkdv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2rgxiolpl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2esjgwyau.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2mjcripon.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2lldgfmmj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2drhsemqx.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2wrxmdieh.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2tficnrwk.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2dyisblje.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2qvplxotu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2gltcmpbf.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2pzvqcqkf.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2adlvjrig.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2ncyatjmw.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2hdtimdzd.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2uodyvwfu.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gdxqpixt.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2sljqrprm.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xzhwdlnv.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2laymmggk.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2iqcbxtxx.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2cptkbdmx.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gtdszyjx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2dtopzwxx.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xjqjqkdr.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2xfxnlxdt.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ykqehqgj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cfmrtvut.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2idxcenom.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wkbfhnix.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cpbmnzyu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2culwqrlf.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2peeqtwfq.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yshjkriq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zzonduge.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ctutsgyh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jsdyuxmc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kgpzyfnw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2nyxxiwxo.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2efxlhwwc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2oeqvbqvs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2gfljlviy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dbgxechn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2bafmjiwu.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2kxmiawxz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2bfexbpia.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2xzjjfpzc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2fxduects.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2belzkalr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2esdqynev.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2jfwwzztw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2zbjnmtlp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2tdvfbsif.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2itmwnyhv.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2gzfedkkx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nfqwsion.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2iahycdng.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2scvmpwje.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2ppmpbwub.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2izucwpwz.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2gcxgnkpz.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xhxbzdqg.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2aiogpzjf.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2vcpzwnsu.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2jubttbpk.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ldykgwcy.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2vmlmwsco.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qhdjsbrw.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2qaxdnkxh.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2zgrztsja.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2kinfcbjk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2wzunkhas.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2upmvflqq.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2eadzotci.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2tfqkafqn.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2qwmndlyp.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2iyuawnec.html


<!-- 参考信息 -->