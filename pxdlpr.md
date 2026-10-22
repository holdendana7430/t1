代发 wailian999

C#:   s.Replace("a", "b")
来源：http://www.52xcode.cn/Article/details/gt2jnvjfvti.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt2cpgmqksr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt2eiyygxrs.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt2bjimyije.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.52xcode.cn/Article/details/gt2rjdqsnxc.html

TS:   s.split(",")
来源：http://www.ydjk.org.cn/Article/details/gt2ebukbjlm.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.52xcode.cn/Article/details/gt2odzxogqf.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt2tnrxaolv.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt2ufypzdyi.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.52xcode.cn/Article/details/gt2bspyhmie.html

[E08] 数组按分隔符合并
来源：http://www.52xcode.cn/Article/details/gt2ojpmtsvs.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt2ufwfzykj.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt2rpqdihkm.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2uvisxgni.html

TS:   items.join(",")
来源：http://www.52xcode.cn/Article/details/gt2cbkyskpj.html

Java: String.join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2sxmeuwin.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt2ejpjslad.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt2iritpwud.html

C#:   string.Join(",", items)
来源：http://www.ydjk.org.cn/Article/details/gt2aomocimz.html

[E09] 去除所有空白字符
来源：http://www.ydjk.org.cn/Article/details/gt2bszvydoc.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt2lpzziatd.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.ydjk.org.cn/Article/details/gt2vqrdypov.html

JS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2nlgjfiji.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt2qvcyogtz.html

