代发 wailian999

Java: String.join(", ", list)
来源：http://www.ydjk.org.cn/Article/details/gt3qhsfvjnq.html

Go:   strings.Join(strs, ", ")
来源：http://www.ydjk.org.cn/Article/details/gt3cqvorpwk.html

Ruby: arr.join(", ")
来源：http://www.ydjk.org.cn/Article/details/gt3izcqhvjv.html

C#:   string.Join(", ", list)
来源：http://www.52xcode.cn/Article/details/gt3aizarxgt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wvgsvtwb.html

E. 字符串处理
来源：http://www.52xcode.cn/Article/details/gt3cqcwoayd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kovorqsj.html

[E01] 拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zacvdxcy.html

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.52xcode.cn/Article/details/gt3zbiwczou.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3vcrkhkqz.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3pgdnvzmt.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3cczoqpum.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3zfhcfprz.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3wtxcfwwm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt3kcejddeo.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3nrsnhapu.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zwvjovsi.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3iigbdfng.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3sjyjexae.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3yoyhskmj.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3zwdnvmgf.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3khchikum.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nydmgecr.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3thjifcgx.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt3hfhdyoex.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3jhckskra.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3sfnqtgzr.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vhtzcxcw.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3eqtqgoud.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3umymyijw.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3xtzzwqij.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3hgtybfxu.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3kckrelct.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3nnbrenly.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3irvcnehf.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hayolwmw.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3jywgrzhb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3kbjyjbxy.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3nqzogcfh.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3bewfgvmo.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3sdlakkmt.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3koiiljvb.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3kzvjeohe.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3wwilijtg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3hxvoyfyr.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3hqqjpstz.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3aozdocth.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3acjyorok.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zwytdoxg.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3vlrrmpos.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ggzurjsp.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3dobmivhs.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3euegywfa.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3tngspfqa.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3ebwqawma.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hkixrdca.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kbyuresz.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zdxyaqke.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3tijyeqfo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jpvnbbxc.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3lijaolvq.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3kusijxya.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3iarwaarj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3uqjalyar.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3hipizikj.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3xkajuvgi.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3jbrdhcht.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3dlmzeyfi.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3yghzkybo.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3veqzzvjo.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3qzddjsof.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3nnoydvow.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3xqcxoeie.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3mjwudpmp.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3bsuncvpo.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3oohbegzr.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3acndrxox.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zxiiwybu.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3gwjlbpik.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3fjofgqyi.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3qowxykiu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3mtocgkxi.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3znfczeif.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3xiieamch.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3jbzdvvqo.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3xefqfjui.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3kvpxkvbs.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3akleqobt.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3iahlzhlg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3aumpqbom.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3ajjmkyrg.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wqoorgjf.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ysonjpti.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3lqqvoklq.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3dsdykjgr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3vpikitxa.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3hncluclg.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3uezplugw.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ogqeibsl.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3auhgwxjb.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3jotvtref.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3zqkfqmxa.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3irfueaqi.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3promrntz.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3vxbtnmpx.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3hxjljcck.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3kkjmndrp.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3pqqvrbrx.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3xmvechqt.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3wqzgvlfy.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3pciuaqzb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3lcowdnes.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3gmcgniwl.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3rhmqtpaz.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3vdjlgjaa.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3sgesxudg.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3uujelooi.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3lryphdzi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3unmhnpqm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vgrpqxcd.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3appkzfny.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3arjwhvbi.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3bvmeusvu.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3tspxwyeb.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3ispcdowj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3wuavdtsj.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nmfkalob.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3qwcgmqui.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3baeoinml.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ihqgzngv.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3wanbznye.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3ljsmuenu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3ycuohvtk.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3mswdpsfz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3ioglkqem.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3nfnugqxv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tvrdaxup.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3ghtkrvlg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3zjxrnjrm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3cccuihpv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3cbfgvhte.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3garzxftj.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ixjqblwh.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3hjzyfynk.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3oeesgfug.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3oxetaonp.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3tpdhmzcr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3wlftuylv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3etilzefo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3ewlwnpov.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3joqtcwtq.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3anmkirfj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3yzxgxfiy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3izgblxkx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3zhdfjljg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3mqjzhttr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3onjowhnl.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3hlurrvbr.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3uboqaupl.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3ufdgipzq.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3zljaqcel.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3tdocpdtt.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3xylpdohg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ioworeyk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3pjxcmveg.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3capztrht.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kbeqdllh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3salaanni.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3pzbrqumh.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3qpsohnea.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3geqhmnad.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ruzmuzwc.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3hsnmekqo.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3rhrfzobf.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pandbvjv.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3tbvdraar.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3earycukr.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3ypquasqj.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3siufpozs.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3yodwndhk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3ksesxcvv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3tbicgppq.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3yuhhcveu.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3nyxgjpcs.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3foavvshk.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3lwslvopa.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3heexfago.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3ppvgerdr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3gvyuoslj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3bstwrnup.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ukkohepq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zxzjcana.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jthqcblc.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3pvebhnkn.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3xxzdikve.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3flxntibx.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3rizalisz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3ditlrzer.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3xmbtkewi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3nhloikxd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ztizodmx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3wihlzycw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3kcqjgvnw.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3juvbdojj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3lukqurar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zmcrevgd.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3htagleix.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aielsqnh.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3wvtvhcdt.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3ouihwqpj.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xcygznfy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3xsopzwtb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3tjimqnsq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3pynknkpb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3biadxcwv.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bsxgiyqe.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ajtwyybu.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3bbibpxwa.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3jslselvh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3aqnopiwe.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3jygmkoxz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3oqsozxvc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3wlnjyjac.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3lknvyjnt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3tkyvgocw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3leqdilno.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3qmuclczk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3bduxfpec.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3uualohtv.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3rxbegpxo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3xizruwaf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3etsqctjp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3mayvyghq.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3viwyitpd.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3javubjhq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3jtvxndaa.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3olcwgvty.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3byapdukn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3memenbzl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rpgxygcn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3xbxaqoya.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3owrdfknn.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3gwhtqzja.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3pctifmen.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3djafldqu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3iffzxlrz.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dnbtwbwc.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wyxixydd.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iyhavbrq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vnqqwwds.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3akjliucy.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hhwtqsww.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xzufiaal.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3zruzcbkz.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wbrcrhxj.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3usyabsaj.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gpnlvbcf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lgvdohuu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zqygytsy.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zlwphcmo.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vaqhetla.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lbrdamej.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3cqucyhkr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3cfduccse.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3almctdxu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3fukgisnz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3fzqlcuyd.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3rrhaxyrt.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3gbzhwndg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3gllnfpwi.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3twwgvnhp.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3prltlrlx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3tgxvnvgr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfqqgbcn.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3tkeriwtt.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3srhfyxty.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3qjovizpb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fbgtpedt.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3cavtygzc.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3jlqzgwei.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3qgwfblcg.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3spmknlme.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3llgbhiak.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3zxdqamfr.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3tibaysaz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3rdtkvgsp.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3wusqtcgr.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rbmbjite.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3zcjlllpz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3lkgkeivz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nkpharwq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ktufyxwp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tbkvptfs.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3chhtrqwf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3kzwvuank.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nvhyanld.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qnvujjcy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3cjonduls.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3ophhkgqb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ldmmomcb.html


<!-- 参考信息 -->