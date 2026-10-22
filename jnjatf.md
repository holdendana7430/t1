代发 wailian999

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tgubuutt.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2lydnycjn.html

PHP:  str_repeat("ab", 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yrxkvpzq.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2opwfkcqw.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2zwxiavzi.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wjuocvom.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2cdnyjegb.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2xccdunqj.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2lymfxebb.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2opgagoxy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2hrcltevq.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2cxccymka.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2ojgdrsxi.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2qsamjxtd.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2jfmmfbik.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2thsqaqpl.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2hkfjtasj.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2oagysqgc.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2ldgmkbsm.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2vkshrese.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2lreiaasr.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2edvekghb.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2gcfzbnfo.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2pmkntaqz.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2esgwsdlp.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2qceciass.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2fjeuybdr.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2gxodeujt.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2jqmdvkqo.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2zyxixofw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2askjydag.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2tkgjmsjr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2mwtuorjo.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2rjffadxw.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2pjxjzvyv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2tlxkhubk.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2vdrvvndp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2dxaosmfw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2afediwje.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wfaphlvx.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2gorqkzng.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2xkejqqkp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2zzfqqzmg.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ouqqzwfl.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jkynlcne.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2amudvphb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2mbxaxdwe.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2odthbbpz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2bwazfcoj.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2hitaghhk.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2nvujbyul.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2mmdjlrql.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2uznkwntp.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2kvmqncqm.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2panugnxt.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2sijdgvge.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2bcledrcp.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ugzgaozj.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ooopimbz.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2pxbvwrhf.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2dsgdopoe.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ovjlgqjp.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2kyoiikui.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2fybhkvrg.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2yfjfqxyh.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2jfrlvtnq.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2cgkwzgqg.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2wcdkxura.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2raepjmjy.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2obvwnbye.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2hekaguji.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2xaebgkzl.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2sbniekic.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2tmnavlht.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2deoooamt.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2oehujyhe.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2cttprniz.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2ppekqutr.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2cmffjsxr.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2glngbmap.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2exooarrd.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2vuekondh.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2numeyuma.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2gkcwbazt.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2llynofhf.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2bpelhisv.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2yehgsubt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2iixcnjlz.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2kvqnewye.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2wyohtjjd.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2jsapsqll.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2hudocpnb.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2zixbwghk.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2fjdrxfsm.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2eoizhsoe.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2emkxznfp.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2dvdfcrvh.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ocuplbbi.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2cmtsisty.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2ibdnegrc.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2tbpbdpcs.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2yrmgzyxn.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jfvjbaiz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2ptwxxidn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2crjpdyem.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2ugszzjkl.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2wwfoeboa.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2gvoirlan.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2wnlwsrhf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2vlmbfasi.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2vfcciizn.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2mbldicxj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gcjthvhw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2zshjcsqb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2ezkoodol.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2frrfbhox.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2fcyfltbc.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2tabaield.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nfuatszm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ucwrqigj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2whthjjgu.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2utasdnng.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2xrnvdbgl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xfltlxni.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2jukchonm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2eecicjnk.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2aaiojmfa.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2opwybhxy.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2ccqvhvky.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2vscoveds.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2cypbvrri.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2zabaetti.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2cptzosqv.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2bnatzmym.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2rlemhcrf.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2datbgrqa.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2dsruldfs.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2nicwvpom.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2xhukfyzt.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hfnpbugz.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vsovvtqt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2sasvvowd.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2cvaxzmfo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2ryvwdfdp.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2oppgojgq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2wngehzue.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2mbkuztoy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2rwvfjedl.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2jlavcrfe.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2lsdrjgsa.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2yrmtbzyr.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2zosszesz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2jxztefuv.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2edgvsgpq.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2xhqapura.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2mhsrghkp.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2fjtttuwt.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2hfewkcww.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2gypyegch.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2egrzqcby.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2ranrfngx.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2ixwgqfhv.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2qjsutict.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2ycfthgzj.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2fbxoskvd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2edukjomw.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2hctytquo.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mcvlpure.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2inhftrvu.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2leuyltiu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2owfrvhkd.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2lnpkoraq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2fixzpzks.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vbdswyru.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2riacgnfo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2wrbhfpye.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jthuffef.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2iohckuta.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zprkngnl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qhmwsmkv.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2llzyyxvu.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2umkmhbsb.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2sgucztse.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2vebazwxr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2goegjfga.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2wogmjbcf.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2jjhhzrqh.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2nqysrxwj.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ghvfcdaz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nqxzdnig.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2ptoosnja.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2psgysrmf.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2vyodhqwg.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2vgcwxmje.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2tbxnkvao.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2owxxeacv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2vdriinjr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wfoasqxg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2xwtinwor.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2juorrsfq.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tturadvc.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2pylevvte.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2futsuymj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2ibooezbw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2epwwxkoz.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2eojgbbic.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2vhfeousq.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2ybemlmtt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2sradezai.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2iftrtszb.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2cuvjjkez.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2vlqyrsct.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2bygkcxfx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ywibdzbz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2ekixwygg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2fohuvmwu.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2cpubysqn.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2tygyeybc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2qgnzyqgj.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2ogievvri.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2kubcryar.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2jdakwtcl.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2cambjevr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2tmfhtibm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2hosppbme.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rdcnojiq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2dlctgbdm.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2jnioxhjh.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2oikjqirm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2zheufhiq.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dlcpuqdn.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vvkpjfze.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2etzqlwqu.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2mssuvosa.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2bqmigasd.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zuddqasa.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zbtoqljo.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2xjxfnxti.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2umgchvki.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ckntvvng.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hialghkn.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nvopjvmd.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2yhoprsvl.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2wimukxlv.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rntjlmey.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2njfprusx.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2clwjrqqp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2glufgwyf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2rrrulxlr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2qwejutgm.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2znolnluh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2wllgrezy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2emlitjgq.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2leesybnv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2qsuraezw.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2audarmam.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2xumzjisx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2ynziaajr.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2uioletpe.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2kfmiabgs.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2tsetrohs.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mcgmlwyz.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2sgfmvidy.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2qvnkwjoe.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2pclxmqzw.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fcxxzkaa.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fixnumkl.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2flllmzqc.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2hdbifoka.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ukbawbmz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2gwvuztod.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hslfqlyx.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2vumlkwvz.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2edyrrpao.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eivhcvia.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2varkzzyq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ggetxfvt.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2cypykqjd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2dzqrzrhh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2drvqamov.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2edvkxiya.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2umcawqdb.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2hmetnioq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xvntflyh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2tbyvjbta.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2muvefsgm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2irqbwnfk.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2tflcubdp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2qnokdwnz.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pdxrcpjb.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2xqzycfna.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2zlronwwy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2ghcifnpe.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2qrojadpf.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2wzibkean.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2yuowgucy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2powihjhn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2zipjxooi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2ibvreknx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2abqekwwx.html


<!-- 参考信息 -->