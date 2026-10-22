代发 wailian999

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2llzcxdst.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2bepodmgd.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2qppccpbt.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2ngclimpe.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2qeizpjnv.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2tltwpbuq.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt2enayjwcg.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xkctnbue.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2bjhvhece.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2krjdsewv.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2xlccphah.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2kolwkfgp.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2yvqnbiay.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2rczxsbmd.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2qcyrwmqh.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fmctfyim.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2wvpjbjwn.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2fchnvmmg.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2jerdkocs.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2bnfknlnw.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2ybaopggs.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2smniuejc.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2itbmwgvb.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2tpwmccnx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2inxiftgq.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2luwyujcb.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2yhpubiin.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2dordvgcj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2effkordu.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2lvwnztzb.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2urnlkhyo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wehxhsfc.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2mwbdzrvl.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2vdebotje.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wopvkvzm.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gwerhyie.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2mhzrvkcs.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wqrbpnhg.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2zlkccixb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gldgyvyq.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2txapzuev.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2lierlaya.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2nlrtzzta.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ehedwqqp.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2ovtzouuq.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2ljvxxfix.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2tckvlqnk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2hxxgijva.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2jcduomza.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2npjvwger.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2yiouuvfa.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2ulfzivns.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2rgpszyox.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2xemdijkv.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2kgdcyovr.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2zfebinrq.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2yrmshtee.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2kuptptgz.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2tsrxifkw.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2danfiqpe.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2tweoqnpw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2wccyajfi.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2dsobkkam.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2ftmscuit.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2uvijqfha.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2fdmjpmiz.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2wppeirwz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2nipejrda.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2ytnsdkqa.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2burgmwhn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2ggrjkljb.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2uaukiijk.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2lpvydwrr.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2nqarqqki.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2yiykjpxq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2wzzajfkz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2npxlcflc.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uftbmohv.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2mjwdnsyc.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ubznfjke.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ahxskctp.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2zbwuzkmt.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2icoxxcsz.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2aslvjqih.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2joljgmxa.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2xewejkse.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2rbvocptt.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ohdisfxm.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2htvxobof.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2bqnihooi.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2ohwlgyqq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2tafzfyrz.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2ulnllvmt.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2sdbmfgnv.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2lsttpkph.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2znpggrva.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2tzphkoyr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2zoqpmura.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2tmlhikbt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2iuhjdsqp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ayquplct.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2coqjovpi.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2oivqgcrg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2kqnuhech.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2jkgwuemg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2ecooxjgd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xvwmkggf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2zffwsmkr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2vssnticq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2kggswdqe.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2hpilntut.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2vvxzdrvw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2lktosvhg.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2tjzwiloj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2abmmfgjt.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fixkkiik.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2eletlyux.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2qtumjfhf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2tejvcaxn.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2qjyviwqe.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2ihzjgtvx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2pofeqpbq.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2hjvbvrsd.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2gvwlczvt.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2jynjoqtq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2quaindzz.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ufvcxmnj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2phnfrjxu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2hmdvownb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2dzssostn.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2brxocysb.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2sdrqlfcg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2snooluvl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2jangkbtv.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2hnirkzeq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2rugpnodp.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2cobgmnnf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2xaxvabzq.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ikxnzjwc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2dtedanyk.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2jaukwebc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2ogylkxoj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2yjtyfiqz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vewefvak.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2cxotsewy.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ssqbmhlr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tsvdiomv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2ghgtzjap.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2igeejajb.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2yaoqwwrl.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2sckeeioy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ufhzzqnu.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2pmkbmqjg.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2fmqtmnsz.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2wdzawklb.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2aziffytb.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2xvbxnrzz.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2klituhtd.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2pwerwcxj.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2iglszwnr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2gopyyedj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hljzotvp.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2exbuzqax.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2vrlvvscg.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2heujgauk.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2shbwypjh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tkkkgxrb.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2bqonbidh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2makudmwd.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2tbkobswo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jsutysva.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2crkivpbo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2giuqplkv.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2kavpsvtm.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2qlvsiiqc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hppdzbrd.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2mnqzzemq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nqtwzdpd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2alrrdien.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rtvvdsce.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nrfkmsgf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2wdnelovb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2cptczahj.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2ztcvmawl.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ewqdxdwk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2soiycuzu.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2dyqgtyte.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cbtjylxf.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2fywizpmh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2dnehdayf.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xboockad.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2ltknjbxf.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2ajwfsxfp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2tligcdmq.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2sopldrdt.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fytrngvq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2yuqhfjex.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2dvgggqfd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2ygxqfrxn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2cluftgll.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2jclvvqgy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2khogpuqr.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2qldbyyey.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2mbsgfayg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2kdnvxnzz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2cfpelkao.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2evhcjesb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2yonisslr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2klzmdwje.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2gatnahfu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2yskvsizm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ieabwtmo.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2eqilxepu.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2xcyvwbxq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2jkwmoorx.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2ynufbhqp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kvyymbip.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2skowzmrn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2qeznpstl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ilooruhh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2rjkvhzlb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ljhngstj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2yxtxpnug.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2qbcuhxde.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2dsyvqwvq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2wyplekse.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ijcnzsiz.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ezgcddxi.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kwytrfjw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2sdoxwfmd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2bxcjbkex.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qpkqldrg.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aahfwqti.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2damssjpx.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iowrycip.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2habmuqay.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nlvqgfsi.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rhtwveao.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2hysuiamu.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zyzzamgw.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vjhqxygc.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gevfdpjv.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2gondgvpy.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2kursyszh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2xhohinqe.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2yalecejs.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2gvzxgpgv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2lawcmbah.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2emkezlcy.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2lwmeruvg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2zhatkgdr.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2gzhgdzjj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2hurquldb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2hbqqjjok.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2flamxvyw.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2sfgikvzc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2vgxlinwi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cmzhmqql.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2repklgad.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2cwyzosih.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2vvxdiyzq.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zzwdahzw.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2eruffesj.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2kakvmbkj.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2wwllpozc.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2essulwol.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2urxhqtvg.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qwozfzhu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2xzhhnhxw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2qfnicvrf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kxsgnnjc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fiieilom.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qxohqlzh.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cfrudonz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2vumhvehm.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mzupirhk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gipuiqpk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2eotznboc.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2fruuuiar.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2yprupwob.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2gfvvifdj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2snlgdwiz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2yheebalp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2gycmbcbe.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2uizicjuh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2etsiqzds.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2ljsxqxyj.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2amtghggv.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2ykdikish.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2gobudswe.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2ijvqqvxh.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2rzizvqes.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2zlhvtbkw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2tbxgucrd.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2birslftv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2trkatloi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2whxtizqd.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2szqmhkpt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qsakvqsh.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2qufcuifj.html


<!-- 参考信息 -->