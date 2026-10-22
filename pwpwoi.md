代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2ihipsmmv.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2fjhwcldx.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2masvpicl.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2nttskimq.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2nkholpec.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2sjhtexbm.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2xrxfveom.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2pmhwfcjw.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2bxsiowpm.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2zllquywm.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2ftgapjta.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2qngcnltq.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2iadfqbne.html

Java: "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ljozgskx.html

Go:   strings.Repeat("ab", 3)
来源：http://www.ydjk.org.cn/Article/details/gt2pdpcdznc.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2muueegao.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.ydjk.org.cn/Article/details/gt2etlcoytd.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2wqwbugfo.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2spdwryrn.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2gtolokhs.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2dhjiejrm.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2vodfayte.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2pabnnktx.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ddrnajzd.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2kdtkmfrf.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2zpbmiubp.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2svwdbrac.html

Py:   s.find("x");  s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2oqvokewu.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2fjlgzlbq.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2oklmzuyn.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2dkipgvpd.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2giyaimwu.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2thceisce.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2xiohybmr.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nhtgvoif.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2racuiizz.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pruzdkmp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2faextumu.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2xsnmzueb.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2cidrvtaw.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2uyxqsxld.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2uyorxuju.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2gptvjlqw.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2isqmubuv.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2oqwsvrwq.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2osnlhvdn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2umfyjtsq.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2lwcwxlqo.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2jmolukiq.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xuyyrgld.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2szxnttzz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ahvihfvp.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2tumzzqyo.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2lkmjawbt.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2tzxunowj.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2tqgabmum.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2atrbqnvk.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2vrhxfhcf.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2mavqykhg.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2fwanrdfz.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2xmnxgwnv.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2qixmtdbx.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2mjprpbab.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2nrzxyglc.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2lbgxvkvz.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2mvnczyka.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ltesqqoi.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2cpgfyujy.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2eyyszccv.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2elfnugag.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2wpqjfumw.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2bgkpuedc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2qydqnmat.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2qtnmafjb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2hpgsixgi.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2vshzxvcr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2mnddqpma.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2tcpnvdrm.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2bycyotvf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2sszkitcu.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2brkqtqxg.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2gzlohkbw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2tethyche.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2swxffpwf.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2cueozfum.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2wkjiqcqx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2kgbgxlsc.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2jywczskq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2bicmihbp.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2fzlomoqf.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2serimhfg.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2hoqocvnw.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2hcfgatap.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2gvywmgbf.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2nhtkrxcq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2vyrtrfmn.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2grlnpeui.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2pxtdfcrj.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2fioermdb.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2tmlrsgwa.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2maepjhse.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2yrqjlvdz.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2kbrvwqqe.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2qmsqojuz.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2ehzyimtg.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fuduyqze.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2rhpnpsah.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dchzoxqm.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2ginsktxs.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2grxdhrte.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hiftmvem.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ctztflov.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jzoaiikq.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2cfvskkpb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2czdrmmkm.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2doqrkwiw.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2bdtvxeyh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2aafoyxss.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2asvfmsyj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2jltreblc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2lyjvshje.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qbnxxmop.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2uimxklbh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2zfhrqhtz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2aoaipgec.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2jbktbsld.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pepisfbk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2etolkano.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2wzjznolr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2fepzsxjj.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2sfyghtop.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2herppcsa.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2tkhijkzk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2rnymzowi.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2gotheget.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2brzprvsu.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2eyfblnfq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2kfrbhhmw.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2hkrsagvb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2mziggwym.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2vadnolsj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2nasmkvbg.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2swabksam.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2iskcjahh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2fprjdegp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2ylgzfhmy.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lhtwcgrt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2etkkjveo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2mxovefbb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2eqzczfnd.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2skcgaamz.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2hcfglzdr.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2icbkhgtc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2mvukbwbx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2njdsxnlk.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wszitsav.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2eajbugur.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wthgexja.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2pyobnmwq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2dsezkzke.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2dnpuujbm.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2hzeubhaa.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2csncucri.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2fecmqias.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2tvpivrmf.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2owjeayxg.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2qlthyvmy.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pvxakvut.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2xeillskq.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2mcqpjmvw.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2yhwyrkky.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2kpufgevu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2ehcvjzvz.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2bhqtzxbh.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2lzqvcxct.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2rxpesski.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2hqksclhb.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2emcjndqb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mqtutrfs.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2rxhgnlxt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2xpclttei.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2ekovxybz.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2hmpfswxa.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2sksytmbs.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2fhvrvkte.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2gfitemsv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jelvlcmc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ofjlrarv.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2tjcgryrn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2nqorxceb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2rrplzpup.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2equmhvhq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wgkahcth.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2onitwsgh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2dvobnymy.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2qmlvyqcq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ygibiler.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qgswkled.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2xwwnprlv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2spevrywm.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2pyhxlwmj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2uirabvit.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2jjyzldze.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2dnshamlp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ecjmaknc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2txwlvnic.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2wqrxzibn.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2azjthfnh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2wykvdrzj.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2bfsspsoi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2dqkhbmyv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2sssiborc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2kwvoinyp.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ruxeisin.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2xllyhyoq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2ekcgzvyq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2efqnpdye.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2tgkphlcj.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2bcjplybj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2qrvoswag.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2uzuyobam.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2mkppnlid.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ismugwxv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2ehsejauh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2gtvboenn.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2uaksevfc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2jjkjirot.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2kljggnrm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2qhmlhacu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2kjjlspru.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2exxamrpr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2gsttseub.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2cdxssppq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2nshlnpyr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2tgecnjms.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2mqdmecjl.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2wspigymh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2qpkfpumc.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qccajdwd.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jlfvladu.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2sizjtdmu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2jixvaxgo.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2gznmaxsy.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zxumnumz.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nhfhrqat.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2ekgizmnh.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2edcpougi.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nyuvhbrc.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ptcjlcfb.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vvkavmxw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2sqlzpmot.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kjicefum.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hpwmrnyy.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lvcoemso.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2akosszab.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2uklktjfn.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2zswzhwrx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2zmxymcnu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2dxytcvpu.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2tvsvyzsm.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2eocoafmn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2pndiamyi.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2eaubchqk.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2oonauiqh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2iiszmogf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2xagemijj.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xuwwslln.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2ddpuyywb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2olpwwxof.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2fwjnruie.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2vhckfmbl.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2xuutbqji.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2podmzcgv.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ehbgdlkp.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2qpgbqwyx.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2ezuubhvg.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2oquretvt.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ipwuqgsx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2htrobbdd.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ltmcxhsw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2vopgwnqg.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2fckqwrzo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2uoiqfkiu.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mjmhrdqu.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2reidorug.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jdpdtcnk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2zkjyuohb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nrptknme.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hqioldss.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yevdqwxe.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2anupjeso.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nmhbgsjd.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ahbgostb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2urbrhymz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2omhkdnex.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2dkqqkbzm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2iqvjjkox.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2gxqriynz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2ljafykwz.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2zwbiqmex.html


<!-- 参考信息 -->