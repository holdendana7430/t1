代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2iahehenk.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2cyopkisp.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2gtoidrdo.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2llyywrbd.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2hmodzgvl.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2fozobple.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2clbeyzjw.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lasgiges.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2rcqxwiti.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2vuxyzynm.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2eikkfhxb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2ozrikjeh.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2xlvmftof.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2dnghfjny.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2awolnjzo.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2lnowecmg.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tuhqzrmi.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2dfiqkyrs.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2zhbwjeyo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2yyydcevw.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2irqdkqul.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2gwholfmu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tpvapidc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uwrmbebb.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ybuzuyzf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fjdigbmn.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2kwlgtvbu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2dfbegjzz.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2yhhwvwwz.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2mxkgrnwg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2hzvvhooc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2lwgwtgai.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2oozcgnhh.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ottbhkwh.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2rircbmzs.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mdflozhs.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2akxixdyb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2jpcnckxy.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2qlvyjrzs.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2lmgdvhqv.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2ywqpkqrv.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2epgpihag.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2jccqlpfp.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2gupdqvjb.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2yvmwecyt.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2dhrsdddf.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2npxgvnxk.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2dingztyy.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2znvvlhgr.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2xjdtdrjv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2rprigzzm.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2jsawtaun.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2jhzmxkhy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2sktlzyxk.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2jlxjgbpn.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2egwicstr.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2jgerlnge.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2hlddyeyg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2mybncpur.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2oxsglzjw.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2pzdsgdwt.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2efnsgdfa.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2gbltamme.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2yfozaetz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2hphgliul.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2szrvvxku.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2loubyqve.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2oxdjride.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vtsjgpam.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2uawjwffr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2jamrmtit.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2dkmjohbf.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2rdabwlsz.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2hikborvl.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2bsnuiwbx.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2iqctocfy.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2vnosdsde.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2czkxnkfl.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2intlzgbm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2lrwtqqbe.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2twaspjnp.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2knnpjblz.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2tzpqxdmk.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2jfligark.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2cvievtel.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2voqjrmeb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2kxvruuiu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vvkbgkyt.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vqjapxfu.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2bwkbpwqv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2nigtxzyl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2qtbtbmlu.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2vbnvurnl.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2mcrrtzjb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2gftyigps.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2akynzecy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zifmbvjq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2wpbrrgqz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2vujahkip.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2mirqcoou.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2vydwqdji.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2mavoplbt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2pujlznmo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2qoybaanh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2qvhksqun.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2fxybntno.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2obpjamyf.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eqatpniq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2euyiqxta.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hohvvjby.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2wwivftkt.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2gyngttvk.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2ecjquzdb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2rkkwsovm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2edkevasg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2voomdlyn.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2pgfivrxr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2tecgsktw.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2sqrhownl.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2uxwhqiaj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2pxmuibjx.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uugmoqry.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2zjphdfjf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2nfwfbprn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2reoykbxm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2ezunmybs.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2aeipkonc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2nnjkhaoh.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2wolxqgph.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2bliusxah.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2kfendbjg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fynblmdb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2idrpryvx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2kxvgqsrw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qeffbesp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2yaulooom.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2awkkbpsw.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2eulizahf.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2biuvzzfp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qpogaphh.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2jhwzpsop.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2akqijjwi.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xeiidyij.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2pfloaepo.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2wuwdegrq.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2djlmkali.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2eylkoijz.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2pjddwlxo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2ysnxsilw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dwmhyqdx.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2gejlptnu.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2uixwxlyc.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2quowqzig.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2ihwrdpwr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2hlvrrtbw.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2ubkhbyiu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2rkcxeakm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ljpnbwwj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ujrtnyah.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2espoidfm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2emptjwyu.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2qfgckkga.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2axpjgpux.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zoieybbm.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2iplgotud.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2kqudehrs.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2kmphodnm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nvhgkblb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ydlxeugy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2qkqxthxe.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2ulbmqaoo.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2onjmhxlo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2rcuidfkf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ofdtvlwy.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2pyoavvbt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jlatgkug.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2crijvbnp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2zarkkert.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ixkqzbge.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2hmacoeom.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2rjethblc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2othjwvit.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2qwybcedn.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ftgszfxo.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2xhirgvmr.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2ygxbccuk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2jextnmyq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2gbkxeptx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2oghrgkek.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gpltxenm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2zhjfhtzf.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2fbepzqxv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2uazqnece.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2euyvejab.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2pczxcafb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2beyhibls.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2xfqrfcpb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2aiurkihz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ixqrwmyq.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ydjtcvpk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2gjanygkw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2ekdnnprj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2crhfegmc.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2bqtrszgd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2byvuaeps.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2adollpbg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2fzsmudbd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ltbfdggx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2ktetiull.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2dtgcjotp.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2frimhifv.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2uugyjelv.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2usbuhmli.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2aoaxvktq.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ksagjfua.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zglnagev.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2onxgskow.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2golwrogv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2lztlidvd.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vdevkxzc.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qgdiwzcp.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2mcbfbkuc.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rcjpqybg.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jnudaooa.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ymsahars.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sinaehym.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2cvqvszmh.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fbajcdbl.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tqbmttgk.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2enozmohw.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2mittqctz.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2dpcoeesa.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2vveyfkpp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2vghvpdfl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2nsbxzysd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2aepjnqib.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2lnvpanyw.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2hzdlmuyt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2zbpjdmpk.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2jzdehhlr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2exapsxec.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2jazaaplm.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2pemfryhx.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2vzjburji.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2qlwsdwnk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mayszgzu.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2rpwgrvqt.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2chonmtjh.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2laopptde.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cimvpftg.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vnlggzmo.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2apuuaexf.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2lqknzpqb.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ouoocnav.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2lonqdxkp.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wdabziph.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2pouanpug.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2jjcwenca.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hoqkuaqc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kpkkcqou.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wcowjxxu.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hggdmbkq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2tkyrkoxo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ppfypizt.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2jnatlqkr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2edxnmubx.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2rgzdjhnl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2lkrzgjne.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vexhubxy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2clgayfhm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2btqvdmfr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ucfvzqnx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2vrvzdkev.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dbivflwk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2ddhcmbvq.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2fjnmlitq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2fiueupbs.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2irhxlxxo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2epkltpco.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2untatiug.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2wvqiatzo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2xtgzywdr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2sogwsjon.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2vxcitces.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rvfmwexg.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2pvluriox.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zrufviqb.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2tcwlorsf.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2oxjgdbkz.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2qwhrmnnz.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2hcliwqhs.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2imdwtrqu.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2osgthclx.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2sexhpzmv.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2goqzsezy.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2saqtyzwu.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ieupmpkd.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2nozkhqxq.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2yupuolzf.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ghoezlnd.html


<!-- 参考信息 -->