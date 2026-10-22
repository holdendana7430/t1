代发 wailian999

Py:   "a" + "b";  "".join(["a", "b"])
来源：http://www.ydjk.org.cn/Article/details/gt2wmslvojw.html

PHP:  "a" . "b";  implode("", ["a", "b"]);
来源：http://www.ydjk.org.cn/Article/details/gt2nnfkehln.html

JS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2diiquibp.html

TS:   "a" + "b";  ["a", "b"].join("")
来源：http://www.52xcode.cn/Article/details/gt2qkvcopix.html

Java: "a" + "b";  String.join("", List.of("a", "b"))
来源：http://www.ydjk.org.cn/Article/details/gt2acdgdhlb.html

Go:   "a" + "b";  strings.Join([]string{"a", "b"}, "")
来源：http://www.ydjk.org.cn/Article/details/gt2iqkztqsc.html

Ruby: "a" + "b";  ["a", "b"].join
来源：http://www.52xcode.cn/Article/details/gt2xffucgpn.html

C#:   "a" + "b";  string.Concat("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ecfjihsr.html

[E02] 重复字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uhvxvrje.html

Py:   "ab" * 3
来源：http://www.52xcode.cn/Article/details/gt2szfvuqph.html

PHP:  str_repeat("ab", 3);
来源：http://www.52xcode.cn/Article/details/gt2secwwfkw.html

JS:   "ab".repeat(3)
来源：http://www.52xcode.cn/Article/details/gt2nrttbexz.html

TS:   "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2uwprlbsu.html

Java: "ab".repeat(3)
来源：http://www.ydjk.org.cn/Article/details/gt2kgdqxhcs.html

Go:   strings.Repeat("ab", 3)
来源：http://www.52xcode.cn/Article/details/gt2bwxhwbeu.html

Ruby: "ab" * 3
来源：http://www.ydjk.org.cn/Article/details/gt2rqxskgti.html

C#:   string.Concat(Enumerable.Repeat("ab", 3))
来源：http://www.52xcode.cn/Article/details/gt2ewqfwvne.html

[E03] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2gvtlyrcy.html

Py:   s[1:4];  s[:3];  s[3:]
来源：http://www.52xcode.cn/Article/details/gt2megymmbd.html

