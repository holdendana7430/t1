代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.sufxvd.cn/gtjkxqjkgv.html

[E11] 反转字符串
来源：http://hz.shangyingyoupin.top/gtvvtwhovd.html

Py:   s[::-1]
来源：http://hz.zhongyouzk.top/gtapijamlx.html

PHP:  strrev($s);
来源：http://hz.yongpay.top/gtvhezuguj.html

JS:   [...s].reverse().join("")
来源：http://hz.hammf.cn/gtzellebjx.html

TS:   [...s].reverse().join("")
来源：http://hz.ydjk.org.cn/gtckluzyrb.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.aibaodan.cn/gtrnzilzda.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.jinghuilouyu.cn/gtuxbeobvq.html

Ruby: s.reverse
来源：http://hz.chenjidiqi.icu/gtmpvlrnsg.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.nanxuanxn.top/gtfhwemref.html

[E12] 统计某字符出现次数
来源：http://hz.quarkkingdee.top/gtiuffsiev.html

Py:   s.count("a")
来源：http://hz.birdmap.top/gtduvgwwvz.html

PHP:  substr_count($s, "a");
来源：http://hz.sysykeji.top/gtmmpzjlks.html

JS:   s.split("a").length - 1
来源：http://hz.vqdsnc.cn/gtpumvlnkl.html

TS:   s.split("a").length - 1
来源：http://hz.shanyushiyangkeji.top/gtqhrogcbn.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.xinyue.icu/gtmaqzkatu.html

Go:   strings.Count(s, "a")
来源：http://hz.yuxming.cn/gtvxfyoghc.html

Ruby: s.count("a")
来源：http://hz.redwolf501.top/gtdnytfjdl.html

C#:   s.Count(c => c == 'a')
来源：http://hz.snrcjt.cn/gtfvmwzutu.html

[E13] 逐字符遍历
来源：http://hz.jqgufenzy.top/gtqlgogsjh.html

Py:   for ch in s: print(ch)
来源：http://hz.aizwys.cn/gtyzwrjasv.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.quarkkingdee.top/gtslcargxy.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.sufxvd.cn/gttekfulga.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hywenlv.cn/gtpkmltjhk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.hywenlv.cn/gtiumaxrqr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.ehwqpu.com/gtltyieufc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jlsjyb.cn/gtemseyuij.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.ydzc1.top/gtdwrikkvv.html

[E14] URL 编码与 Base64
来源：http://hz.0kj1m.cn/gtbfanvjqx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zhiwuduotai.top/gtgmydowtr.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.hnqzz.top/gtodgabrgl.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.tian-w.cn/gtpgzfafzu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yvedp.cn/gttlzyhoti.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.birdmap.top/gtowjndsoj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.guannengcc.top/gtvrlcrlur.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.aibaodan.cn/gtievqnpxy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.svipenyu.cn/gtooefvfcl.html

[E15] HTML 转义 / 反转义
来源：http://hz.yangfankeji.com/gtvejrapdi.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.feifeiyinyue.top/gtzhvbzagr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.zhoulong.xyz/gtlqhjwxfo.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.zycfv.cn/gttbrouaum.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zdqjudy.top/gtnwbmsvyk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.dashuyun.cn/gtcopkjbhl.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yj20258.top/gtczgknxly.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yonumen.top/gtdqgondxt.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zdqjudy.top/gtyeykomfa.html

[E16] 数字千分位
来源：http://hz.iojbl.cn/gtaljygwle.html

Py:   f"{1234567:,}"
来源：http://hz.zdqjudy.top/gtolyhxoca.html

PHP:  number_format(1234567);
来源：http://hz.fzhhl.top/gtarjuxele.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.shzxlz.cn/gtiuqyiqow.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yanxiufei.cn/gtelnrxvmo.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.dianchejie.cn/gtzjhhjhcl.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.xingfuxueyuan.xyz/gtuwsrvcdn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.jyoumei.cn/gteqowjayb.html

C#:   1234567.ToString("N0")
来源：http://hz.smart0.xyz/gttgjnjhvz.html

[E17] 首字母大写
来源：http://hz.zhongyouzk.top/gtldhoaieo.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.shuidangran.top/gtmygibwbe.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jianghu66.top/gtrtjwohts.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ydzc1.top/gtfommebqq.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhijiandao.cn/gtihogjafx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.dianchejie.cn/gtvxlcizdt.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.aibaodan.cn/gtuswkmzrw.html

