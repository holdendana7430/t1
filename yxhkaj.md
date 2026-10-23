代发 wailian999

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt3ddhkiazf.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt3ogzuzlvy.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt3xgaxoavl.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt3zabdrifd.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt3ptviqgpy.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3rzgkybfe.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt3rfhgcpfz.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3mjyitnja.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3lcxonpro.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3mqstuyei.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3uurercol.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3iznpqvyq.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt3atnuhzfz.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt3xshdfngf.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt3qtgafapw.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ejckcula.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3gdkxvmvq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3wjwxzvgj.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3hamriyyt.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3efyvcwrr.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3kzudezop.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3ujvcmqnw.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3luxnkdxa.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3robmgsvv.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3aunqhmmi.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3ncyxvfyu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3idgrdrko.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3iwdbjgtt.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3bionsdle.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3jdfusbrl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zilebuwg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3nnxrhbdv.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3hpzrflwo.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3qlijtyeb.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3pozlcvev.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xshgqsao.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3elhvaysf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3izrcezou.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3sphowxns.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gcvqkrku.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xbnnecvy.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3swxymjdz.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3jywnpxwe.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3hxthfvge.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3euhuctgt.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tpswodwi.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3qudwkaxv.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3qsurfevq.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3sqqbodac.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3uwbghbfn.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3mpxflssg.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3zobvkacx.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3phevuiuo.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3iojtrogb.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3inomueyb.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3xmhgqfak.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3hhyigshx.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3xhapnhli.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3qtzvsgoa.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3untfkwbm.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3dbwacrbi.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3dkjoqxli.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3emsnqatq.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3dzoxncny.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ahyplvip.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3gvdgtyix.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3ympehgtp.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3bfhgmufz.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3xleqxpgu.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3fmskiseg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3rynlkeug.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3zswvgeno.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3txuhmvyu.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3mxodfxvc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3gekjurfs.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ncchgmfk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3okssqoml.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3dgefzaed.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3czreuanp.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3edcnbjhx.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3cvfhxdwc.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3gnhrobrd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3houmwkbi.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3xcooaiwr.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3mnrghbax.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3hecuznkp.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3fyewwfqq.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3dkywxuzg.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3icosnfhr.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3zcpjtqqr.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3xoilblwe.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3trphjokv.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3zjkjsivu.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3shyxppue.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3vxkmrjog.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3ddbpqbya.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3syftzgym.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3ejlomdvy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3ywrhpylt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3bedneknp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3gxnyovqe.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3fgcyjdoe.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3lcyjhslg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3cmtxcbpd.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3qvyglpkh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3fxdoxpvq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3irbhhayk.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3cgcdepyj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3gcwxhusd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3ugendgdd.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3erbnhdva.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3rspttikt.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3xkycztop.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3siyhlijr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3quxakmiy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3kjdalpfp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3zevwlodl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3rkbpinqi.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3huuuzerh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ndgtjdcf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3eohiddlc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lhrirxtt.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3bstkkeaa.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3euchjqyv.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3vbjesydq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3dcbcrqoj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ylkolxbn.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3smjkkhqe.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3wpbmspbc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3nzsjjdrl.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3emlgirmy.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3wvqqwrnj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3ujdawbzz.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3ikbkujon.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3rweepjwh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3gocqtnjq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3xayboomk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3joxkwrhr.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3lhdxklyt.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3ifijnshs.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3rodxzvnp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3dtxwyltm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3zgcjfxad.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3yijalxpn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3vozixmfh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3pelirekk.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3aqbpvmay.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3zqwkblfx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3jtxgoray.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3duzoczox.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3njpzirgr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mqfmfhjf.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3hdapbbxz.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3dlmyqanu.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3tdcvdegm.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3fglmnwdu.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3ciodkrga.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3asbexcas.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3kdnfpstp.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3nbdwbjfz.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3szcggdkp.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3psqxexpd.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3kbukpoib.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vykcjeyl.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3gsoojnna.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3kmfdlyil.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3vehznerc.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3jrsmtlxz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3nmmcxvzr.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3wursnlfu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hhpjwbkj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3eygpydrr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3trpzcvyr.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3gnhtxzhb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3akbzgede.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3eyefzici.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3dpuurvth.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ogeteggj.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3yekfriyu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3kvenxfzq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3djigouyx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3szwnlyjh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3kqmwuvle.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3sxhragdv.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3qhdpuiqy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zsgkobqz.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3jeabgjdj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3eybrnerw.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3pdiubnwd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3ondyrfhp.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3gcxlutci.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3qipzgpiq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3zbjosspj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3nsamyzib.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3pfqdfevn.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ecpzdhzb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3umldwphb.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3kcyfdowe.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3dsqwumtw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3djgbabda.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3gqqpkkyn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3nckuadnq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3zpvkrwbr.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3tiboqgfz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3ifmbqylw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3jrnflwrf.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3kiywspoz.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3weyxzoes.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3rcyybnym.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3qqkfhjyn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3qvcnsjqt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3dpywyskn.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3qudufihw.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3gncwgdma.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3erfwvocl.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3nxjylvhv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3vtneppqr.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3ylcokmkj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3kkqruepr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3cadmxmqj.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3toydqqqt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3owdrdpsb.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3auntjbmx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ejfbyhql.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3eggrkdjd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3zdmgkbba.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3koheethn.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dcwtvexx.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3azucpzdm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3sngplupb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3hlkqufnn.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3coddeyea.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gcejmaxn.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3eyolwdcq.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kmmhsjmu.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yygvbrpr.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uhevqxzp.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hxlzzxzo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3jwmvppfp.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ugqcqijs.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jqwrvpss.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3oqwhpynp.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3niuqusyv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3qafejgtj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3gfbjvhqe.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3tlludztg.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3nfwaddzz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3axlauuvx.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3rytewgbd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3nxhghjhc.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3cdsmtmvg.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3ntlqfmda.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3amzdocux.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3dykohtwv.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3iowzwogv.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3wgnhbgef.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ojjkqywp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3coloxgoc.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3aucgmyka.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3hpirvwrt.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3xtmirlhg.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yrdietwo.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gebnwcxi.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3kfskslki.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3ihjrbbrn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3gatyozay.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3pignjtsk.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3oainxcdd.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3tmtkywwp.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3aldppwvd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wnlctllr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3odmnbeyc.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dnzexomu.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3snzhlawo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3tufcrfuu.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dofgcbue.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3psikonqy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ebiricem.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3quvunkcp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3kglwbtyl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3lmfifxal.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3afwycpgv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ppcjnuyy.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3cwcgieuf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3ufuzlauv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3yyztpfsx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3xyfxahnx.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3nihyjmgf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3zbqpnfma.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3jgrqhkat.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3qmvmvpet.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3dylfqkbl.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3gnlpgojh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3hogunzkx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt3izwlwfqn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3tqcopmdy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3imxtxtqz.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3gqmxwege.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3tovhaomv.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3hcqblyex.html


<!-- 参考信息 -->