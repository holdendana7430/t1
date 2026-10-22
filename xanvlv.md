代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2gxdscxzt.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2vzkprowf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mvrospki.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt2fbjvxxqb.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2ccdihquc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2qhxdxssh.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2iuqyhdpf.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2luytanit.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2oiqarsgy.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2jxiymiyq.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2xnwatuxh.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2geefcfnp.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ipjlrfnd.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2znjdkpzh.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2jjbvghmw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2zighreah.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2owlrxolk.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2cvrvjviy.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.ydjk.org.cn/Article/details/gt2rsnhnnfc.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2bdiazswt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2vqxafgod.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2tzvlvdmy.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2vhsgmlkq.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2ylatkjrv.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2oqkfiwoj.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2vzjtszsr.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2ysndwzar.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2cstqvltp.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2znaneqkm.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2vkujjckh.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2sotlcvbr.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2bawqjqls.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2lxvfdisl.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2udhtlhfm.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2dgqqdeom.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2ukpdjhav.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2urumajcd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2gauozzju.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2mwwohtpw.html

TS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2lhfbdqzy.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2nzvfdepv.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2hnqgzuxs.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2jkbdjvkt.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2nazbhdwo.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2cuvlqzom.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2rcgjqjdu.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2kubnuolj.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2mnqerzal.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2iyxgjpoj.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2gltwwrfl.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2uzpfwjeh.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2rvbegggh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2qkofpcza.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2ebylueqn.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2mjwuecwo.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jggerhad.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2wtziqaon.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2bxvinjqk.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2zqiqxpfx.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2ukjzrdoe.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2xogdhiyz.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2sdvcxohy.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2tzwcgmtr.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2yfylogdf.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2pikfrnzv.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2nbpjacet.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2hqeokpku.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2zxtsuzdp.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2jbhnqqpp.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2evhrszmn.html

C#:   s.Count(c => c == 'a')
来源：http://www.52xcode.cn/Article/details/gt2ndztldax.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2uinccstj.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2clkfhhgp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2lzunamzi.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2qbqacpgm.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2fkxwygjp.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2brrszalx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xhibtrhr.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2hpcyeilt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vzdiexwu.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2htawvnlj.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt2sjmoblwr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2pecjtxqa.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2vvwjerwj.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2itybjwup.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2lykaobmo.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2qtxgsulo.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2irpfacpg.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qxdxrmso.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2holxirgd.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2assiyknd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2xtisnopm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2khdhvivn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2umdnduzk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2vmkdvgpi.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2hshbdqpe.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ztxtgydc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2gfpvjywv.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2ealcfmsp.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2tmvgbrdc.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt2wpxjjdwb.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2gsqtvofl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2uubbggva.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2hzpchuqr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2ojflmzxp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2hglalbeg.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2dskdgijl.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt2eqobhewu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2bgaryhpq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2bhogmmhb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2ivvjgebz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2zqgwwggq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2chlsapkn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt2afcwrmnr.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ixysyqrf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2vefxnttv.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2gtumukkr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2vnmxllfh.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2fvlcpfzy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2cpbjayym.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2hjcsdkyt.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wvamurod.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2efhftxac.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2phmvlryq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2rgeazeoo.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2hjwjuobe.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2awgdivnh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2ohfdytrr.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2apzoxceu.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2qwzvwcso.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2xcatbqmc.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2xubbdnqc.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2sphrngzl.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2onzjkxmv.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2veekdiux.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2hijitxar.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2mbkvpnit.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2obcinmnt.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2kgkzfnnz.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt2tjgdnfjv.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt2sxdejpzx.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2bsjbrclk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2augoycuv.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2ynmcfhxq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2xcgjxwap.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2atqbycfx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2puslwcrv.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2upbduznp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2cwibqqsm.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2bhlyeshh.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zrdslfdo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ytlssuco.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2vfvyvpif.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2uhlkahyr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2qbzkgzre.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ejyzqjth.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2nbwceegk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2vwsqsvmp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2foirmbwb.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2rqqzrxlb.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2moqatpyx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2naoqjbfo.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2fifddqfi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2frcuqbvs.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2vqyuqrhb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt2xwideyoz.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rivnktgq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2rdlckqsn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2szlwvonq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fxdhplhc.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt2dypqiyrf.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ndqfdbup.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mtdcympd.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2xnintabq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2eitlvgni.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2hwcahbbe.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2oozflbug.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2jvygqfjh.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2othocnbi.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2qflijare.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2rsxxnrvi.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2tqquiiwp.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2cunhlckg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2ejrzujgo.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2mbguuryk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2duaxnwhl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2uiyakdfo.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2trseqjcq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2qzsmdijo.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2tdqtgqjl.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2tmstzjca.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2xoqeynub.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2velnqayy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2yblmszvf.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2vxawiwgj.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2pxhmtbic.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2drjcquob.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2ynplhebk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2tevqgwea.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2emodunrv.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ajswyove.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2jxqzusjq.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2mocpvkvu.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2oonzxieo.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ssqbdfms.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2tcekqpsa.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2vlrjihwz.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2pghrpmpj.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tjgggvwm.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2suobiaua.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2lctvgztd.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2beuiafyn.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qyirvuii.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lnujwscv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2cqldzjdh.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2slegzxdb.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vvxcopze.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2laopadfs.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2jhhzltpv.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2vtbikuur.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2hmackmfa.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2kxpvfatd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2zxbwvugv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2stwxgrpp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2hlobbzgm.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2mjhavbzy.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2mgsttymy.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2tpwcamxb.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2nxbtmfri.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2herlnbjt.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ekdakgzq.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wnvxvfgb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2tbcqocor.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ikfuhapg.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2fpluitdu.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2abbwwgzm.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2kstfuubz.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2iogfralt.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2ekirbxmt.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2lpfjvfny.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2qjwkovxh.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2hhuvsvlu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2qntxywwr.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rdzunxsf.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2gfjcjtzm.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2tmwhabxv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vmdzwpbc.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2nsihodhd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tlctxdvm.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vkbaxdch.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2fnnqpsey.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2iqmavqnk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aikjpjjv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2aczttbkd.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2lxagowco.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2atcgiahv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2ugjtgltm.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2katekepr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ttpstwxz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2btwetbij.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt2dvybbobd.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ryfbpxtf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2vhpdpeto.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2kxnwpgtq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2rcusydnt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2mgphajcp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2jlnctzvg.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2kstqigcj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2jtgwdjfq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2ewsjigtr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2wvarxqve.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2wryqspsy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iunzyipy.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2pmpoouuo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qursbzab.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2pkfhqdmr.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2pdrrbdfd.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2zabexyrh.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lcezmzgq.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt2smbgmzyx.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2proxkrdc.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt2pgqjdtev.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2hyjrdilv.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xxfamyif.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2deeduzha.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2tfcbaoas.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2bvrhbbmr.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2jmxuexsm.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2eihsvmqy.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2bcjzence.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2ufhuvnhk.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt2cfixscqf.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2uscqpxrg.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2qjxjovwp.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt2yqatanfv.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2mrswdnmp.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2ihvkmqus.html

TS:   name: string = "x";
来源：http://www.52xcode.cn/Article/details/gt2bnpjfzap.html

Java: private String name;
来源：http://www.ydjk.org.cn/Article/details/gt2yaazaanr.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2gvnjvzof.html


<!-- 参考信息 -->