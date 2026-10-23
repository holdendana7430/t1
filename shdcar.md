代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3huhplgwz.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3jpkjrtdd.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3xjiqqmfc.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rxslacjn.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3vwvaccow.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3tohqsjdq.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3dfujwsej.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3kljhqref.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3cbqaoomj.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3ofdsncdv.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3wdlfirdm.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3bfpbbqrs.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3owvcvrvk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3dsjoajpi.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3xhnksexu.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3obrrurxi.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3hpmaekzs.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3fmdywdfj.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3wdxnlfvl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3acfpvqux.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3nvwgtwax.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3eerdnpfx.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3twppkzoc.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3lbtsfjeo.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3kfaipcoe.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3ilbsxpfa.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3fpvvxfda.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3zldnnifm.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3sexvuuup.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3tulmxlqa.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3bfqgshwa.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zieveczl.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3qeejlnaa.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3auqnuxsd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3wjbugtph.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3gsodcbov.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ioxisysu.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3ublkzgsk.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3jselyica.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3ftxwsfrm.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3obtpxwjf.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3fghihkvd.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3lgzgeapa.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qwcbfbfa.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt3uiiidbdp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3ftztjcth.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3tceduiuy.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3emprdpkt.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3ttyhxxzx.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3pquifmuf.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3cdyawpnk.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3sgggbegz.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3poelwwjd.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ayneueyv.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3eidxisgd.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3dfbmkhkx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3vxncvetd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cpnnqdyh.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3cgwchiqs.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3zzekddfq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3esdgsttm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3fdrikyzm.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ihdljmxs.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3cgtzeupx.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3ishczcjl.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3tsphymyq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3wfwjedgz.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3nxszbmls.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3ynphsdzo.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3jrzpbuep.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3gtrgkjcl.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3uflcqovd.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3tmslbquz.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uihlmwsy.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3hwaxerpz.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3odreaayx.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3cepvtsht.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gthsaemw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3xwdqgsrt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3msemwsnt.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3jcbmocxq.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3qurefvop.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3ejeigzhj.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3rhkwfnda.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3rbouqakw.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3zshgnrhw.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3mbwhybug.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3ixpfmsnj.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3kpixastl.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3lscjzouq.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3hixekpim.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nfhqyjkd.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3xeibckqq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3rexsfalw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3dlgnrrlj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ztrlcgdj.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3qjryokti.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3eaietsno.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3nbhppnrb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jyweoqfn.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3geyzbdeg.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3bvypqapv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3swfkggfq.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3fejbvyxs.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fjuwthfn.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3lkcwqvqy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3eivqjtvv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3kllbmpxj.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3usfxmnif.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3uhmhphlc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3zmielgbd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3peuswrmv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3tmjnquea.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3afnoumpp.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3pwidcsyk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3nnpbnxfo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3ukgetomo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3jqucpwyc.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3atayrife.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3gntdmnhl.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3drywpdrl.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3tjahsztt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3ognrpkbt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3dyyponyb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3tncvvjtr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3kgodbwwf.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3mphuigso.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3gpdffymv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3yoknmesl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kczpmovc.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ptiwices.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3xtoqvgvq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3tmcufyzu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3fguqcdga.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3miywfvyp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3obisgfku.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3ltavrmht.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3otyzodtx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ggbimopw.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3etcaavja.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3qahvxrfj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3plqaneqr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qjogroyy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3fyllnegk.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3hxbzzfys.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3unkplqwv.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3vkyaeyxs.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cvyhxwsq.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3wyvvucqs.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3sgeppovo.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3xbmtpbeb.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3qxxzdglx.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3knjwtdyz.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3bjfjgyxm.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3hugeqhps.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3msnqcasx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3bctfwehs.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3xaxjdsrv.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3phufqoco.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3fmjitbhw.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3iprjibml.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3hzkbbdje.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qgidcfji.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3dbsulyzu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3jgwvxagr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3pvzgqhuz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3qiewzfuj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3knmmzspd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3bhqzcxan.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3zlhzendf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3tbzlpyhs.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ckmnayek.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3gnwsindr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3jujfccea.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ckrbvaaj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3mzypreug.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ovezmwtw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3hxrjmxpi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3xfcjwitd.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3nawvdrmw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3zrnnpvyj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hvftrckb.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3qornzzif.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3maoqaeds.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3mnlsdfzm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3mczencbk.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3lavipshd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3tcfggwvl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ippkkuga.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3nrchvihu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3lpylewij.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3njjfnmzw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ghkjnetv.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3mhptzptr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3itvxntfj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3vbikcsdy.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qzxhmybh.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3uzjyiqdu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3rbdvclre.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3uzlfztzb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3rlurfquw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3odxuakaj.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3hxcnjtyr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3fxajsygj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3dtlgsoyw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3wcgxorud.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3wblbxosg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3fdnvullm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3fdotxumk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3dpkfdsqx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3stpnmfrc.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3zjvztqan.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3eirbuaqg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3hbrqvxlz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3xfiwsejo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hynjpumd.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3qgjojklu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3rptuppwz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3rxueaxzj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3peglcwqn.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3jnezslkr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3aevkynmp.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3uvzjjmfu.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hywhyfiw.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wsiyrlln.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3hvkzibrw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3qtbxomvc.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bknzyaks.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3mzxotfqb.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3ognqwwfl.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nthuudxe.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3oxtdfblh.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fuhkoyxy.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3udbigpwp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3yjcjjvnb.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nwsvlrgm.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ihrgjhza.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3snicaqlq.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3qmvocami.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3qiooopjy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3lssbkgpl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3wqzjemrp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3iotbacym.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3wtschwba.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3gzgkcful.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3qflqetnp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3qfixtbxp.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3coppjwzk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3keiqmyog.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3szozgxar.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3fatwsyhu.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3tbcactlb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3wsvoyiue.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hwsehiuj.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3slrchcpz.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3cunpsezq.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3wfyjxvnd.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fwdlyaao.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3xisjxlef.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3lulehenm.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3wfngeuct.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3yjwtpjnw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3abfaiske.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3arxjcida.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3utfaghiu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3eebutfww.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sserkfjx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3erhxhjqo.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zkeakcim.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3soakdacq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3jrmpnanw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dbogzfjo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mndrpzts.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bnyopvof.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3vmzgbtcb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3upyidaft.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3dfyutvxd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ngvmbrng.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hwjpozfd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3zibchhhz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3sismucuj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3xbhiqokc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3fzvdbfqt.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3zumolapd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3klfmgocj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3gykolotf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3zvdmhtff.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3ijkbxjrp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3tvqfbgfp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3fpnqrupc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3wmrbuypj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3xswgland.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tzdjeclf.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3irtqfyak.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3idydadsl.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3cdkkuyrp.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3hfkpkkyk.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3qzvongpn.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wbhmylkq.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3aeavfmsf.html


<!-- 参考信息 -->