Java: s.replaceAll("\\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2lvbuztpf.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt2uzlcfjsg.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.52xcode.cn/Article/details/gt2nnoeorps.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt2atyawywy.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt2equdsqvn.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt2cqavcibw.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.ydjk.org.cn/Article/details/gt2fgdwvndc.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2pvfliqcr.html

TS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt2cijeelwj.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2hzlptyhc.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt2aeuaudag.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt2mhgwooge.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.52xcode.cn/Article/details/gt2zjgaxtcp.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt2gluynkvv.html

Py:   s[::-1]
来源：http://www.ydjk.org.cn/Article/details/gt2ntdojhmf.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt2wvmrwigq.html

JS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2vmppmgrf.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt2duaemhti.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.52xcode.cn/Article/details/gt2dsnxigec.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.52xcode.cn/Article/details/gt2jlwdpdlu.html

Ruby: s.reverse
来源：http://www.52xcode.cn/Article/details/gt2ddglvyjn.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt2givsosou.html

[E12] 统计某字符出现次数
来源：http://www.52xcode.cn/Article/details/gt2slyyyvki.html

Py:   s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2dipbmttq.html

PHP:  substr_count($s, "a");
来源：http://www.ydjk.org.cn/Article/details/gt2ocqjdbam.html

JS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt2imzxhzke.html

TS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt2ryscqrse.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt2cgbgktms.html

Go:   strings.Count(s, "a")
来源：http://www.ydjk.org.cn/Article/details/gt2ddzjifbd.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt2pswzgeic.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt2gbjtjjwo.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt2harfccpt.html

Py:   for ch in s: print(ch)
来源：http://www.ydjk.org.cn/Article/details/gt2bvrowsoc.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.52xcode.cn/Article/details/gt2ixmcagdt.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt2nusfbpmn.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2vrhtjlgc.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.52xcode.cn/Article/details/gt2hyevsltl.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt2iaibiyil.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt2nwmcfmrr.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt2anjejvbc.html

[E14] URL 编码与 Base64
来源：http://www.52xcode.cn/Article/details/gt2bcbvjcqp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.52xcode.cn/Article/details/gt2hguivomh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt2ekorhmrw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.ydjk.org.cn/Article/details/gt2wmckaftd.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt2faajwoqj.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt2lqioxctn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.ydjk.org.cn/Article/details/gt2juttwiac.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.ydjk.org.cn/Article/details/gt2tkkfnpho.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.52xcode.cn/Article/details/gt2bqwyxudy.html

[E15] HTML 转义 / 反转义
来源：http://www.52xcode.cn/Article/details/gt2nzyoocyq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt2usmykdch.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt2xbcztmme.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dvgwnlgg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.52xcode.cn/Article/details/gt2ldpabbwo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.52xcode.cn/Article/details/gt2qjdnmyza.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.52xcode.cn/Article/details/gt2nrlpxoyx.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.ydjk.org.cn/Article/details/gt2ijvegieq.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.52xcode.cn/Article/details/gt2hufboseq.html

[E16] 数字千分位
来源：http://www.ydjk.org.cn/Article/details/gt2rfiulmxr.html

Py:   f"{1234567:,}"
来源：http://www.ydjk.org.cn/Article/details/gt2yoaeiblt.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt2qgwffujv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2pucyeecb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt2smxweocf.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt2djiamaow.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.52xcode.cn/Article/details/gt2izbqcjou.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt2ybvuvjwd.html

C#:   1234567.ToString("N0")
来源：http://www.ydjk.org.cn/Article/details/gt2qwvrkdyl.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt2nigyxsnq.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.52xcode.cn/Article/details/gt2lissajgi.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt2zofdmnad.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt2lkqzocjk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.ydjk.org.cn/Article/details/gt2gatyqile.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.52xcode.cn/Article/details/gt2itrrtxeo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.52xcode.cn/Article/details/gt2oirclvzs.html

Ruby: s.capitalize
来源：http://www.52xcode.cn/Article/details/gt2wumekvcx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.ydjk.org.cn/Article/details/gt2niqhdwng.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt2epzruadl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.ydjk.org.cn/Article/details/gt2dmfapuaj.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.ydjk.org.cn/Article/details/gt2qliteuum.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2llxnopcm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt2bwbzqwza.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2pjvgmsla.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.52xcode.cn/Article/details/gt2cbdceenx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt2oxmsvyhs.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.52xcode.cn/Article/details/gt2nnzrwyfq.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt2nlxojger.html

Py:   s.splitlines()
来源：http://www.52xcode.cn/Article/details/gt2fkkyhzrx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.52xcode.cn/Article/details/gt2recjpwbh.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2fkdzmrrz.html

TS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt2bjxcsqqa.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt2ovdtckyj.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt2vrbjsfun.html

Ruby: s.lines
来源：http://www.52xcode.cn/Article/details/gt2kawbttfz.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt2ojxcplhr.html

[E20] 判断字符串是否为空
来源：http://www.52xcode.cn/Article/details/gt2ztizfwji.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt2rvnpwwgw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt2lfzsutgx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.ydjk.org.cn/Article/details/gt2webcmlmp.html

TS:   if (s === "") {}
来源：http://www.ydjk.org.cn/Article/details/gt2xtkonowa.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt2qtesxkja.html

Go:   if s == "" {}
来源：http://www.52xcode.cn/Article/details/gt2ilfswvqk.html

Ruby: if s.empty?
来源：http://www.ydjk.org.cn/Article/details/gt2nlvevrho.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt2xksfxmzb.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt2ysycrlnq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.ydjk.org.cn/Article/details/gt2lkdfunxq.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2pnditoag.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2gccvqdka.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2fskxgrzh.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2dlsnyncs.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt2zoykexrl.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt2ppuobieh.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt2eizsujjv.html

[E22] 字节长度与字符长度
来源：http://www.ydjk.org.cn/Article/details/gt2gdtqccvr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.52xcode.cn/Article/details/gt2uyzvyucr.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt2rrchnwzn.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt2eohhaaud.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt2fbxmpifa.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt2davwqxlv.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt2ophnednz.html

Ruby: s.bytesize;  s.length
来源：http://www.52xcode.cn/Article/details/gt2odxrxrgs.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt2zawiqkym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jwyexknn.html

F. 文件与目录
来源：http://www.52xcode.cn/Article/details/gt2xcbtbgqb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nugweymu.html

[F01] 读取整个文件
来源：http://www.ydjk.org.cn/Article/details/gt2gqchyasp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.ydjk.org.cn/Article/details/gt2fubvzqod.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2etfswqoc.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.ydjk.org.cn/Article/details/gt2ilpyprur.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2hzytdtbi.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2adcjewte.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt2rmjeiyzu.html

Ruby: File.read("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2vzhdziqw.html

C#:   File.ReadAllText("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2hbilhtof.html

[F02] 逐行读取文件
来源：http://www.ydjk.org.cn/Article/details/gt2diakghnk.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.ydjk.org.cn/Article/details/gt2dmdsohnu.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2hnuyfjyc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2ypvtkfgr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt2shanjdxp.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2gtiqjfbp.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt2ngzqspfi.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt2bgnnjhod.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt2haqsbrou.html

[F03] 写入文件（覆盖）
来源：http://www.ydjk.org.cn/Article/details/gt2zwgtbtpf.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt2uabuffkr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2fobmftzt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt2atfxhjbt.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt2wpnzmkgj.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.52xcode.cn/Article/details/gt2svjpjrmt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt2enytqpam.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt2tlemzyks.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt2kvokiesy.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt2wiasmsph.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2kjjjzzxt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt2saxluvsg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt2yzymnzjn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2dreottiq.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.52xcode.cn/Article/details/gt2dtgkqkme.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt2fishulvz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt2txahkuap.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.52xcode.cn/Article/details/gt2swmegjit.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2qzkfinen.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.ydjk.org.cn/Article/details/gt2bnceaunu.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2bpgreito.html

JS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2rattcxvk.html

TS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lnwmxfxq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt2fqnanyrn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.52xcode.cn/Article/details/gt2bhrymoei.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2fstrzkrs.html

C#:   File.Exists("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2yifqkzve.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt2bkzbjubo.html

Py:   os.remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2werzgsqf.html

PHP:  unlink("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2unixllkd.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2nwobovwg.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2imqjibgy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2ejzycrma.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2epxhejrg.html

Ruby: File.delete("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2emminpxk.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt2lokztvsq.html

[F07] 创建目录（含多级）
来源：http://www.ydjk.org.cn/Article/details/gt2monvghux.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt2wkwhushe.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt2xmvmkuji.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2taozytbh.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt2mbpmowob.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt2mkquienb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt2yowzznxv.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.52xcode.cn/Article/details/gt2ocoagjaf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt2aibuuedo.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt2mqtzyjvt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.52xcode.cn/Article/details/gt2kcsurmqj.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt2extotkwc.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2srbvedzg.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt2cqeungsh.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt2gloganev.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.ydjk.org.cn/Article/details/gt2gzkszkwq.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt2mldmgsvh.html

C#:   Directory.GetFiles("dir")
来源：http://www.52xcode.cn/Article/details/gt2igxtbkvd.html

[F09] 获取文件大小
来源：http://www.52xcode.cn/Article/details/gt2sysyobbe.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2ldbstwwq.html

PHP:  filesize("a.txt");
来源：http://www.52xcode.cn/Article/details/gt2oixclpff.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2pbliqyxa.html

TS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt2fddgahzz.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt2dxpipfqh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt2njcuhxfn.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2bikfzepy.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt2jtnuazbt.html

[F10] 取文件扩展名 / 文件名
来源：http://www.52xcode.cn/Article/details/gt2ltcztuhx.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lusqrytb.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.52xcode.cn/Article/details/gt2drmxivqk.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2lrwmwgjy.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt2wqimvdcj.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt2blxzucjo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt2gjbmotjt.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2dluldsuk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2gytmwwzl.html

[F11] 复制与移动文件
来源：http://www.ydjk.org.cn/Article/details/gt2hszxmfzc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ekgxtdro.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.52xcode.cn/Article/details/gt2udeeotqd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2ncvbfpka.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt2xgdbmybw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt2evevgxyp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt2hxgqvqed.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt2zmabpjeu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt2irhremjv.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt2qtlcinrt.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt2zqdoylaj.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.ydjk.org.cn/Article/details/gt2luzmjzpp.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.ydjk.org.cn/Article/details/gt2zbykxocl.html

TS:   // 同上
来源：http://www.ydjk.org.cn/Article/details/gt2rdscjcqf.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt2rsvcisel.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.ydjk.org.cn/Article/details/gt2hzrcxeol.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.ydjk.org.cn/Article/details/gt2njtgivlg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt2cslumclj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2aolzoknc.html

G. 面向对象
来源：http://www.52xcode.cn/Article/details/gt2yxiruwti.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zfxrdvtg.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt2lxwskjqb.html

Py:   class User: pass
来源：http://www.ydjk.org.cn/Article/details/gt2nydbvisf.html

PHP:  class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2xipdesfu.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt2vskikgps.html

TS:   class User { name: string = ""; }
来源：http://www.52xcode.cn/Article/details/gt2naslgyua.html

Java: class User {}
来源：http://www.52xcode.cn/Article/details/gt2ezrxcqpb.html

Go:   type User struct { Name string }
来源：http://www.ydjk.org.cn/Article/details/gt2txrqrdae.html

Ruby: class User; end
来源：http://www.ydjk.org.cn/Article/details/gt2ycxewafu.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt2rlxjrfol.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt2nexahetl.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt2fhqeszny.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt2iblnsgeb.html

JS:   constructor(name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2vstvyfeg.html

TS:   constructor(public name: string) {}
来源：http://www.ydjk.org.cn/Article/details/gt2vhjmvwrw.html

Java: User(String name) { this.name = name; }
来源：http://www.52xcode.cn/Article/details/gt2hnokdhln.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt2dtpblhcy.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt2nxaxuxqx.html

C#:   public User(string name) { Name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt2bjbkohto.html

[G03] 实例属性
来源：http://www.52xcode.cn/Article/details/gt2ywlvcuib.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt2mmmgjlga.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2krwfomfb.html

JS:   this.name = "x";
来源：http://www.52xcode.cn/Article/details/gt2nasmmssi.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt2solyacbq.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt2hxmjlzag.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt2rirhxjgl.html

Ruby: @name = "x"
来源：http://www.52xcode.cn/Article/details/gt2zykleurf.html

C#:   public string Name { get; set; } = "x";
来源：http://www.52xcode.cn/Article/details/gt2emjqbvfi.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt2nxvwotps.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt2qvqvaxmc.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.52xcode.cn/Article/details/gt2nzewxexa.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2yhvubwab.html

TS:   greet(): string { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt2xayqziem.html

Java: String greet() { return name; }
来源：http://www.ydjk.org.cn/Article/details/gt2ficdhtug.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt2dfmvsubg.html

Ruby: def greet; @name; end
来源：http://www.ydjk.org.cn/Article/details/gt2gmietzob.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt2avwupxoa.html

[G05] 继承
来源：http://www.ydjk.org.cn/Article/details/gt2bbornvqd.html

Py:   class Admin(User): pass
来源：http://www.52xcode.cn/Article/details/gt2cibycpmx.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2rpiampyc.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt2pmbtcuuf.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt2qtvkkqzm.html


<!-- 参考信息 -->