PHP:  substr($s, 1, 3);  mb_substr($s, 1, 3, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2glmntarh.html

JS:   s.slice(1, 4);  s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2pfgfamzz.html

TS:   s.slice(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2umvvjcot.html

Java: s.substring(1, 4)
来源：http://www.52xcode.cn/Article/details/gt2zcszczkg.html

Go:   s[1:4]        // 按字节；中文用 []rune(s)[1:4] 再转回 string
来源：http://www.52xcode.cn/Article/details/gt2dlpghcbt.html

Ruby: s[1, 3];  s[1..3]
来源：http://www.ydjk.org.cn/Article/details/gt2xhqhngqm.html

C#:   s.Substring(1, 3)
来源：http://www.ydjk.org.cn/Article/details/gt2lhjzipsj.html

[E04] 查找子串位置
来源：http://www.52xcode.cn/Article/details/gt2jvezcucj.html

Py:   s.find("x");  s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2vvgjgxpb.html

PHP:  strpos($s, "x");
来源：http://www.52xcode.cn/Article/details/gt2dioeypsb.html

JS:   s.indexOf("x");  s.search(/x/)
来源：http://www.ydjk.org.cn/Article/details/gt2jtgnjdrj.html

TS:   s.indexOf("x")
来源：http://www.ydjk.org.cn/Article/details/gt2lcuqybsz.html

Java: s.indexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2xggkkryd.html

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt2fatjfqyx.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt2fiwzrqrj.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt2pjacbbel.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt2ynciukkn.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2dcnqhiue.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2aobgiycw.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2wrhimisg.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2hkrpynod.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2bxqfqngs.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2onwbqkhf.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.ydjk.org.cn/Article/details/gt2mvzgjomx.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.52xcode.cn/Article/details/gt2dbylilkg.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2ggmsrtzr.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2vjhjfehm.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt2vxuezzaz.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2pjcbaufr.html

TS:   s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2wdvhjljy.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2rrlvzdly.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2aqqejidw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2cijhzhtz.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2vueejbun.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2pvvudvuv.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2gktlvuow.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2tjoqyhot.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2liqaybpa.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2vsiltike.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2yswonijf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ssfisvbr.html

Ruby: s.split(",");  s.split
来源：http://www.ydjk.org.cn/Article/details/gt2iranfusc.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt2bidpzjye.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2kcifhlrc.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt2bvpetcgd.html

PHP:  implode(",", $items);
来源：http://www.ydjk.org.cn/Article/details/gt2imhcweyr.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2yvjealtx.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2eukpfczx.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2gmtezeae.html

Go:   strings.Join(items, ",")
来源：http://www.ydjk.org.cn/Article/details/gt2ghhzdnbv.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2iejrquhs.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2vwjxdqhf.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt2ouavbnwq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2zmrtrusk.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2bohpfekj.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2zvorgsbg.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2wpxhfnmi.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2wibcamnw.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2babjxyzw.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2ccebpmfb.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2ghvmguit.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2mvbfwwfj.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2frmommxl.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2ywzurrpb.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2cmkebuup.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2chnhanek.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2xggiirlv.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2fqqxyyvi.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2umqnjsmn.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt2tahwogab.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2witwnnof.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2bcvryisz.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2sggzupku.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xukezodx.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2fafxwdzb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2vtjlhdat.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2zzcvkrrv.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bjoakgxm.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt2nldunvqt.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2saokksml.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2guthlazp.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt2pgwibujr.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2zdgcgkdi.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2nlzxqrgt.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2eouxyggr.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2ighpsnjc.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2ecwfpjxq.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2tcmhtwsv.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gqflshrz.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2lkkiikjd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt2hazzmmlm.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2hkqgvrua.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2jlorgkiv.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2mxiswegj.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2tnzyumql.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2znevtogg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2ihyxmayg.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2kshfswrp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2ubyrjdxc.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2susqsubc.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2nrsuwyvp.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2rprqlilo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2dpmbdkmy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt2pghqrioq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2vjhwzyzt.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2qetocxpj.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2fxmbyorj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt2fvqcwzdv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt2kojgrbxo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2xdeovpir.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt2kusdbhvz.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt2spyynfgo.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2cnerdlku.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2nnabidge.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2brnvnmnl.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2fghuvhnu.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2vwycjarc.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2yqeyhvhn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2wjgzqkvs.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2cdmjyfei.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2ibuunmoj.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt2pnlabryc.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt2zldgohlz.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2ykdcoxor.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2sfjwfeiw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2ehvnhood.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2ulbgexjt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2hgckrxyc.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2giyunltx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt2rcbvlpts.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2qkyhwsdi.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2ncydwaiw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2aekmuevy.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2ibdtsqom.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt2mpsxeykz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2qtgrwgya.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gnsgeazw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2iqnzxacf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2pghsuvfx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2qnqsdqiq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2kkktkdgs.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt2xlvvjjsm.html

[E19] 多行文本按行拆分
来源：http://www.ydjk.org.cn/Article/details/gt2mefobrli.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt2axkbdims.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2sneysosl.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2eaozblgc.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2tvkerhyc.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2fkjepqie.html

Go:   strings.Split(s, "\n")
来源：http://www.52xcode.cn/Article/details/gt2iojbtmer.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2vjgmnusb.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2sjtdewfn.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2ggctbrye.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt2ppojhxdh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2psypfdxk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2quaulzev.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2irhxkcrm.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2mtkoaaab.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2xhacljep.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt2otixjyke.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xwgtzqek.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt2okmynkxq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2vwejcedw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt2bavlauit.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2mmnuowes.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2mbdxsglk.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2xhejsqmv.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2skheckbw.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dgovcxhg.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2lbwbaorq.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt2ygmxxtjs.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2shapkegq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2xzqblmxr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2lhjeozed.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2qpnodfvr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2ttjzvidw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt2sjnuuqoc.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2ccugnpyp.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2povcston.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qcwisgbq.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2tavobnwb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2prcsrmvy.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2fxaphxsk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2noknpigx.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2cogfsilu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2gssardea.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2htcjqsjq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2legzhxgl.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2ewhqkgaw.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ztastxsh.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2fvxewtnq.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt2tnqaimqs.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2wctlxebb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2lyqmuyfd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2npqwqajy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2tabztohl.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2gwrjsxgp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2rntjtwtx.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt2tczmjipt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2pojkttiq.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2levsrucr.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2byfzhoxc.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2koukdvav.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2hfokczvy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2hepdgzlx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2chnavuzs.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2enjbzerm.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2rwerrxzx.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2prdffojv.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2sjlqrxyp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.52xcode.cn/Article/details/gt2ewxjiuzc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2eqlezclc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2zkarnhsx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2tzsrlmfr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2jlgzsasc.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2rblvuyvx.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2ygzzlaue.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2iwyjdbnb.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2bgdxales.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2ldfffhqa.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rltgyubr.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2vwsajtal.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tmrfphxj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2fpbegrur.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2dnwewfca.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2sbcxumly.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zygfsqhs.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2vfibajvb.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2pwgtvygi.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2trhmyzss.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dpjkunis.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qparsqnm.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2nwvdufab.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fzekrqfr.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ictpspfs.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vacafcag.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2tspafsos.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2qloejfyz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2qoxiccob.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2nlckqpau.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2zlnmyjuy.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2pebbpguy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.ydjk.org.cn/Article/details/gt2gkxwknsk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2ooqhsury.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2urfvrijp.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt2uoksshul.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2pnodgxhc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2eybyalhm.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2cmlwsife.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2dxcwofwy.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2grztqnwg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2jqasnvae.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2wenxihlk.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2raaulqkm.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2rjeffcdd.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2tgugypso.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2igvidesi.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2urcpfmiq.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2rlizlyem.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2lmibmycu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt2vgjoqnpg.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2toexdkvi.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2xkxgzklu.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2bjqedovg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2tgdiuplb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2vsdfmitd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wasuukbc.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ndxhkdhy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.52xcode.cn/Article/details/gt2fwxggjen.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2cfsvdyqz.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ebrwisvp.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oefytqmu.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2qasfshup.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2gqnxdalv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cyqmtfot.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ofpvlmoi.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2lzvybgyf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.ydjk.org.cn/Article/details/gt2wigoqrlu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2yefdkyhn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2apdgdkim.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2spmlpott.html

[F12] CSV 读写
来源：http://www.ydjk.org.cn/Article/details/gt2vcmckgun.html


<!-- 参考信息 -->