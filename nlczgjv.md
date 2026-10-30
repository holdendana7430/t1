代发 wailian999

[E02] 重复字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gdmorkhjq.sHtML

Py:   "ab" * 3
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthnbbbsd.sHtML

PHP:  str_repeat("ab", 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gjkvafiwe.sHtML

JS:   "ab".repeat(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhbcemil.sHtML

TS:   "ab".repeat(3)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfaxonwrw.sHtML

Java: "ab".repeat(3)
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcitngaw.sHtML

Go:   strings.Repeat("ab", 3)
来源：http://www.share.fanxiaobao.xyz/Article/details/gbmxwadys.sHtML

Ruby: "ab" * 3
来源：http://baike.fanxiaobao.xyz/Article/details/gaarhwtua.sHtML

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gveibtqcq.sHtML

[E03] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjwglsii.sHtML

Py:   s[1:4];  s[:3];  s[3:]
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzofpcoz.sHtML

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://blog.fanxiaobao.xyz/Article/details/gtcvpgdnu.sHtML

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdwitrdt.sHtML

TS:   s.slice(1, 4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gflidteju.sHtML

Java: s.substring(1, 4)
来源：http://3g.fanxiaobao.xyz/Article/details/gyfnagkpr.sHtML

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqwnagxp.sHtML

Ruby: s[1, 3];  s[1..3]
来源：http://blog.fanxiaobao.xyz/Article/details/gwyhtuckh.sHtML

C#:   s.Substring(1, 3)
来源：http://mobile.fanxiaobao.xyz/Article/details/gbkwxxxra.sHtML

[E04] 查找子串位置
来源：http://mobile.fanxiaobao.xyz/Article/details/gooxzrmpl.sHtML

Py:   s.find("x");  s.index("x")
来源：http://baike.fanxiaobao.xyz/Article/details/gskearylo.sHtML

PHP:  strpos($s, "x");
来源：http://m.share.fanxiaobao.xyz/Article/details/gcuioknas.sHtML

JS:   s.indexOf("x");  s.search(/x/)
来源：http://3g.fanxiaobao.xyz/Article/details/gwbqcbbdt.sHtML

TS:   s.indexOf("x")
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzuqxypg.sHtML

Java: s.indexOf("x")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggykbitnw.sHtML

Go:   strings.Index(s, "x")
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxfphrrr.sHtML

Ruby: s.index("x")
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvyzbbgr.sHtML

C#:   s.IndexOf("x")
来源：http://wap.fanxiaobao.xyz/Article/details/gzmzqxqqo.sHtML

[E05] 判断包含 / 前缀 / 后缀
来源：http://baike.fanxiaobao.xyz/Article/details/gtiyfjpsd.sHtML

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgeortkm.sHtML

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://mobile.fanxiaobao.xyz/Article/details/gictxvnvd.sHtML

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggkxqadpe.sHtML

TS:   s.includes("x");  s.startsWith("a")
来源：http://mobile.fanxiaobao.xyz/Article/details/gtawvargx.sHtML

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://read.share.fanxiaobao.xyz/Article/details/gabcjoqog.sHtML

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjtlicby.sHtML

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://mobile.fanxiaobao.xyz/Article/details/gclrdjxhx.sHtML

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://wap.fanxiaobao.xyz/Article/details/gszahjgne.sHtML

[E06] 替换子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/guimegqmu.sHtML

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/ghedtenjo.sHtML

PHP:  str_replace("a", "b", $s);
来源：http://baike.fanxiaobao.xyz/Article/details/grrrxakrq.sHtML

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmvltvhu.sHtML

TS:   s.replaceAll("a", "b")
来源：http://mobile.fanxiaobao.xyz/Article/details/gndzufwkx.sHtML

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgwyymvx.sHtML

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gbpaxwxgf.sHtML

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://3g.fanxiaobao.xyz/Article/details/gqrbdtawa.sHtML

C#:   s.Replace("a", "b")
来源：http://read.share.fanxiaobao.xyz/Article/details/gbbegpsmq.sHtML

[E07] 按分隔符拆分
来源：http://baike.fanxiaobao.xyz/Article/details/gymzsbwwz.sHtML

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://wap.fanxiaobao.xyz/Article/details/gehbqcnow.sHtML

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijsikmgq.sHtML

JS:   s.split(",");  s.split(/\s+/)
来源：http://wap.fanxiaobao.xyz/Article/details/gajzvrcid.sHtML

TS:   s.split(",")
来源：http://3g.fanxiaobao.xyz/Article/details/gzdkajyup.sHtML

Java: s.split(",");  s.split("\\s+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwznycbe.sHtML

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbwthfzu.sHtML

Ruby: s.split(",");  s.split
来源：http://blog.fanxiaobao.xyz/Article/details/gbsfcwmpw.sHtML

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.share.fanxiaobao.xyz/Article/details/gaoqlgmtv.sHtML

[E08] 数组按分隔符合并
来源：http://m.share.fanxiaobao.xyz/Article/details/gijmyejny.sHtML

Py:   ",".join(items)
来源：http://3g.fanxiaobao.xyz/Article/details/gyrycdlqz.sHtML

PHP:  implode(",", $items);
来源：http://3g.fanxiaobao.xyz/Article/details/gcemmxiix.sHtML

JS:   items.join(",")
来源：http://3g.fanxiaobao.xyz/Article/details/guxrxvhsl.sHtML

TS:   items.join(",")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozvhwpbv.sHtML

Java: String.join(",", items)
来源：http://blog.fanxiaobao.xyz/Article/details/gheyivbnk.sHtML

Go:   strings.Join(items, ",")
来源：http://mobile.fanxiaobao.xyz/Article/details/gedrtxqza.sHtML

Ruby: items.join(",")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gigdnrvgz.sHtML

C#:   string.Join(",", items)
来源：http://m.share.fanxiaobao.xyz/Article/details/guvpvsmrz.sHtML

[E09] 去除所有空白字符
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwuxqicn.sHtML

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gewuztwdb.sHtML

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gecckciop.sHtML

JS:   s.replace(/\s+/g, "")
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxnqzdag.sHtML

TS:   s.replace(/\s+/g, "")
来源：http://www.share.fanxiaobao.xyz/Article/details/gssfoauvp.sHtML

Java: s.replaceAll("\\s+", "")
来源：http://mobile.fanxiaobao.xyz/Article/details/gqstwmxca.sHtML

Go:   strings.Join(strings.Fields(s), "")
来源：http://m.share.fanxiaobao.xyz/Article/details/gqlvbjlos.sHtML

Ruby: s.gsub(/\s+/, "")
来源：http://blog.fanxiaobao.xyz/Article/details/gwujtctwn.sHtML

C#:   Regex.Replace(s, @"\s+", "")
来源：http://wap.fanxiaobao.xyz/Article/details/gevrywsfv.sHtML

[E10] 左侧补零 / 定长填充
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdluzlhm.sHtML

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://read.share.fanxiaobao.xyz/Article/details/glooaltzn.sHtML

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://mobile.fanxiaobao.xyz/Article/details/gccxzungv.sHtML

JS:   "7".padStart(3, "0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghxbirnxf.sHtML

TS:   "7".padStart(3, "0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcivauass.sHtML

Java: String.format("%03d", 7)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsvqeoatt.sHtML

Go:   fmt.Sprintf("%03d", 7)
来源：http://wap.fanxiaobao.xyz/Article/details/gyupdkhki.sHtML

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://3g.fanxiaobao.xyz/Article/details/gfocotysb.sHtML

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://3g.fanxiaobao.xyz/Article/details/gqrkfojwf.sHtML

[E11] 反转字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gftyphcyu.sHtML

Py:   s[::-1]
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqjuzobt.sHtML

PHP:  strrev($s);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgjurjud.sHtML

JS:   [...s].reverse().join("")
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxqjdnnj.sHtML

TS:   [...s].reverse().join("")
来源：http://mobile.fanxiaobao.xyz/Article/details/gojgwgpnp.sHtML

Java: new StringBuilder(s).reverse().toString()
来源：http://mobile.fanxiaobao.xyz/Article/details/gzqhbyhhq.sHtML

Go:   // 转 []rune 后倒序再转回 string
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzwdvdtt.sHtML

Ruby: s.reverse
来源：http://wap.fanxiaobao.xyz/Article/details/gsjtlkwxj.sHtML

C#:   new string(s.Reverse().ToArray())
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtzpnlek.sHtML

[E12] 统计某字符出现次数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjzjqxhya.sHtML

Py:   s.count("a")
来源：http://www.share.fanxiaobao.xyz/Article/details/gfhxwdgwr.sHtML

PHP:  substr_count($s, "a");
来源：http://3g.fanxiaobao.xyz/Article/details/gphenehte.sHtML

JS:   s.split("a").length - 1
来源：http://m.share.fanxiaobao.xyz/Article/details/gsbndhhfj.sHtML

TS:   s.split("a").length - 1
来源：http://baike.fanxiaobao.xyz/Article/details/gdwxosrnq.sHtML

Java: s.chars().filter(c -> c == 'a').count()
来源：http://read.share.fanxiaobao.xyz/Article/details/gnepqvixo.sHtML

Go:   strings.Count(s, "a")
来源：http://3g.fanxiaobao.xyz/Article/details/gyhmlpjgz.sHtML

Ruby: s.count("a")
来源：http://blog.fanxiaobao.xyz/Article/details/gmcjmwkat.sHtML

C#:   s.Count(c => c == 'a')
来源：http://3g.fanxiaobao.xyz/Article/details/gdzzlwfgo.sHtML

[E13] 逐字符遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gbdsgkvdz.sHtML

Py:   for ch in s: print(ch)
来源：http://mobile.fanxiaobao.xyz/Article/details/gdopxmokq.sHtML

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfwyhxyr.sHtML

JS:   for (const ch of s) { console.log(ch); }
来源：http://baike.fanxiaobao.xyz/Article/details/gzgxsqvcx.sHtML

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.share.fanxiaobao.xyz/Article/details/goibcuqbj.sHtML

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvtwhowl.sHtML

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gpskzmhfw.sHtML

Ruby: s.each_char { |ch| puts ch }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmhmzqyj.sHtML

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.share.fanxiaobao.xyz/Article/details/gntuwlpsk.sHtML

[E14] URL 编码与 Base64
来源：http://wap.fanxiaobao.xyz/Article/details/gerdcmavt.sHtML

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmzsnahl.sHtML

PHP:  urlencode($s);  base64_encode($s);
来源：http://3g.fanxiaobao.xyz/Article/details/gcbsrhydl.sHtML

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctvlxvqj.sHtML

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/gucjvxbyq.sHtML

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://wap.fanxiaobao.xyz/Article/details/gzkosgcqd.sHtML

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gheelxiad.sHtML

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyokdsxso.sHtML

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://baike.fanxiaobao.xyz/Article/details/gkxswefpi.sHtML

[E15] HTML 转义 / 反转义
来源：http://m.share.fanxiaobao.xyz/Article/details/gnimwidft.sHtML

Py:   html.escape(s);  html.unescape(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gvzkfprxv.sHtML

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmokocqud.sHtML

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gfcagynig.sHtML

TS:   // 同上，务必做 XSS 过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gagrtturz.sHtML

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://m.share.fanxiaobao.xyz/Article/details/gwyfrzpok.sHtML

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giykwjfde.sHtML

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/glwoslneq.sHtML

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbjqkgey.sHtML

[E16] 数字千分位
来源：http://blog.fanxiaobao.xyz/Article/details/goiqrsxbz.sHtML

Py:   f"{1234567:,}"
来源：http://blog.fanxiaobao.xyz/Article/details/gqdqeneqe.sHtML

PHP:  number_format(1234567);
来源：http://wap.fanxiaobao.xyz/Article/details/gasmeafec.sHtML

JS:   (1234567).toLocaleString("en-US")
来源：http://m.share.fanxiaobao.xyz/Article/details/gunxnqucg.sHtML

TS:   (1234567).toLocaleString("en-US")
来源：http://blog.fanxiaobao.xyz/Article/details/gxklnptpq.sHtML

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://mobile.fanxiaobao.xyz/Article/details/gakkcnmum.sHtML

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://3g.fanxiaobao.xyz/Article/details/gozewdkut.sHtML

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://3g.fanxiaobao.xyz/Article/details/giwyajzkz.sHtML

C#:   1234567.ToString("N0")
来源：http://3g.fanxiaobao.xyz/Article/details/gflptnoxs.sHtML

[E17] 首字母大写
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvlgenli.sHtML

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://3g.fanxiaobao.xyz/Article/details/gwfcljulb.sHtML

PHP:  ucfirst($s);  ucwords($s);
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhdofdvt.sHtML

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gwxmtdsiv.sHtML

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gphddhsrl.sHtML

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhqkwree.sHtML

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqzdepwv.sHtML

Ruby: s.capitalize
来源：http://www.blog.fanxiaobao.xyz/Article/details/gantotzlj.sHtML

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://wap.fanxiaobao.xyz/Article/details/gqgtthynm.sHtML

[E18] 模板占位符替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gndhclmfb.sHtML

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://read.share.fanxiaobao.xyz/Article/details/gabevkabd.sHtML

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://blog.fanxiaobao.xyz/Article/details/glvjvxnuo.sHtML

JS:   tpl.replaceAll("{name}", name)
来源：http://baike.fanxiaobao.xyz/Article/details/gkgmjabka.sHtML

TS:   tpl.replaceAll("{name}", name)
来源：http://baike.fanxiaobao.xyz/Article/details/gqbffuqlu.sHtML

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsboqdcw.sHtML

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtftkdca.sHtML

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://baike.fanxiaobao.xyz/Article/details/gimndzikt.sHtML

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://blog.fanxiaobao.xyz/Article/details/gtmclbqjt.sHtML

[E19] 多行文本按行拆分
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpuzlfcd.sHtML

Py:   s.splitlines()
来源：http://read.share.fanxiaobao.xyz/Article/details/gyhjjynpm.sHtML

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqjwlwtl.sHtML

JS:   s.split(/\r?\n/)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glehdohgj.sHtML

TS:   s.split(/\r?\n/)
来源：http://baike.fanxiaobao.xyz/Article/details/gsgxfshgr.sHtML

Java: s.lines().toList()
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdfsvlxj.sHtML

Go:   strings.Split(s, "\n")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvyicthqr.sHtML

Ruby: s.lines
来源：http://3g.fanxiaobao.xyz/Article/details/gkpaculon.sHtML

C#:   s.Split('\n')
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqlewvrb.sHtML

[E20] 判断字符串是否为空
来源：http://read.share.fanxiaobao.xyz/Article/details/gqksllhyt.sHtML

Py:   if not s:
来源：http://3g.fanxiaobao.xyz/Article/details/guzykmnoi.sHtML

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqanlwbp.sHtML

JS:   if (s === "") {} 或 if (!s) {}
来源：http://3g.fanxiaobao.xyz/Article/details/gxwrtksia.sHtML

TS:   if (s === "") {}
来源：http://baike.fanxiaobao.xyz/Article/details/gqrrktcdp.sHtML

Java: if (s.isEmpty()) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/glcsbbpmw.sHtML

Go:   if s == "" {}
来源：http://baike.fanxiaobao.xyz/Article/details/gmgjtqcbz.sHtML

Ruby: if s.empty?
来源：http://baike.fanxiaobao.xyz/Article/details/gaqcxufqm.sHtML

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://blog.fanxiaobao.xyz/Article/details/guplxwwft.sHtML

[E21] 超长截断加省略号
来源：http://baike.fanxiaobao.xyz/Article/details/gjabyqzzj.sHtML

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://mobile.fanxiaobao.xyz/Article/details/gppogfwan.sHtML

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://baike.fanxiaobao.xyz/Article/details/goeophohp.sHtML

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmdivodwx.sHtML

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicyblruy.sHtML

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://wap.fanxiaobao.xyz/Article/details/gfhdmwezy.sHtML

Go:   // 按 rune 判断长度后截断
来源：http://3g.fanxiaobao.xyz/Article/details/gnfaeeigf.sHtML

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkaeuvwlu.sHtML

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://blog.fanxiaobao.xyz/Article/details/gkzsdisgn.sHtML

[E22] 字节长度与字符长度
来源：http://3g.fanxiaobao.xyz/Article/details/griwgejfr.sHtML

Py:   len(s.encode("utf-8"));  len(s)
来源：http://wap.fanxiaobao.xyz/Article/details/gtpvakwob.sHtML

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://blog.fanxiaobao.xyz/Article/details/gnwbyjtvs.sHtML

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.share.fanxiaobao.xyz/Article/details/grzliuaob.sHtML

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelpcdzmb.sHtML

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsqrbvda.sHtML

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://m.share.fanxiaobao.xyz/Article/details/grggwfeqf.sHtML

Ruby: s.bytesize;  s.length
来源：http://read.share.fanxiaobao.xyz/Article/details/gastlgqmt.sHtML

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzdykuiq.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gfltrywyy.sHtML

F. 文件与目录
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzfpbbam.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gcszvndwk.sHtML

[F01] 读取整个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjcpjnwm.sHtML

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://wap.fanxiaobao.xyz/Article/details/gpazbmgpr.sHtML

PHP:  file_get_contents("a.txt");
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgoslmfq.sHtML

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://blog.fanxiaobao.xyz/Article/details/gqzmnstpr.sHtML

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://wap.fanxiaobao.xyz/Article/details/gezbnpcnj.sHtML

Java: Files.readString(Path.of("a.txt"))
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrywmccp.sHtML

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.share.fanxiaobao.xyz/Article/details/gohsqktjr.sHtML

Ruby: File.read("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gaffcenni.sHtML

C#:   File.ReadAllText("a.txt");
来源：http://3g.fanxiaobao.xyz/Article/details/gpyizzdtf.sHtML

[F02] 逐行读取文件
来源：http://wap.fanxiaobao.xyz/Article/details/gxvtfmmyg.sHtML

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.share.fanxiaobao.xyz/Article/details/gdyusglwt.sHtML

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbxmbamkz.sHtML

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://baike.fanxiaobao.xyz/Article/details/gbynrvynd.sHtML

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcicbqzjh.sHtML

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://baike.fanxiaobao.xyz/Article/details/gebgdpbfu.sHtML

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gckzscbfv.sHtML

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqerunkob.sHtML

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://wap.fanxiaobao.xyz/Article/details/geprjiksx.sHtML

[F03] 写入文件（覆盖）
来源：http://www.share.fanxiaobao.xyz/Article/details/gxuzwjrbr.sHtML

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://wap.fanxiaobao.xyz/Article/details/gntlgdovz.sHtML

PHP:  file_put_contents("a.txt", "hi");
来源：http://wap.fanxiaobao.xyz/Article/details/gsmyzcdjq.sHtML

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpnhtvwd.sHtML

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://m.share.fanxiaobao.xyz/Article/details/gyjvypleu.sHtML

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://mobile.fanxiaobao.xyz/Article/details/guajzwynh.sHtML

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gylkkuujl.sHtML

Ruby: File.write("a.txt", "hi")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwlumbsg.sHtML

C#:   File.WriteAllText("a.txt", "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/glwbmtlwt.sHtML

[F04] 追加写入文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwoqfgfng.sHtML

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://blog.fanxiaobao.xyz/Article/details/gjkmcoyid.sHtML

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://3g.fanxiaobao.xyz/Article/details/gnpnmevdu.sHtML

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://3g.fanxiaobao.xyz/Article/details/grjwjejpf.sHtML

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.share.fanxiaobao.xyz/Article/details/gggpoipet.sHtML

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://baike.fanxiaobao.xyz/Article/details/gflhtavdb.sHtML

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcaineds.sHtML

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://wap.fanxiaobao.xyz/Article/details/gneptjixd.sHtML

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://wap.fanxiaobao.xyz/Article/details/gtmyrhhtq.sHtML

[F05] 判断文件或目录是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlmupuat.sHtML

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://blog.fanxiaobao.xyz/Article/details/gfkwausxp.sHtML

PHP:  file_exists("a.txt");
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwtmmlrf.sHtML

JS:   fs.existsSync("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gjpyozbpj.sHtML

TS:   fs.existsSync("a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gxskmztbd.sHtML

Java: Files.exists(Path.of("a.txt"))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtynmtijk.sHtML

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbymdugj.sHtML

Ruby: File.exist?("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtbeuuiy.sHtML

C#:   File.Exists("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghllbdvsf.sHtML

[F06] 删除文件
来源：http://blog.fanxiaobao.xyz/Article/details/gvvsqzlfe.sHtML

Py:   os.remove("a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjjdwgas.sHtML

PHP:  unlink("a.txt");
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpyavyyb.sHtML

JS:   fs.unlinkSync("a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gateqehrm.sHtML

TS:   fs.unlinkSync("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/ghbixvfsm.sHtML

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.share.fanxiaobao.xyz/Article/details/gseeanyqo.sHtML

Go:   os.Remove("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsrxuyxu.sHtML

Ruby: File.delete("a.txt")
来源：http://blog.fanxiaobao.xyz/Article/details/gtfexewjh.sHtML

C#:   File.Delete("a.txt");
来源：http://baike.fanxiaobao.xyz/Article/details/gqvqmcedk.sHtML

[F07] 创建目录（含多级）
来源：http://read.share.fanxiaobao.xyz/Article/details/ghossyvmh.sHtML

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://baike.fanxiaobao.xyz/Article/details/gkobvcnjw.sHtML

PHP:  mkdir("dir/sub", 0777, true);
来源：http://blog.fanxiaobao.xyz/Article/details/glddswqzl.sHtML

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://baike.fanxiaobao.xyz/Article/details/gjofmbvju.sHtML

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://3g.fanxiaobao.xyz/Article/details/gxjafblnj.sHtML

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://wap.fanxiaobao.xyz/Article/details/gvttzzqil.sHtML

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://blog.fanxiaobao.xyz/Article/details/ggdlbyuqm.sHtML

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://blog.fanxiaobao.xyz/Article/details/gcdaxluiy.sHtML

C#:   Directory.CreateDirectory("dir/sub");
来源：http://baike.fanxiaobao.xyz/Article/details/ggvgdlocn.sHtML

[F08] 遍历目录
来源：http://3g.fanxiaobao.xyz/Article/details/gkgbppwvo.sHtML

Py:   for name in os.listdir("dir"): print(name)
来源：http://blog.fanxiaobao.xyz/Article/details/grheswmjo.sHtML

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://baike.fanxiaobao.xyz/Article/details/gyghaltcg.sHtML

JS:   fs.readdirSync("dir")
来源：http://3g.fanxiaobao.xyz/Article/details/gadrjrsdk.sHtML

TS:   fs.readdirSync("dir")
来源：http://mobile.fanxiaobao.xyz/Article/details/glzrjpxgn.sHtML

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzfsjawg.sHtML

Go:   entries, _ := os.ReadDir("dir")
来源：http://wap.fanxiaobao.xyz/Article/details/gkdchgwvf.sHtML

Ruby: Dir.children("dir")
来源：http://www.blog.fanxiaobao.xyz/Article/details/giihwthwt.sHtML

C#:   Directory.GetFiles("dir")
来源：http://m.share.fanxiaobao.xyz/Article/details/gyroubson.sHtML

[F09] 获取文件大小
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacuvwltm.sHtML

Py:   os.path.getsize("a.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrbfmkou.sHtML

PHP:  filesize("a.txt");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctkfxiqk.sHtML

JS:   fs.statSync("a.txt").size
来源：http://3g.fanxiaobao.xyz/Article/details/gzdfnlkmt.sHtML

TS:   fs.statSync("a.txt").size
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjekzkdux.sHtML

Java: Files.size(Path.of("a.txt"))
来源：http://3g.fanxiaobao.xyz/Article/details/ghxnhfuop.sHtML

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.share.fanxiaobao.xyz/Article/details/gykvjyxhi.sHtML

Ruby: File.size("a.txt")
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxqhsqdp.sHtML

C#:   new FileInfo("a.txt").Length
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvudpckx.sHtML

[F10] 取文件扩展名 / 文件名
来源：http://3g.fanxiaobao.xyz/Article/details/gmhiomgvo.sHtML

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gqbhahqwt.sHtML

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://read.share.fanxiaobao.xyz/Article/details/gonrydeei.sHtML

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://wap.fanxiaobao.xyz/Article/details/gtensviva.sHtML

TS:   path.extname("a.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/ggonhdvxo.sHtML

Java: // 手动 substring(lastIndexOf('.'))
来源：http://read.share.fanxiaobao.xyz/Article/details/gwszumkxb.sHtML

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://mobile.fanxiaobao.xyz/Article/details/gchhgojnh.sHtML

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gqojyynvo.sHtML

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfndjoyb.sHtML

[F11] 复制与移动文件
来源：http://read.share.fanxiaobao.xyz/Article/details/glrgsmury.sHtML

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://baike.fanxiaobao.xyz/Article/details/giockeheg.sHtML

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://wap.fanxiaobao.xyz/Article/details/gqfjvhmcv.sHtML

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://read.share.fanxiaobao.xyz/Article/details/gxruplcos.sHtML

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://3g.fanxiaobao.xyz/Article/details/gklhnjbao.sHtML

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://baike.fanxiaobao.xyz/Article/details/gjbkwhpzj.sHtML

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://blog.fanxiaobao.xyz/Article/details/gqtphjhfd.sHtML

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbappwcn.sHtML

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpwfrvza.sHtML

[F12] CSV 读写
来源：http://read.share.fanxiaobao.xyz/Article/details/gaircrcjh.sHtML

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://blog.fanxiaobao.xyz/Article/details/gwqhnvnrp.sHtML

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://blog.fanxiaobao.xyz/Article/details/gyonofkht.sHtML

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.share.fanxiaobao.xyz/Article/details/gkdqfqtsv.sHtML

TS:   // 同上
来源：http://wap.fanxiaobao.xyz/Article/details/ggoonrlfa.sHtML

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://baike.fanxiaobao.xyz/Article/details/gywymdtfh.sHtML

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://blog.fanxiaobao.xyz/Article/details/gprvycxce.sHtML

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxekwdvpu.sHtML

C#:   // 无内置：用 CsvHelper 库
来源：http://blog.fanxiaobao.xyz/Article/details/gwugpahyc.sHtML


<!-- 参考信息 -->