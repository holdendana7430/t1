代发 wailian999

JS:   [...s].reverse().join("")
来源：http://hz.ydjk.org.cn/gtirpepqpq.html

TS:   [...s].reverse().join("")
来源：http://hz.chenzaomai.com/gtboymvjyc.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.c1oappe.top/gttvgzvrou.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.c1oappe.top/gtjwhtmovx.html

Ruby: s.reverse
来源：http://hz.yongpay.top/gthsrpsthg.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.yj20258888.top/gteqjezotg.html

[E12] 统计某字符出现次数
来源：http://hz.wangshuangyany.cn/gtkssqagyk.html

Py:   s.count("a")
来源：http://hz.bjfxy.top/gtfmebvrhe.html

PHP:  substr_count($s, "a");
来源：http://hz.andypj.xyz/gtbokxmlfc.html

JS:   s.split("a").length - 1
来源：http://hz.jinqigufen.top/gtimjfnxve.html

TS:   s.split("a").length - 1
来源：http://hz.yonumen.top/gthrlbklje.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.ydjk.org.cn/gtnahcylsv.html

Go:   strings.Count(s, "a")
来源：http://hz.52xcode.cn/gtablmesef.html

Ruby: s.count("a")
来源：http://hz.gzhubu.top/gttuqcyanb.html

C#:   s.Count(c => c == 'a')
来源：http://hz.xylfe.cn/gtrdlvfhns.html

[E13] 逐字符遍历
来源：http://hz.ydzc1.top/gtrsrbpwau.html

Py:   for ch in s: print(ch)
来源：http://hz.zhoulong.xyz/gtmvaxityk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.hnqzz.top/gtmeoewwve.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jinqigfzy.top/gtximfpxed.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.nwbrower.top/gteawsgxzn.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.birdmap.top/gtltueaotv.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.cdnleiting.top/gtaqldgwoz.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.ivvv.top/gtvwauqxla.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yuxming.cn/gthpclryjc.html

[E14] URL 编码与 Base64
来源：http://hz.ybcxt.top/gtvuqiyrlf.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.hfpthk.cn/gtflyawifl.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.zhongyouzk.top/gtivuhspxo.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.sysykeji.top/gtbrblxbyz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.sysykeji.top/gtwfiouqmo.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yvedp.cn/gtddzhetdk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zhongyouzk.top/gtsmfoaapj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.ywan-chungtsiang.top/gtykkhzmkc.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.hongshengwenyu.top/gtnevzliyo.html

[E15] HTML 转义 / 反转义
来源：http://hz.guowangkeji.top/gtwgagtmdv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.mhx1999.top/gtyhiwyzby.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yuxming.cn/gtftsemgdw.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.daxiang520.top/gtatubvgcl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.snrcjt.cn/gtmpsudvlm.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yanxiufei.cn/gtmvctrfer.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.gogol.net.cn/gttpqznoms.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.hysaishi.cn/gttdvlaohe.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.chenlongwang.top/gtbvgcjzsz.html

[E16] 数字千分位
来源：http://hz.guowangkeji.top/gtemmoqete.html

Py:   f"{1234567:,}"
来源：http://hz.snrcjt.cn/gtsnaatsju.html

PHP:  number_format(1234567);
来源：http://hz.yonumen.top/gtjlwistho.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.quarkkingdee.top/gtktcfmrmk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.xuetiantiany.cn/gtlcwnaumr.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.guannengcc.top/gtfdbivvoe.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.ydjk.org.cn/gtdgmcfgoy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.jqgfzy.top/gtuopdctaq.html

C#:   1234567.ToString("N0")
来源：http://hz.fzhhl.top/gteawhnrhf.html

[E17] 首字母大写
来源：http://hz.gogol.net.cn/gtmkuhanea.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.smart0.xyz/gtsmvyujgf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.pengpengdd.cyou/gtlfvilzlf.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.fzhhl.top/gtidokwacj.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xylfe.cn/gtxkardemq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.xingfuxueyuan.xyz/gtrjqcejmk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.nanxinkj.top/gtflxiyzsi.html

Ruby: s.capitalize
来源：http://hz.yj20258888.top/gtccbaxqmk.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yanxiufei.cn/gtkvpddmov.html

[E18] 模板占位符替换
来源：http://hz.gaohongyu789.top/gtijpbgxeu.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.zhoulong.xyz/gtgayfzqyl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.chenzaomai.com/gtnxwcstpq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.vqdsnc.cn/gtvilplggf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.hfpthk.cn/gtcjdncioe.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.sufxvd.cn/gtcigmqqjr.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.sufxvd.cn/gtmmjxriiw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.gogol.net.cn/gtfwbefoif.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.52xcode.cn/gtzxojsnuf.html

