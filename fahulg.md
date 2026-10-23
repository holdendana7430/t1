代发 wailian999

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt3vldnurmb.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3iobdppps.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt3rvxsilws.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3xeycycuo.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt3hwfjopns.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt3xxkabluf.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3neqqjzni.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.ydjk.org.cn/Article/details/gt3bmdazaii.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3dmrsabwc.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3inthlror.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3bewbuuxe.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3jridzapu.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3ujcjxazg.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ouvlzagt.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3htyoglhc.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3bblttnse.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3mrhzdmlb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3xpwgyhta.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3gxbeczcu.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3dnvtqkcn.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3ohqapstl.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3yutgpyry.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3zdnoxkfe.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3mmcbdpwa.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3gqcbclvr.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3ehvpioeo.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3pnputwgd.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yczcklgp.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3lfozyvyg.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3ttstvyao.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3adrndmml.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3dqwljzdj.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3rkpjvraz.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3ipkiwoyz.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3zdfsaluw.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3fskllfae.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt3iidlvqdg.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3cjtfjabw.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3xqhwcgpd.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3uljxeqxf.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3hnzdxlim.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3oprhmows.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3ixneykgl.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3xwhwsbgz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3cpptpkdl.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3ziietibe.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3mamgjtrv.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3choixifa.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3yysawswp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3bkkstmay.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3cdplrdhb.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3vtuksqgb.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3liegosaf.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3ajebwpqu.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3lwmotpre.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ltnllvfz.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3ndchxdlw.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3lqhsaeqg.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3vgstduxr.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3mnvliuwk.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3dcxemwmw.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3vyzpyovh.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3cxsosexq.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3fyzbprnx.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3stfehpkm.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3clkvlgap.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt3izlwpebt.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3aommlxhd.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt3vhkmpwna.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3rpjvvfun.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3ahalpqdm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3pycdthlj.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt3bxmblqxc.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3ebukfcru.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3eitnaahq.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3kzrjiisf.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3dxnjrqgr.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbttmynd.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3zjjlhnkw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3yspuvguf.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3oaixfckj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3svlvpras.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3wepaltnt.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3vavqjpst.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt3ejnxsfzl.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt3ibxgydxh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3qcfcmxap.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3hbgerncg.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3evijavnp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3adknahct.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3cudljdtp.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3tsbyugfv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3mtdxftcy.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3owztikke.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3acsbkkvb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ufnfpqah.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.52xcode.cn/Article/details/gt3tshoscua.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt3seupxxim.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3xcqfxvkx.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3wvaxcbvc.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3tiffdbtm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt3qocyxpqp.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3njxauhqs.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3hapfxdwa.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3emjpoanu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3rrhqnvmu.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3kigdadms.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3safcgsdr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3bofzompp.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3euzjsidn.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3guxeutrm.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3ogzddltu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt3kbumuykf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt3ptvxrlnr.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3cqayghiy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3dfzdhbhs.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt3eagnzkbw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3nnsssqku.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt3apoahfog.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3iktvqtge.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt3doyvowcs.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3pzxyyplv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3ccannipd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3yzsrarcn.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3duhycogl.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3bevhyzve.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3eqiiirti.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3btuvtmpj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3fuyqzufu.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3dplsyzob.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt3vnhemher.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt3etpvoyyb.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3yupofqqv.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3yslajodz.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3rdirmyps.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3lvtfibit.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3jczxsdph.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3bujdsjub.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt3pkvqgfcd.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3qxgtwayc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3bnfzepii.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt3tohatqlq.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3lgqexydx.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ylqajjok.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3nmqcsmrd.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3ogxyjess.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt3riygonvc.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3agwcdlnc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3bkplufvo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3jrpbcqzw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3szwnvify.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ngfvgfoo.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3nxeeugzm.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3ccdlgnpl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3hmixocxn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3djactxmt.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3xpgkdior.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3agrvacya.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3lozjdvdj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3btrgfnez.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3vqckwlda.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3xfdkgjxl.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3eirqclgc.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt3chwnnwma.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3ozidwxig.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nurewogu.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3ihvenxhe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pnuzokmr.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3ecgvoykk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3xyzydnws.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tjcldjhd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3axpwxfgn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3cyjpwzkh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3kxjbvfej.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3joftpmwi.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3zaxrjkas.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3idwvxroq.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3bjcjujev.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3yzclahxj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3mduqcmrs.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3bvscipri.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3wlnnpjlv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3qzsbdqln.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt3isewzgxg.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3tzxdpsdd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3evaqprrv.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3qesytgws.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt3afshutll.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3conigawc.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3bivxnlqe.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3fkveepaf.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3zhzrbaxq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3fvqpmhrc.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3txhyhvzc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3zbxcqkxi.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt3gtjtqfcv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3alaldcsk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3etmhomps.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3vmjbuxgi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3ujnilmiz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3dhcxsghp.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3hnfgfifa.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3gerhihxo.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt3kdsbluva.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3cymtqhnf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3xsxeqjpd.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3llovuwlo.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3gusjnksj.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3iqohjwng.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3szsmmicw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3lhtcgxrm.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jediaxob.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qrusyuhe.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3lioinwbd.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3nzpegvfd.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3taxeormz.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3sewqnuhv.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wqdsdfro.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3qhvehxhc.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3sxdpayrb.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jczfeziy.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3jlnbnygk.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3rnlyidkr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt3xxclwflj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.ydjk.org.cn/Article/details/gt3hsomoumu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3qrsfmstz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3rriactto.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3lcjharsk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt3vexkesti.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3opymlnrb.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.52xcode.cn/Article/details/gt3jknfiewq.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3cleeadku.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt3jqwinayh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt3qvdlttrk.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3qkoixzha.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3isgusqvt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3ivhrahmc.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3ivrnubfm.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3xrnswcml.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3aheysldh.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3ahgnrvqt.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3krgpoizb.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gdzinagg.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3xqylhudh.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3vhegmlwj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3wqvnxybk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3wldvrvze.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ibrvgslj.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3cqjojepw.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3ottloqcc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3dhbdbmtk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt3kfanosup.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xxqgyubp.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3crbaxfyk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3eynztvja.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ostnwdcf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3jrgyrvwz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3bjmctdkq.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3lbqnlmlf.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3eqjcvgxr.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt3msrcoivn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vdrvieid.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3hjddfbdz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3ckthcwwz.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.ydjk.org.cn/Article/details/gt3jrsqgjlj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3narxzgrx.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3nvkklpue.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt3mvwlqgzx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt3vrwrvkwu.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3ffcanmtp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt3nqynnnpp.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3gjwqdixj.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3eikoyxqd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3gskzlpts.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3pycwkyxp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3ozjfnpfn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mmwpntze.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3rcvnvnit.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3chaaaqew.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3wlpifjbe.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3wfshrsii.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3koezomws.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3ornevtmq.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt3eoqcfsws.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3xviztplp.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt3hnaidefv.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3zgocdvjx.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3jmzitmqe.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3rusfvjga.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt3tsbxjhmy.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3jkkaszwg.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3brektypd.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3mvzlxasg.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3bekyuvou.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3vddsfdwr.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3tqniyjiq.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3wioyiyed.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3thzqduty.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3aonfvoxc.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3udspztrb.html


<!-- 参考信息 -->