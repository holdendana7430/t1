代发 wailian999

C#:   7.ToString("D3");  7.ToString().PadLeft(3, '0')
来源：http://hz.xuanzx.com/gtnrvpliah.html

[E11] 反转字符串
来源：http://hz.0kj1m.cn/gtbhmieskv.html

Py:   s[::-1]
来源：http://hz.fengsongda.top/gtrkedvdnm.html

PHP:  strrev($s);
来源：http://hz.fzhhl.top/gttwtcgkqr.html

JS:   [...s].reverse().join("")
来源：http://hz.vqdsnc.cn/gthzfathnh.html

TS:   [...s].reverse().join("")
来源：http://hz.daxiang520.top/gtaxbbbtiu.html

Java: new StringBuilder(s).reverse().toString()
来源：http://hz.shanyushiyangkeji.top/gtxmucimgd.html

Go:   // 转 []rune 后倒序再转回 string
来源：http://hz.zhiwuduotai.top/gttmbktxcp.html

Ruby: s.reverse
来源：http://hz.pycfn.com/gtbxmkznxr.html

C#:   new string(s.Reverse().ToArray())
来源：http://hz.zhaomingkeji.xyz/gtyinjfzlg.html

[E12] 统计某字符出现次数
来源：http://hz.hywenlv.cn/gtgxjlefax.html

Py:   s.count("a")
来源：http://hz.iojbl.cn/gtoaisfmur.html

PHP:  substr_count($s, "a");
来源：http://hz.shzxlz.cn/gtosimlxnu.html

JS:   s.split("a").length - 1
来源：http://hz.zhiwuduotai.top/gtoxkmlfwx.html

TS:   s.split("a").length - 1
来源：http://hz.gotoacloud.top/gtayyaxoav.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.ywan-chungtsiang.top/gteeqbusav.html

Go:   strings.Count(s, "a")
来源：http://hz.zdqjudy.top/gtwldrevhn.html

Ruby: s.count("a")
来源：http://hz.guowangkeji.top/gtarkznfqq.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jinyuanbaomall.cn/gtjnkippno.html

[E13] 逐字符遍历
来源：http://hz.dashuyun.cn/gtsixgkxmb.html

Py:   for ch in s: print(ch)
来源：http://hz.tianlin.xyz/gtitezctsx.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jqgfzy.top/gtgaczjrve.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.mhx1999.top/gtvpsqptbr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jqgufenzy.top/gtabanufkh.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.shuidangran.top/gtpbjfcsmx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.fengsongda.top/gtclwyzwwd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.haohaochexian.top/gtymqnlapw.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.c1oappe.top/gtilktaryt.html

[E14] URL 编码与 Base64
来源：http://hz.mhx1999.top/gtwmpyrvut.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zhoulong.xyz/gtrtfbprgn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.meibo888.top/gtkcurejlw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yuanzhike.top/gtotfokajt.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.sysykeji.top/gtauvtwksq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jqgfzy.top/gtlthzvcfj.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.hammf.cn/gtbeqthaiv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jiagoushi.top/gtpvcumsuv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.zhoulong.xyz/gtxfdittbp.html

[E15] HTML 转义 / 反转义
来源：http://hz.sufxvd.cn/gtcruryjow.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.sufxvd.cn/gtnwpdmxgc.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.c1oappe.top/gtlqhyihvy.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.ydjk.org.cn/gttorusvyn.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.9152youxi.cn/gtspqrtibb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.jinqigfzy.top/gtvtviavyb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.chenzaomai.com/gtkzonldkn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.xziqi.cn/gtchhbdnop.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.shanyushiyangkeji.top/gtmldamkcy.html

[E16] 数字千分位
来源：http://hz.bjfxy.top/gtwntezhcm.html

Py:   f"{1234567:,}"
来源：http://hz.vqdsnc.cn/gtjgssoyne.html

PHP:  number_format(1234567);
来源：http://hz.yanxiufei.cn/gtlracmoum.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.gotoacloud.top/gteodycowa.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.tianlin.xyz/gtlhjnvzex.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.tanke756.top/gteznspwhx.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.xziqi.cn/gtnsdcmnag.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.shuidangran.top/gtwhoilztg.html

C#:   1234567.ToString("N0")
来源：http://hz.ehwqpu.com/gttmwadaok.html

[E17] 首字母大写
来源：http://hz.yj20258.top/gtyfevdtky.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.guowangkeji.top/gtqxduxomr.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.nanxinkj.top/gtgjdrofeh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.tianlin.xyz/gttbwcxbsb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.iojbl.cn/gtifirkzfb.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.hammf.cn/gthojfczxa.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zhiwuduotai.top/gtmzfsvhpp.html

