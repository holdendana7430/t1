代发 wailian999

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2ddzfcjqf.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2uvvrdydj.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2nnamokjt.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2midwjadc.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2lrsoqjmf.html

Ruby: s.index("x")
来源：http://www.ydjk.org.cn/Article/details/gt2phoajbjt.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ojdogmum.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2luseuypa.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mlynubqf.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2wtxqknxr.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2zyhoneca.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2byswvemr.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wqclfgql.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2ecyagaec.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2xzmsccpk.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2kngokphe.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2pptqtych.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2hhxgdvdv.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2mipibhhv.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cbwmxufh.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2cjnqblvt.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2alvwhkqp.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2anhpkvvk.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ggdjfwgo.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2deuxcxxa.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2btmtmjcg.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2wjlqcrci.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2vgywapac.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2tbakqber.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2abufnggv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2oiiykcfw.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2zlkbuhqy.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2tykeaetn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2ikcucgnt.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2todkyekt.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2jtqqnqaw.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2ckqrfgay.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2lkxzixyg.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2yrimkkof.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2mwfgyigs.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2hixktpwu.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2kljcfqlg.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2pyfxwpjb.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2wpjayfrv.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2abthdzvg.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2govuicrb.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2obpquqlf.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2mzlxrazm.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ncltcdrf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2hpahokgh.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2mvxyszoi.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2carzctbd.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2rgsoaquz.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2ohqheweg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2ejobjtak.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2plgmdlwq.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2qlsdefez.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2xkblnafv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2snmjlpnh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2sekbdmbw.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2lrlupajd.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2khwrjmql.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2gjkybbsv.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pveyxvxe.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2cfzxfrwm.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2yovydmjy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2wyajzpdo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2msbceplo.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2kzzddcel.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2qlkauguu.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2eatqbame.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2afdqbsxq.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2ehhhnpld.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2hxrezjyr.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2dumowhhx.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2boetcwrt.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2lefwvjzk.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2kefoyoxn.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2oapedwjc.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2sgrmcqrr.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2wdofcnjw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2yjgegxba.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2wlektwst.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2dvqdvuzi.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hxaonabm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2xmmhcobk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2rbxegkbd.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2xxzumtzo.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2evwibyrh.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2atfzptrt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2rrsdgzmj.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2hcnjmmle.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2olgjnzbj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qxblhrba.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2rwvlfdpg.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2dhbjkyxx.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2ihdqdgpb.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2xklhuxii.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2hicnjqgf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2uedrppeh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt2ckpadfqw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2rwmgektc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2ijakhwup.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gsjommsl.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rphdwzrg.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xtibsqys.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2xntjxdbt.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2sirdwhlg.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2czbfukvg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2mvnmwjmf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2xwqpxgyg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2lxwvnjai.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2nbdeebbd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xpptlbgx.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2pvusnfnp.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2uosxfeus.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2efgvwuaf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2kvpjqsyz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2vqgxztnf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2xztincyw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2qqsvsqlt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2qgiyxhnz.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2dhroubwy.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2qnebzmjj.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2leblpukt.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2tdjftaof.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2pjuffxhb.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2tnqwybhb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2rcxfcaor.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2pfddtmvs.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2qcgcibgv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2iubwnabq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2ulzovfvy.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2nmizcvii.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2abacbbce.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2hljvexma.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2capuwgmw.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2mfcchfdt.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2nprchpsa.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2kjrujqkz.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2awhmjldp.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2gqyjwgcq.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2panxpfob.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2oeluhkxi.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2wmrhbzgo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2aubwwknd.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2urdgdvrz.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2citqiydm.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2hqomtgut.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2eapgnhdb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2oyqkqkua.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2cqydlquz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2ividbyko.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2pjrrmesy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2chtsrqjn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2schsqsdb.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2jimiffyr.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2nuvtyero.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2wvrqndjo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2jsrjjfeq.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2qorjezmj.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2yzkwbpez.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2ariydleo.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2aofwezjk.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2tdsidbra.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2ibqeepys.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2znrtssrv.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2cawrdcwm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2qmhusqpw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rxnyswmg.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2llxykglz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yjcifmwv.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2kjjysmax.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2tgwcfdar.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qjooyvqe.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2ywobwrct.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2gwsgwvvi.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wuxsqvli.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2iegnrzue.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dztsrzod.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ygihkcql.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2blvzpiyi.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2sdqrwooh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2fpbzsupj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2tlvgqbeq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2oxbmnivx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2zyxcjdxl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2nvcubeju.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2tkjijllx.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2gpcfmopo.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2lmougoma.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2pvquoftm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2jiabbkdp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2pnzevzwz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2misezrys.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2djswbpzc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2hhhlehay.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt2lyluaqvk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2rikycvax.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2atgxuvzx.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2fifqlxfw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2rampoqqe.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2gfwhqury.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2heaxtpgs.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2lfyaadcq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ozugacvf.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2fkelriii.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt2drnyvktj.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2cgwpucru.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2pjhvmfwj.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2aoetppoi.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2kfdqscpc.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2blycukhw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2dvepzqcw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2dstdlukd.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cbsiyklo.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2dxccqnvu.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2eldwhgwb.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jqvupwcb.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2inikgchk.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gelydkhr.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hxvnkbih.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2lqqhjhgg.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zqxogfmq.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2trkmsrky.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cyjgasph.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2xilxyukp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2aelfeefw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt2whfymghz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2pavvafco.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2ozeptazw.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2mgsepeuu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2hecnhoop.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2deujgurd.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2ivgceroa.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2iaqxgwpg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2gjrsvgpv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2bcdyhuka.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2xmiddxwr.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2lmcimtyk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2nyfczzoi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ygvfkvfv.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2okwdrduk.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ppiiawrb.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2uvbmofdb.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2prcswxfn.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2kaxewajv.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2kquxwkpv.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2pappitrg.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qdkyhxjn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2xrujnjlp.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ivpjaccj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2vxvczxow.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2plgqhsmz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rtxgvnsn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cwmxdkrd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tqotbazr.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xgehxqkw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2btmrxiwo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zjrhndwo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2alcisikr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2olcznuxx.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2izfdavtt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2eiiuzrus.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2wxcdxhig.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2sbkxhezf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bkmapacq.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2yphvghqd.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2hqabdxmk.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2oedwgyog.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2wgyykvky.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2adakqvqb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2omztngix.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt2csjpocpy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2rtuseqyd.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2inyhutme.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2ccmmndvh.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2blohgifw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2xhnumwgr.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt2soeideej.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2toqbiuqu.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2oybvmmid.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qznvqcbw.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2ydwwbcrp.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2ilklwftf.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2nelbrvld.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2fmgwqjcc.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2tvbkixwn.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2zmwpvbsn.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2hmbiigdv.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2bnuxhdlk.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ejwgwhza.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2zvgeewld.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2rotteoeb.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2tsdnpbyh.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ygmmntgd.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2hnupwxor.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2yboukmyl.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2ltsdhute.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2vtgotyir.html


<!-- 参考信息 -->