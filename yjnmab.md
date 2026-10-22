代发 wailian999

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2isfwipqi.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2uodqaync.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2cwtqyagn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2itltllmv.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2tugfpjod.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2gzftqpvb.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2mptosywd.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2qoknqrxj.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2gpmmamcm.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2qfpymeza.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2ftioxoyz.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lcgdsbvy.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2rtuldalr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2vuhkudyn.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2fioiwczp.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2uplaoabx.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2rhxelhrd.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2cglcyivg.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2sfizldgk.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2hmujexpr.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2zoiwceuf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2ikstaqlu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ykxtdkjd.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2lgyefxyy.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2mqvhlcca.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2pbecyanh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2bbtohqbr.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ovxjorlm.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2intvyifv.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2ubkjdtcs.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2hpxycpsu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pezgkpef.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2kfclklli.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2aykxruwq.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2vtkyhdnf.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ptuqpzcz.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jibhtueq.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2sfdqsxqi.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2wantroft.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2rsjvmfhj.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2tchcrsrb.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gekvjizb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2emobsuah.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2qtvfeihu.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2vqturyku.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2vkhxbhmn.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2enfepqab.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2yewlwtkg.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2kqkluyxo.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2bfyfqutj.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2vhsjmsnh.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2vgouhvjy.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2fturujxd.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2sjbxqlsw.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2llqdupbd.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2oqhxvmzx.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2gowgoqla.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2tptdkyon.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2kanujpss.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2zfhzgibe.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2hezmgocj.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2fmrkoabx.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2xufefpev.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2luytumkv.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2jmbpvdlp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qaupgulf.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2epzanmzn.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2fenqgjcj.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2izjmtkpj.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2upkyotfo.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2narhvdrz.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2eyvsriqv.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2igahcucu.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2tfshahid.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2dvvvxgec.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2hmhbjeun.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2gezpzvwh.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2edttzzto.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2yvtrekju.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2psixqrke.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2dhulfnyh.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2hlyzlxpn.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2fusgeeqb.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ovbxlfgx.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2pyplctwo.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2tpazrioi.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2obvygfqc.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2aowsncru.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2qteqinhj.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2vpjrfefw.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2jftjjpxv.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ztvzpisk.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2gdmemdiq.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2cdxavzrd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2sjopuxgu.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2bjgtcxha.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2uffoupva.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2xnyqsyxj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2ccjmllpy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fcnzgfdh.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2xdisvicq.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2qpdaqdlb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2rvwqlufj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2irxvowfb.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2qzvcxdlx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2dtcnabsa.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2hdtieheb.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2nbghglbd.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2qxfuzhpl.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt2ebvudesk.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2epwqjnzb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qteuqmzx.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pvqwikjw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ecfqgifm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2btdpudjm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gsstcuan.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ostxkubq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nvcighzg.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2bpvfbeuy.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2invhoowe.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2kqitciqz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2jpqhepas.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2twhufbtc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2dqctrrmh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2siazfgwn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2erhkwdju.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2clwcekyv.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2mesohpwt.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2dlgrduer.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2gtohaybw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zxdhdvlg.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2fhqovnun.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2mcemisxc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2iminrsmd.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2fadropwd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2kyivbavk.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2ecxfuewp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2cigoqsrs.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2mpihthdt.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lrrpuopq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2xbajoero.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2vchinetv.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2syhthpfy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2tnmcebmx.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2fxsxltrf.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2qgpeoeid.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2mslntcgs.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2qdpkfojv.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2trixxfcv.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2bsabrzkx.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bvtmonts.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2rixqnqsx.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2jdxduvda.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2tygxiaaq.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2rsmlltix.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2krzlieup.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2vihlrtpf.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2apntyrrf.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2ryksoxxn.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gyvmompe.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2iqmvioyx.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2tczfyumn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2olxdwhpr.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2sszwahgs.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2phwmbwrc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2afdcjvle.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vxzqnazd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ddlxtall.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2crmgcpko.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2zjnpklxk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wypgbanr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2flrttgyx.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2xzashmtc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2ejhhgqnd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2agxwrmua.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lqxmqtrb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2gtjtvlal.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ojfelvmk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2hvcejomw.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2awhldmge.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2jgugwmms.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tebzffbe.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2tjzfbjrf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zzblvhde.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2uxaeyduc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2csuvmsws.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2codwzsgg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2pxbkaalb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2djvolvce.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2nqwildtz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2xtprmtpl.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hrqnhryp.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ihkkfphn.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2kwclgejn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2cypfycwu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2gtvsbbtu.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2tdgsrsfl.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2vgqyqlrs.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2hlrnvgis.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2fsjsgwoh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2fewhvyrg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2tpfrbhfh.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2efqtdyxi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2weqreyop.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2oemzljqs.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2fqpbrkwl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2hqwaxcyn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2qzzowtzy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2tsgphqta.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2sfucwlwk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2himebhji.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2wyuqrujz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cfjstquq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2cdnjputz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2egmymffc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2bfebrwmr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2nrisccgs.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ffifmhyi.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2vayaqcvy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2zoteupix.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2nnijvmef.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2ppkhxdod.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xktbwvcx.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gswqnenw.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2degqlafg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ggxnmluv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2obntodeb.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qnydufzs.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wnesfchs.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2bcidwfct.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2efqybmno.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mhjrkxtt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ijniyyyi.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ltjuwzca.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fhcuohpr.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xwmkgnps.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nhibsues.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2xqblrqqz.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2jcagbfuj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2dekkjcfq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2izseswrs.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2ocsvvkhd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2xizoafuv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2bkeirtlf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2wrdgkjnv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2olhijhcr.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2qzninbjc.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2jwbazrhb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2jacrrlgg.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2plgkaooc.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2rwvnbobq.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2rkqiwyth.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2bupewyas.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bodyajnd.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2grlcqsei.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2dmzattsq.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2ukzoxznm.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ucbogjba.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2slokvlwm.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2rkhzqcdw.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2taykifge.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2eonnxhwa.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2vsszurve.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2spekdefv.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2gnbjftvr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2jjeywmuo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lbkypoga.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2evezckpz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zfibkddi.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ucpxapax.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2kupxmrpj.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fnfqaygh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xwgkrtio.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ptiqmfra.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2uqzgubji.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eftdnafc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qoygfnbp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ihwqybnt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2jmklwljo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2vvinrapo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2frxviugh.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2hhdqdsyl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2ureamckh.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2ejrunwqj.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2bqfvuifp.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2zbqfsdpw.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2htkznswq.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2ntzljwyc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2dqniguds.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2foaoviov.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2hupfbtov.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2dwvgtgwn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zobxssqd.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2juiqgxfr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qrwgqhap.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2vcuvnfqy.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2amxkkeia.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2ogavgjdf.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ijfyfjlb.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2xdvkufek.html


<!-- 参考信息 -->