Ruby: s.capitalize
来源：http://hz.chenlongwang.top/gtdbcsownj.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.sweek.top/gtluhijegd.html

[E18] 模板占位符替换
来源：http://hz.tianlin.xyz/gtinjmuhfz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jlsjyb.cn/gtarrwufzn.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.dashuyun.cn/gtcgibetzc.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.cqqwz.cn/gtyebxzyoa.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.fengsongda.top/gtcoymqtuq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.hammf.cn/gtrkjsisqa.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.shangyingyoupin.top/gtxcqvhxek.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zycfv.cn/gtwzsdrfqa.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.cdnleiting.top/gturzpsewf.html

[E19] 多行文本按行拆分
来源：http://hz.jinghuilouyu.cn/gtdwvacttk.html

Py:   s.splitlines()
来源：http://hz.ehwqpu.com/gtbafckwem.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.mhx1999.top/gtwuenzbiz.html

JS:   s.split(/\r?\n/)
来源：http://hz.xuanzx.com/gticaxfama.html

TS:   s.split(/\r?\n/)
来源：http://hz.dianchejie.cn/gtflfwdfzy.html

Java: s.lines().toList()
来源：http://hz.jinghuilouyu.cn/gtbakbjrvo.html

Go:   strings.Split(s, "\n")
来源：http://hz.nanxuanxn.top/gtfadebxgk.html

Ruby: s.lines
来源：http://hz.havefunace.top/gthavnjofy.html

C#:   s.Split('\n')
来源：http://hz.aibaodan.cn/gtlcywbkfg.html

[E20] 判断字符串是否为空
来源：http://hz.wangdashe.top/gtgqadcsvj.html

Py:   if not s:
来源：http://hz.hongshengwenyu.top/gtssjwwklo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zdqjudy.top/gthdxvzfwn.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.ydzc1.top/gtijjnaoqu.html

TS:   if (s === "") {}
来源：http://hz.smart0.xyz/gtxijyizqj.html

Java: if (s.isEmpty()) {}
来源：http://hz.hywenlv.cn/gtlukinzyd.html

Go:   if s == "" {}
来源：http://hz.dashuyun.cn/gtlnmhuzxu.html

Ruby: if s.empty?
来源：http://hz.yongpay.top/gtvzstjjtn.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.dashuyun.cn/gtmhzjtziw.html

[E21] 超长截断加省略号
来源：http://hz.gaohongyu789.top/gtindvywoc.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.gotoacloud.top/gtxqlhohuk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.sweek.top/gtpyeqwada.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yuanzhike.top/gtvvughcsx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.fzhhl.top/gtjrtnnrvm.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.chenzaomai.com/gtavoahjir.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hongshengwenyu.top/gtjztnmxkx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.vqdsnc.cn/gtjjeecevc.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.feifeiyinyue.top/gtfhzqgbut.html

[E22] 字节长度与字符长度
来源：http://hz.smart0.xyz/gtzvsntwhm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.cucudq.cn/gtangpkgem.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yanxiufei.cn/gtorkkrkrp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cheryme.top/gtvdlverlm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yangfankeji.com/gtascmgdbx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.dianchejie.cn/gtvzudmgpd.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zdqjudy.top/gtajoxpmdm.html

Ruby: s.bytesize;  s.length
来源：http://hz.0kj1m.cn/gtoccverwf.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.sufxvd.cn/gtgupaueem.html

================================================================================
来源：http://hz.jinqigfzy.top/gtbvngmahw.html

F. 文件与目录
来源：http://hz.aibaodan.cn/gtrenbagck.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtnhaobnsr.html

[F01] 读取整个文件
来源：http://hz.nanxinkj.top/gtwkvjrwzk.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.ppjwa.cn/gtsjknlhzq.html

PHP:  file_get_contents("a.txt");
来源：http://hz.wangshuangyany.cn/gtehxfaufu.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zhoulong.xyz/gtxspqjtfl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.nwbrower.top/gtqzhftdob.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.hammf.cn/gtvzpldnrd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.gzhubu.top/gtrvdwfyjh.html

Ruby: File.read("a.txt")
来源：http://hz.havefunace.top/gtftyymlhi.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jianghu66.top/gtztjwzcng.html

