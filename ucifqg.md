代发 wailian999

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2cpkruilk.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.52xcode.cn/Article/details/gt2xpkstaqv.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2vkdvmdxm.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt2itoxlxev.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2wxrspxrd.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.ydjk.org.cn/Article/details/gt2jnakcusj.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt2lupgppow.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt2qpmnhnja.html

[E06] 替换子串
来源：http://www.ydjk.org.cn/Article/details/gt2dykehuht.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2rumdtvcg.html

PHP:  str_replace("a", "b", $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nixxjjiy.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2kxyfvvts.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2ltynmdor.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2fqmiehza.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt2yntofdbb.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2dklxmivm.html

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt2sfoitkkt.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt2dxexfjht.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2kuxtdfbn.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2nmfcoigt.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt2xhwspqfj.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt2xocyeqri.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt2qlnigqze.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2aqeeykxm.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2qxfjntig.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2zuvqjcaw.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt2zmzezaif.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2oztrmizi.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2fjxmcszr.html

JS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2cdhqfahj.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2lkwtqpnw.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2txqvsbvy.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2gwefldmr.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2rfeltlqk.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt2hcsokmnj.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2qdgcoxat.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt2hjkeujqp.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt2mpodbesc.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2mmewexvv.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2pucvtbmr.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2rzrididd.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt2qgzhmiby.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt2yavhrnje.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt2hdgirlel.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2ylnvtpvc.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2nlvpyskz.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt2gktlpclp.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2kxzlaunj.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2bjqpiaoo.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2oxkjbkjp.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2emkgxoad.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2nljdcjfm.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2uchtxfjl.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2jeputubm.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt2htyjrmjq.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt2vykczyfm.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt2xtuivmhd.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2yhkjqdpu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt2admmmhhh.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt2hurrbtzp.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2mozjntgz.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2firzmlgg.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt2jhlifpdg.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2tjrlrbah.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2rwqkefhk.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2acypyrmg.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2pmxzixfu.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2auwharup.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt2uqanhqsi.html

Ruby: s.count("a")
来源：http://www.52xcode.cn/Article/details/gt2rilfshzt.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2osgnxxla.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt2popntqiw.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt2smjgtdsx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2mjngxuuk.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2sbdoriza.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2mucfbdzy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2sfnerlgo.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.ydjk.org.cn/Article/details/gt2uikjhhts.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt2dhcyhdki.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt2vhlbwrin.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt2irxywwci.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2yzuhflyl.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2lakrxlhf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt2huczznwn.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt2bgwvwjji.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2nynvuaaz.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2fzczoceq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt2bgkgfssn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt2rxnpeadx.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2wpgvqaux.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2lwvhmqjd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2uofkmafu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ypcahago.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2zulsecch.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2cbaepgzl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt2nhhlpvok.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt2yddwpjuz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pzzjtvph.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2wvdvojxf.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2qtsjbtcf.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2wjgamcdg.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2journajn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt2edklgfjy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.ydjk.org.cn/Article/details/gt2judoooxb.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2aezsjadk.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2bccdljrj.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt2jvkrbdez.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2zwvhmway.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt2zldbfbvu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.ydjk.org.cn/Article/details/gt2yxejnekq.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2vknznjfo.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2lfbbfyys.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2eiwvbfhr.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2dcnmhuus.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2crwnorvu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2nigybqqz.html

[E18] 模板占位符替换
来源：http://www.ydjk.org.cn/Article/details/gt2hdblqsaj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2dsvzscjm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt2viwxxnmi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2fgdfovat.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2bsplnoie.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2gbxiqwwt.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2dhvhnxev.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt2kchaoufs.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2bpwnqzrl.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2kesvejrq.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2iqhdjrqr.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2tyenzbnd.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2byygxldc.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt2bygpxmxe.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt2ucyoxvyw.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kkkettqv.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2waihhpaq.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2tnocjiva.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt2ncankzwm.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2qkcfhoho.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2fnfffhra.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xdzwssct.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt2seycrykr.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2djbkmkuu.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2fttvsxzi.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2ozoeostu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.52xcode.cn/Article/details/gt2qaqtkaio.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2ysgvnwxr.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2vwyaiepu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2iboiertc.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qzryucpf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2fyiwgvwl.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dwoouytg.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt2dhzluqum.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2qrhajfml.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gtssiffx.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2nethqpgn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2hmaizdfz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2lnvftdan.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2swiyjsux.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2lsbjxzwz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.ydjk.org.cn/Article/details/gt2fiiqyesc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2buzhazrq.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2jqrjycga.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt2xoeapvdk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qxjhzavp.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt2ilmfhdyn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wdapcjan.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt2funagkiz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2glpmynwn.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2gxaocjur.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt2frgzuypa.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2nvuuwkcc.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2zvnibooo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2vjiugigp.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2asjeioce.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2vtfcrbbo.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2wlpcszho.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt2cprsomoh.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt2jqgnhowh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2kyxscnyf.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt2luezlbpz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2ozxrnikx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.52xcode.cn/Article/details/gt2yuopjplv.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2pzqoowib.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2txxeetrb.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt2hrrujmmg.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.ydjk.org.cn/Article/details/gt2gsqsyjit.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2rzepbpgp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2cwmaasvs.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2aygnxvwg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2vjolwhrx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2elujeftf.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2nlwaqkza.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2cxrcwmmp.html

[F04] 追加写入文件
来源：http://www.ydjk.org.cn/Article/details/gt2vbpfqkud.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2jmthmbvy.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.ydjk.org.cn/Article/details/gt2uhoiwotz.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2dmaorojh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2gkvsouzs.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2dcvnofki.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt2kresbnlh.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2qmkbrbxz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2qayphfpc.html

[F05] 判断文件或目录是否存在
来源：http://www.52xcode.cn/Article/details/gt2grdcdyka.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt2cadeyrrs.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2tchaqbqv.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2qrmhtngm.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2qtrsqaix.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2aaofirri.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2jkyhwicr.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ynmbnrma.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2goaexluo.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt2mwznbjhy.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2hmxmkxtp.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2cuvyfcwq.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2oflvvqmz.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2smgffgtt.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2bkjadygo.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2ygavlbto.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zkxtpxqh.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2sqmrkayw.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt2qwfkiepc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.ydjk.org.cn/Article/details/gt2utxxbxpz.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2cpdnbhzr.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2pcamjrvr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt2egnrwyay.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt2pyyzyjue.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2jeocamui.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt2pjhdzoph.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2yvqhlmnk.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2ctnytmib.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt2uwnqmklw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.52xcode.cn/Article/details/gt2bfilnjqm.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2idssurft.html

TS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2mfahzsjc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt2qpjiyjwi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt2oublbsfx.html

Ruby: Dir.children("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2ycirfwrh.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2cmykaycn.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt2rmydvryc.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2rzuyorob.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2mymwiaks.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt2qkbowmfj.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2vlyupnqw.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2gnldgejz.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2qrnhquqn.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dulcvcjm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.ydjk.org.cn/Article/details/gt2bfztjxky.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt2ajbrzthw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vlnodvfz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2ailkqzeq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2hbeiuflw.html

TS:   path.extname("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2bdjtjtjk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2ptgnbcpy.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2zwfovofi.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2eijzuryi.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ymscocsl.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt2cthlwpkl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nuuacvlo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2rzoibqrw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2uxappsxr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2udbvadlc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2gbksagqm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2qvbedkrw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2qsekoacd.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.52xcode.cn/Article/details/gt2gmctcqvl.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2fcwmoqxu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2gkaitsey.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2tuanmshb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt2rojhqhdb.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2hthsfjvc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt2optbjbfy.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2clxmhyor.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt2hjdoitvs.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2mzluffyg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cmlrsafh.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2jjwhpgjp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jxuucyrc.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2cytqbpdh.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2wbboaxhk.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2ilebgskb.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2lrzvdqjt.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2lbehgigq.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2pfjvhint.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2tnokbwpm.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ujjahmxu.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2nvjkohza.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2olhmpcck.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2ykmidbix.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt2rqzaguge.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2nemkhbdy.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt2koihtccc.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2zkvkkmkt.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.52xcode.cn/Article/details/gt2stcdodca.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2rzkbvsqi.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt2krgmgmnm.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt2kywzkhqe.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2kjalfpzq.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt2mrqnpznq.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2rrnsjzlf.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2kmeodvmw.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2kzqevkht.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.52xcode.cn/Article/details/gt2umeagccx.html


<!-- 参考信息 -->