[E19] 多行文本按行拆分
来源：http://hz.yongpay.top/gtzfafpumc.html

Py:   s.splitlines()
来源：http://hz.guannengcc.top/gtpkmmhkmh.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jinyuanbaomall.cn/gtpxrrqwzg.html

JS:   s.split(/\r?\n/)
来源：http://hz.cqqwz.cn/gtlnkewbnf.html

TS:   s.split(/\r?\n/)
来源：http://hz.jianghu66.top/gttxvgifhz.html

Java: s.lines().toList()
来源：http://hz.hfpthk.cn/gtyfaxzxjc.html

Go:   strings.Split(s, "\n")
来源：http://hz.jinyuanbaomall.cn/gtgjfjapvt.html

Ruby: s.lines
来源：http://hz.316326.xyz/gtvnyevxkj.html

C#:   s.Split('\n')
来源：http://hz.nwbrower.top/gtbdwmtwnw.html

[E20] 判断字符串是否为空
来源：http://hz.cdnleiting.top/gtjmgvornt.html

Py:   if not s:
来源：http://hz.cqqwz.cn/gtmiqwggce.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.gotoacloud.top/gtlmdvglcb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.sweek.top/gtxajkghmj.html

TS:   if (s === "") {}
来源：http://hz.ivvv.top/gtmzhugjnu.html

Java: if (s.isEmpty()) {}
来源：http://hz.9152youxi.cn/gtejyjiryq.html

Go:   if s == "" {}
来源：http://hz.nanxinkj.top/gtbgzipfxw.html

Ruby: if s.empty?
来源：http://hz.xuetiantiany.cn/gtsstillnx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.yuxming.cn/gttlijjcrw.html

[E21] 超长截断加省略号
来源：http://hz.yj20258.top/gtavruaxoe.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zdqjudy.top/gthylgfrac.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zdqjudy.top/gtovezacpb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.feifeiyinyue.top/gtqzvgbkse.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.smart0.xyz/gtewiqbmpd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.gaohongyu789.top/gtqizxveys.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jianghu66.top/gtpcqhiqru.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.wangdashe.top/gtjbngjsas.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.shanyushiyangtech.top/gtcdwbyxsk.html

[E22] 字节长度与字符长度
来源：http://hz.chenzaomai.com/gtsehlmggm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.chenjidiqi.icu/gtifkjcmbe.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.snrcjt.cn/gtzbdizqsv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhoulong.xyz/gtwnvaeuoz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hfpthk.cn/gtvjbyqwgy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.gzhubu.top/gtoseemqlb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.ydjk.org.cn/gtpynnlana.html

Ruby: s.bytesize;  s.length
来源：http://hz.yuanzhike.top/gtofpruhca.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yanxiufei.cn/gtttouoctz.html

================================================================================
来源：http://hz.cheryme.top/gtgicvdfgz.html

F. 文件与目录
来源：http://hz.ehwqpu.com/gtoqvqmvkn.html

================================================================================
来源：http://hz.52xcode.cn/gtynhlolpf.html

[F01] 读取整个文件
来源：http://hz.snrcjt.cn/gtljmhfpul.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jlsjyb.cn/gtvtdkekis.html

PHP:  file_get_contents("a.txt");
来源：http://hz.c1oappe.top/gtlghksyit.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jlsjyb.cn/gtcilajhgq.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yvedp.cn/gtxilokefh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.gogol.net.cn/gtwriqgmof.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.cheryme.top/gtjrzhewkb.html

Ruby: File.read("a.txt")
来源：http://hz.haohaochexian.top/gtqxsazrif.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jlsjyb.cn/gtzbwtnbxv.html

[F02] 逐行读取文件
来源：http://hz.hfpthk.cn/gtbhharwto.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yvedp.cn/gtqxlyvmyn.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jianghu66.top/gtfdtcksas.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhaomingkeji.xyz/gtmqiytmok.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.nwbrower.top/gtrqhsooak.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.aizwys.cn/gtbyinxlen.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.hnqzz.top/gtwyssuufa.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.dianchejie.cn/gtilnlbhbo.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.hongshengwenyu.top/gtennxabur.html

