代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt3bbqzyjkx.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt3hedbefzo.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt3fblwkxyd.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.ydjk.org.cn/Article/details/gt3evjufxxi.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt3fnqeoqfu.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt3vhowsmtu.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.ydjk.org.cn/Article/details/gt3xaikscqf.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3typzdsbr.html

[E02] 重复字符串
来源：http://www.52xcode.cn/Article/details/gt3qfrlmjhq.html

Py:   "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3pdahplxw.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt3qcmcbnyn.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3xlsknytm.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3isxnvqgu.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3omccsmau.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3ocxgbple.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt3niqnigcy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3pqvycfkd.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3hdrkywws.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.ydjk.org.cn/Article/details/gt3jqjpqlyn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3atlakmbz.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3hrlqdgmd.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3exwqlwal.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3kgufdnpg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3idmwvwvj.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3ikhqljto.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3vxnhccac.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3vtfmedko.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3wdvlypul.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3dpqftcnq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3wnwdasgv.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zqogsabo.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3cmwlkudt.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3jqpahccp.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3symhylsp.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3smhcstqt.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3alohsnfx.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3gomcwfve.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3ayxycuol.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3umgnztfq.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3laclrdrw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3mqpfgdbt.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3eaztrfev.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xfzlzplr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3abermnql.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3hxbmbylf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3pctttodb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bxxizaic.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lxhvqird.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3pbwfumtw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3egalkrod.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3sdscyvlg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ycvfmrww.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3orsxoiyb.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3hjeadpsm.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3foakzhzf.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bdciyeuh.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3kjhyahau.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fhdzpalw.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3gthdlqwk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rfbklahj.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3mzpqqtqy.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3cmawhnhm.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3faqoynzs.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3dxemfjtl.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3loyqptxw.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3gvdtlbst.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3uxawiyhj.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3mhchkoaw.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3kgiutxqy.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3yahdxhxs.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3vdndredh.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3rkajmgri.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3xmkszjte.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cyayhgbg.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3blvccgkj.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ohtjlhey.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3mxpvnnjp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3iubtxaym.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3ygtvsxfk.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3geqoctbn.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3yhkmtdky.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3ygygrkxd.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3frjrdlfj.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3aehqahcb.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3nfhzduwg.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3xqsnacze.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3rnbwodji.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3yeqnrrzq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3gkryzoka.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3osuhfzom.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3yncuenjt.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3yfajdmsp.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3otrlgmnc.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3ybeznjgh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3kxuzgwqf.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3qnyuxwfz.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3mwexgjnv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3dhrkpjyo.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3fedfhnrd.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3aimqwtom.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3yqlujbep.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3vtcgkmmf.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3mddwozdy.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3bvdudqwe.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3mvwooyic.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3lsmunbvy.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3jtckhgmt.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3ckhbzvnw.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3taduzcet.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3isyaezcr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3gvecxdio.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3sellwzno.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ztsudptb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3idibkiii.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3fzdpfioj.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3nkvywusg.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3iwfkdlih.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3rsuzgyae.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3caimashl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3tprdgrcc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3prowlqzr.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3txtmcknn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3kcqxbjgm.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3iglykhat.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3wjnbrsty.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3fvuskztl.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ptpxddlc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3uptksbah.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3phjrkzzx.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3tsxbejig.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3folhipda.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3rlvrryqb.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nolqadwf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uvuddfil.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3gvhaowae.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3cnaoxoqp.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3vllgrlaz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3yiuqmkyn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3bmdwegwd.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3sgyuxhix.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3adzgjabj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3gqcjdkea.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3jjbmqqfp.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3uskulhnw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3posrejun.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3lvzivniz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3owwghymk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3dwmisvel.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3nkpjjzyt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3hfizhxql.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3dzabxqob.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3yoybmtvs.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3rhxrrmrd.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3onahdjsh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3nyduneif.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3otifehgc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3najvyrhf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zdcwbsqz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ioeynxel.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3wwufakio.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3slkhewpi.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3tvxohbhw.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3nutzuqcd.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3kozpdqfo.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3qwycyiaq.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3fsjnenhw.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3gweyaxie.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3watqyojf.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3poehgetz.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3kyymsywb.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3xowsxxjq.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3fmosrxch.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3todxbupt.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3kmrwkutx.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3bwgyswoz.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3ijtyyneq.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3wofozros.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3athxwguc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eoofjiue.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3jyewxpqr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3qiwnbter.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3vprqxoth.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xzdmnlbj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3uaiyvuug.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3dxfgknoh.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3rrcdvmjl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ctzdjecz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3lznjvxef.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3xfbxfnio.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3oexwaybf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wmpmrthu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3qdkoeehr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3tbvvjsdx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3ynpsazhf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3mddskxnk.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3budszvsv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3cbownzhd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nlnkcszk.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3kihspaxz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yxbdlmiu.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3mseganio.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3ggauahzu.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ntczphup.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3kmsivxqa.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3yukkglog.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3apqerirn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3tqfkuucp.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vdqfgfzu.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3drcbyrju.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3alsoqeqy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3pbkkiapk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3grzxqorq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3djowqifd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3useyoqbx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3wgcrlzht.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3qsxzfovr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3lbpqotfy.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3omzyueji.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3kxydnpdl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3hrdxtoyr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3xypjsghm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3zohkrfcy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3gigbzwbg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3doiswfch.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3hocfydkl.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3elxwkjcm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3tafpszkm.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3dnvyeqgp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kbwcfhlg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3ajzulqhs.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lqspciav.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ictclnqa.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3qrjgjtdn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3rqanrhcd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3swpocjwe.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3ynxiutgc.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3cpxtymfj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3xvkgslpn.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3qnlbryvp.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kjzgkgwx.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3cysdmzsj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3dwbvxjhx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3wmdcuvjq.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ijedhriw.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ulbuoalg.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3vmomxvuk.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rousmqik.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3hsodcqdb.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3paxemyxd.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qicguqcr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xizatpbr.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3njwpiwgw.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3crglfxaq.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xhfuufaq.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3xfrfdyjv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3sitqkqhc.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3pymlxekk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3pvwcwcsl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3vmcdgdso.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3hxvaraox.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3wlktpxpg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3ialoqcxv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3kcsxiyhl.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3mvmnjuqx.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3peoqmsfo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3gwzqvetv.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3xkpiforl.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3odotkuty.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3frdsryco.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3xjjwxfxu.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3xevathut.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3bajoskus.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3swmywozo.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sbqftocg.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tszsdkvz.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3mjlxyngc.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3euhaidro.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vhzachgz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3vafenonj.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jrkazgax.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3fqfinust.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3iknfiuej.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3aiaiymeh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3opqkyjcn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pzgnshsk.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bbqdnogm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3eehgerbq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sozoztkk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qfkyhnqi.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3vsjvhfzd.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3tcjgosbw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3zwkwccae.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3tecqwgmp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3eeqphgml.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ggjdswlp.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3zoqriulh.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3xgekwcbt.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3segyeyox.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3noxmeqjd.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3zaanqqoz.html


<!-- 参考信息 -->