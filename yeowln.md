代发 wailian999

Go:   strings.Index(s, "x")
来源：http://www.ydjk.org.cn/Article/details/gt3tqlqtofn.html

Ruby: s.index("x")
来源：http://www.52xcode.cn/Article/details/gt3rouzijhv.html

C#:   s.IndexOf("x")
来源：http://www.52xcode.cn/Article/details/gt3lwchhosn.html

[E05] 判断包含 / 前缀 / 后缀
来源：http://www.52xcode.cn/Article/details/gt3ndqjgtmq.html

Py:   "x" in s;  s.startswith("a");  s.endswith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3ybayxkuy.html

PHP:  str_contains($s, "x");  str_starts_with($s, "a");  str_ends_with($s, "z");
来源：http://www.ydjk.org.cn/Article/details/gt3zeclgiov.html

JS:   s.includes("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3nkvtsrtx.html

TS:   s.includes("x");  s.startsWith("a")
来源：http://www.52xcode.cn/Article/details/gt3srinkinc.html

Java: s.contains("x");  s.startsWith("a");  s.endsWith("z")
来源：http://www.52xcode.cn/Article/details/gt3ahrkbkes.html

Go:   strings.Contains(s, "x");  strings.HasPrefix(s, "a");  strings.HasSuffix(s, "z")
来源：http://www.52xcode.cn/Article/details/gt3shunkqyi.html

Ruby: s.include?("x");  s.start_with?("a");  s.end_with?("z")
来源：http://www.52xcode.cn/Article/details/gt3opwfjvza.html

C#:   s.Contains("x");  s.StartsWith("a");  s.EndsWith("z")
来源：http://www.ydjk.org.cn/Article/details/gt3afissokt.html

[E06] 替换子串
来源：http://www.52xcode.cn/Article/details/gt3jaqrnbih.html

Py:   s.replace("a", "b");  s.replace("a", "b", 1)
来源：http://www.ydjk.org.cn/Article/details/gt3odblagqy.html

PHP:  str_replace("a", "b", $s);
来源：http://www.52xcode.cn/Article/details/gt3mryrohat.html

JS:   s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3zlsaxxmd.html

TS:   s.replaceAll("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3wxtzmzeb.html

Java: s.replace("a", "b");  s.replaceAll("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3kjynnygd.html

Go:   strings.ReplaceAll(s, "a", "b");  strings.Replace(s, "a", "b", 1)
来源：http://www.52xcode.cn/Article/details/gt3bthuuztw.html

Ruby: s.gsub("a", "b");  s.sub("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3vrfgttma.html

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt3hgciouat.html

[E07] 按分隔符拆分
来源：http://www.ydjk.org.cn/Article/details/gt3zmcjmydb.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3rsonqjgt.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3lxmfjywg.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3cwdadyuc.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3crpocytb.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt3eziudula.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.52xcode.cn/Article/details/gt3egmkjmfd.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3uvufypiz.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt3eyvesxto.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt3iyodcmfn.html

Py:   ",".join(items)
来源：http://www.52xcode.cn/Article/details/gt3ouzjfejf.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3qogxcpii.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3wdzradqu.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3zdrxifec.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3rzyzfqys.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3slfxsyav.html

Ruby: items.join(",")
来源：http://www.52xcode.cn/Article/details/gt3zrdioqpw.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3jshtsfgv.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt3tkspwwqq.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.ydjk.org.cn/Article/details/gt3zshvkbpt.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3tirlqpai.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3afxxzdps.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3qjdfcbnz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3waspbcnz.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.52xcode.cn/Article/details/gt3pajfnspe.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt3yropswxm.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3gwqwqham.html

[E10] 左侧补零 / 定长填充
来源：http://www.ydjk.org.cn/Article/details/gt3nfvunkfv.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3tdxgvlvx.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3ksljlkph.html

JS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3tamjflap.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3zsdixjbp.html

Java: String.format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3vedcqwbf.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3ehtvbriu.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3fkylrggh.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3qvmvinqb.html

[E11] 反转字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uuidqrsu.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt3pmbcdxuz.html

PHP:  strrev($s);
来源：http://www.ydjk.org.cn/Article/details/gt3bzczrynd.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3lhiotcss.html

TS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3lxyzrfha.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt3lrsffilo.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt3mxxnyzfq.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3rchjqxps.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.ydjk.org.cn/Article/details/gt3picyoyfg.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3zanwjrpl.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ilxhycws.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3cvcleruj.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3hosnymnq.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3cvkasjhq.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3fzcyqnxb.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3mjwmgeyl.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3ramxgxjz.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3ddjawkjj.html

[E13] 逐字符遍历
来源：http://www.ydjk.org.cn/Article/details/gt3hmwbxpgq.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt3mfxstmxo.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3vlcyykkb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3mmamgmkq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3dyecogvg.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt3lksdpkah.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3wiubqjch.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.52xcode.cn/Article/details/gt3aqoljdsc.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3htavrgvb.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3gbzbqaff.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3evnvpmqu.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3etxwkywy.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3upzcpybm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.ydjk.org.cn/Article/details/gt3rxyefxus.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3aljhycyw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3lwogpqum.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt3earmkruw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt3kzzbuvyc.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3htootgke.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.ydjk.org.cn/Article/details/gt3onpmtcqn.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.52xcode.cn/Article/details/gt3kpbrfvfy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sotdtgxg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3lpmyvozg.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt3jjytwolw.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt3kjxormhq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3ueaxhuwr.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3byigzhog.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt3lzvpavlv.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt3baowhbnk.html

PHP:  number_format(1234567);
来源：http://www.52xcode.cn/Article/details/gt3eavmsgtv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3xneqqiho.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.ydjk.org.cn/Article/details/gt3abtsvlvo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3honcpbam.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3euvktaup.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.52xcode.cn/Article/details/gt3sufsxsxa.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt3lhdfspnh.html

[E17] 首字母大写
来源：http://www.52xcode.cn/Article/details/gt3zztizvwr.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3mxsjduuo.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3wcmmtztg.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3jtmybebu.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt3wathdwhh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3rldeozfp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt3fxggpwzc.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3dgipsaqx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt3itixjlbg.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3ephocjkj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3xwectkof.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt3ovajzzbn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3mqcggslj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3udkuxkhh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3doungkjc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3mtwbczih.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.ydjk.org.cn/Article/details/gt3hbuczzub.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt3unezvsce.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3cvpqhsus.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3vueryipc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3cysgvdpd.html

JS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3tdzbdrgh.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3hvpeiwig.html

Java: s.lines().toList()
来源：http://www.52xcode.cn/Article/details/gt3hovbtctc.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3nufgnliu.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt3vumdxqkl.html

C#:   s.Split('\n')
来源：http://www.52xcode.cn/Article/details/gt3dxwjsmnt.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3pqewtgyl.html

Py:   if not s:
来源：http://www.52xcode.cn/Article/details/gt3psciqqhn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3oxxszbtw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3lqpeuvsm.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt3maxnjsof.html

Java: if (s.isEmpty()) {}
来源：http://www.52xcode.cn/Article/details/gt3sfglfdtq.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt3cxpolkiz.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt3optvdavq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3aavmbjhi.html

[E21] 超长截断加省略号
来源：http://www.52xcode.cn/Article/details/gt3jqaksuim.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3irrfkqoj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3umqfqjub.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3iyndmpbd.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3lbadnzcf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3olnofcbb.html

Go:   // 按 rune 判断长度后截断
来源：http://www.52xcode.cn/Article/details/gt3zhnjyxsj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3yjkpsgrl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3gyndspdh.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3akumgmrc.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt3owmrdvfn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.ydjk.org.cn/Article/details/gt3rferzhpx.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3civjskah.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3txgwlcbi.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3isusiwwm.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.ydjk.org.cn/Article/details/gt3kuelfstq.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3uzvyszgy.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.ydjk.org.cn/Article/details/gt3nbexuifz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3lhvduihz.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt3plsvpkph.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3qrdobkte.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3xyozxeev.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt3gckkcock.html

PHP:  file_get_contents("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3igqxjnbn.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt3niowldqa.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3bvbafbqo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lzdwsbtu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.52xcode.cn/Article/details/gt3rxlvahdg.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3erzrohuz.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3eyiqhzrs.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt3eiwpdibs.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3erhwvujt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.52xcode.cn/Article/details/gt3naceehts.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3rimztqvo.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.ydjk.org.cn/Article/details/gt3pmxbbafb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3mwrwmcse.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3lyfyqwjf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.52xcode.cn/Article/details/gt3akghcktg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.ydjk.org.cn/Article/details/gt3xatfrvqn.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt3ccmvqxru.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3kruvtbkp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3lngtcvyq.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3ktbdetjb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3edoulgil.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt3aikayosb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.52xcode.cn/Article/details/gt3iafvkdld.html

Ruby: File.write("a.txt", "hi")
来源：http://www.52xcode.cn/Article/details/gt3emrrgdbb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3kkhltgol.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3kjrgkrtm.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3bfvdkiau.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3ienskrnp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3roxoshnb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3obvhzalu.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3vfsjcvbz.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3esbxonpw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.ydjk.org.cn/Article/details/gt3jjqvbffp.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3glkexpzd.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3tuvqfpvf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3jtytpxic.html

PHP:  file_exists("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3vwkjjixc.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3hqvxmtlr.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3kiofcpze.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3fhqmwlxf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt3zjncxvqh.html

Ruby: File.exist?("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3hhefwyaf.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ifduszik.html

[F06] 删除文件
来源：http://www.ydjk.org.cn/Article/details/gt3argsrnul.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3xhwotnoo.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ctexiihw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3zjhqpevl.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lrpyzalc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3naovgvjz.html

Go:   os.Remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aykdmujg.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3ledlordc.html

C#:   File.Delete("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3deydvzfq.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt3noujffui.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3pruajngd.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3vmrdyldl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3vhccefta.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3ggzuable.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.52xcode.cn/Article/details/gt3bumwmstg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3qgjqvrcj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt3fcxonhll.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3huebdisa.html

[F08] 遍历目录
来源：http://www.52xcode.cn/Article/details/gt3opzvrzol.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3lmkynzaf.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3slsduqew.html

JS:   fs.readdirSync("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3dzlsvjed.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3bepkmgyv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.52xcode.cn/Article/details/gt3iopmkefp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3lhhneoen.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3njcyidxq.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt3psdieawo.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt3nrckquic.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3alxklcur.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt3ilcuukzh.html

JS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3novaxtep.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3yeucnyvz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3xcseuyyn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.ydjk.org.cn/Article/details/gt3lttbpian.html

Ruby: File.size("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3dngkxsmm.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3knaydenq.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt3sjpfdntl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wertwoxk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3trkbbhow.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qgkmclzm.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3qxjmxnfl.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3nfkcffew.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3uxiemckj.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3oipjboke.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3rprtpxya.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt3vrrfnmer.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3fzoqqcaw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3czqlrwbw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3adkitaom.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wflbefdf.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3pdyjybkk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3okxiltjp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3egghecct.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3lzzgykrb.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3zpgpbniq.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3uuahuapm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt3vnmjgejp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3xmkvbusv.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3fvixvgep.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.52xcode.cn/Article/details/gt3jtxilils.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt3dwbzwinf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3viaixodm.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.52xcode.cn/Article/details/gt3ztiutlab.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ubxoflhe.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt3wuzwuaxq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3leifyhou.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3qflqcxcq.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3bbszqlvz.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3zmdpzgqi.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3hmiiflyt.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3hbokxdyx.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt3mocnfrkk.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3bonlqtoi.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3seskhmrd.html

C#:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oihjujpb.html

[G02] 构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3sshptyqt.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3lwmlrttp.html

PHP:  public function __construct(public string $name) {}
来源：http://www.52xcode.cn/Article/details/gt3pfmztnyy.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt3mdmhnocu.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fwfvmcmo.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fdisuzfy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3evvafrfe.html

Ruby: def initialize(name); @name = name; end
来源：http://www.52xcode.cn/Article/details/gt3spppptjs.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3atwgrcss.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt3jsuxnwge.html

Py:   self.name = "x"
来源：http://www.52xcode.cn/Article/details/gt3ghfemvto.html

PHP:  public string $name = "x";
来源：http://www.52xcode.cn/Article/details/gt3prcxnvsp.html


<!-- 参考信息 -->