[F02] 逐行读取文件
来源：http://hz.tian-w.cn/gtfxzlnjli.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.quarkkingdee.top/gtmzjcjapp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.xingfuxueyuan.xyz/gtjccdzwii.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ehwqpu.com/gtklmbwctd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.birdmap.top/gtgdenrmte.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.svipenyu.cn/gtiotmhrpu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.hnqzz.top/gthgpfpugm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.c1oappe.top/gtwgguxfwv.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.shanyushiyangkeji.top/gtavjivhtt.html

[F03] 写入文件（覆盖）
来源：http://hz.hysaishi.cn/gtdaiemiyy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.birdmap.top/gtaejfpcgi.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.redwolf501.top/gtoycabbyp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yj202588.top/gtilbdglfy.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yangfankeji.com/gtvzoilpcz.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.birdmap.top/gtnofcircp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.xylfe.cn/gtreawhphq.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.ydjk.org.cn/gtklzzjxgv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.sxryk.cn/gtyaikbwta.html

[F04] 追加写入文件
来源：http://hz.hfpthk.cn/gtpazisyzq.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jianghu66.top/gtkgdrhpjt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.hammf.cn/gtfyukkqfu.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jianghu66.top/gtizuloznu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xuanzx.com/gtkvgdzsxo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.hysaishi.cn/gtuujnudip.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zhixingplan.top/gtrwrefnkl.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.hysaishi.cn/gtajqntwye.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.chenlongwang.top/gtenxdzget.html

[F05] 判断文件或目录是否存在
来源：http://hz.xziqi.cn/gtiosjwwaz.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.ppjwa.cn/gtuzrakeff.html

PHP:  file_exists("a.txt");
来源：http://hz.feifeiyinyue.top/gtsewatxcf.html

JS:   fs.existsSync("a.txt")
来源：http://hz.sweek.top/gtibinlrbo.html