Ruby: s.capitalize
来源：http://hz.dashuyun.cn/gtatkxhkfh.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.gotoacloud.top/gtzgtdfnhj.html

[E18] 模板占位符替换
来源：http://hz.cucudq.cn/gtmjlwehlk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.hammf.cn/gtpntimuun.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.guannengcc.top/gtttpnohto.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhijiandao.cn/gtluushnuy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.haohaochexian.top/gtasteonrv.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.xuetiantiany.cn/gtujxvsdmd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.bjfxy.top/gtgbicqjpk.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.gaohongyu789.top/gtfjngnoao.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.ppjwa.cn/gtlsibwhof.html

[E19] 多行文本按行拆分
来源：http://hz.zhoulong.xyz/gtrygjwtyy.html

Py:   s.splitlines()
来源：http://hz.jqgfzy.top/gtsynrsinn.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.tianlin.xyz/gtlmbvggpl.html

JS:   s.split(/\r?\n/)
来源：http://hz.guannengcc.top/gtwposzaip.html

TS:   s.split(/\r?\n/)
来源：http://hz.jiagoushi.top/gtzzahijaf.html

Java: s.lines().toList()
来源：http://hz.nwbrower.top/gtrzjaitnd.html

Go:   strings.Split(s, "\n")
来源：http://hz.shuidangran.top/gtkrqzggav.html

Ruby: s.lines
来源：http://hz.yuanzhike.top/gtyybezxpn.html

C#:   s.Split('\n')
来源：http://hz.shuidangran.top/gtabuusren.html

[E20] 判断字符串是否为空
来源：http://hz.shzxlz.cn/gtwgllfnqu.html

Py:   if not s:
来源：http://hz.zhijiandao.cn/gtdfhmkqqe.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.fengsongda.top/gtgpmvkeii.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.ydjk.org.cn/gtjtnnrisq.html

TS:   if (s === "") {}
来源：http://hz.shuidangran.top/gtaxivcuvs.html

Java: if (s.isEmpty()) {}
来源：http://hz.kuanghao11.cn/gtbhybfwlp.html

Go:   if s == "" {}
来源：http://hz.sysykeji.top/gtdudjcigd.html

Ruby: if s.empty?
来源：http://hz.snrcjt.cn/gtgwhaoxzk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.cucudq.cn/gtyxkmxnvo.html

[E21] 超长截断加省略号
来源：http://hz.c1oappe.top/gtompqxcco.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.daria6918.cn/gtfwyksdcp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.chenlongwang.top/gtkcitulff.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.smart0.xyz/gtzuzukrck.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.nwbrower.top/gtojsboyfp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.guowangkeji.top/gtdmukxgmu.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.daxiang520.top/gtgpwbmswy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.ppjwa.cn/gtsjgzonpn.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.c1oappe.top/gtfselqjit.html

[E22] 字节长度与字符长度
来源：http://hz.andypj.xyz/gtjdasbcov.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.sxryk.cn/gtkfpbgpqy.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.52xcode.cn/gtinkehtyk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.redwolf501.top/gtbexqutsm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shanyushiyangkeji.top/gtqufjdybj.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yuanzhike.top/gtlgvuqlop.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.meibo888.top/gthkrzvozp.html

Ruby: s.bytesize;  s.length
来源：http://hz.daxiang520.top/gtncromgmo.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.guannengcc.top/gtsfrjhfpq.html

================================================================================
来源：http://hz.gotoacloud.top/gtzlpjtbzm.html

F. 文件与目录
来源：http://hz.jianghu66.top/gtoxuxfbpe.html

================================================================================
来源：http://hz.hammf.cn/gtxjdlhwsf.html

[F01] 读取整个文件
来源：http://hz.dashuyun.cn/gtekvlcrkj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.zhengqikj.top/gtawgytxxt.html

PHP:  file_get_contents("a.txt");
来源：http://hz.birdmap.top/gtdcofifxl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yanxiufei.cn/gtcdzlidev.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.hammf.cn/gtnwkqaevu.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jqgufenzy.top/gtqsjmtrux.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.tanke756.top/gtwagauguh.html

Ruby: File.read("a.txt")
来源：http://hz.fzhhl.top/gtibarnxwp.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.feifeiyinyue.top/gtiaqsrxyc.html

[F02] 逐行读取文件
来源：http://hz.vqdsnc.cn/gtuornjwah.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jqgfzy.top/gtpcmcttjp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.zhiwuduotai.top/gtbglylvjc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.316326.xyz/gtlrrguill.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhixingplan.top/gtwzijlpdm.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.andypj.xyz/gtfsqhthns.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jinqigufen.top/gtcmeahbbj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.dianchejie.cn/gtrhoyiwlf.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jinyuanbaomall.cn/gthgvycavj.html

