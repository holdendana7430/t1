代发 wailian999

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3tgonnazw.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt3preimhlv.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt3hmmwfzee.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt3btnrmjgl.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt3ojepipag.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt3whrwbgsr.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt3prmzwyto.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3xifrzktm.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3mmhztlbv.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt3jnhehhej.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3htkyjxul.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3fvymylix.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3copikojr.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3wjbboyto.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3qmmamgws.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3pqaygudg.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3skqjhhkp.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3wngtjfkq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ikjihbxz.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3gwjpebbe.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3tdbbqane.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3tpjzjxoa.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bibjcpfs.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3hvcmwavx.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3ittfsodp.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3nnruenup.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt3txmhgtrj.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3spfnruev.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3quehootb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3hsbektsl.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3wxkxmjiq.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lmimghoa.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3uyzhnrhv.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3qfboezwf.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3tmekuiea.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3eubriubt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3gfgjkbsj.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3recuqrkc.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3qyskczfh.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3dopkprzx.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3rzqviowm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3kbuleqjo.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3ywkmjfew.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3oawquuew.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3czsshltc.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3swjtntxg.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3npxbitxd.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3iacuoebc.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3wdzihjea.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3soiuzoic.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3wpzyqytu.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3rqraadlp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3copdpliw.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3nfothsmw.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3yatjtljt.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3vxfrscla.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3yldosdtn.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3pxrvmmdr.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3yzhhxnui.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3awquhsyq.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3kedtmcrm.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3qldqieuq.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3ggsernnk.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3blchkacr.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3jcbfnfpd.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3eaefiuwh.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ymutsjmb.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3uqqxjsyz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3czbifnro.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3kznszykw.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3pcbfobbd.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3xgppqtlh.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3oazfgurm.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3fxsrzgyc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3uqebxuwv.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3ifmuwahz.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3bbouzurs.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3dehuijtl.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3lespxpwz.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3owwxtyst.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3qzqllgtp.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3nrrrhkce.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3pabhqgxs.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3fakidnid.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3degwuokr.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3szhshrqk.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3btpiqewy.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3npfklklx.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3cgoixtgv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3btyilnkr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vhlgpnmv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3evcotodc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3pertatox.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3szelysgu.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3skotfqif.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3axfcmbho.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3heftkgeb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3xrshbaxd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3hxaetrzx.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3egyjzobg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3qbcmaagv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3rwztpwea.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3nsuwgnbe.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3vzpnrhre.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3puduxeuk.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3jcfkhktt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3suwifchm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3kjvldvxz.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3ysumbmvg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3agwrxloa.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3rvoodntm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3pcqnpzif.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3etdtofwd.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lqsmbblz.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3cjkqzuxq.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3jdipsbpu.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3moeqzmpw.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3rgcghequ.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3xoszfvdv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt3anhaidno.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3upheyfie.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ivbcvqin.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3rcnzoixp.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3loylacwb.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3glotomcu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3cdsxyjvb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3prpyjgms.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ogcardku.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3tgdralhv.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3dpbzlkoy.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3nmygbyhg.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3txfrbjev.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3dwpdidpb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3zsaobrxs.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3slzqovso.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3kyxqpvvw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3rbuvkual.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3zezpueng.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3eyxklovc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3aifogoas.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3yyhzshlw.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt3vtmgizlz.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3vehpzwxu.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3gxytizau.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3lfnacbmd.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3qhtuvehb.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3pientykc.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3fbxbpmjx.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3thscqwqa.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3vrmrpnda.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3tqmbxffe.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3poveyldd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt3omjeixmv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3zwackwwo.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3bxdtwyed.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3bujbwfdp.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3sahqcgcc.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3qnzzgyfm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3nlqvcyle.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3luavuexu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3heavdqqz.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3xmesuddo.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3stkfmfxt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3czgngtno.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3prkettal.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3vnnlsrhr.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zxgsuror.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3ahckwphi.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3znbcwlgk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3osgmlnsd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3btrnyeoz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3gxgkinud.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3dgalzplj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3jivgoesk.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3bzhroxqo.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3dughjmir.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3ewjyibkp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gmpzzstz.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3mvpfhhbp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3otusdskw.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3vjyqlkyr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3dllkwvgp.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qilgrlof.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3fcdmefry.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3vfsfvviy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3nktqohin.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3tmktprxr.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bweicabb.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3aqluarzs.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3nfpgwmqi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3aqnuuasf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3sltulhfr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3yemqwqdn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ryygqbyv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3qeoqzxur.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3zqunzpnr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3sffwlbsp.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3xfsnwbzc.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3rrhggwvl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3njpdzuss.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3dmauunee.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3whlcfips.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3nucnrcbm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3cfwvdnii.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3ggbnmesi.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3dvhkfkyw.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3woojadym.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3vdnfxzkw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3ixsradyn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3kerakjzh.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3wnhiidfu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3znvhranp.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3ugkvwqbi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3plwpvftg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3aylqqhfy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3oncgunfh.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3rcxasrfm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3eybxtgwx.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3syzuaxnp.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3tbjymwez.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3duzwshws.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3ijjloieg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3qoawwnhe.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3abtfgqha.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rgzrsqwu.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3dpivzjmz.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sejrvtuh.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sqmhwhbq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gooiwrqv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rfaqrmma.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3jaqyxbes.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pvrceqrh.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pyxyaogp.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yqneolln.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3hphynvln.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3umojiart.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3nhvwwkwl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3jbygfzpt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3lbkiabho.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3paxqmupv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3fizmxaxn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3oqgzhsdp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3thzslbtp.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3xhzllgol.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3gdaynipj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3smzwpnwh.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3bacyljay.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3bmcjoqmz.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3fjkpwgjp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xgjwsdzx.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3bzsfgnef.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3lfwghyrv.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3blnlziqy.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ctqlbgsd.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ormgoifg.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3jpagavxm.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3egnbmnss.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3tqwgzknh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3xzwspegd.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gnljbghn.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3jpuzvwxr.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3pgwdjpja.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3deuqnfkb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nzlbueeg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qixecftf.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3afjxzdoh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3tuqowzsr.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3blxjqibf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3olzhhbhg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lempjfpl.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3dqhboheh.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3kudqzxbb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3nezrgctp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3gbffdgjj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kfpgjywt.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3fykqmmyv.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3tjqpgqrg.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ngjaxyyi.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3flylzaps.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3mirtmhmi.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3iwamffjw.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3imwyjjdg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3wijemlxc.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3dormxtoh.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3zgzcamtv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3zbicjojq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3cqletdkx.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3sstnswzb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oqeyjtsj.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3cizpdifu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3osxrgmgu.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3uipyijby.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3iznjbggj.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3xganfcoe.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3wljjjosz.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3yihokldv.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hvpefhfn.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3nlcstbvl.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3ppernrlr.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3rpnijhyw.html


<!-- 参考信息 -->