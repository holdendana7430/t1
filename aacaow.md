代发 wailian999

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xvvemvgu.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3arjsuksc.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt3jbdcecqi.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3bhoyjool.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3gmeeobct.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3czeoowjs.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3nlvzpjne.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3hjgncjph.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3gmamxdap.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3esodvkju.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3sktjbeqx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3bahmukrr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3iskkpozi.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3xysydhea.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3kxuxrsvf.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3jszpphim.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3qsccgunn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3safaimsi.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rbfwygcy.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3icxbdbiz.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3tigvyiam.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3tpyiqxxc.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3hmkuwugp.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3wekdlilw.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3ssablyrf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3qtxahdrk.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3cakkhjdt.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3vsaagous.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3epmfctiq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3dpuosdkw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3nkjpggov.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3flflzuzu.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3caqffevb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3fjkbzlgu.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3thqwakoa.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3cttqurmj.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3iaxxutqg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3fvhjjewc.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sxpyeice.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3jgtstlhj.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zcivcrjw.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3qhzcizvv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3zdsabmwf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3hpwqopcx.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3ezzgmnso.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3morqmmji.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3vggsuuyc.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3juvtozao.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3goazocpt.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3wgzooalf.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3cbmydczm.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3uvwbqqfv.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3wpgrrmvr.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3wxauhcel.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3esysulov.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3chjdpcjg.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3ndrojvqp.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3ksxqhfsa.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ujrbqzce.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3gimibqel.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3pymttdrs.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3gtoubxdt.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3qnoptjdy.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vipafwng.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3xsfmuuej.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3ezdlcrst.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3jxtyyefq.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3sjtmfvlr.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3ampnjdqk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3wzgrakma.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3gqnsdtej.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3uutfgtjw.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3yhigydhn.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3sgplgixe.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3eweixevy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3rfacmych.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3najplwhz.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3wncrkjwv.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3euvybfjo.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3optaygqa.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vjjowxlg.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3jxqxsrpo.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3dpfysrzl.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3knmrdeya.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3onzszvec.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3weslmawn.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3dcbylkfy.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3gydjcaat.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3ntxnuynb.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3flkoruey.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3ovwktejw.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3tutumzcm.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3mngqwqtg.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3rjzucsvt.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3clqxlqpv.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nczeqbqy.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3bckgkfky.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ffoyepps.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bcoirthf.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3sqconewo.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3vjmpwdvq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3boqfmsof.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3ndhabeay.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3tgczxydv.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3niwsihhq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3cdrnvrdw.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wlgwwnju.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3vkpbzerg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3lyjhpbrb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3dlflfxtk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3ybyiycmp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3chmrgmjf.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3zuuytecl.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3ctbxlpat.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3hcrowmkr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3sxezxwzi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fvaxoeew.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3cscrbzjg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3zmkdtjvb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3iawlklma.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rxofysnc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3zggbaifi.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3uqcxagzw.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3rkpckhei.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3nwbnbpdh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3otfwgjqb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3byyejjze.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3onernxyv.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3rbabblbo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3ltoelsig.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3jpastfsd.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3mvwoejyk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3vpvzijox.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3krepivfj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3fkfzybbc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3cjarptxf.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3hyldvvum.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3quqgbump.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3rqsunuoj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3cebkzuar.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3yriavxsr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3tkcsuyur.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3fpruwffr.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3kvqxxbyx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3dwijyxae.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3hvhtdquj.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3otjldkoj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3ydbekywv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3lrkjwqde.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3mstbpyir.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3bjhnamby.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3bmumpzpf.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ryqhsvec.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3gopsfpro.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3pnznbxeg.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3alvhztys.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3rafgyzyc.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3soycgaxm.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3jdrpepdn.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3uzmcqdya.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3rsxliund.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3pfbhyamy.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3ppptpnap.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3dgddjwch.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3dgfmiouy.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3scfraled.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3sprhawnj.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3wlfxrkrf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3unclgbsj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3hlcnwoxm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3cavobxaw.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vzezajzr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lhopzhwj.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3ygjzbrvk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bpywscmn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3obhrlhya.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3ddcbkvxn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3fqsvftuc.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3fksmikgc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zwtnrrbd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3nxeyjctu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3kkcrhfti.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3hqevpmbn.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zhlipocn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3wkzkfyna.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kghivpew.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3kmadkdkz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xjayxgsg.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3wgpeffkz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3pgxcueeu.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3forpvlnp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3vabtfmxi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3dpisdjxg.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3bxntkywn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3qwjapkmb.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pqyryemy.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3bxnelpdd.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3bvodbosv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3dxsimpmt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3gdysxakd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tezxljep.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3qzhycwzi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3acbvazem.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3unvpjtfd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3jlgenlqb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3mvijcpwm.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3mhuninjx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3ueljsmdx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3pamyxtem.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3aukdcszd.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3kdkiqtmh.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3ekdmbsya.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3pcbpvhdr.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3safqobkh.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3tzhkonvm.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3wpjcvosu.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lzvocvbm.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3jyshpowt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3llfqomta.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jffljayy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3kajnjfol.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jummzmky.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3gyrsdexd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3ihpvsdzz.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3lylfsvrz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3orztwucm.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sbfhgazv.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nggfczyj.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3snjozlxm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3ikjuuygv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3dhpldlcn.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zckrnfrk.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tkxywwte.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3ztgumbjo.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wobbwhoa.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3sfrtokyn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kazzrkca.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iaigvfzh.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3pmdreqjq.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ljfwsyja.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wbaqiiaa.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3fgwazmyb.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3gvugoqjf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3dckriqml.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3wsrlxswv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3aihwbytu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3pgsvxmbq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3mrvyxijz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3enuzywrg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3fgsxlfdk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3rknwkjda.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3uyrdkbbe.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3jjxzhlkc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3ndnltvuj.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ijtjtufk.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3fgxyfchw.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3jzuvbfho.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3mjiisoib.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3pudrmrnv.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3rbnayprc.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3tdmgphtf.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gsoyikhc.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3unygdkwf.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3phfhncfl.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3llrcdvuk.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3mxdllkhy.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3qkdddjjg.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xfsnmsnd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3vxwdgsge.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3erkmsbpk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hdmhhric.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ptjrrlis.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gfvzaotu.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ujppcjpd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3ralippii.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3utytgjhu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mccfnlae.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ynwfzwgw.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3dmhardjv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ntmksche.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sphhhzjd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3oslpdehw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3buorabyw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3oflakymn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3tpizwhbh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eegrscbz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3xjjsxtdq.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3vzrfacrh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3bycwoggx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3djwixxfe.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3nxhzlzmq.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3qmucxdve.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3unktpxsf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3wlcorhjj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3qonurlvk.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3fhslpczz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pekoqklz.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3lgfckivb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zaykfuhh.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3uxkmvigt.html


<!-- 参考信息 -->