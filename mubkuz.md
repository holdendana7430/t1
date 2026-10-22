代发 wailian999

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uemxolbl.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2bjsozmlc.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2bwzhpjyl.html

JS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2lllkysbn.html

TS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2ktnkthld.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2wxlcipkf.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2etaeuurm.html

Ruby: "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2aketyghy.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2qycjvbrh.html

[E03] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2zkflurpl.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2mkauiylf.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2hrhzaukt.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2mrjtlpzo.html

TS:   s.slice(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2hbqkahcc.html

Java: s.substring(1, 4)
来源：http://www.ydjk.org.cn/Article/details/gt2cveiooxb.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2jcobpddj.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2rnjqafwf.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2aunanixn.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2urcjyeet.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2vgzshsxo.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2vchiqpew.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2tchdzqzx.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2lzmnmmoe.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2haqjlszs.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2hijaeskl.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2geispmjr.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2uiunrhsn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.ydjk.org.cn/Article/details/gt2grvtnqhc.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2ebbfzjoj.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2krjhttni.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2hexiyhjf.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2tginxwll.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2bktywshe.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt2tvatdbut.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2ljngbkji.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2kikzrfmj.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2czjzmnfb.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2sdopohfn.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2roykgyxy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2gskupctx.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zonnnttg.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2egzqnuhi.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2osnhecnc.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cxmelawb.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2goiepfxu.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2olbkymfl.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2sidwtsot.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2ttbvumpk.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2wjaxogbr.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2mmiieeue.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2qgxyvoea.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rtfnellq.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2gzbkqwdn.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2jmzwbqdh.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2ihtemktm.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2veeunnle.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2seaqtvqv.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2qjgwgoql.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2txhogdaq.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2gckdupjk.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2igiczxcl.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2xxzcubxd.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2xjvwpqrr.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2buctpwvp.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2hoogxiwj.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2kuxtaguu.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2urioyqxs.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2csnnirzw.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2qrmlcrqv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2qojvypfu.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2giacdtpy.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2zgfrwhlm.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2dvlfcfsk.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hambzgfj.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2stdeympo.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2jqxhozfg.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2doghbpri.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2rdobmtxx.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2vpuvmjud.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2voebeihk.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2coynxhht.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt2nwsfdciq.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2veykxfkd.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2dogevfil.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2lkvpvqwk.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2lqhsmaig.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2tiautfyy.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2jgggbdec.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2vghpsywn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2cyzfhknz.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2gjpsxylv.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2lbpedvfe.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2ngwovpie.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2orrkbkcb.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2emkjuslp.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2jtidseuv.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2uscnhvkj.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2bxwiguws.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2lrhebdam.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2kyrmdhek.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2egnoqeav.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2zsxakfad.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2yvhhyjkk.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2zlpvojuh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2dtzduzpy.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2ruloymhk.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2pdoamebo.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2tvkncaaa.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2jsnybekw.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2qqoiukqp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2zgzupoam.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2iucpwrhr.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wltgkzip.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2oqjdbjup.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2upwichlx.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2ctcyppei.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2wchncdwc.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2afewcwza.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2zgcarchw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2wxbzrjoc.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bwxzzdco.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ktecgtvz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2dahsqnwc.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2efelpwsd.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hkbvhset.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2ikauoiwg.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt2ivjhmhlk.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2jbcldywd.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2opgpalrq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2srnwmsua.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2ryfhxxrf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2mpmzyoxr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2ubuztrdy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2svnekwgm.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2lasckawf.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2trviaywj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2rpcnnolb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2mkvcoxec.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rgxanzay.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2nwiwmxzn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2qxtlaknm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2dphoxeej.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt2mjxaasni.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2btgqnbwi.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2zhssqbyi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2ymwupirb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2moakjdiu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qwavcoya.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ljqdmpsq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2wtnwlyec.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2mffrqhbg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2amxjtoah.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2tscxgphz.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2bvanssvz.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2myyceilv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2mohzymkt.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2dumutuom.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2ibpsiyxm.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2bdswlbhy.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2xclirirt.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2ymkhfukn.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2npvldrqa.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2zhxscwun.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2bwcjzkkf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.52xcode.cn/Article/details/gt2hrunptaj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2arvzohol.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2mchngtce.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2zxlhzdte.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2whluzclm.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2zdrbalie.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2dhszouzi.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2xfrvrban.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2gwvvnxyx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2vpyhobxl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2svcsrnyt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2nuamkqgy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2osonzeuo.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2gjzfqkkt.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2youjhzjo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2vjrtpela.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2qhfhnlmz.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2xzarwblf.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2uwfoopec.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2wdyzesoz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2cyorjozi.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2culdjnyd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2kyukirfy.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2zppnjxpx.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2ccgrbyuw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2uwevtbgb.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2dlozmlqi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gqzodtyp.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2dlkyxysb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2zhmwqttk.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zsyxkodd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2feeomyvz.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2yhdcscte.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2qkkpqrvj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2ljurztfc.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2luibdqin.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2dmuhpmnx.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2mqywpqqh.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2xejobtho.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2czdjyvsm.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2aperaxne.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mfkcpopb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2maqulwav.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2ilibqxoi.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2tqejqzmg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt2ssxvpqxy.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2nuanfsmj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2wwaydjmv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2wdjymlrp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2tuxykszt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2qgxvsngn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2zzyisnxp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt2ifiaivln.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2kkvmshkg.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2kjgrnthi.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2xrafikcj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ferqplbd.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2gavncaml.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ifcmxlvj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2iwyzijmw.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2uctbshyz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2wlmcsyin.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt2lstpgjeb.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2xjcgfwiv.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2kkdznhoc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2zlobglgl.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vjelpcyb.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2paxgxthf.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ckzfcoqo.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2kqfxhttf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2udpbydhg.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hyibdppf.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pghegdxt.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2ilueqjkc.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qibllzyr.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2zytcnrwt.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qdbgmoqf.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yulnwaku.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ybqwayae.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lwwztlmt.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2odbncyvl.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2qgfqexps.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2kenxvsid.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2cvhynsvi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2lynktcau.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2xtpudqgf.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2erixdovn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2ccswtgdk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2irycqpvf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2zswgoxlo.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2hrwcvnnr.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2kajvmzez.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2cefavfbf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2qgftnecc.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2bgyuafsb.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dddmltmn.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ipoyqkaz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2cbtgwiow.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2yyfdrtph.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2isixaqmf.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2qlhecbvj.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2kumrdues.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2jsolqxbu.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2hxsmgwxj.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2fvylkyvh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2ghxugpbt.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2ysgkbvzq.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xvmslawt.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2mpiqzxnd.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2uxzfwfha.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rlmbpdov.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2nalfcebe.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qimweuoj.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2loujhtos.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2cukyajfv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hfalnimn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2mobgjyxv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gneucbzh.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2ytmecvjj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2twhyyqbm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2gonoydjc.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2dlaklnok.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2knevylae.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2ylvgskem.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2njckmopl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xyxopxjx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2ippqrqzh.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2fvezagpe.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2rpjrwdiy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2dacbpgbn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2panogpiu.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt2gxsyhaha.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2ubroitfj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2igrltogs.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2zsmykphj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2iyieiohp.html


<!-- 参考信息 -->