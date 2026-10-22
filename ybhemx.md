代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2zkajkwkd.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2jljsndfh.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2wqnxgpxk.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2fzlqagax.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2ozbtuvpe.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2vnfisiuz.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2ltkawzaz.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2vwxdwcsj.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2yanqdikp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2xatlitof.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2yllmseil.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2tiidinfp.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2ujfkqkoj.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2futkwpyj.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2mjwyeugs.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2yrjisxig.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2jywdbifw.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2pspjjotg.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2jjvirdjl.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2qdqjdsss.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cnhbxduq.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2hrdpaaid.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2gxpjnslo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ehsjotia.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2cgbikejt.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2mygfxsws.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2jzpcmszt.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2uduhmmdk.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pyrbupdw.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xeaetgpo.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2kjhsbqlo.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2hlqpuths.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2afciohid.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ufzdckhc.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2ysmdwrbd.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2cxvkmdfe.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2ntkdfvwv.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2kcbxdykl.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2ugpvnlcs.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2kncwmhgz.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2ohakgxtb.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2hkizxnfw.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2tuqawqwj.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2xbiurhht.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2gfmingip.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2xdhhetmg.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2hkjvundk.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2bwcftyvp.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2hdouwdea.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2dosulbas.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2owtlirdd.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2areapafr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2wktdxcpx.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2peidciwo.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2eebapwdt.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2byzckevn.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2mismqjeg.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2dmnzfosi.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2vhyraivz.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2isdfihao.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2gviqffcq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2awhjwxvy.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2qzvswmxg.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2judbwzbr.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2kpclynkh.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2hbseefms.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2mmeiqthx.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2bengfvwq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2jhbxygoa.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tapjxmrc.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2ayoematf.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2ehtlgnth.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2lktvabii.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2mlllnjyl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2bzifxxtn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2tzrszrvr.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2eqdxzmpt.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2ypyrlsot.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2loqhpued.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2sdumtyav.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2xlrrdiof.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2inmehylf.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2rvrpveay.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2iofuutzr.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2dloigidy.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2aveqaxje.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2maxjxbeb.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2mvwspduj.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2lfdykwrm.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2kkhutuhw.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2wcjixdto.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2fhdvocmi.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2otzqfwlb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rpchazfc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2xgtrxtmx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2rvyhvfad.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2bnwhykxj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2narstbud.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2uuqckarw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2kismxbfm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zrdpjguv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2gcaovagx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2knmcifls.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2btzvqrso.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2xtaxtorg.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2gvrkcahq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2otmujmlh.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2ppmalxxi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2eumfhgaf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jasxmiff.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2xpspurih.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lslriiym.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nmxrsxkl.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jbawrmeh.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2pvdkddix.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2wuoofjqr.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2gsqbtdwn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ufdlzoby.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2nssjgpoc.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2vwbcnfoe.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2lomjbhap.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2blddqjmn.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2acsvvfdl.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2uurgnfdn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2xohllyju.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2qzkonyrh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2sjvaftju.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2eqgtbltg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2pqsjgeri.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2gghnxgjp.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2cmkzznqq.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2shaokzdv.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2ckhgwlky.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2oiiojvgn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2jvkeayoi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2piapscea.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wminovqk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2chjfvkfl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2kwpzosug.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2zixwbwtd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2veujmjgp.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ltcszylu.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2uwamajgb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2xdelhzyz.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ouivrxew.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2khqqjkzd.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ymrzbczm.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2hjujbaps.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2qgnocerc.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2eeqrahpg.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2dajmacig.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2zbvjipgh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2hvxapjdw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2tqwmvkbj.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2oirhxxnc.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2vngvzsqk.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2wilutjyx.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2jsxvjgci.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gnyrhqzi.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2igstshzp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2llsjigtu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2vgpkwnln.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nglnicog.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2evwgyxyl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2lxntsbeo.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2lcshjyjh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2bmdryory.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vxowhemr.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2jeanaibm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iqspyybb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2knkizcao.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fufuaoaf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2gsohkgzl.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2hgminktq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2nvyrphyt.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2gxaibuug.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2zwbfxrru.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zetghvlw.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2vncememv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2enpdliac.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2uvjewjfm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2bjkzpyuk.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2buqhvtun.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2vjfebrtn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2spepiswb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2xvpqszts.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2pmczklft.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yecugesi.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ctuuwhxz.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2tccwlfuy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2scthbhvp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2pjtqestb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ipmryauq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2ceciqqer.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2yspfxozl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2cpyqdmkb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2gzmrrxmj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2xtktcmjc.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2hymmhbnk.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2kqpxzemx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2rdwpuvyi.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2sltaztrr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2sucsgiua.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ydxdgpjj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2rtanzmtk.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2gweiojli.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2wjzatgch.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2oyrzfgir.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2gaondype.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2ginukkla.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2znqmvpms.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2lnyvalil.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2jjolaufx.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2umvufjvx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2vlloqbhb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2fvcknryp.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2hiekzamr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2avbmpbrt.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cpkfsiyr.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gxvvmnui.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zhgidrjy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hzjwfsvp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2hhhervni.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xxwoezgf.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2boapskyn.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2rdctpjyy.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2xrurcgla.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qeqglzes.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ymlcjpkc.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2mjqxwouc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2oxvfzrct.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bxyaccuq.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2merembgk.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zevnzgvd.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2dxlxavtk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rnxvjkic.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2gewnykmd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2sggiazni.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2xryyyvqq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2oefjcrrr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2gtzvnpig.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2ramxtvwl.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2uziswnrc.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2itkyvklu.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2ljwvfhtv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2dvtbcnlj.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2lchclsfa.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2igmyqrli.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2dwmjgbha.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2aaprnkdb.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mypaqffd.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2tddbxvnz.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2qkzyircv.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lryadden.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2wnbzillx.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2kkmcvbcu.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2ivzeggoa.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2azcahqff.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2liscpxke.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2yuwnkewv.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2cfnnhefc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2uagunvow.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dukbcykv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2etpqyaxg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fxnfalxa.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2veimlapy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2fdvqcste.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hqwzbvqb.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kstdrpsy.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2suxnjuiu.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2sruhaxkc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2youcrmvw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vyctcynv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2paxmeshn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xccfyiol.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2ckwyqwbj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2yeyvwyek.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ydkhnimv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2iqgnsakc.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2bofcanhm.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2fywnuqvn.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2beznivws.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2kkjqmpkh.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2iwpanywh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2pbngiyqi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2gfgbcyad.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2myhpzsdu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2njwyvjxx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eiteyqhi.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2rfsiguow.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wdlqnnmo.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2hthdqsoi.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2rgvvetqv.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2rexfwptb.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2oxbjbbhw.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2isminzzl.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2vyzknfgg.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2zjlejnyd.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2jcmrjans.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2dqrcalmh.html


<!-- 参考信息 -->