[F03] 写入文件（覆盖）
来源：http://hz.jiagoushi.top/gthmaplkbd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.xuetiantiany.cn/gtwavtfsjs.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.gotoacloud.top/gtvhknnzwp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.snrcjt.cn/gtspbtheug.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hnqzz.top/gtrildlwok.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.kuanghao11.cn/gtoxbmhezj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.vqdsnc.cn/gtdjwvlvch.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jianghu66.top/gteipdgqev.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yj20258.top/gtvhiuliuf.html

[F04] 追加写入文件
来源：http://hz.aizwys.cn/gtojfaaozl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.guowangkeji.top/gtiknmxopo.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.shanyushiyangkeji.top/gtcwnlvhep.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.pengpengdd.cyou/gtgqxsrszi.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.smart0.xyz/gtswlapibl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.sysykeji.top/gttbbcpewi.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.chenjidiqi.icu/gthouyiazd.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.52xcode.cn/gtwhnicngo.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.cucudq.cn/gtqdzufkje.html

[F05] 判断文件或目录是否存在
来源：http://hz.aizwys.cn/gtmcvxrbfo.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.mhx1999.top/gtjgqjloyc.html

PHP:  file_exists("a.txt");
来源：http://hz.sysykeji.top/gthmfovtli.html

JS:   fs.existsSync("a.txt")
来源：http://hz.xuanzx.com/gtkaaxnrrv.html

TS:   fs.existsSync("a.txt")
来源：http://hz.gaohongyu789.top/gtephzbfkc.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.ppjwa.cn/gtpjgrmseb.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.sysykeji.top/gtxlyvdacv.html

Ruby: File.exist?("a.txt")
来源：http://hz.guannengcc.top/gtywresiqp.html

C#:   File.Exists("a.txt")
来源：http://hz.0kj1m.cn/gtrfpbtngh.html

[F06] 删除文件
来源：http://hz.cucudq.cn/gtyjeuzbkj.html

Py:   os.remove("a.txt")
来源：http://hz.svipenyu.cn/gtdcwccpha.html

PHP:  unlink("a.txt");
来源：http://hz.smart0.xyz/gtjfjuypyz.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.feifeiyinyue.top/gtvtxjcpws.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.cucudq.cn/gtcggukiks.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jiagoushi.top/gthhryyuau.html

Go:   os.Remove("a.txt")
来源：http://hz.316326.xyz/gtsjtxauaj.html

Ruby: File.delete("a.txt")
来源：http://hz.hnqzz.top/gtqvjnbznx.html

C#:   File.Delete("a.txt");
来源：http://hz.gzhubu.top/gtzkpbdrmo.html

[F07] 创建目录（含多级）
来源：http://hz.yj20258888.top/gtxgcwlvba.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.chenzaomai.com/gtbysnwngr.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jlsjyb.cn/gtxbdfefcx.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.nanxuanxn.top/gtxozduopa.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.chenlongwang.top/gtddnhbhhl.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.dianchejie.cn/gtzplxnlle.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hongshengwenyu.top/gtmkrribeg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yonumen.top/gtfblptomn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.hnxiangtu.top/gtzfnrxsno.html

[F08] 遍历目录
来源：http://hz.sysykeji.top/gtsqijknzc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.kuanghao11.cn/gtmjlynfux.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.chenlongwang.top/gtjxlbpsfb.html

JS:   fs.readdirSync("dir")
来源：http://hz.jinghuilouyu.cn/gtocxinmav.html

TS:   fs.readdirSync("dir")
来源：http://hz.sxryk.cn/gtfuhtlktj.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.hnqzz.top/gtrjwzuxam.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.vqdsnc.cn/gtgbmtoofm.html

Ruby: Dir.children("dir")
来源：http://hz.zhengqikj.top/gtdgeyrisf.html

C#:   Directory.GetFiles("dir")
来源：http://hz.redwolf501.top/gtludjprsd.html

[F09] 获取文件大小
来源：http://hz.daria6918.cn/gtuajpbpwk.html

Py:   os.path.getsize("a.txt")
来源：http://hz.ppjwa.cn/gtrhuokrxr.html

PHP:  filesize("a.txt");
来源：http://hz.jiagoushi.top/gtwbzcbunf.html

JS:   fs.statSync("a.txt").size
来源：http://hz.daria6918.cn/gtzsdcbjuy.html

