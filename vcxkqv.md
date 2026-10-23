代发 wailian999

C#:   s.Replace("a", "b")
来源：http://www.ydjk.org.cn/Article/details/gt3kanimnwi.html

[E07] 按分隔符拆分
来源：http://www.52xcode.cn/Article/details/gt3fpdmocyr.html

Py:   s.split(",");  s.split()      # 无参按任意空白拆
来源：http://www.52xcode.cn/Article/details/gt3kkpttuno.html

PHP:  explode(",", $s);  preg_split('/\s+/', $s);
来源：http://www.52xcode.cn/Article/details/gt3hcvrjriu.html

JS:   s.split(",");  s.split(/\s+/)
来源：http://www.ydjk.org.cn/Article/details/gt3vyffvljq.html

TS:   s.split(",")
来源：http://www.52xcode.cn/Article/details/gt3vdkpqkxv.html

Java: s.split(",");  s.split("\\s+")
来源：http://www.ydjk.org.cn/Article/details/gt3lxowlrqr.html

Go:   strings.Split(s, ",");  strings.Fields(s)
来源：http://www.ydjk.org.cn/Article/details/gt3hpwhiiez.html

Ruby: s.split(",");  s.split
来源：http://www.52xcode.cn/Article/details/gt3biqqztak.html

C#:   s.Split(',');  s.Split(new[] { ' ' }, StringSplitOptions.RemoveEmptyEntries)
来源：http://www.ydjk.org.cn/Article/details/gt3kigpuhca.html

[E08] 数组按分隔符合并
来源：http://www.ydjk.org.cn/Article/details/gt3fjxwleuz.html

Py:   ",".join(items)
来源：http://www.ydjk.org.cn/Article/details/gt3crnntcpf.html

PHP:  implode(",", $items);
来源：http://www.52xcode.cn/Article/details/gt3rhsjihmz.html

JS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3qyyygint.html

TS:   items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3flbgfdja.html

Java: String.join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3hrlhsiai.html

Go:   strings.Join(items, ",")
来源：http://www.52xcode.cn/Article/details/gt3ufocyzok.html

Ruby: items.join(",")
来源：http://www.ydjk.org.cn/Article/details/gt3udavvmbp.html

C#:   string.Join(",", items)
来源：http://www.52xcode.cn/Article/details/gt3firitdtm.html

[E09] 去除所有空白字符
来源：http://www.52xcode.cn/Article/details/gt3lxyqyvtr.html

Py:   "".join(s.split());  re.sub(r"\s+", "", s)
来源：http://www.52xcode.cn/Article/details/gt3vkqqledv.html

PHP:  preg_replace('/\s+/', '', $s);
来源：http://www.52xcode.cn/Article/details/gt3whfjlaoi.html

JS:   s.replace(/\s+/g, "")
来源：http://www.ydjk.org.cn/Article/details/gt3souhbydx.html

TS:   s.replace(/\s+/g, "")
来源：http://www.52xcode.cn/Article/details/gt3gqhgvsnv.html

Java: s.replaceAll("\\s+", "")
来源：http://www.52xcode.cn/Article/details/gt3ktsskjnb.html

Go:   strings.Join(strings.Fields(s), "")
来源：http://www.ydjk.org.cn/Article/details/gt3ahehhqch.html

Ruby: s.gsub(/\s+/, "")
来源：http://www.ydjk.org.cn/Article/details/gt3bqgvixza.html

C#:   Regex.Replace(s, @"\s+", "")
来源：http://www.ydjk.org.cn/Article/details/gt3ozwsreiu.html

[E10] 左侧补零 / 定长填充
来源：http://www.52xcode.cn/Article/details/gt3hyulaykh.html

