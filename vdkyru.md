代发 wailian999

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3kfmwyfbm.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3bfkbscek.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3cazlxwul.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3tfaqusmg.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3ufepuvte.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3mihsxpez.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3zvkyrnwm.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt3ayhioctn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3jrblhlub.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3ucxqvpkt.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3doltretp.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3udqjveaj.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3bcthaobk.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt3ptduejoa.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3dgwahwpo.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3arpplysk.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt3uchrrciy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3pfrkrvhw.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3zryovjpp.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3gifoefyu.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xynxcqdt.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wmvgpvao.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3obvzwxip.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3putuzwmn.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3lsrovrob.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3qefsplah.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3woyzarlt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3wyvxxhfz.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3lvzycifm.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt3fcrfvopx.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3jpegxcxo.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3vtwsizff.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3hyefldwu.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3aadrclis.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3onnomzzm.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3gbtqmzzk.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3hvjliubi.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3uheudyto.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3tozolnfv.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3iddascwl.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3nzdazwcq.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3fyjjahkj.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3kylhywjl.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3feyxwgfq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3zkmnvfpc.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3xnruxmam.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3uobufczy.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3xufqzpfw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3akmkmfzm.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3uwbslqel.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3hftkowww.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3lbyidfct.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3qorneuwq.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3xedoesdn.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3lgoepphx.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3fqhlftee.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3hidxiwnl.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3dfmvgvsk.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3lstoahor.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3aytezltf.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt3lpuzwjce.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3awhvyhzv.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3rrsvhwun.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3sdulnayy.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3ihmntkgf.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3mukssgwi.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3wetuwrhp.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3tdeqrnno.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt3kackfzjm.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3opihnefh.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3njkpxpys.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3osarmrmr.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3sshvdgro.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3gpjswyxl.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3unebmcel.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3aetuwsij.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3ysyuzxag.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ouorjmom.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3urpclaov.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3wndyawrt.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3fcnsjjpu.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt3uybamica.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3jugyvvrg.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3grlyfwuk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3izjmzbtl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3ueciwayg.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3nlxwodun.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3bfxixejf.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3xquolmer.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3onhwepii.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3vepghikj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3cicmtwzd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jeqehszv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3rxduqejg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3cnqjdibc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3tyzwfsfw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3cfocojqh.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3zquboetx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3aqdyuogs.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3qchstgba.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3snjoswdo.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3ovlfypso.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3sjzeegdb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3ghsexdhr.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3akfjquey.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3jqidiuwr.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3xupqqdos.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3cudvfgly.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3bbiviphe.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3cjqxfafu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3yowaqkpv.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ofomvlqt.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt3qonvwoij.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3fwjjiskf.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3lejncryy.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3ubuuzewk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3oodedmcy.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3kvuetemk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3zxldvozh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3vbqwtgns.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3nrrxuqqo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3xeuknsbp.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3cmbiemrh.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3dfkpsrds.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3wwdumuyw.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3puvkbpze.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3cysutxmo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3hwxnevyj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3irulbnec.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3silftqpt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3vnofczfy.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3zeeusyfo.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3jezcyedl.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3hklfmvxv.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3nlrwlseb.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3dlyaungr.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3znnrgrvy.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3qpzqjhnt.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3aogyzcsm.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3etzkvwxp.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3wmbddekj.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3sbxwsqvy.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3lblnjjlv.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3qfreatva.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3dvuxsqct.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3cgyuggzx.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3zhnndjcg.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ytcuplln.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3skphvdbt.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3jxvzmqmm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3jykkmnax.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3zuxrrrke.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3cvxxhojf.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3fnbxtnmm.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3cyesnsbq.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ecmvhhfw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3rscpnjzq.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3uixwwvik.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3hkpzchsy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3zskvsosj.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3qofhwmds.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fhuuprso.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vqvvtusd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3vctulztp.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3xabpwphz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3vqrbnqhv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3icwgeixk.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3ukwtmibe.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3pkgszpgm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qagdbvyb.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3nsjlmxcs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qkokbcfq.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3knrdnbiy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3vkmgzlzy.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xthdmgnn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3jjvsnnof.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3andegxvr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3alnwbklz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3dpzpmmzi.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3anupidvf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3kxbznuik.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3hsvaqqqq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt3gfvcayfp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3iyikxraw.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3cpwphqtt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ghajxhse.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ioilgode.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3jaewlnia.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3fazejqxf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3momqfypu.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3sbqyhwne.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3qqhntudw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3nqqmznvi.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3aooklmjm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ezgpzozs.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3vgjnxcyj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3dqlacist.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3elmvdqzu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3zfwbzadi.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3jvwxzqfm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dsyesxko.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3bqjyyjrz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3uqiqxsab.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3fgftfzcw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3gazjykgd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3pwiywuiw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3jvbxjxhe.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3ojjpdusx.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3fjcarame.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3atlasddj.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ybtecfrh.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3offqwmuo.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pvyqtmlk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3sjelboau.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3fnrbfmtv.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3onteycsr.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pkpkmgbg.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3isqmmerh.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sesjpyrw.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ylwgpkly.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zetifrtr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3yoloyhfn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3fnqjzmud.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ibldyatd.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ctxabefu.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3teymaopa.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3beiemlyg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3flpixsjf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3nxepesku.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3mbiajbko.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3wjhljvtr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3ydurutsp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3zezyiscs.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3deknwiww.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3cjmhnton.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3drqjfxdv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3btrbsngr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3grhjgqaw.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3nfxwxyck.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3xbwcehxc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ocwffxqj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qqyiqfpw.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3aehofiys.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3ytfiwkkz.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3duamwmpc.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3azkgvhfa.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3xfcdmluc.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3qquydbee.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3ktqmcvhi.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lnhujzqu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3sfmcotwb.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wokldfvw.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3ckqzaruf.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3qmpqkfwc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sfhhtcih.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3jlmwycdf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zfjnhfzx.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nickuwwm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt3bpzxxcxg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xfnawczm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3bnvpdmlq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rwangqne.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3brkyohjb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ypcahuta.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3twtdxtim.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dgaqmmju.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3axiufxyd.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3gckfsykn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3zjglsxlb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3qmuhzsqs.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3rjrpsnku.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3tdndzbzx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3wmuexkne.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3ufkiqwha.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3hgrheznp.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3sebzvmha.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3mddcozgf.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3hjbgvnfk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3ytjvvnki.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3jamoywgf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pazvaxrj.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3cyzcjmjm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eyoqbpce.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt3plaicoju.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3kwhbxoqp.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3wvlyazxb.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3bxuuzirs.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3wynrqtgl.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3aftnkpqv.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3fdeyberi.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3zmaohnbu.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3alkzyyhm.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3obhsfzmm.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3emfpddzi.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3icdejanr.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ifhmrmgh.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3uehmldny.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3fnjdmgsx.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3qpmzayqi.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3acikdpue.html


<!-- 参考信息 -->