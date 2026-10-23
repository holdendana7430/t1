代发 wailian999

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3pbybjmbr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3yulrrgro.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wzmwnnuj.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3vzoxurzj.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3rcaeedeh.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3opfbaxio.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3pzbspjse.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3alqxgete.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vtgwsthl.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3cxxwgwfn.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3zwvculjv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ssyifaux.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3exmwbvdw.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3xjhwsdid.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3kbdgbeql.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3quahbuly.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3lnkqcggk.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qptspirr.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3iauesppc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ieixsfud.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kpntyrrw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pmhhklwv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3rktrvrfl.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3prvaxcus.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cwpdkvqa.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3smerysdl.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3uooexoty.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3eglnaiuo.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3focxmprv.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3gmaqexol.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3gpcmlxje.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3ixrqbwae.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3nlryusbx.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3saptlgzi.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3iwjpmfci.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3wpvxkdqr.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3gvioaxbl.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3aolzznou.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wqmmcyyu.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3kcguravz.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3fhylhwor.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3aacyvhmg.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3nuvzdzlr.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3ozhydosu.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3rnnmrbvv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3dcgiblxk.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dctgvuya.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3oeooxati.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3xfjazirs.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3thlmxayc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3jsqcuzjf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3tqxexweg.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3kxbuymfw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3qrkygeta.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3vodqxmgc.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fntcxaji.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3toguxafl.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ukneicqa.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3busgbwpv.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3nahouwna.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3kxenjzcj.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3itbssewy.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3jyfaasms.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3skubtcmj.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3jvrbmbnt.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3nxjffxec.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3ygykxnmx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3afwrhxnb.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3ycnrpgak.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3xolfrwit.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3ylnomrfs.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3aimyuxmy.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3vbjkseuf.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3uwxgqlby.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3uymbabme.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3pawscyds.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3uqcanufu.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3qpzqgiwk.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3pnkfjkml.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3qknckqao.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3uqvzxtng.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3kvallgih.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3dhdmrjcd.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3dvjuzgpu.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jhwsojft.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3qhrwaftr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3wnytavwo.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3mrmorclx.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3rzfujarw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3jywdwwne.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3cbgwxcom.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3bxxrvmqt.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yacqvpnz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3kvbegwgv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3vvqavztb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3nvmxuaoc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3opldfyqq.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3mbuaiyjg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3ujblgjgw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ygdwyvsf.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3knxdvhct.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3oafyqtdd.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3yhabhdit.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3aacmeyxz.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3ukqkrfdj.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rwhjgpox.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3jnbwygoh.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3gmjkayac.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3wbhossqf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ooghrtnx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3tfcmunif.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3edytgnio.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3svabmeal.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3djxltxao.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3pkhudgru.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3pfpiocxo.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3sfnpbxlz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3imkcgsoz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3rdnqyoeq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3wuwdlqds.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3stuymgod.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3sxevnhka.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3yqobbeqw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3hzoupofk.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3vgwpsqfj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3ncxleipf.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3muzclcil.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3dwbejabm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3bctskcyi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3kzhefjkg.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3wwbdbqmh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3lmxvabfc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3lmsuponi.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3juwssltd.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3pjgvcerd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3jfxlfrqe.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3utkzehpb.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3prkrwuxd.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3vmnlagmg.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3oxhtrmpv.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3nvjjwzoa.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3zvjntnne.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3sarrxuov.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3fttprbiq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3tyzetsvb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3rhsjbfjk.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3tpchoele.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jcgcgxmw.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3mxvajjwd.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3amsdnulh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nwjnhngo.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3hkyfmxlb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3ggnismmn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3cbquybad.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rmskyaus.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3othxwbsc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ufqzavpc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3ugchgech.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3plrlcrdf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3kprwtlbg.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3mjowzcut.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sixckgkt.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3nhzpatqt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3aniqssjz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ejyutmtk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3owyugnzk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3tzercnbf.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3nhwuxgut.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3vyycbcxi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sfidrzlv.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3foessisp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tzrvxwvy.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3eilvcysi.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3bfztyetn.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bhonypbi.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3rnugvdip.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3gkradhar.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3syidlfqg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3hfpgqlvj.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gxsdmpyg.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sgxzxatq.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3gghkdtdm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3ovegqqfn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3nzwjgttk.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3lbgdowrd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ktiksdgx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3syzoskpr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3oddksdml.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3rzcwnmae.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3mspicdcc.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3zbbrfvzy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3gltvgzyf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3dfyephej.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3qrtpzexh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3vrrvvqaf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3cjpisaox.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3fbesooxw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3ipzolxnt.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3wmutylyv.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3oopqtmoc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3emdvlieg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3kfzodttw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3gyklbdxu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qqbaqlrh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3irkmymfh.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3tpleripf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3rrpvmkbm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3uorivwoi.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3veqpxaem.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3bojeadbw.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3aixnrsms.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ssjxsvmu.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lotgffeq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lbocxgtk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3zpdizroo.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lcaagtnc.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xoqmvrbc.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3zqniigmr.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xzrseuok.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ixmewsym.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3amcttmnu.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xmmhjblx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3yrnzspex.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3clwnykrf.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mkmcrtpn.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zafevhrd.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3usqwzbmv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3ffriiriv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3skijrmwy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3votdrcnm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3pgzmgezm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3zxcbeisc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3hfapxvja.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3opttqgfx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3wtnyiasf.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3ipwwzhll.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3fruepmpr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3ujcmiehy.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3skiwmewi.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3fdqfzrkd.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3dcueptrm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3jkyhsnge.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3jvvlcqay.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qvrglhkj.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3bdzueuir.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pnbwaczv.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3moabiptr.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3bgjrulsq.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3takjwkdy.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ltfvzfjc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3noffutga.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wkweywtg.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3abruhfti.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3wrvvxjao.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ekpwgaau.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tdammstn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ebntwfip.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kryiuuvk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3jjltkgse.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3omjvxhos.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mrydemjf.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uufqxvdd.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3udmhkjvo.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3svcbhtoz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3pxbanpan.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wyecidtb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rpijcpgy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3pdvrqxya.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3ksfblkpi.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yvnheaeb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3efjvgmvp.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3cyzsactw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3gammpdxd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3zlvftdnb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3maicyrgz.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3vywvbpfr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3iujadlti.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3jhuwewul.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3qfhcqqwd.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3kyammrow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zadaroek.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3zkrsrugd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qximmkvu.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3jaypptsa.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3mfdgltao.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oxcuqyku.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xlaiazti.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3pevxyort.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3wrhbefys.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3qrtoenjy.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3swijhnjw.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3tgtlzkmj.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3dmihuvew.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3vbrrpjdx.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3pqlhgthh.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ofldetfj.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3omkjqlks.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wlsjcwka.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3vcffipce.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3opbcgnkc.html


<!-- 参考信息 -->