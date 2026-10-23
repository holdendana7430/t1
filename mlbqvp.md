代发 wailian999

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt3dzhbyvmk.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3xxwcwfso.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rprnmvjp.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3egtsmxof.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3ghyetqqy.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3fadziosi.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3nflhwrgl.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3hkvixwxb.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3muldpisb.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3rschaqkp.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3kqvjpbim.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3oholpbvm.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3vrrxfpyo.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3qtgfzalt.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt3vivuefmf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3sthnnnfc.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3pjhwexem.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3kuvpmqou.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3rdbqgcjk.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3pkgctuce.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lkpimucf.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3oytaugyt.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3xvgqiqxu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3diilrsrw.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3awumoipp.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3sgrrhdcj.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3abbsvcrc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3cnbksiom.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3vonyvkpa.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3gulqvsbq.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3amflafhk.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3hhdyciov.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3cosfzwfm.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3fslrxzmh.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3lyitikgs.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3cqvokemn.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3lipfggsh.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3fuqgnatg.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3yiwgelwj.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3ribxoetz.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3odntzouv.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3uphddbhs.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3wcyzbmop.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3wejhexxf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3morsufuz.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3rvilmcee.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3ytqtbxdi.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3adgpzcyo.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3taogmwpp.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3crhujseh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3teowetzf.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3rxesxiri.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3zbnkyqsa.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3rbqwooks.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3wewwpcrt.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3iobtqbvg.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3wiqoxjyb.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3wwayashu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3pqhpcchq.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3tlmemgqz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3edsfdwyb.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3othinumr.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3ghfxpcvr.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3cpowwsrf.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3sombsssa.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3tsbozqjl.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3fzaoqrsh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3lfegzegg.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3yktsaprk.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3niyutxxx.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3inlgfdjf.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3swcmfybv.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3zzjmpggk.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3szdepuou.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3xrhfxqtk.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3ccplxpfm.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3toffxcbb.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3wfrgcnpr.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3gmhushej.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3ruqqtgsp.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3xdpsicmj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3mysitzuc.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3ntedrmog.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3btadagmi.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3gzpsjjmk.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3vuyjssvb.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3ccjfzocq.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3meumrrdh.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3emacfazt.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3ccyxekvt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pczpwooo.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt3mhvmjdnl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rwzhixlx.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3rqdpllkg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3lyjlusza.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3eedbzojh.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3nsefpfof.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3pibuzvpg.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3hbdohtiy.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3wijcsqin.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jrejrzci.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3qetbfesu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3lqfrmddy.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3bqrmdizs.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3ftjmduci.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3lkqranpu.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3ehnwiend.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3vdmkjqtn.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3kcftxhhk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3sbdgekrg.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3exqnhiqo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3lwrdaiox.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3fgwyeitw.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3tfujwbcr.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3wijobzjq.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3xrvwvhzv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3znxhecwc.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3pcdsuxqd.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3izlyrpdv.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3yxnifhwa.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3tuiklfxh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3idwkszgd.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3gpyexoya.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3swgkorvq.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3gvevgqeq.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt3iiynfgjg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3estgqapo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jofqjypr.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3kppplhdi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3xmbetfru.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3rrxysmge.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3oyceewhp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3bdkytuhh.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3agunfocr.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3jubzgxht.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3gbbhlqtu.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3hhgzlzqc.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3wycxeylr.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3ajrqqblo.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt3prvxlrft.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3qsljmofz.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3ipnawcyq.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3eeknprwu.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3eoitdpzu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3xxigjnvj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mthladyo.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3jgbciixg.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3hxspcrqn.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3ocadnnuh.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3qijheugv.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3qquikmes.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3fbleqftf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3hpxoduji.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3bsrbaiqa.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ybrrajih.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3bwtsbbvt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hxwaqhuk.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3uyntvhvy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jqsahpak.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3jpgdfpjo.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3yndhpink.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3clyubxdi.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3bdhuodtg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3spaidcxg.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ypnrfens.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3zgokonks.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3qrhgfwwt.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vwlmqzsz.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3erdtdfem.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xocopxlc.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3xenhuezd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xcentpcw.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3qvcskvsf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3zgifjmet.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3dzlqyjnl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3kngpnenn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3futnemcu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3tcievygw.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3llotpiqd.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3tmvyvtax.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3tqhzgdge.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3ekooklno.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3ssdurpno.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3bidbnrnd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3eozqpxci.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3lptaiiue.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3enyawkti.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3wvfcanuu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3ogzprouv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3sgsvdpje.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3wuudnmlf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3wistetwf.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3fycgzzxp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ghluvutw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3qoaztgix.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3cepcmrvk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3jjubgcpl.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3pqjjmrgx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3myhjykoq.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3bzatcpnp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3cubjepaz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3piamaojt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3imamjysz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3wdbeltie.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt3gfxaxdnl.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dlnjgenm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3mkfkyhxx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3gnpnarxc.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt3jstwvhps.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3lfyndxdk.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ynjcvuqb.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lruwneya.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lhapfkib.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3wtqsoano.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3berlovvb.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3phibvtgw.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wccaxbjc.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3kizozqnr.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jmrstfhe.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3yvgifomn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ykazzycm.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3psdhzsob.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3zlkgtsqk.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nwbjbbka.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3prfqbngg.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3efbpslqc.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3cthuassu.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3idfttvvv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3jsqpnnsl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3rmpmerra.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3ypdlzums.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3awuthttg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3qvywqdxh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3jpsjzslp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3azxgslwn.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3weunjuel.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3bvmogvdq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3eyqnpxam.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3kiijtvsn.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3peqmssvv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3xrcnalal.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3qrfrqnfv.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3fgwniltk.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3ezlbaffo.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3fxctljyh.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yifyzrri.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tsmlkpxn.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3iaczpxff.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3jamjvrmg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3pzzwyrnx.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3krtlbftc.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jovaseby.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3txusclim.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3xqfucngg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jxmvcwfl.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ecurfuxd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3pvushnjn.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3airaclzq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3vzkekvgq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3plaqorvj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3axjtygvn.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3duadbubv.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3xvtjjjhb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3kdajbrgs.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3lfljziwl.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3xhahtkkh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jiygzezx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ehfdqrcd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3clvncyur.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3dmqcvvag.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt3vveooaei.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3whhxraaq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3rtfonqpy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3sgjfsrfc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3asdtwgso.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3nazlyatq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3mzndwchi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3lryefeli.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3yczidlkc.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3fzjgxgvx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uyqrmykz.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3ooidpxpf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lgpjlgtn.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3iyguerwn.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3zwobsejv.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3pwjpefpx.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3vdkoevbm.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3pjhauopo.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3lkewnfcx.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3vqdkkrtz.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3wdvhytag.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hhkrswqx.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3siaszdvf.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3qlwtmyun.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tmvebakd.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3zpkwyyak.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3vquaatbw.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wlmrxgrf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3ztawnrvu.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3osiqydjy.html


<!-- 参考信息 -->