Py:   str(7).zfill(3);  "7".rjust(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3xwrnhtma.html

PHP:  str_pad("7", 3, "0", STR_PAD_LEFT);
来源：http://www.52xcode.cn/Article/details/gt3pmmikvim.html

JS:   "7".padStart(3, "0")
来源：http://www.52xcode.cn/Article/details/gt3lngffncm.html

TS:   "7".padStart(3, "0")
来源：http://www.ydjk.org.cn/Article/details/gt3cpvanuzk.html

Java: String.format("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3hsbxumax.html

Go:   fmt.Sprintf("%03d", 7)
来源：http://www.ydjk.org.cn/Article/details/gt3vuqogida.html

Ruby: 7.to_s.rjust(3, "0");  format("%03d", 7)
来源：http://www.52xcode.cn/Article/details/gt3utnfkvuq.html

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://www.ydjk.org.cn/Article/details/gt3sgijiwbt.html

[E11] 反转字符串
来源：http://www.52xcode.cn/Article/details/gt3tkgsaugk.html

Py:   s[::-1]
来源：http://www.52xcode.cn/Article/details/gt3hrepagco.html

PHP:  strrev($s);
来源：http://www.52xcode.cn/Article/details/gt3xvhbasdd.html

JS:   [...s].reverse().join("")
来源：http://www.ydjk.org.cn/Article/details/gt3qldpdiqv.html

TS:   [...s].reverse().join("")
来源：http://www.52xcode.cn/Article/details/gt3vmeblhxd.html

Java: new StringBuilder(s).reverse().toString()
来源：http://www.ydjk.org.cn/Article/details/gt3jmafftyt.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://www.ydjk.org.cn/Article/details/gt3jrepulco.html

Ruby: s.reverse
来源：http://www.ydjk.org.cn/Article/details/gt3bdillgnv.html

C#:   new string(s.Reverse().ToArray())
来源：http://www.52xcode.cn/Article/details/gt3jemkpnjs.html

[E12] 统计某字符出现次数
来源：http://www.ydjk.org.cn/Article/details/gt3jsdeirsa.html

Py:   s.count("a")
来源：http://www.52xcode.cn/Article/details/gt3bbydkyil.html

PHP:  substr_count($s, "a");
来源：http://www.52xcode.cn/Article/details/gt3rwfazxal.html

JS:   s.split("a").length - 1
来源：http://www.ydjk.org.cn/Article/details/gt3jeljerff.html

TS:   s.split("a").length - 1
来源：http://www.52xcode.cn/Article/details/gt3bqwwuklb.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://www.52xcode.cn/Article/details/gt3lzrrmfic.html

Go:   strings.Count(s, "a")
来源：http://www.52xcode.cn/Article/details/gt3abpuyczo.html

Ruby: s.count("a")
来源：http://www.ydjk.org.cn/Article/details/gt3vycjevom.html

C#:   s.Count(c => c == 'a')
来源：http://www.ydjk.org.cn/Article/details/gt3blpxqemb.html

[E13] 逐字符遍历
来源：http://www.52xcode.cn/Article/details/gt3rwfwjcqn.html

Py:   for ch in s: print(ch)
来源：http://www.52xcode.cn/Article/details/gt3gvwhtfrp.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://www.ydjk.org.cn/Article/details/gt3iwjehmko.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3gjxnvmmw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://www.52xcode.cn/Article/details/gt3kqihaimk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://www.ydjk.org.cn/Article/details/gt3eohqnpor.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://www.52xcode.cn/Article/details/gt3kbxxnowi.html

Ruby: s.each_char { |ch| puts ch }
来源：http://www.ydjk.org.cn/Article/details/gt3mwluuutk.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://www.52xcode.cn/Article/details/gt3piqhvfaw.html

[E14] URL 编码与 Base64
来源：http://www.ydjk.org.cn/Article/details/gt3osyvpajc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://www.ydjk.org.cn/Article/details/gt3roxwkeqb.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://www.52xcode.cn/Article/details/gt3bgxbbyhh.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://www.52xcode.cn/Article/details/gt3haaaxvwc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://www.52xcode.cn/Article/details/gt3bmqugtyw.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://www.52xcode.cn/Article/details/gt3gykplolu.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://www.52xcode.cn/Article/details/gt3nyduqura.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://www.52xcode.cn/Article/details/gt3webfpdqb.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://www.ydjk.org.cn/Article/details/gt3dzupdzne.html

[E15] HTML 转义 / 反转义
来源：http://www.ydjk.org.cn/Article/details/gt3aaheaxft.html

Py:   html.escape(s);  html.unescape(s)
来源：http://www.52xcode.cn/Article/details/gt3mpdjfvur.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://www.ydjk.org.cn/Article/details/gt3dbvxmhgj.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://www.ydjk.org.cn/Article/details/gt3kqlttnuh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://www.ydjk.org.cn/Article/details/gt3snowyzpf.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://www.ydjk.org.cn/Article/details/gt3iiomlkzu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tufxdyyu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://www.52xcode.cn/Article/details/gt3oepkrwtu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qlnhgpss.html

[E16] 数字千分位
来源：http://www.52xcode.cn/Article/details/gt3myoigyzy.html

Py:   f"{1234567:,}"
来源：http://www.52xcode.cn/Article/details/gt3pbdcmngz.html

PHP:  number_format(1234567);
来源：http://www.ydjk.org.cn/Article/details/gt3xerphdzj.html

JS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3lyianbcb.html

TS:   (1234567).toLocaleString("en-US")
来源：http://www.52xcode.cn/Article/details/gt3vaykcwga.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://www.52xcode.cn/Article/details/gt3lpmpjzyu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://www.ydjk.org.cn/Article/details/gt3aklclqck.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://www.ydjk.org.cn/Article/details/gt3ukspormx.html

C#:   1234567.ToString("N0")
来源：http://www.52xcode.cn/Article/details/gt3glabhyod.html

[E17] 首字母大写
来源：http://www.ydjk.org.cn/Article/details/gt3speuzvgh.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://www.ydjk.org.cn/Article/details/gt3idxchfkm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://www.52xcode.cn/Article/details/gt3xyvbedce.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3mpxsuaxs.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://www.52xcode.cn/Article/details/gt3ciodmxpi.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://www.ydjk.org.cn/Article/details/gt3ywjgkxdc.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://www.ydjk.org.cn/Article/details/gt3uvmqfytm.html

Ruby: s.capitalize
来源：http://www.ydjk.org.cn/Article/details/gt3jgblilll.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://www.52xcode.cn/Article/details/gt3gangqdpt.html

[E18] 模板占位符替换
来源：http://www.52xcode.cn/Article/details/gt3ytqzfymr.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://www.52xcode.cn/Article/details/gt3sycqbvjt.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://www.52xcode.cn/Article/details/gt3qtayvqak.html

JS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3zjjzzlnz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://www.52xcode.cn/Article/details/gt3ylsnkwef.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3anqolclu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://www.ydjk.org.cn/Article/details/gt3cwdykrzc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://www.52xcode.cn/Article/details/gt3oemwxlyv.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://www.ydjk.org.cn/Article/details/gt3oyboqnux.html

[E19] 多行文本按行拆分
来源：http://www.52xcode.cn/Article/details/gt3jrfrbaud.html

Py:   s.splitlines()
来源：http://www.ydjk.org.cn/Article/details/gt3peygzccq.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://www.ydjk.org.cn/Article/details/gt3bzpfaqmz.html

JS:   s.split(/\r?\n/)
来源：http://www.52xcode.cn/Article/details/gt3swpyucbf.html

TS:   s.split(/\r?\n/)
来源：http://www.ydjk.org.cn/Article/details/gt3fklokymu.html

Java: s.lines().toList()
来源：http://www.ydjk.org.cn/Article/details/gt3isstvaku.html

Go:   strings.Split(s, "\n")
来源：http://www.ydjk.org.cn/Article/details/gt3dioktjed.html

Ruby: s.lines
来源：http://www.ydjk.org.cn/Article/details/gt3kymxhkum.html

C#:   s.Split('\n')
来源：http://www.ydjk.org.cn/Article/details/gt3djdzkbnq.html

[E20] 判断字符串是否为空
来源：http://www.ydjk.org.cn/Article/details/gt3akqavzir.html

Py:   if not s:
来源：http://www.ydjk.org.cn/Article/details/gt3pwelnnkx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://www.ydjk.org.cn/Article/details/gt3mchaawnd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://www.52xcode.cn/Article/details/gt3pvdsagbv.html

TS:   if (s === "") {}
来源：http://www.52xcode.cn/Article/details/gt3zzsoeuvu.html

Java: if (s.isEmpty()) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ndviiops.html

Go:   if s == "" {}
来源：http://www.ydjk.org.cn/Article/details/gt3vqsmmhnj.html

Ruby: if s.empty?
来源：http://www.52xcode.cn/Article/details/gt3ocoglexj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://www.ydjk.org.cn/Article/details/gt3ijzokjad.html

[E21] 超长截断加省略号
来源：http://www.ydjk.org.cn/Article/details/gt3bfvtfeyz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://www.52xcode.cn/Article/details/gt3plhitwfj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3mjsddyke.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3snlphvff.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3civgzuln.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3ezhfnsuf.html

Go:   // 按 rune 判断长度后截断
来源：http://www.ydjk.org.cn/Article/details/gt3jsixwdfd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://www.52xcode.cn/Article/details/gt3zewtiiqu.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://www.ydjk.org.cn/Article/details/gt3xerkuftp.html

[E22] 字节长度与字符长度
来源：http://www.52xcode.cn/Article/details/gt3llxgizhk.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://www.ydjk.org.cn/Article/details/gt3slfxyxnp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://www.52xcode.cn/Article/details/gt3czynsbsw.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3pkvfczag.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://www.52xcode.cn/Article/details/gt3blrsnbbz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://www.52xcode.cn/Article/details/gt3lvxdyhec.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://www.52xcode.cn/Article/details/gt3mdbgkxvc.html

Ruby: s.bytesize;  s.length
来源：http://www.ydjk.org.cn/Article/details/gt3zmswnmrq.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://www.52xcode.cn/Article/details/gt3vmkhkhof.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lwhbngrj.html

F. 文件与目录
来源：http://www.ydjk.org.cn/Article/details/gt3viajslar.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3orisikzp.html

[F01] 读取整个文件
来源：http://www.52xcode.cn/Article/details/gt3cecrmzym.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://www.52xcode.cn/Article/details/gt3kqybhwoz.html

PHP:  file_get_contents("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3ltbcuwrp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://www.52xcode.cn/Article/details/gt3uxoekrwe.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3tbetiwua.html

Java: Files.readString(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3gvdejuyi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://www.ydjk.org.cn/Article/details/gt3dmxzhvpu.html

Ruby: File.read("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3psxuyjbg.html

C#:   File.ReadAllText("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3leklfvyr.html

[F02] 逐行读取文件
来源：http://www.52xcode.cn/Article/details/gt3kmzbntch.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://www.52xcode.cn/Article/details/gt3ozffxgup.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3wxlpvube.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3ztmilpmc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://www.52xcode.cn/Article/details/gt3qrotethz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3twfpiudk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://www.ydjk.org.cn/Article/details/gt3clkoolbl.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://www.ydjk.org.cn/Article/details/gt3oxqoxxdi.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://www.52xcode.cn/Article/details/gt3xvcuktil.html

[F03] 写入文件（覆盖）
来源：http://www.52xcode.cn/Article/details/gt3zmggazkp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://www.52xcode.cn/Article/details/gt3mfzxaopw.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://www.52xcode.cn/Article/details/gt3bknjzqbm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.ydjk.org.cn/Article/details/gt3zlsjmuqu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://www.52xcode.cn/Article/details/gt3yahgyllp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3mynihdix.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://www.ydjk.org.cn/Article/details/gt3dyixlbjg.html

Ruby: File.write("a.txt", "hi")
来源：http://www.ydjk.org.cn/Article/details/gt3ssogclhu.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ilnqjtmm.html

[F04] 追加写入文件
来源：http://www.52xcode.cn/Article/details/gt3wfykfrdn.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3btnuyasf.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://www.52xcode.cn/Article/details/gt3wetkrrrd.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.ydjk.org.cn/Article/details/gt3jhuuwmlg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://www.52xcode.cn/Article/details/gt3udxvvrnc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://www.ydjk.org.cn/Article/details/gt3xijgkddm.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://www.52xcode.cn/Article/details/gt3xaxaynnm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://www.52xcode.cn/Article/details/gt3fspzecjy.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://www.ydjk.org.cn/Article/details/gt3zmbnvedu.html

[F05] 判断文件或目录是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3fczbnsic.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://www.52xcode.cn/Article/details/gt3izvfywag.html

PHP:  file_exists("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3tzjnmyql.html

JS:   fs.existsSync("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3vuphymzo.html

TS:   fs.existsSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jdjvvskd.html

Java: Files.exists(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3lhiprbdu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://www.ydjk.org.cn/Article/details/gt3fjgkeujs.html

Ruby: File.exist?("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3lgmvequp.html

C#:   File.Exists("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3wqcrndvi.html

[F06] 删除文件
来源：http://www.52xcode.cn/Article/details/gt3atttsofs.html

Py:   os.remove("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3aoovljwx.html

PHP:  unlink("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3gdfoyaiw.html

JS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3avnyokhq.html

TS:   fs.unlinkSync("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wublexpr.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://www.ydjk.org.cn/Article/details/gt3gydphwbh.html

Go:   os.Remove("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ctxmffzn.html

Ruby: File.delete("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3ujbzfwju.html

C#:   File.Delete("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3hvgdxxkf.html

[F07] 创建目录（含多级）
来源：http://www.52xcode.cn/Article/details/gt3proznzdr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://www.52xcode.cn/Article/details/gt3kvbxwtvp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://www.52xcode.cn/Article/details/gt3gnzopdzl.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.52xcode.cn/Article/details/gt3zzmsprot.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://www.ydjk.org.cn/Article/details/gt3iitdvebf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://www.ydjk.org.cn/Article/details/gt3ovarcdnd.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://www.52xcode.cn/Article/details/gt3urkbqbhi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://www.ydjk.org.cn/Article/details/gt3wbwaoazp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://www.ydjk.org.cn/Article/details/gt3dvsixvkz.html

[F08] 遍历目录
来源：http://www.ydjk.org.cn/Article/details/gt3egbpnqvm.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://www.ydjk.org.cn/Article/details/gt3dmrgpnrh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://www.ydjk.org.cn/Article/details/gt3aweznzlc.html

JS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3gqqkapuf.html

TS:   fs.readdirSync("dir")
来源：http://www.52xcode.cn/Article/details/gt3ykfkalzf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://www.ydjk.org.cn/Article/details/gt3tgijwper.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://www.52xcode.cn/Article/details/gt3oghxfgeg.html

Ruby: Dir.children("dir")
来源：http://www.52xcode.cn/Article/details/gt3bqumrbes.html

C#:   Directory.GetFiles("dir")
来源：http://www.ydjk.org.cn/Article/details/gt3ryasubnf.html

[F09] 获取文件大小
来源：http://www.ydjk.org.cn/Article/details/gt3vfditrmb.html

Py:   os.path.getsize("a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3lcvzrvre.html

PHP:  filesize("a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3vtkfhxmv.html

JS:   fs.statSync("a.txt").size
来源：http://www.ydjk.org.cn/Article/details/gt3lncdnlcd.html

TS:   fs.statSync("a.txt").size
来源：http://www.52xcode.cn/Article/details/gt3whfweytn.html

Java: Files.size(Path.of("a.txt"))
来源：http://www.52xcode.cn/Article/details/gt3syhbqkhj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://www.52xcode.cn/Article/details/gt3afurynpb.html

Ruby: File.size("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3jsxsrksu.html

C#:   new FileInfo("a.txt").Length
来源：http://www.52xcode.cn/Article/details/gt3oohycvmk.html

[F10] 取文件扩展名 / 文件名
来源：http://www.ydjk.org.cn/Article/details/gt3cmcwffxj.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3rkofhzdn.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3iajoscmz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3fduysawn.html

TS:   path.extname("a.txt")
来源：http://www.52xcode.cn/Article/details/gt3nnbrjkkc.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://www.ydjk.org.cn/Article/details/gt3qbsfvefo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3wtwbrbyp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3esagfaxo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://www.52xcode.cn/Article/details/gt3mqcmwthk.html

[F11] 复制与移动文件
来源：http://www.52xcode.cn/Article/details/gt3iolilvbl.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3bahewvfu.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://www.ydjk.org.cn/Article/details/gt3sikatfih.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3czieorla.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://www.ydjk.org.cn/Article/details/gt3weazjfvs.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://www.52xcode.cn/Article/details/gt3vvkzelxc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://www.52xcode.cn/Article/details/gt3dymnsfud.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://www.52xcode.cn/Article/details/gt3bcsxjhlk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://www.ydjk.org.cn/Article/details/gt3amzoaaqc.html

[F12] CSV 读写
来源：http://www.52xcode.cn/Article/details/gt3judgzkgc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://www.ydjk.org.cn/Article/details/gt3lsntsvyk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://www.52xcode.cn/Article/details/gt3dhiyikwh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://www.52xcode.cn/Article/details/gt3hgilrgxg.html

TS:   // 同上
来源：http://www.52xcode.cn/Article/details/gt3ggziznti.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://www.ydjk.org.cn/Article/details/gt3yjqdeycs.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://www.52xcode.cn/Article/details/gt3pjxhdzcs.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://www.52xcode.cn/Article/details/gt3utqqumgv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://www.ydjk.org.cn/Article/details/gt3fcixoxjc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3szsvrphy.html

G. 面向对象
来源：http://www.ydjk.org.cn/Article/details/gt3insafrsk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aqovhqhw.html

[G01] 定义类
来源：http://www.ydjk.org.cn/Article/details/gt3jzzlashb.html

Py:   class User: pass
来源：http://www.52xcode.cn/Article/details/gt3blzdwzfn.html

PHP:  class User {}
来源：http://www.52xcode.cn/Article/details/gt3ypgxtkek.html

JS:   class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3oxaqlzkh.html

TS:   class User { name: string = ""; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqnptrld.html

Java: class User {}
来源：http://www.ydjk.org.cn/Article/details/gt3viplblem.html

Go:   type User struct { Name string }
来源：http://www.52xcode.cn/Article/details/gt3wolufdzc.html

Ruby: class User; end
来源：http://www.52xcode.cn/Article/details/gt3uhjiovmn.html

C#:   class User {}
来源：http://www.52xcode.cn/Article/details/gt3atpsuhqm.html

[G02] 构造函数
来源：http://www.52xcode.cn/Article/details/gt3qqwdgcwn.html

Py:   def __init__(self, name): self.name = name
来源：http://www.ydjk.org.cn/Article/details/gt3qlhyebmt.html

PHP:  public function __construct(public string $name) {}
来源：http://www.ydjk.org.cn/Article/details/gt3fxaxvjri.html

JS:   constructor(name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3hcxyfioh.html

TS:   constructor(public name: string) {}
来源：http://www.52xcode.cn/Article/details/gt3mzhgafsy.html

Java: User(String name) { this.name = name; }
来源：http://www.ydjk.org.cn/Article/details/gt3ougyqket.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://www.ydjk.org.cn/Article/details/gt3gbwrrhuq.html

Ruby: def initialize(name); @name = name; end
来源：http://www.ydjk.org.cn/Article/details/gt3basmtkye.html

C#:   public User(string name) { Name = name; }
来源：http://www.52xcode.cn/Article/details/gt3ubbfgnic.html

[G03] 实例属性
来源：http://www.ydjk.org.cn/Article/details/gt3wpkvotcd.html

Py:   self.name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3nbuvlglx.html

PHP:  public string $name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3pjutteqa.html

JS:   this.name = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3sbwfkpnp.html

TS:   name: string = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3iokhjrae.html

Java: private String name;
来源：http://www.52xcode.cn/Article/details/gt3hdvehjdu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://www.ydjk.org.cn/Article/details/gt3vmbosbco.html

Ruby: @name = "x"
来源：http://www.ydjk.org.cn/Article/details/gt3gslgxvoq.html

C#:   public string Name { get; set; } = "x";
来源：http://www.ydjk.org.cn/Article/details/gt3iynrhdbb.html

[G04] 定义方法
来源：http://www.52xcode.cn/Article/details/gt3myqtzdan.html

Py:   def greet(self): return self.name
来源：http://www.ydjk.org.cn/Article/details/gt3gliurjyl.html

PHP:  public function greet(): string { return $this->name; }
来源：http://www.ydjk.org.cn/Article/details/gt3fwlryvzi.html

JS:   greet() { return this.name; }
来源：http://www.52xcode.cn/Article/details/gt3oktwvbja.html

TS:   greet(): string { return this.name; }
来源：http://www.ydjk.org.cn/Article/details/gt3umvsdewk.html

Java: String greet() { return name; }
来源：http://www.52xcode.cn/Article/details/gt3awosgagt.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://www.ydjk.org.cn/Article/details/gt3ydthxwhd.html

Ruby: def greet; @name; end
来源：http://www.52xcode.cn/Article/details/gt3hyquesif.html

C#:   public string Greet() => Name;
来源：http://www.52xcode.cn/Article/details/gt3iteynpfk.html

[G05] 继承
来源：http://www.52xcode.cn/Article/details/gt3nhonimae.html

Py:   class Admin(User): pass
来源：http://www.ydjk.org.cn/Article/details/gt3sspxuubp.html

PHP:  class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3hsfuakzc.html

JS:   class Admin extends User {}
来源：http://www.ydjk.org.cn/Article/details/gt3mlafrtjt.html

TS:   class Admin extends User {}
来源：http://www.52xcode.cn/Article/details/gt3erxrbqqt.html


<!-- 参考信息 -->