[F03] 写入文件（覆盖）
来源：http://hz.quarkkingdee.top/gtirvdoinp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yuxming.cn/gtmvpbfyyt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.chenlongwang.top/gtzwznynvj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jlsjyb.cn/gtklfpdpqz.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.aibaodan.cn/gtjbvywlmp.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jlsjyb.cn/gtrgvndnjh.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.daria6918.cn/gtsdnocvdl.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.dianchejie.cn/gtyilgeyls.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.guowangkeji.top/gttbuyzgtc.html

[F04] 追加写入文件
来源：http://hz.andypj.xyz/gtlrogrssp.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.nwbrower.top/gtgvdrcljg.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.birdmap.top/gtzhkjxjta.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yuanzhike.top/gtxzsamjjd.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.nanxinkj.top/gtxgjrbbub.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.dashuyun.cn/gttjinvmcj.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.wangshuangyany.cn/gtoaoibfhr.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.haohaochexian.top/gtknbxhzhh.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.havefunace.top/gtknedurky.html

[F05] 判断文件或目录是否存在
来源：http://hz.nwbrower.top/gtmgbifmdd.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zhengqikj.top/gtfcvdlvbb.html

PHP:  file_exists("a.txt");
来源：http://hz.hongshengwenyu.top/gtnmbnnewj.html

JS:   fs.existsSync("a.txt")
来源：http://hz.guannengcc.top/gtxlvaxlid.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yj20258.top/gtxxiyjnqp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zhaomingkeji.xyz/gtyaxtkudf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jiagoushi.top/gtsdezwuqc.html

Ruby: File.exist?("a.txt")
来源：http://hz.tian-w.cn/gtsaaslksi.html

C#:   File.Exists("a.txt")
来源：http://hz.yueranfly.top/gtfwnlbfco.html

[F06] 删除文件
来源：http://hz.chenjidiqi.icu/gtljrlcuhj.html

Py:   os.remove("a.txt")
来源：http://hz.9152youxi.cn/gtthvuwruk.html

PHP:  unlink("a.txt");
来源：http://hz.shanyushiyangtech.top/gtgwialfzx.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.mhx1999.top/gtewsdnayz.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.iojbl.cn/gttstrdrbj.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.cqqwz.cn/gttokyldop.html

Go:   os.Remove("a.txt")
来源：http://hz.yuanzhike.top/gtrzdecyru.html

Ruby: File.delete("a.txt")
来源：http://hz.chenjidiqi.icu/gtfjcjpyal.html

C#:   File.Delete("a.txt");
来源：http://hz.zhiwuduotai.top/gtxycjlesx.html

[F07] 创建目录（含多级）
来源：http://hz.dianchejie.cn/gthhkkqvyg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.nwbrower.top/gthbbrmltl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.9152youxi.cn/gtaurhfgur.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.haohaochexian.top/gtlgorcdir.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hongshengwenyu.top/gtxcgpfnup.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.ehwqpu.com/gtwrmjbcfb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.cashguo.top/gtcpnpdbdc.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.guannengcc.top/gtmixzblik.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.hnxiangtu.top/gtkpxkwclb.html

[F08] 遍历目录
来源：http://hz.feifeiyinyue.top/gtglkvooqr.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xuetiantiany.cn/gtyzgqsqsb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jinyuanbaomall.cn/gtwimhemmb.html

JS:   fs.readdirSync("dir")
来源：http://hz.yj20258.top/gtrjbmksrm.html

TS:   fs.readdirSync("dir")
来源：http://hz.cucudq.cn/gtxzyjryvb.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.hnqzz.top/gtigtefxho.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.jiagoushi.top/gtkmvcfknl.html

Ruby: Dir.children("dir")
来源：http://hz.hnxiangtu.top/gtxsawltjx.html

C#:   Directory.GetFiles("dir")
来源：http://hz.cdnleiting.top/gtfuzwawof.html

[F09] 获取文件大小
来源：http://hz.xuanzx.com/gtxwdgobhw.html

Py:   os.path.getsize("a.txt")
来源：http://hz.316326.xyz/gtyeqctbkh.html

PHP:  filesize("a.txt");
来源：http://hz.cucudq.cn/gtcrhdqtcg.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yuxming.cn/gtorllbkup.html

TS:   fs.statSync("a.txt").size
来源：http://hz.xinyue.icu/gtagaucngz.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ydzc1.top/gtoahvdook.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hfpthk.cn/gtjdtrmvro.html

