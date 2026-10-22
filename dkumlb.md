代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2xillztxf.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2nrgyuaen.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2nvoorxhj.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ojfigpcr.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2expgwtjb.html

C#:   s.Substring(1, 3)
来源：http://www.52xcode.cn/Article/details/gt2lafwwghd.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2zqhhwazs.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2nqpoqgog.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2jriaqiqp.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2sixwpjuj.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xgdxejwf.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qcjnqvqx.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2orpukmuh.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2igdvxlrm.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2lfjgbvhl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2jdurpyac.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2duexhigi.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2rycmjasq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2obfkoada.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2yaqwettk.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2wfmhxhjr.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2takoqdci.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2sztwlgju.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2zehrknow.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2pdjnplmd.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2sgpivlwg.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2brdladcd.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2rnlnjcvm.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2fzophdho.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2oqlyiega.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yxhenvwj.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2sfkslsym.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2tcshlmnx.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2ywqtakjd.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2vxtikkze.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2mkggqwep.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2zocuidek.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2amyjnygc.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2mjpzdhug.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hrtiybvd.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2gfjvipqf.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2zswdmgtq.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2gsglzekp.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2wgfnhswi.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2mayeyhix.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2tmdtblks.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jowxloos.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2apmmirsb.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2khpbzszs.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2gdesvnog.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2dcykhwfc.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2tsdefywj.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2dvhfdwur.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ddcmaktv.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2jmmxuppk.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2psnynuvy.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2engkfjvi.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2tbcmuwmk.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2ytpujfmb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2eoyjviaw.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2xpkihamw.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2tcqxgzpk.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2laigigok.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2vejhdepm.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2zcvlmtwr.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2ydxtload.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ljkfoxbj.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2icthndji.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2nsxarmts.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rrcfidfx.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2yocmhvph.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2jifezpht.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mrvlacdh.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2mcipwzcw.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2kkwbythn.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2fzqewjpr.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2hvuuxgrp.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2qhghawim.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2dsrmfjgv.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2wntoqvky.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2xnyboaax.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2mjinesox.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2obhloinp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2isgjfhxb.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2fbwezsik.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2wzzauybn.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2mxwahlgu.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2xxckyvqr.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2qifpqpqr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2irpynxiq.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2peiveeqt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2lvujfftk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2lefxupft.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2vicllbdv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2pjsdygrx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2oyibzgcs.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2bvkfbvqc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2vrarakre.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hlzamykx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2iphospwc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zsayycuw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2gzbtynbu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2yndkfxui.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2eifvzrgo.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ejekynpl.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2pgajfwxn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2emmtivej.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2lsjduuwo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2hfoshdmg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2unketobm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2jygaarlc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2jnlgeczo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2gujwqozp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bliratoo.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2aqgfthpj.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2trxdcbvp.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2exbaxijb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2fxourefo.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2ctmhkchj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2hghijvyi.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2ssqdhcsy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2omgclkrx.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2zgajyggn.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2oimlwuei.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2nccbnfcy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pccshuwd.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2sbvgkvhr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2shqkfiwb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2npwajbke.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2vjvovlqs.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2pliapbel.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2jjvzdjsp.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2erzzmbzp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2fjiotxcc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2vgojkfdg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2nnosnqrs.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2uucjuwjx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fuaupdqn.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2lckisiom.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2qbbewytv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2jqmyojbg.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2cldarcyr.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2exlqvxwb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2mlroleec.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2lxpliadn.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2cxmabtul.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2krddggct.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2smsuylpu.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2bogsvkuy.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2fpvvtuvr.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2oxwlosya.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2jbdfhazk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2bjfqfzdb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xknvsbtw.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2ncbjbhgo.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2zukcjrtd.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2rmepqaoi.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2jmbbrknq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2rihlmrqd.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2oszhgcnh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2pwqbfnmc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2kcrfkkim.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2epuddibi.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2otvxpuxv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jvwguqoh.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2swmunkno.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2umlokgsm.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2inyxirfa.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2pgbehzrn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2exisdaie.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2sxuwzald.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2yugipugu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2prvphjne.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2amlaouws.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2dfnuzcyl.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2bkmvkgap.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2qitfkwmy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hptsivep.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2dhtigtmg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nfqfjizy.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2xxrzgpkh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2xcposrxk.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qjgvdbws.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2esalgief.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2tdlzhagj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2xfyiamgm.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2vnskxiig.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qvldbfov.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mgcpdglx.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2chogtqog.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2zopmbxwv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2judnrclt.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2wmornzbd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cmzhjpzb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2byuyytqo.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2qvumjrmn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2kxejzqcd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2cxnfackt.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2mjlqcpyy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2ctnpzeao.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2btdxwgrw.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2gqrmgwap.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2plvmynfl.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2gcqfvazl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2hpdhyzrf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2nhkhzvsz.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2neooqjdi.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2hzofxwqf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2sbtvuwee.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2rssiovcm.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2jnbcmntl.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2rdgxyzxm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2pruttuui.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2mvlfcrkj.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2jnjdqnzr.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2vdwlwsma.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jmifzthz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2wjtijwul.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2yvhqimxb.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2leyijbyf.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dpqvqpxs.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ailukurl.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2ohscfbai.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bfbijvsj.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yqvdnfwu.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2pbzkuibt.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tsizrsvg.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2pqywvlgm.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qtgnsjop.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lrddpmrb.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2kuhonxao.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wlzwqsam.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wabidtcd.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zsnaxljo.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2ldlziwhg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2cxdmomgn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2ocfhyzdd.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2xccafnhm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2syatgenm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2vdcjoece.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2olbquvck.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2fhzsmzmx.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt2msvxtcnm.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2tsegykwg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2lknxhqvu.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2mkwytilc.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2bplpchsv.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2gaseegbh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2nswzdurm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2hugrjfkq.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wftimzeu.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2dhsolzgi.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2kljieaqr.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jingcphr.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2owbccjux.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2wzmxrnkc.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2zgwiwdpo.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2vxdzvdih.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2ztbgyyao.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2epkjxjia.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2igrzjhto.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2zyrqiaht.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cugnnrco.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2fdqldljk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wchnugig.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ytlallmc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2ahvbequp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wbehukeg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2prxknvej.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xuxerjmu.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2qohbjqbk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qjatacjk.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cauaylqy.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2whvbctfw.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2twptoiwt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2olxmunjx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2olgbhobp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ylmgwxiq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2uqgtimor.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2lsellitt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2ovdpqhyd.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2vtlooiww.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2sxqhbovo.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2nvhfwcce.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2eqigupnt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2xbvxwvwb.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2alhanuwi.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2twlaglwh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bsdbsiml.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2goyesecw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2glvijtym.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2zlizkkje.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2lpbbonar.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2msotozuy.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2udfjvewh.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2cfphjrei.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2mfypnknh.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2fdkwyxar.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2gelqzejb.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tudnvmpz.html


<!-- 参考信息 -->