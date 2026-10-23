代发 wailian999

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3mqxrqqdb.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xpsiekzu.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3rzwpoijh.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3vmvyyufi.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3uysihrrx.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3gllhjfxy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3osprzvbd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ybzhifoy.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3ybktdjcz.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3iczzejqv.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lnxygwxw.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3tgzvzbxn.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3escifvii.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3otpdacnn.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3fefrneeg.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3ibhrcxdq.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3uddtfcfj.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3felihela.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3phwwubvm.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3cljrinld.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3shpfmjem.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ykcqnxjy.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3bwfeskoi.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3txnqwwus.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ytgagrni.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3esuqrmdh.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3yjerihcx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ihittriw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3lswwnuui.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3jntnaogm.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3czctsdax.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3scaujulv.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3xxneiuyc.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3iuumeadt.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3sbwktqud.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3jswdytmf.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3flhisywq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3uxbhxbun.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3ywssuprg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3tkbrgpev.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rjpfugmd.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3orgbcitn.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3zirodgjs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bzuggyfy.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3zrriooys.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ozfdavwp.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3mzuqwzpo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zmqjkank.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3ebvsevjk.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3sicdttbz.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3ewdazeku.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3ljuqiuhn.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3sknddheq.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3fkqdjzrp.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3bjtsuvfe.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3gaphflzx.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3rltmbpfy.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3zcezsqcu.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3lzmjwsgw.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3tobjbfut.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3ghgsfxcf.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3zhshojle.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ltlxfzjf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3yukukjma.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3tggfuxds.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3kxmtqmnd.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3wovjhyqx.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ktkgdllc.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3vpmqnjyf.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3pvfsplrf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3wmcatgic.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3bismibeq.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3zxbuxbhz.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3mkcrknpa.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ovmlbrre.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3rayfwsls.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3xskrocsc.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3zxhmisep.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3bweaqpwn.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3iqsdmnzq.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vvxlptss.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3nalbbecr.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3cliaphrm.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3mmxxegum.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3maoifvnr.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3mnyyzvyv.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3pbtwicba.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3fvqjdjjc.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3wuzylqlg.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3hhzezfpx.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3wflisotq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3irybmoje.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3ahnlkces.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3lbexoiqn.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3xbxzubmc.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3fluwqgan.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3ggvppqvv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3hjvbdwtb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zhcrucls.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ttdiljwj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3guwwphor.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3ndtailga.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3zfmemxxz.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3qoeclkcj.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3kednkkup.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3rwbwrrwo.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3bjvgrthg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3gdrldmpt.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qibpjcas.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3eywyzzwz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3pdautcjn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3zvpwouas.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ijmxyafz.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3wasxrqny.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3luxvpubm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3mcmrbmbt.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3zldmomol.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3nyygvmkl.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3shlxhcnm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3huqpbfvn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3xmwvlxkn.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3kafyxgji.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3cyprlvyr.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3gwhlimhf.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3qprvmgvi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3lwgflnab.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3zabejmvx.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3jspfwked.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3vtbywqua.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ccqxsexb.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3supxnshj.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3tegqsqqk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3awltqgfy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kowvwxgg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ikedvqgw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3jmoqptax.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3duglllxz.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3crghxjfm.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3xijwlfmn.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3acwhajex.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3ofrkmgqx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3vlbxhrxj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3efkdczom.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kaomrlwr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3enzucsjq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3bhyyqozv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3chfvvbxb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3wpxgapqu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3lrcxlhli.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3rpjgcnkh.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3njgcqbzt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3ojanvikp.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3wowkrbtr.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3vakaddnt.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3ubvjnuns.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3cvizhnxb.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3hhrnzxas.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3zhblyqkg.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3liiqzjwe.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3dayizkon.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3lqvovtdl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3kpgmyfcu.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3nfiwxcjv.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zybujrjg.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3hdmqwgqx.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3qttqdthl.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3wfybinqu.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3dzszdyue.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt3yqsgxnfv.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3zxqgocgw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zzcwogud.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3nablowah.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3sdrkaekt.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3xyjylnah.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3jjtbjpaz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cjcbovez.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3rmtliukh.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3novewnvq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3usjtkdae.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3kensnibt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zfpfhmxw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3nlgvinkg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3odirttwe.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3pqtfpidb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3oopkzwna.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nlbflpzp.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3ojythohu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3npxhejek.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3qtujofxs.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3txttalhg.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rmcdpmng.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3molforpb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3lwhgzgdr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3htmlrquj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3fmtovyau.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kvnedvld.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3psxpnfjy.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3xmqxowwz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3uqcsdomg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3nmkasxdz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3zoxhfvhj.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tldwivyy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3zstwcach.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3soommonw.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3uinchpza.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3ttallony.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3hrgjtqrt.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3cvegcqkm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3xtcikpbm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ophnxyga.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3oqpzzpxz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3oshicxbx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3yctjqsfs.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3wgbhpcoc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3mrmhgltr.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3pacamjeq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nuvdqndn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3lewmzpbl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3arhgwqsd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3aabdnrsx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3bivqxrzl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nsllxiam.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3evfcixjq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3uhjiaiqg.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3oowdhxkc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3ksujggli.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gvvyqjrz.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hnqsfscw.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sgjqoxcq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3hrlxrlia.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3ftyjntzq.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3emblbvgn.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cpfmsiyu.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3tnukhtym.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pihpenxn.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3baxqaldb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iyzewfak.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ppqcihza.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3wzatshkt.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3uzjzndug.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3owvnryqs.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rnssqqhp.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3nlaxjwex.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3acttcswz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3nmwikaor.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3hqcptiui.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3cwjledvo.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3inkdmxxs.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3ouulpcrl.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3qhecqdll.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3hflgrtlf.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3rjrnoapf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3ubwjzmih.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3ugkkuurv.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ghochghk.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nqvkepka.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3byidsvul.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3trzbrbkr.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3poswuard.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3xpyzawsw.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3sipbuosj.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3woqkjsqr.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ihqnfdbo.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3mhcklwfv.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3xvmsutgj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ucepzher.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3aceryfyi.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3knubmpud.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3yjfvxpdq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3qrlmdbsy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sqjctnuc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3emxokbhn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3membloed.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3koikfrce.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3edtzwbbl.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kmmrdikn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3yrzkiyni.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lpijsfok.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3qpbouqkl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ewwuhrsx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nqnvjfej.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lgjxlveu.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zaorozng.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3jwxxcwxb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3inahjftm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bqshsajd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3vhxpafbc.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3jazquppz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3btmwdzge.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3ylyixwum.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3uyeprilc.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3flcabbqw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3kvvbgtiu.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3liccreqs.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3utlzpcfw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3yufrzoxk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nroxisvc.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3fhutrvck.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qwkstgee.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3aaafkcuw.html


<!-- 参考信息 -->