Ruby: File.size("a.txt")
来源：http://hz.dianchejie.cn/gtboakwynt.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zhongyouzk.top/gtjtxtfsbv.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.shangyingyoupin.top/gtioqadjhq.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.havefunace.top/gtjiomaiui.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.hfpthk.cn/gtsdvyannn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.sweek.top/gtljdhaxkh.html

TS:   path.extname("a.txt")
来源：http://hz.yuxming.cn/gtbxjltdvg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.bjfxy.top/gtudqxsabx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.ivvv.top/gtvlnfdfwn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.redwolf501.top/gtldtmlyjr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.aibaodan.cn/gtvoqvrphq.html

[F11] 复制与移动文件
来源：http://hz.zhengqikj.top/gtbynwatve.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.dashuyun.cn/gtsxnvdyhz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hfpthk.cn/gttqujivqg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gotoacloud.top/gtuzumqnss.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yongpay.top/gtitwlzyvu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.hnqzz.top/gtsrhflgqo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yueranfly.top/gtukxnflxl.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.quarkkingdee.top/gtxgbukcjz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.gzhubu.top/gtlshlwkgf.html

[F12] CSV 读写
来源：http://hz.tanke756.top/gteudgdlou.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.sysykeji.top/gtlgvmzmql.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.smart0.xyz/gtxluemjws.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.meibo888.top/gtyywlgsrb.html

TS:   // 同上
来源：http://hz.jianghu66.top/gtglcytxjz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.shangyingyoupin.top/gtykghcywi.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.yangfankeji.com/gtianhhjpc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yj20258888.top/gtskgyqgze.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.c1oappe.top/gtwucybdca.html

================================================================================
来源：http://hz.guannengcc.top/gtuzyluppv.html

G. 面向对象
来源：http://hz.ydzc1.top/gtlyolnhhg.html

================================================================================
来源：http://hz.nwbrower.top/gttlhwnptc.html

[G01] 定义类
来源：http://hz.yvedp.cn/gtkfmcitlc.html

Py:   class User: pass
来源：http://hz.aibaodan.cn/gtglrlcevc.html

PHP:  class User {}
来源：http://hz.cashguo.top/gtrpokypgu.html

JS:   class User {}
来源：http://hz.andypj.xyz/gtmyvzjesp.html

TS:   class User { name: string = ""; }
来源：http://hz.jqgfzy.top/gtiyvistcg.html

Java: class User {}
来源：http://hz.quarkkingdee.top/gtgsvxfrfs.html

Go:   type User struct { Name string }
来源：http://hz.shangyingyoupin.top/gtvqvznqmc.html

Ruby: class User; end
来源：http://hz.jinghuilouyu.cn/gtqmwkzuoy.html

C#:   class User {}
来源：http://hz.shuidangran.top/gtfgxpsknn.html

[G02] 构造函数
来源：http://hz.tanke756.top/gtdrjuocin.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jiagoushi.top/gtwsxskhrc.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.tian-w.cn/gthgutwody.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yj20258.top/gtwfldselz.html

TS:   constructor(public name: string) {}
来源：http://hz.snrcjt.cn/gtdgwftyqm.html

Java: User(String name) { this.name = name; }
来源：http://hz.ydjk.org.cn/gteaqbfwot.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.fengsongda.top/gtcicwposl.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yuxming.cn/gtqhtcdhjr.html

C#:   public User(string name) { Name = name; }
来源：http://hz.xylfe.cn/gtsbnszayp.html

[G03] 实例属性
来源：http://hz.yvedp.cn/gtkgrdifsh.html

Py:   self.name = "x"
来源：http://hz.aibaodan.cn/gtomrtdwqq.html

PHP:  public string $name = "x";
来源：http://hz.ydzc1.top/gtkvinunkf.html

JS:   this.name = "x";
来源：http://hz.fzhhl.top/gtpznvhfez.html

TS:   name: string = "x";
来源：http://hz.zdqjudy.top/gtjsmsqcvn.html

Java: private String name;
来源：http://hz.yvedp.cn/gtfstoewly.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zhixingplan.top/gtttkdjtti.html

Ruby: @name = "x"
来源：http://hz.hnxiangtu.top/gtvqwxcugt.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zhengqikj.top/gtdyuyhxem.html

[G04] 定义方法
来源：http://hz.shuidangran.top/gtnskgsfgd.html

Py:   def greet(self): return self.name
来源：http://hz.yongpay.top/gteiqptdlf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.haohaochexian.top/gtoturzrch.html

JS:   greet() { return this.name; }
来源：http://hz.feifeiyinyue.top/gtnodorzer.html

