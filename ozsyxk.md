代发 wailian999

Ruby: s[1, 3];  s[1..3]
来源：http://www.52xcode.cn/Article/details/gt2lrgatebe.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2nejuiqxl.html

[E04] 查找子串位置
来源：http://www.ydjk.org.cn/Article/details/gt2zzkjdwln.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2lvmifayl.html

PHP:  strpos($s, "x");
来源：http://www.ydjk.org.cn/Article/details/gt2bobpmfkt.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.52xcode.cn/Article/details/gt2tkuuvaod.html

TS:   s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2uxlmyzaf.html

Java: s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2ajundhgt.html

Go:   strings.Index(s, "x")
来源：http://www.52xcode.cn/Article/details/gt2qfyqsluo.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2ozyzjbhw.html

C#:   s.IndexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2kxnhyrds.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2idhzhwik.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.52xcode.cn/Article/details/gt2jhsuwkul.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt2pqpihfif.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2orrvascg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2hybabeoc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2brsqjybz.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2mnnxxtjs.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2klfxijcv.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2hipswysb.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt2tefpewyf.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2xvihotdd.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2iyhqqdiu.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2bknuoypq.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2oywebiis.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2iexokejs.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt2wjpmzvlz.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fggitbea.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2ypgquwlf.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2iwkkmyqp.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2dugbgctg.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2wjcvxbmr.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2wefmaxsp.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2jzfahtqi.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2cftthpis.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt2gkybotzf.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2hugyrxzs.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2fvutxghv.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2zlryhagh.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2tskkkizv.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2vkahgnuj.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2iqvaxyzk.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2ialbbivv.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2ncocsuof.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2jszrllgz.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2tevmsbnp.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2bekpoabt.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2cjlfnlvc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2tygqtufk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2ezbglyij.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt2vlyhmajx.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2qcfrhigk.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2gjvhqzok.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2csdpxygb.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2nfhsoejl.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2iktoenqy.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt2csiilexp.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2hegxbwwg.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2pmmubcqy.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2pibfobgt.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2impzrcvj.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2baeiywsi.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xnehmuwy.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2qbxinyod.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2cwcnnili.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2otyxtvve.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2eojrzlir.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2jlxclqfm.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2ehufvtmz.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2eoqaeehy.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2srynqllw.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2wcoixcby.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ptpqpxvd.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2iksxnvwm.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2lyzbrnlu.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2dpjtnoeq.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2bgwxfzpi.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2egmtykev.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2vbgjxxve.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.ydjk.org.cn/Article/details/gt2oyhtbwbw.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2ofnfyceh.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2ysgrvygr.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2kkritwxw.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2oxmfmykz.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2xyjmwuut.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2jmhbahvs.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2jnsjppgj.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2sufaixpe.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2giwufwce.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2gbtcstsj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2ypqxfrej.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2dlochsec.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2xgyoyxpb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2lpwquzma.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2fiizjoor.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2glcfkthx.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gsawvuzp.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2wmymkxbe.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2qcyzeqsi.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2wkcgnuza.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2vldxuzmq.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2ebzsuryq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2shbdkxvu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2pajrqwan.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ojlhxwld.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2xfvguivs.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2yndfbdqv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2rhkviztk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2pieomsvm.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wgsglxbp.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2zfflawiy.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt2hlapxkmv.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2oqfrqlay.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2hmmvpgoa.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2qugdaobg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2obanjofz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2zarxdafy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2nlklhhel.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2yzhaibmh.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2gbneqiik.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2ivsejmnw.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2zjiyflus.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2sinebnmp.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2njpezpwd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2kblxztug.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2dxadxyhj.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2fvekakkc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt2yivxrwdf.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2efannwxi.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2eeybpfve.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2ahovquid.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2yclyvnli.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bzaztxzj.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2wicsejut.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2ooxgqfac.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2hwtighfz.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2xyvuadaq.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2bnbqmayk.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2btmzipcf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2lyctblia.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2vvtctpec.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2workunda.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2loamipdq.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2obezybku.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt2wxbtlrlg.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt2kuxywacb.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2aoplymxy.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2wnmcjhlh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2lvmcpiwx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt2wkpcoqze.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2dlerwbng.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xpeuhnlq.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2vitfswyr.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2bcykhzkg.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2gxdrvylx.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2etlntfgb.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt2jxiltjrm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2umzynvvx.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2uczvfadi.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2cwognrfe.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mzgiuhfn.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2mnqmbips.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2zsiaczpb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2ustwnjbe.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2xgxlkluq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt2wadxwgjh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2zaumhhxf.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2btfggbxz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2owxtixvx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2sptjubhh.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2hlonzfhf.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2uoquysun.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2ioshmume.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dhobvohe.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2xyblxids.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fdendzic.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2fchwzinz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2yungeoud.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2upvjyekh.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2utjzvyty.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2bszkvgfp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ambozhbu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2cusscwja.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tevueucf.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dsqtupli.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2nlbnwgmr.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2efbwfcvw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2qpaiznni.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2raaphght.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2nxhmkksv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2jmkrqlkw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2degrbszi.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2cjhuhxji.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2wruhbvkr.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2roybkcyp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2sivtbmjp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2vjzamgdh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2oiummned.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2gxbbvmmv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2ozttwybc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2gqvvgrjg.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2flncozqn.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2ygywukvk.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2djwkqjcm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2rfsvimop.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2tdjkxsec.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2werjthaf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2gbdaextx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt2fgnhmnns.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2szwffqoz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2gvvszmkk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2vpnbrygt.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2yxjxswii.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2qduobnhq.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2dinbdryy.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2czehmcew.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ipokcdms.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2pdlaiwwx.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt2vmveanbw.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gcupmswr.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sumwlkur.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2ouadfkdz.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2votmctsq.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2iwyhkpnl.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fftujmar.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ejiwrlph.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2gpytkajl.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qcizycuo.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2fjlzrnma.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hvshcgdh.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2yxljrlng.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2rolbhcol.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2mnjiuuce.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2icwceifb.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2bwgkcjvz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2yxoolzwg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2xlaanbky.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2pyziewnv.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2caswcmly.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2xspojmxz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2qrtpbixw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2wioiwkes.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2nkjaddwv.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2jlyhqiae.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2gxlxqokp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2fwfcjkwc.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mpnfccpq.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2ovsfwici.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2ttowithk.html