TS:   fs.existsSync("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtcefyqhoi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.dashuyun.cn/gtmemkwhoi.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.havefunace.top/gtltxxneek.html

Ruby: File.exist?("a.txt")
来源：http://hz.sysykeji.top/gtnauzpswp.html

C#:   File.Exists("a.txt")
来源：http://hz.wangshuangyany.cn/gtlbmzsgha.html

[F06] 删除文件
来源：http://hz.shuidangran.top/gtenuhqznk.html

Py:   os.remove("a.txt")
来源：http://hz.52xcode.cn/gtllicvftj.html

PHP:  unlink("a.txt");
来源：http://hz.sxryk.cn/gtpcrgkrtl.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hnxiangtu.top/gtvmlquzhx.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.nanxuanxn.top/gtgkdtqsiu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.redwolf501.top/gthdbrktem.html

Go:   os.Remove("a.txt")
来源：http://hz.guannengcc.top/gttjwlvdfh.html

Ruby: File.delete("a.txt")
来源：http://hz.nwbrower.top/gtjdtodrzc.html

C#:   File.Delete("a.txt");
来源：http://hz.zhoulong.xyz/gtvlldmmkg.html

[F07] 创建目录（含多级）
来源：http://hz.daria6918.cn/gtdtxqopnw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.nwbrower.top/gtgvovdvfb.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.ybcxt.top/gtfjsiukvb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jyoumei.cn/gtlbsqyjam.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ehwqpu.com/gtifzckixb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.sweek.top/gtbtdmncia.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.shzxlz.cn/gtkiyxgsza.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.shzxlz.cn/gtedgzclbu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yanxiufei.cn/gtbcydiste.html

[F08] 遍历目录
来源：http://hz.shangyingyoupin.top/gtkgfnucpc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.sxryk.cn/gtqrqxcqnz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.hywenlv.cn/gtppfzvizy.html

JS:   fs.readdirSync("dir")
来源：http://hz.hfpthk.cn/gtqkutvleh.html

TS:   fs.readdirSync("dir")
来源：http://hz.wangdashe.top/gtkauglnsk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.fzhhl.top/gtsxvrvpzs.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.chenzaomai.com/gtlohopaqj.html

Ruby: Dir.children("dir")
来源：http://hz.guannengcc.top/gtjkwiqsjb.html

C#:   Directory.GetFiles("dir")
来源：http://hz.tian-w.cn/gtkwywevhi.html

[F09] 获取文件大小
来源：http://hz.zycfv.cn/gtsscehrbm.html

Py:   os.path.getsize("a.txt")
来源：http://hz.redwolf501.top/gtgirnrczv.html

PHP:  filesize("a.txt");
来源：http://hz.sufxvd.cn/gtiepgqswr.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yanxiufei.cn/gtjxctjofa.html

TS:   fs.statSync("a.txt").size
来源：http://hz.sweek.top/gtczdksaby.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zhijiandao.cn/gtjefxvgkq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.tian-w.cn/gteuvssnlj.html

Ruby: File.size("a.txt")
来源：http://hz.tanke756.top/gtlofslibo.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.ydjk.org.cn/gtybbuspcd.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.guowangkeji.top/gtkhoeywll.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.andypj.xyz/gtdkzhxwuf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.xingfuxueyuan.xyz/gtemvcvnbn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.snrcjt.cn/gtegyhykse.html

TS:   path.extname("a.txt")
来源：http://hz.c1oappe.top/gtxjtvjykm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.shanyushiyangtech.top/gtgljrnort.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhongyouzk.top/gtmxnapboh.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yonumen.top/gtsshfvhbz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.nanxuanxn.top/gtbtwzilrs.html

[F11] 复制与移动文件
来源：http://hz.haohaochexian.top/gtcwvgkgdv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zhijiandao.cn/gtleqillbi.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yj20258.top/gtepzveocu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sxryk.cn/gtbdqtzopl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhiwuduotai.top/gtulpcfzzm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.shanyushiyangtech.top/gttorguepo.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.chenlongwang.top/gtkilzpbmw.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.9152youxi.cn/gtxkzrkprq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.meibo888.top/gtedqkwfmd.html

[F12] CSV 读写
来源：http://hz.yj20258.top/gtxzpbipof.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.tianlin.xyz/gtnbykyvlk.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.pycfn.com/gtpjritwve.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.xziqi.cn/gtglxngtyg.html

TS:   // 同上
来源：http://hz.ehwqpu.com/gthnzhzjik.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.guowangkeji.top/gteyqtmgni.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jqgfzy.top/gtokvoeeye.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.quarkkingdee.top/gtdowqdgtv.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jiagoushi.top/gtgkvegyjb.html

================================================================================
来源：http://hz.cucudq.cn/gtomuoyoqn.html

G. 面向对象
来源：http://hz.sxryk.cn/gtncpneupk.html

================================================================================
来源：http://hz.xuetiantiany.cn/gteruakkbq.html

[G01] 定义类
来源：http://hz.vqdsnc.cn/gteocnmxic.html

Py:   class User: pass
来源：http://hz.yanxiufei.cn/gtzfpjhouk.html

PHP:  class User {}
来源：http://hz.bjfxy.top/gtsqkdfybk.html

JS:   class User {}
来源：http://hz.zycfv.cn/gtwhztsrou.html

TS:   class User { name: string = ""; }
来源：http://hz.zhijiandao.cn/gtemuexphb.html

Java: class User {}
来源：http://hz.gaohongyu789.top/gtatsdclxa.html

Go:   type User struct { Name string }
来源：http://hz.feifeiyinyue.top/gtkluodeqc.html

Ruby: class User; end
来源：http://hz.sufxvd.cn/gttyfkfudf.html

C#:   class User {}
来源：http://hz.ydjk.org.cn/gtlfvgwbqo.html

[G02] 构造函数
来源：http://hz.jinqigfzy.top/gtqpjnkiic.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.smart0.xyz/gtvmbojgqz.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jianghu66.top/gtfyoqagjh.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.shzxlz.cn/gtvjdaubwy.html

TS:   constructor(public name: string) {}
来源：http://hz.ppjwa.cn/gtwvwqcpie.html

Java: User(String name) { this.name = name; }
来源：http://hz.pycfn.com/gtrkukdkxn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.shanyushiyangkeji.top/gtpflbwpzz.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.mhx1999.top/gtdlfoinnk.html

C#:   public User(string name) { Name = name; }
来源：http://hz.iojbl.cn/gtyhqiloqr.html

[G03] 实例属性
来源：http://hz.daxiang520.top/gtedrxouyj.html

Py:   self.name = "x"
来源：http://hz.chenzaomai.com/gtubppjcgr.html

PHP:  public string $name = "x";
来源：http://hz.yj20258.top/gtearyfsuu.html

JS:   this.name = "x";
来源：http://hz.sxryk.cn/gtxuogfzun.html

TS:   name: string = "x";
来源：http://hz.feifeiyinyue.top/gtvspcbxme.html

Java: private String name;
来源：http://hz.jqgfzy.top/gtechvcvci.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yj20258.top/gtiqscizyo.html

Ruby: @name = "x"
来源：http://hz.316326.xyz/gtqbmhleeb.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.52xcode.cn/gtbfavhyka.html

[G04] 定义方法
来源：http://hz.tanke756.top/gtfwmlmsqw.html

Py:   def greet(self): return self.name
来源：http://hz.yangfankeji.com/gtuetnmqnp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhoulong.xyz/gtvskeygnq.html

JS:   greet() { return this.name; }
来源：http://hz.xinyue.icu/gtpkxgdqqj.html

TS:   greet(): string { return this.name; }
来源：http://hz.shangyingyoupin.top/gtcwfejalh.html

Java: String greet() { return name; }
来源：http://hz.52xcode.cn/gtpmqxnkso.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.shangyingyoupin.top/gtbqiwukmb.html

Ruby: def greet; @name; end
来源：http://hz.tanke756.top/gtejtivjfn.html

C#:   public string Greet() => Name;
来源：http://hz.hammf.cn/gtvglwfjtq.html

[G05] 继承
来源：http://hz.0kj1m.cn/gtfsrwxpia.html

Py:   class Admin(User): pass
来源：http://hz.yj202588.top/gtycpckwwd.html

PHP:  class Admin extends User {}
来源：http://hz.tanke756.top/gtxwmrxbni.html

JS:   class Admin extends User {}
来源：http://hz.tian-w.cn/gtnhmvpomh.html

TS:   class Admin extends User {}
来源：http://hz.pengpengdd.cyou/gtwlcsnkbi.html

Java: class Admin extends User {}
来源：http://hz.aizwys.cn/gtjdbthnns.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.havefunace.top/gttiauwesp.html

Ruby: class Admin < User; end
来源：http://hz.jyoumei.cn/gtmrvsuhyw.html

C#:   class Admin : User {}
来源：http://hz.guannengcc.top/gtxxsquhde.html

[G06] 重写方法
来源：http://hz.sweek.top/gttznlqyfm.html

Py:   def greet(self): return "admin"
来源：http://hz.xinyue.icu/gtpsywthje.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.shanyushiyangtech.top/gtecqywkcz.html

JS:   greet() { return "admin"; }
来源：http://hz.shzxlz.cn/gtudrxbexx.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jqgfzy.top/gtycrsrndy.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.dashuyun.cn/gtpvrsyztu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.316326.xyz/gtmyqmcvna.html

Ruby: def greet; "admin"; end
来源：http://hz.jyoumei.cn/gtfrntcuqm.html

C#:   public override string Greet() => "admin";
来源：http://hz.daxiang520.top/gtrvaazijv.html

[G07] 调用父类方法
来源：http://hz.yanxiufei.cn/gtzkgekyof.html

Py:   super().greet()
来源：http://hz.smart0.xyz/gtdjzotjln.html

PHP:  parent::greet();
来源：http://hz.ydzc1.top/gtfpzbwgjb.html

JS:   super.greet();
来源：http://hz.jiagoushi.top/gtgukkuqpf.html

TS:   super.greet();
来源：http://hz.tian-w.cn/gtuoxdikjl.html

Java: super.greet();
来源：http://hz.dianchejie.cn/gtfyouixki.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jqgufenzy.top/gtwsbjnafc.html

Ruby: super
来源：http://hz.ehwqpu.com/gtgtqjiblk.html

C#:   base.Greet();
来源：http://hz.mhx1999.top/gtahuorxkj.html

[G08] 静态方法与属性
来源：http://hz.jqgfzy.top/gthzgckxna.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.gaohongyu789.top/gtsiedkjqf.html

PHP:  public static function f() {}
来源：http://hz.tianlin.xyz/gtvuqzjvhz.html

JS:   static f() {}
来源：http://hz.zhijiandao.cn/gtdzuhhwor.html

TS:   static f(): void {}
来源：http://hz.hammf.cn/gtcidlykkg.html

Java: static void f() {}
来源：http://hz.zhijiandao.cn/gtppbidofj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jinghuilouyu.cn/gtrmrvwkra.html

Ruby: def self.f; end
来源：http://hz.daxiang520.top/gtpcmmdxxa.html

C#:   public static void F() {}
来源：http://hz.nanxuanxn.top/gtqehcnbjo.html

[G09] 接口 / 抽象类
来源：http://hz.hnqzz.top/gtadqvqize.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zhoulong.xyz/gtnzlmxcyo.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.daxiang520.top/gtuqzuzons.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.cdnleiting.top/gtphvtvrgl.html

TS:   interface Shape { area(): number; }
来源：http://hz.ybcxt.top/gtfovpwhby.html


<!-- 参考信息 -->