TS:   greet(): string { return this.name; }
来源：http://hz.nanxuanxn.top/gtfhcaokre.html

Java: String greet() { return name; }
来源：http://hz.ehwqpu.com/gtpobcrxdn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jiagoushi.top/gtqhdndazw.html

Ruby: def greet; @name; end
来源：http://hz.hnqzz.top/gtvdoudbyl.html

C#:   public string Greet() => Name;
来源：http://hz.sufxvd.cn/gtcihaqfke.html

[G05] 继承
来源：http://hz.hongshengwenyu.top/gtqcsnskas.html

Py:   class Admin(User): pass
来源：http://hz.316326.xyz/gtsqtuxphr.html

PHP:  class Admin extends User {}
来源：http://hz.tanke756.top/gtpqbcmvli.html

JS:   class Admin extends User {}
来源：http://hz.zhengqikj.top/gtqawgwsqy.html

TS:   class Admin extends User {}
来源：http://hz.gzhubu.top/gtaoyxdfol.html

Java: class Admin extends User {}
来源：http://hz.hongshengwenyu.top/gtjhrnoltx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ppjwa.cn/gtxxvxwsno.html

Ruby: class Admin < User; end
来源：http://hz.yvedp.cn/gtvdkqzyoo.html

C#:   class Admin : User {}
来源：http://hz.daxiang520.top/gtftpfvmyj.html

[G06] 重写方法
来源：http://hz.hnxiangtu.top/gtcdmbqwxt.html

Py:   def greet(self): return "admin"
来源：http://hz.jinyuanbaomall.cn/gtculkzuqk.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.nanxinkj.top/gtzxrpazjc.html

JS:   greet() { return "admin"; }
来源：http://hz.yonumen.top/gtrlwpnmsz.html

TS:   greet(): string { return "admin"; }
来源：http://hz.xylfe.cn/gtrnsfjlny.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhengqikj.top/gtvtphbbyx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.shanyushiyangkeji.top/gtnvhfoded.html

Ruby: def greet; "admin"; end
来源：http://hz.chenlongwang.top/gtwprlhkzt.html

C#:   public override string Greet() => "admin";
来源：http://hz.gzhubu.top/gtwgntnncy.html

[G07] 调用父类方法
来源：http://hz.hywenlv.cn/gteuunlcrt.html

Py:   super().greet()
来源：http://hz.shzxlz.cn/gthrsgzmkh.html

PHP:  parent::greet();
来源：http://hz.pycfn.com/gtbmvytslj.html

JS:   super.greet();
来源：http://hz.xylfe.cn/gtqurrkgco.html

TS:   super.greet();
来源：http://hz.snrcjt.cn/gtsmofhezs.html

Java: super.greet();
来源：http://hz.yueranfly.top/gtdvvbgvyf.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.cucudq.cn/gtspdcxtnu.html

Ruby: super
来源：http://hz.xinyue.icu/gtppkychqm.html

C#:   base.Greet();
来源：http://hz.hnxiangtu.top/gtlxnjrtft.html

[G08] 静态方法与属性
来源：http://hz.jqgfzy.top/gtpsybacnz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.gogol.net.cn/gtgzbajmqh.html

PHP:  public static function f() {}
来源：http://hz.zhoulong.xyz/gtqxlfhixi.html

JS:   static f() {}
来源：http://hz.chenjidiqi.icu/gtsoafzenx.html

TS:   static f(): void {}
来源：http://hz.zhongyouzk.top/gtbjnjmmob.html

Java: static void f() {}
来源：http://hz.yangfankeji.com/gttwbusect.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.dashuyun.cn/gttvfcoszx.html

Ruby: def self.f; end
来源：http://hz.shanyushiyangtech.top/gtvoxvikmk.html

C#:   public static void F() {}
来源：http://hz.xylfe.cn/gtqldylgij.html

[G09] 接口 / 抽象类
来源：http://hz.birdmap.top/gttjsgfdzy.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ywan-chungtsiang.top/gtbquwljlp.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.9152youxi.cn/gtpllneylh.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.tianlin.xyz/gtodhzpudd.html

TS:   interface Shape { area(): number; }
来源：http://hz.jyoumei.cn/gtptguentr.html

Java: interface Shape { double area(); }
来源：http://hz.jyoumei.cn/gtpfvaeewm.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yj20258888.top/gtbglgmscx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.xuetiantiany.cn/gtkknovrng.html

C#:   interface IShape { double Area(); }
来源：http://hz.daxiang520.top/gtekjuinxs.html


<!-- 参考信息 -->