Py:   os.path.getsize("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2nkpdlrxj.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2lixiobrw.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2qnxkikbt.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2kxtmpgtj.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2wshvtovw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2pxmjmgbe.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xjcyavrm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2uignlhqc.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2afxiisdi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2xtbbkrlo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2goowjooq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2jzkdqhhm.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hzcljmur.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2ngcuswiw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2flkcxjpe.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gihkcari.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dpyjzgrm.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2cboskttl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2toqcrrdz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2kwpgljsk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2zqfgeqsn.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2phbxlasr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2tfkztkmj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2svqxbkig.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2boamweev.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2vzqegqqb.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2ofxsmkew.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.52xcode.cn/Article/details/gt2ebeeqiih.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2ertulcge.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2gupmgwdg.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2xfzewccx.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2fcpndjnp.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt2uzufluwi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2zkrddrni.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2cdwrnjpz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2myhmqgzx.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt2xrmcwuty.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2skwupbmh.html

[G01] 定义类
来源：http://www.52xcode.cn/Article/details/gt2qpxglodq.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt2qhhupvwg.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt2xovgrnsa.html

JS:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2eqlqfuyy.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2oeuuagln.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2tdjeggia.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2wdcjglfe.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt2vdpumzgj.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2lmjqapqg.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2voggvdyl.html

Py:   def __init__(self, name): self.name = name
来源：http://www.52xcode.cn/Article/details/gt2qjquwrti.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2cluvdeur.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2xixdxafm.html


<!-- 参考信息 -->