代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3lcdkvuek.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3siekwkoq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3ywlkvlik.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xwyixuyf.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3jskxgpga.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3dipkbydh.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3msmxhmob.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3kdikyixv.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3jqoultzr.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xoijgjbo.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3shfdksmp.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3lbzjqbtj.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3xznysnjv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3kyamlfbk.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xiekfuwn.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fuhzevbl.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3meszpxlh.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3obucivrv.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tuepcwyz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3zlybskqw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3sjojcqnp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3sksanmhp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3qjlighcv.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ounfwczj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3qbfufaew.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3cdlvhosu.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3klaoynio.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3uixhrqlz.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3yimmeulx.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3sqyyoyaz.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bvmpaeuf.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bpbmgdtr.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3qkziaoag.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dzwjjqiv.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3qgzaujok.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3omnrtrnj.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wrlftqoo.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3uazzlczg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3vravyrzo.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3nvoflmok.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3eungbkuz.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3qihqyfow.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3pqmpsabq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hyioboke.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3jawjzclf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3duaqbzmb.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3ihldxbqh.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3mlbvciss.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3zuwsdhbw.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3kuudrhhd.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3rctcxvkk.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3uamyzrdz.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3lbitqszk.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3obkqyriv.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3awbomybm.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3jwzlamjj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3raoajyum.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3icsgjcjm.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3rpijbfez.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3zkrnzubi.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3bjiyoean.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3swkfefpc.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3nwmkpnkk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ktyxqnet.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3iikikxol.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3kxaadtlu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3kcipuxtb.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3katlxmvo.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3tsrdwbom.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3zgqwenvg.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3gqtqmhqe.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3xkaizpzi.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3unswllpj.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ambdoxmx.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3pgnnkztj.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3vnarmyzz.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3mmrxnaee.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lhdacgjg.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3xkhrojic.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3yqohjkkz.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3gbhxbebx.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3iqkahqtw.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3gfzvcsbv.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3brimamkf.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3jfdiwvna.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3jmhnqhnp.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3fqwkzcjj.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3oxrbqlmz.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3budzrjmb.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xrboxreb.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ocezdifp.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3nhobfugs.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3brhepejm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3xlbmgjpu.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3pyblsiom.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3alttallm.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3mkllwojf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3kchrjxtz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3emycxdnv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3aibmbvcg.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3adysxwpw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3wwpeossu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3mgzhoaky.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3zbmtruwi.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jljgtkpy.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3fflsrofn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3bcuearfl.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3qujkdyze.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3igwdnaiv.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3cuivyrrz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xdaqmsus.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3lhwxlclx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zcrqhcjo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jfxgnyrj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3ixbdagqr.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3oyintono.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3jqsxygou.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zrccsxci.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3ehyaajjp.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3ujrneiof.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3kqtodnnh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3bomwccpn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3rvcfqmdk.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3momqvxxm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3qarxhmcz.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3yomyekgr.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3uomgjqsh.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3pzdbfogs.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3bwwiikxc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3laizwbei.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xpuxkbok.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3tnelmjfa.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3maxuczzf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3irvjfsgz.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3tnwnxzig.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3xzanbijo.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3bwaedpqy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3yksdaqcj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3fioudgai.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ccicancr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3xzygagso.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3lcjnlqbu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3ykamfpny.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3maoplzvy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3mehzvqna.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3xdzigodq.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3rhlaozkk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rahbrspz.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3fuligooj.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ovjqjoku.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3akjbgqsy.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3goicztqb.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3ebudqivg.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3frcnzled.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3gjydkjvx.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3qqqzxjsm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3bjurhnak.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bbhbwcip.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3qupsxhck.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3yhuirgaj.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3yrymezbi.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3inyunosv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bprxmypf.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3yhdgvzha.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3pjomqmtz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3ubopffpo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nsiqzvfn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3tdzpncfo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jwbbsovj.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3bxzgimcm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hitjppoe.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xfcnrmqg.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3uxhnhhdi.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hadhcjfg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3szrrjnlz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ugvelfru.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3bfumfimy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3xbogywho.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3xgjfclrp.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zxtkpdxt.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ftvvuqzs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rhgtmekw.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3gchfqliz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pxmelpsg.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3mhukkgzq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3jvmnsyaz.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vvgrtttu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3wwvycwnz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3upkkecoq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3aknxnnnq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3jqijonpw.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3obbaxfof.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nbfcerzk.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3adxdknxj.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3yofvzygs.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3ynmipymh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3gkklxwmj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3hcuqpcnc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3oiutmyud.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3yrywunmp.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3vbzbvifo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3gztggddv.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3gukqzwed.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3qcykpimq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3ntkuimxo.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3wlotemgu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3aqshvwzg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3hcclwrcp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3qpfkdbjm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3pjgyycop.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3wqfcymdw.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3ckhmtbea.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3zpuuxqrz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3gjcumrtc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3pillohee.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3dmzjjdkz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3bnvshhtq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3xbcukhhh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3idvsncmq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3twbbnsec.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3zmkirunb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3soutlbys.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jsphacwi.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qltgfuae.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jsfltwcc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3yoltveor.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3hfgvkhsa.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wmpudtfd.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iqqcyxhi.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3eukyhlwm.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hcjjcckm.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3iczodjtl.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yigevmzv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rkoklvch.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3udqjwxrw.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ygvdstbk.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mocvvycr.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3epkbivkw.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3ofkouohn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3awdyklya.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3lthoxvsr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3xgzgjhzr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3cjhzdikf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3amndexma.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3ovltvuir.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3imrggutn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3cmfuvpfh.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3vepyqsir.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3gzagtcam.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3iyrydfec.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rbyptxbf.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3nqiimbte.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3zzfgyucm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3hdknyhco.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3vgmhlmck.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dgnbrsbp.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3lyanvzet.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ycnveqvg.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kogspeus.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3tslpcieu.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3yhfewcdr.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ohlyiqtm.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3ijabkubu.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3msqslzem.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3ajdqaqpd.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3chbxveia.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3isylgufd.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sxmkaysz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gnejcxae.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ydkvncyd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3fmickzfe.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fdlmxxus.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xhiqusel.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pjspffux.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3xjqcxvql.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3bymmnrmz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3twkmyhsh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3haksgeoe.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xrdwssnx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3tlrtypkq.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3hxcbeted.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qxubbfmg.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3bdbfukss.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3obwooiwd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3cufsyamv.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3vlfyeusg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3ikgypikm.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3lolkwzok.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3hwvnulri.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3nrvbbtyz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3driwafwu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3dxnbihtu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3noxaqcax.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3usqqzbdz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bjuiajwu.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3yhrczqxs.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3ozxblckt.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3yjrsehjf.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3sqsnwstg.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3wjuddgyx.html


<!-- 参考信息 -->