TS:   fs.statSync("a.txt").size
来源：http://hz.shzxlz.cn/gtzryorpvy.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.shanyushiyangtech.top/gtbbiktkmg.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.dianchejie.cn/gtgbdrauek.html

Ruby: File.size("a.txt")
来源：http://hz.hammf.cn/gteenbvczc.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jinyuanbaomall.cn/gtsrbgusel.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jqgufenzy.top/gtsbkuyvcy.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.gzhubu.top/gtfdrhnfaw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yongpay.top/gteagodybm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.hongshengwenyu.top/gtnmihchhg.html

TS:   path.extname("a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtkxueyrge.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jlsjyb.cn/gtnpqgovdb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.cheryme.top/gtilqswmve.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jinghuilouyu.cn/gtlcxqmvwk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.xuetiantiany.cn/gtyeykqbfs.html

[F11] 复制与移动文件
来源：http://hz.aibaodan.cn/gtsfsoceaw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.ivvv.top/gtpibkdzpb.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.svipenyu.cn/gtttgagdjt.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.c1oappe.top/gtdacafetj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.dashuyun.cn/gtvaxtkqvb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jqgufenzy.top/gtomlnvncs.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.bjfxy.top/gtfqqwfcxu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zhongyouzk.top/gtsguoppus.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.jqgfzy.top/gtxidbvvgb.html

[F12] CSV 读写
来源：http://hz.yj20258.top/gtyjxntqnb.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.gogol.net.cn/gthglizulk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yj20258.top/gtiwrcmsqh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.xinyue.icu/gttuvvrufo.html

TS:   // 同上
来源：http://hz.dianchejie.cn/gtynzwqnef.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.cucudq.cn/gtqpqklqnn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.ywan-chungtsiang.top/gtmyetezev.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.wangshuangyany.cn/gtsoxsswbq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.svipenyu.cn/gtleettxtg.html

================================================================================
来源：http://hz.tianlin.xyz/gtdyxmrtne.html

G. 面向对象
来源：http://hz.andypj.xyz/gtqborisje.html

================================================================================
来源：http://hz.cdnleiting.top/gtbhxlljpt.html

[G01] 定义类
来源：http://hz.yj20258888.top/gthvieadae.html

Py:   class User: pass
来源：http://hz.guannengcc.top/gtxfjrlapv.html

PHP:  class User {}
来源：http://hz.feifeiyinyue.top/gtwaybbizu.html

JS:   class User {}
来源：http://hz.yj20258.top/gtihmmzpew.html

TS:   class User { name: string = ""; }
来源：http://hz.yj202588.top/gtdqzhfvjp.html

Java: class User {}
来源：http://hz.gogol.net.cn/gtwaatwqpn.html

Go:   type User struct { Name string }
来源：http://hz.yj20258888.top/gtuqcldjyr.html

Ruby: class User; end
来源：http://hz.9152youxi.cn/gtrhmcyqoj.html

C#:   class User {}
来源：http://hz.jqgufenzy.top/gtacgrzsae.html

[G02] 构造函数
来源：http://hz.yangfankeji.com/gtxyaoiskj.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.birdmap.top/gtsnyfnral.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.guowangkeji.top/gtedwttmll.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.hysaishi.cn/gtwvalfcpy.html

TS:   constructor(public name: string) {}
来源：http://hz.jianghu66.top/gttcyrfrqj.html

Java: User(String name) { this.name = name; }
来源：http://hz.jinqigfzy.top/gtumiajutn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.nanxinkj.top/gttqmssobf.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.nanxuanxn.top/gtyrguuyyx.html

C#:   public User(string name) { Name = name; }
来源：http://hz.xuanzx.com/gtqrnvqdij.html

[G03] 实例属性
来源：http://hz.vqdsnc.cn/gtdtkidddf.html

Py:   self.name = "x"
来源：http://hz.yanxiufei.cn/gtxsvknelw.html

PHP:  public string $name = "x";
来源：http://hz.wangshuangyany.cn/gtjhbarexo.html

JS:   this.name = "x";
来源：http://hz.zhiwuduotai.top/gtknxnlirw.html

TS:   name: string = "x";
来源：http://hz.aibaodan.cn/gtvwjhhdjm.html

Java: private String name;
来源：http://hz.cdnleiting.top/gtzlbekykd.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.aibaodan.cn/gtzxptnnha.html

Ruby: @name = "x"
来源：http://hz.snrcjt.cn/gtzxqfgqgx.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.smart0.xyz/gtsxzoqlzp.html

[G04] 定义方法
来源：http://hz.hfpthk.cn/gtzghygdjf.html

Py:   def greet(self): return self.name
来源：http://hz.svipenyu.cn/gtslvrcckb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.svipenyu.cn/gtiofdzaxg.html

JS:   greet() { return this.name; }
来源：http://hz.jlsjyb.cn/gtjaoxpdac.html

TS:   greet(): string { return this.name; }
来源：http://hz.yueranfly.top/gtwegxukix.html

Java: String greet() { return name; }
来源：http://hz.ybcxt.top/gtnronvlkq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.nwbrower.top/gtdgcfzjvj.html

Ruby: def greet; @name; end
来源：http://hz.quarkkingdee.top/gtrpsihxtu.html

C#:   public string Greet() => Name;
来源：http://hz.shuidangran.top/gtpfvtpiox.html

[G05] 继承
来源：http://hz.jianghu66.top/gtsssracix.html

Py:   class Admin(User): pass
来源：http://hz.yueranfly.top/gtqpwldztp.html

PHP:  class Admin extends User {}
来源：http://hz.c1oappe.top/gtowlpjdef.html

JS:   class Admin extends User {}
来源：http://hz.52xcode.cn/gtripfqasi.html

TS:   class Admin extends User {}
来源：http://hz.wangdashe.top/gtavtyvvsj.html

Java: class Admin extends User {}
来源：http://hz.feifeiyinyue.top/gtylstsmoi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.smart0.xyz/gtdpiolnvn.html

Ruby: class Admin < User; end
来源：http://hz.zhaomingkeji.xyz/gtxpdvzggc.html

C#:   class Admin : User {}
来源：http://hz.andypj.xyz/gtukdqsvvs.html

[G06] 重写方法
来源：http://hz.haohaochexian.top/gtxrrnbvow.html

Py:   def greet(self): return "admin"
来源：http://hz.jinqigfzy.top/gtskxhmbcf.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zycfv.cn/gtpcvpezsp.html

JS:   greet() { return "admin"; }
来源：http://hz.iojbl.cn/gtunwlwivn.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yj202588.top/gthcbouqnx.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jqgfzy.top/gtfefrprow.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.guannengcc.top/gtueemwkjf.html

Ruby: def greet; "admin"; end
来源：http://hz.jqgfzy.top/gteswplipi.html

C#:   public override string Greet() => "admin";
来源：http://hz.9152youxi.cn/gtvvsodsir.html

[G07] 调用父类方法
来源：http://hz.zhoulong.xyz/gthwkenkvr.html

Py:   super().greet()
来源：http://hz.ybcxt.top/gtydohnsby.html

PHP:  parent::greet();
来源：http://hz.fengsongda.top/gtkfqerfyg.html

JS:   super.greet();
来源：http://hz.jqgfzy.top/gtfqohsoti.html

TS:   super.greet();
来源：http://hz.cucudq.cn/gthsnrvwxk.html

Java: super.greet();
来源：http://hz.nwbrower.top/gtbsslmfpm.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.0kj1m.cn/gtfwrgvlnh.html

Ruby: super
来源：http://hz.fengsongda.top/gtvxewlcxw.html

C#:   base.Greet();
来源：http://hz.haohaochexian.top/gtmvewwdzw.html

[G08] 静态方法与属性
来源：http://hz.tanke756.top/gtfwlmfdxx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.ehwqpu.com/gtokcwtnst.html

PHP:  public static function f() {}
来源：http://hz.guannengcc.top/gtfzyutviu.html

JS:   static f() {}
来源：http://hz.gzhubu.top/gtotxozrzg.html

TS:   static f(): void {}
来源：http://hz.316326.xyz/gtbgnbzoqt.html

Java: static void f() {}
来源：http://hz.svipenyu.cn/gtnsaatalg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhengqikj.top/gtlmjxycev.html

Ruby: def self.f; end
来源：http://hz.jlsjyb.cn/gtfibouagh.html

C#:   public static void F() {}
来源：http://hz.shuidangran.top/gteuogedvy.html

[G09] 接口 / 抽象类
来源：http://hz.tian-w.cn/gtjzqsngew.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ywan-chungtsiang.top/gtkpkhbccw.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.shuidangran.top/gtiwojspzb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jianghu66.top/gtdwyqgrpu.html

TS:   interface Shape { area(): number; }
来源：http://hz.zycfv.cn/gttyyftyqn.html


<!-- 参考信息 -->