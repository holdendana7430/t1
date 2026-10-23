代发 wailian999

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt3pgkwyptw.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt3qrtxujae.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3nfmpbuiq.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3rjhvkyih.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3oehbyqet.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt3hnsocprf.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3yavlmpiz.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3hrsfpied.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3kejuwpct.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3vfkppfdq.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3xmnxxapg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3fopijhlz.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3zwkszlls.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3pfdmtzxl.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3epopchxg.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3acwifxef.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3wyftbfon.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3aoynursv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3xxyeymxa.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3rggmejki.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3zdwwgbum.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3ktcifgcs.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3lyoxtclu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3vdcevtrd.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3wujuqupy.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3ippnxdme.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt3dxfhewoh.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3uhiziaxu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt3bpsylafp.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3bgwvnuju.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3dmjejinr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3ymtkwaxz.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3snnemkiw.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3dsxzcgni.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3yklvhtdc.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3inpmpqey.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt3mirglzvu.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3txlxhfqh.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3vjgtvbcc.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3ititcrbx.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3drbmsnco.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3jlgnxnhe.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt3xovbntls.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3qsnuqoca.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3worayztu.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3giylcccj.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3pjtatojc.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3pmatftvq.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3eeslcudk.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3aykqbnar.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3ehjbyzjv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3vjnnddlw.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3zouxfvzv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3twduhvbt.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt3isdeomrg.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3yvtajvcl.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3rrfpzlaf.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3uvcdztyn.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3iuicbmoe.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3iuyuqehs.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ppwvrlsk.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jyzphfzd.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3vvrfglfl.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3nmthfrff.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3gbmycxat.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3amgmuclx.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3dtniusis.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3otvcszfq.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3fhohosnh.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3hfdjcowi.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3abgdhgmm.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3mhglfraa.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3jfsssavd.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3kkwnvudn.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3vknvoeap.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt3vdfzxqnl.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3zajntzdx.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3xqboutpf.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt3egsjhsjs.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3qhstgyjh.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3swwnyhjj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3bhcaevue.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3jytuytfv.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3mhgucist.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3nodulmjf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tljhlmri.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3zetmucsh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3walxokqi.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3vdztrtke.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3zdhrqjgd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3qjeyatvt.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3bsccigcc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3mklnsaub.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3hnvbxnqr.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt3witovunz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3wylaklvz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3flcxzndh.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt3waunggtm.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3hbjampce.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ddpntbcd.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3nlhhsjio.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3wzgnlvpe.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3gzaqclel.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3umpnbqxu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3eybhtota.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3jwmzkany.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3hfnfbvgf.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3vkgdjblg.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3nfqtvvku.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3blynqqpd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3ihbkjuie.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3ugvfoiyy.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3wavmupcj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3dkaeevbm.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3brshenyd.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3rywuimna.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3eeqrpduq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bqmgvxec.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3pwxtwauf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3oxveezvc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3ewypukjr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3ndabzqaf.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3yyotxcpo.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3rkgzedoa.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3rfprjeos.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3jhgjxwxx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3cprtjbme.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3iksmyzsc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3jnlzvkul.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3qbqxfvpz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3whcefuks.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3wksnoicz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3hwprqnmz.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3tlesebaz.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3qafrneok.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3bicegxbb.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3psnyifiq.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3ztmlhylv.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3heasqvvx.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lbwttbtr.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3mhezjort.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3hplyrnoh.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3rvdglmsb.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3lolygyqi.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3gayyajoc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3hrhxmqdc.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3luxzkmam.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3pfmhkqsb.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3zbzvfnrm.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3yvdnnamc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fxndvplf.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3zojvxlgj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3ghpqdife.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3ljhbecos.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3vzmfuwrn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rankypaz.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nfpdjmpb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3uyeosimp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3rcwubzbo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3icldhvsb.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt3dgrqomij.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3nawshcvw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3vjstpvhc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3htyintuq.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vmqszwdi.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt3hyspxwmw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3tfcgseuo.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3foxqorkn.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3hdnuythl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yjxubdjn.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3zfvkanru.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nqdsbhsf.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt3umifmjez.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3gvmzpkex.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3nqbmajst.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3bzwwvjlw.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3stfbzayu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3uxtykfzt.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3zskmhkdw.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zcoxvjsf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3zwgnatwh.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3eooopeit.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3ldgmyjbg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3mlxdxuey.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fsghbahx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3szdkoczp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3ykjafxxd.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3sncbpuqf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3zvvxecap.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3xjtquykn.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3sclzwmst.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3mhjfcaod.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3zpdikdma.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3elwvvdgq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3zqvzstfy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3tulojtqq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3bonaizqd.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3pfnzbwmi.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3penufphq.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3fqgehyjt.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt3gpbvannb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt3bqhdiilt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3vpqopyik.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3jksdeqbs.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3dikixtxg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jzrhadqi.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3xngbcrep.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3vrqeiqeo.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3drzjkamx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt3kehqicbb.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3qooqsooo.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3qapwnmbr.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kcecouqw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gloufbkv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3soixfobt.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uaignmej.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vcobbhuz.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3qbemwsmo.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ntjmflfu.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hoyhwsqa.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dxotshkq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3peauqmlq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3vguytyva.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3pnmacsmq.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nzznasgg.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3rhlcuwlr.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3kwxqshcx.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3jjzszwrf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3fvheujce.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3cnqgyuag.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3wjuptuas.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3uxnikprv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3oxwowadp.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3agahmijq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3vilcucoz.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3qfmrspso.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3pkpzljoj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3ymzdhplp.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3yousfswa.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3eflevypk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3wusauxdh.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qhazumxf.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3uxphgdkl.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xhrtuxdd.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3cjodtxwl.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ebwizqpd.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3swkwnzzu.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3zoqygllg.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3uqbqwxss.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lrjeggns.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3lkavrydl.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bbbamkze.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt3swxppluy.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3eythmiav.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nuqzszmr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3wwpkzjth.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3umllgdjs.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nbflvgpd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3voqorcle.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bpraovri.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sblxtkkt.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mtxbbook.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3gavdvfkn.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3gdoixsba.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3kscmehtx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3itgctkfn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3ywwdfjcw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt3padfpoee.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3qoibpsmo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3whpxkdgh.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3hhukmggi.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3mpvbqbdy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3ixrxgnav.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3etpungoz.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3lfwsdyco.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt3qmfndklr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3srfcdvqx.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3kzoqjeqx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3zubniaqf.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3yjinhmxs.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hoiwpnwa.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3cvtrtayy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yljlzxgj.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3ipclypzf.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt3konviyqt.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3tmrnabvm.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3gnkospet.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3xfkoqvof.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3pilepssr.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3azksgerx.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt3puhvvphy.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3pizlkzdi.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3kqgtaize.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3rakourbk.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3nzizjmsi.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3sddzkwzf.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3zabdbexu.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3lbkjxepj.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt3gfosgrhq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3ldhkrehh.html


<!-- 参考信息 -->