代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.yj20258.top/gtmaxhuvua.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.ydjk.org.cn/gtuhyadllh.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zhiwuduotai.top/gtbcosiywv.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jinyuanbaomall.cn/gtxfyqqwzz.html

[E14] URL 编码与 Base64
来源：http://hz.shanyushiyangtech.top/gtspczwksv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.nanxinkj.top/gtkdbieanh.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.birdmap.top/gtvpqytuba.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.c1oappe.top/gtbclzkktc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.daxiang520.top/gttwfffnue.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jinqigfzy.top/gtkncinxfh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.ivvv.top/gtanozdnxu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.cdnleiting.top/gtqtbqrhpv.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.daria6918.cn/gtnkusxoan.html

[E15] HTML 转义 / 反转义
来源：http://hz.haohaochexian.top/gtkpitrcmf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zycfv.cn/gtlhpckwgd.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.xylfe.cn/gtgbxoorxk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.tanke756.top/gtmjismxcs.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.iojbl.cn/gtvucauppv.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.0kj1m.cn/gtbjhoxmdu.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.wangdashe.top/gtnxjqzjtu.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.ybcxt.top/gtijspihra.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.hnqzz.top/gtjkoehyyh.html

[E16] 数字千分位
来源：http://hz.jinyuanbaomall.cn/gtuypqbqak.html

Py:   f"{1234567:,}"
来源：http://hz.kuanghao11.cn/gtbbqvbdut.html

PHP:  number_format(1234567);
来源：http://hz.wangshuangyany.cn/gtfpzrqtho.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.ehwqpu.com/gtxowjwecs.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.chenzaomai.com/gtxpplmwwu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.shangyingyoupin.top/gtgvtbdaey.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.gaohongyu789.top/gtpowfbpth.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.xziqi.cn/gtphsrmqzy.html

C#:   1234567.ToString("N0")
来源：http://hz.zycfv.cn/gtuqqkvouu.html

[E17] 首字母大写
来源：http://hz.cdnleiting.top/gtjjxekmtu.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.tanke756.top/gtqfrajpvq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yuanzhike.top/gtkkiyfgbu.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gogol.net.cn/gtwzoubbyh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xuanzx.com/gtyetoznwu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.sweek.top/gtiiuwdzlf.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.sweek.top/gtecvqghqw.html

Ruby: s.capitalize
来源：http://hz.sweek.top/gtsinbiebp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.c1oappe.top/gtnyemlmze.html

[E18] 模板占位符替换
来源：http://hz.hammf.cn/gtslohleio.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.c1oappe.top/gtxusmhgqo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.aizwys.cn/gtfdvzyyhh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.pengpengdd.cyou/gtclkatvcz.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.pycfn.com/gtusldpppx.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yuxming.cn/gtinbejeas.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jqgufenzy.top/gtgyjebmsb.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.xingfuxueyuan.xyz/gtwqkprgsp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.sweek.top/gteseypvvc.html

[E19] 多行文本按行拆分
来源：http://hz.chenlongwang.top/gtcuojmrnx.html

Py:   s.splitlines()
来源：http://hz.hammf.cn/gtksmasugt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.birdmap.top/gttyvtetbm.html

JS:   s.split(/\r?\n/)
来源：http://hz.cheryme.top/gtvkwadbqx.html

TS:   s.split(/\r?\n/)
来源：http://hz.zhijiandao.cn/gtoczlsjon.html

Java: s.lines().toList()
来源：http://hz.pengpengdd.cyou/gtzppjebik.html

Go:   strings.Split(s, "\n")
来源：http://hz.zycfv.cn/gtjgtytdpj.html

Ruby: s.lines
来源：http://hz.haohaochexian.top/gtvnjbiqln.html

C#:   s.Split('\n')
来源：http://hz.xziqi.cn/gtdhtvkirf.html

[E20] 判断字符串是否为空
来源：http://hz.meibo888.top/gtbktdwmix.html

Py:   if not s:
来源：http://hz.zhixingplan.top/gtnpsorivr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.xinyue.icu/gtqxnpympt.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jinyuanbaomall.cn/gtlotnozmb.html

TS:   if (s === "") {}
来源：http://hz.svipenyu.cn/gtmyzvftdr.html

Java: if (s.isEmpty()) {}
来源：http://hz.nanxuanxn.top/gtgwjlxccr.html

Go:   if s == "" {}
来源：http://hz.sxryk.cn/gtpnupvjgf.html

Ruby: if s.empty?
来源：http://hz.hnqzz.top/gtwenfniur.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.0kj1m.cn/gtzdzrxziw.html

[E21] 超长截断加省略号
来源：http://hz.xuanzx.com/gtjlbrrjco.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zhijiandao.cn/gtbgmahgaw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.ehwqpu.com/gtfottnugv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.9152youxi.cn/gtdnscxgzf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hysaishi.cn/gtaoptpeib.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yj20258888.top/gtfudzsvxb.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.zhixingplan.top/gtdulrwlmy.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.ywan-chungtsiang.top/gtzylukgfi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.pycfn.com/gtodccwflu.html

[E22] 字节长度与字符长度
来源：http://hz.hammf.cn/gtvefwjbvv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.iojbl.cn/gttnrykbim.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.ydzc1.top/gtgnhljhpv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.guannengcc.top/gtlpcpgpzr.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhiwuduotai.top/gtylvwnjeu.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yueranfly.top/gtftdkxrpb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hammf.cn/gtsacngllb.html

Ruby: s.bytesize;  s.length
来源：http://hz.birdmap.top/gtcxkjaxah.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.xingfuxueyuan.xyz/gtyeintlzb.html

================================================================================
来源：http://hz.aizwys.cn/gtwgxryegs.html

F. 文件与目录
来源：http://hz.cheryme.top/gtfnzwooul.html

================================================================================
来源：http://hz.jqgufenzy.top/gtxfojsctw.html

[F01] 读取整个文件
来源：http://hz.chenlongwang.top/gtkhvlfhuj.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.tianlin.xyz/gtvuebbtjd.html

PHP:  file_get_contents("a.txt");
来源：http://hz.pycfn.com/gtbajdqzcl.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yueranfly.top/gtcbvqytlp.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jinyuanbaomall.cn/gtjktpnauz.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.ydjk.org.cn/gtlcywbdfi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.xingfuxueyuan.xyz/gteggwlcut.html

Ruby: File.read("a.txt")
来源：http://hz.yj202588.top/gtaszxqvct.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hnqzz.top/gtturpwncz.html

[F02] 逐行读取文件
来源：http://hz.0kj1m.cn/gtoozjbzwb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.daria6918.cn/gtlcxuwigo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.andypj.xyz/gtymnczvqg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.daria6918.cn/gtcjmymbta.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jiagoushi.top/gtnsdimnar.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.xuetiantiany.cn/gttmeyvjgi.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.gotoacloud.top/gtsihbhllc.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.zdqjudy.top/gtprmqcjft.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jqgufenzy.top/gtpqhwwbrn.html

[F03] 写入文件（覆盖）
来源：http://hz.hywenlv.cn/gtesjrwxed.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yongpay.top/gtrokihcjv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.xylfe.cn/gtdeckutbf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhiwuduotai.top/gtcbesupne.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yj20258.top/gtzolraiqd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.sysykeji.top/gtofemukux.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.hnqzz.top/gtwjiceyqk.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yvedp.cn/gtfgfewfch.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.gaohongyu789.top/gtzyxjsndk.html

[F04] 追加写入文件
来源：http://hz.yuxming.cn/gtidsregvw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.vqdsnc.cn/gtxzbomejt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.snrcjt.cn/gtihubylat.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.dashuyun.cn/gtgaejjuya.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yj20258.top/gtoooojmxl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jinqigufen.top/gtpbytnyyw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.andypj.xyz/gtibbgpcwm.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.sweek.top/gtlojaenvc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.cqqwz.cn/gtvycrulma.html

[F05] 判断文件或目录是否存在
来源：http://hz.xingfuxueyuan.xyz/gtmmiozkhn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.tianlin.xyz/gthlzdkfhv.html

PHP:  file_exists("a.txt");
来源：http://hz.meibo888.top/gtrcygwxgp.html

JS:   fs.existsSync("a.txt")
来源：http://hz.fzhhl.top/gtxxvrvllq.html

TS:   fs.existsSync("a.txt")
来源：http://hz.gogol.net.cn/gteoodrlsh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yonumen.top/gtbwjjubgk.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.dashuyun.cn/gtcekdszcs.html

Ruby: File.exist?("a.txt")
来源：http://hz.iojbl.cn/gtwynxjsfj.html

C#:   File.Exists("a.txt")
来源：http://hz.xziqi.cn/gtyzkjhbre.html

[F06] 删除文件
来源：http://hz.chenlongwang.top/gtnaycimkb.html

Py:   os.remove("a.txt")
来源：http://hz.jinqigufen.top/gtcjllqkgu.html

PHP:  unlink("a.txt");
来源：http://hz.yonumen.top/gthreaisce.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.xylfe.cn/gtmqrfyhed.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jianghu66.top/gtlmykzbqe.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.shangyingyoupin.top/gtbtcdyqpv.html

Go:   os.Remove("a.txt")
来源：http://hz.sysykeji.top/gtukrybzsu.html

Ruby: File.delete("a.txt")
来源：http://hz.hysaishi.cn/gtyijxqpke.html

C#:   File.Delete("a.txt");
来源：http://hz.guannengcc.top/gtlqwgilnw.html

[F07] 创建目录（含多级）
来源：http://hz.zycfv.cn/gtbfdsyvho.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.jinqigufen.top/gtbcwqtffo.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.ywan-chungtsiang.top/gtopbiupvp.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.wangshuangyany.cn/gtttyvkppn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.dianchejie.cn/gtbnjljvbi.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.wangdashe.top/gtgziloxkw.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yuxming.cn/gttzipcjrj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.havefunace.top/gtqboiqjsp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zhijiandao.cn/gtksyiabda.html

[F08] 遍历目录
来源：http://hz.shanyushiyangtech.top/gtloopkxwc.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.hywenlv.cn/gtrykqcqyw.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.fengsongda.top/gtxwejrfor.html

JS:   fs.readdirSync("dir")
来源：http://hz.ivvv.top/gtqzlkqcym.html

TS:   fs.readdirSync("dir")
来源：http://hz.xuetiantiany.cn/gtbwonmtdf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.c1oappe.top/gtpnsgihix.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yuanzhike.top/gtktakoban.html

Ruby: Dir.children("dir")
来源：http://hz.ybcxt.top/gtlxnwdklo.html

C#:   Directory.GetFiles("dir")
来源：http://hz.haohaochexian.top/gtbvjfxcdo.html

[F09] 获取文件大小
来源：http://hz.zhongyouzk.top/gtsayubuzn.html

Py:   os.path.getsize("a.txt")
来源：http://hz.shanyushiyangtech.top/gtfxicvwjj.html

PHP:  filesize("a.txt");
来源：http://hz.hongshengwenyu.top/gtcwnikgao.html

JS:   fs.statSync("a.txt").size
来源：http://hz.xziqi.cn/gtwopsbmrw.html

TS:   fs.statSync("a.txt").size
来源：http://hz.cashguo.top/gtnvucgkpv.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.cdnleiting.top/gtbuyfzepc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yonumen.top/gtmrqppgqd.html

Ruby: File.size("a.txt")
来源：http://hz.zhongyouzk.top/gtfeuekerw.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.sweek.top/gtftmkgtlr.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.meibo888.top/gtzwbfawtp.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zhixingplan.top/gtnvlioeag.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.sxryk.cn/gtxeavabse.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.bjfxy.top/gtmpnoqsko.html

TS:   path.extname("a.txt")
来源：http://hz.jiagoushi.top/gtewiolirb.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.smart0.xyz/gtxijrgznp.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.feifeiyinyue.top/gtqjrzfepy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ybcxt.top/gtqiizujjk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.daxiang520.top/gteudybqtk.html

[F11] 复制与移动文件
来源：http://hz.pycfn.com/gtkvgvmult.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.quarkkingdee.top/gtilpowjcm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.quarkkingdee.top/gtkrubrkmx.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.bjfxy.top/gtldewiwiz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.gotoacloud.top/gtkxrvsuop.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.vqdsnc.cn/gtqjwlswzg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.birdmap.top/gteeptyvzm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.tian-w.cn/gtkfycooar.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.quarkkingdee.top/gtidfhjqzw.html

[F12] CSV 读写
来源：http://hz.wangdashe.top/gtfmqcahfh.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.cucudq.cn/gtpotsrgaf.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yuxming.cn/gtzeokyses.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.wangshuangyany.cn/gtgdqdbnrm.html

TS:   // 同上
来源：http://hz.iojbl.cn/gthznnfpjc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jianghu66.top/gtjoletbzt.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.chenzaomai.com/gtbxlapzvn.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ivvv.top/gtifopbiva.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.yueranfly.top/gtfipmjpqs.html

================================================================================
来源：http://hz.nanxinkj.top/gtrousjwlz.html

G. 面向对象
来源：http://hz.daria6918.cn/gtcusodlwg.html

================================================================================
来源：http://hz.fzhhl.top/gtydxcwlqi.html

[G01] 定义类
来源：http://hz.jinqigfzy.top/gtmsggmdao.html

Py:   class User: pass
来源：http://hz.jqgufenzy.top/gtytjcjvxc.html

PHP:  class User {}
来源：http://hz.hammf.cn/gtpimphyer.html

JS:   class User {}
来源：http://hz.mhx1999.top/gtddnuphym.html

TS:   class User { name: string = ""; }
来源：http://hz.jianghu66.top/gtkrofjkzr.html

Java: class User {}
来源：http://hz.redwolf501.top/gtgrcxbdya.html

Go:   type User struct { Name string }
来源：http://hz.redwolf501.top/gtnetzhzrq.html

Ruby: class User; end
来源：http://hz.jianghu66.top/gtrjwrhdiu.html

C#:   class User {}
来源：http://hz.zhongyouzk.top/gtkyvtvpia.html

[G02] 构造函数
来源：http://hz.yongpay.top/gtgzditgfl.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.shanyushiyangtech.top/gtfunfutiq.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yonumen.top/gtdsmwxmvi.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.ydjk.org.cn/gtwbwxbqva.html

TS:   constructor(public name: string) {}
来源：http://hz.birdmap.top/gtlemfnpfm.html

Java: User(String name) { this.name = name; }
来源：http://hz.birdmap.top/gtplswjahr.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.shanyushiyangkeji.top/gtiqulqhcm.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.nanxuanxn.top/gthcywyhee.html

C#:   public User(string name) { Name = name; }
来源：http://hz.chenlongwang.top/gtejuixehs.html

[G03] 实例属性
来源：http://hz.jqgfzy.top/gtkgdaxzpj.html

Py:   self.name = "x"
来源：http://hz.redwolf501.top/gtrxufsxyv.html

PHP:  public string $name = "x";
来源：http://hz.kuanghao11.cn/gtserbegjq.html

JS:   this.name = "x";
来源：http://hz.yj202588.top/gtyoaurlkp.html

TS:   name: string = "x";
来源：http://hz.0kj1m.cn/gtkfscfsqd.html

Java: private String name;
来源：http://hz.zhixingplan.top/gtvmtkmedz.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yj202588.top/gtaygjxbti.html

Ruby: @name = "x"
来源：http://hz.yj20258.top/gtxhzgbgjq.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.shanyushiyangkeji.top/gtbpcgzcnd.html

[G04] 定义方法
来源：http://hz.ivvv.top/gtpchhlodb.html

Py:   def greet(self): return self.name
来源：http://hz.dashuyun.cn/gtiwvkgpin.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.svipenyu.cn/gtyrelxsnu.html

JS:   greet() { return this.name; }
来源：http://hz.hnqzz.top/gtsgdeazaa.html

TS:   greet(): string { return this.name; }
来源：http://hz.redwolf501.top/gtemmkttoq.html

Java: String greet() { return name; }
来源：http://hz.yuanzhike.top/gtqyrsiclb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.sysykeji.top/gtibnxowlw.html

Ruby: def greet; @name; end
来源：http://hz.yonumen.top/gtzbsswjsi.html

C#:   public string Greet() => Name;
来源：http://hz.chenjidiqi.icu/gtqlosnxqb.html

[G05] 继承
来源：http://hz.shanyushiyangkeji.top/gticukbixb.html

Py:   class Admin(User): pass
来源：http://hz.xziqi.cn/gthgzfaarb.html

PHP:  class Admin extends User {}
来源：http://hz.andypj.xyz/gtajounwys.html

JS:   class Admin extends User {}
来源：http://hz.haohaochexian.top/gtuccxbzac.html

TS:   class Admin extends User {}
来源：http://hz.shangyingyoupin.top/gtdeddddly.html

Java: class Admin extends User {}
来源：http://hz.feifeiyinyue.top/gtrqsaztyd.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yuxming.cn/gtnixwsbbd.html

Ruby: class Admin < User; end
来源：http://hz.sysykeji.top/gtmtvgodam.html

C#:   class Admin : User {}
来源：http://hz.aizwys.cn/gttlyzjepn.html

[G06] 重写方法
来源：http://hz.guannengcc.top/gtfehvrgdc.html

Py:   def greet(self): return "admin"
来源：http://hz.tian-w.cn/gtneieebhe.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zhaomingkeji.xyz/gtrdfkmjpe.html

JS:   greet() { return "admin"; }
来源：http://hz.meibo888.top/gtntkcayac.html

TS:   greet(): string { return "admin"; }
来源：http://hz.wangdashe.top/gtdnqeumoy.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ehwqpu.com/gtlcxneaze.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.cashguo.top/gtvotqarpv.html

Ruby: def greet; "admin"; end
来源：http://hz.ydjk.org.cn/gtegkmhnud.html

C#:   public override string Greet() => "admin";
来源：http://hz.cheryme.top/gtsdvsgqlf.html

[G07] 调用父类方法
来源：http://hz.gaohongyu789.top/gtwipxkzqu.html

Py:   super().greet()
来源：http://hz.c1oappe.top/gtygerdimn.html

PHP:  parent::greet();
来源：http://hz.jiagoushi.top/gtctsrfksu.html

JS:   super.greet();
来源：http://hz.xingfuxueyuan.xyz/gthtpvjcja.html

TS:   super.greet();
来源：http://hz.hywenlv.cn/gtsyhlcfxu.html

Java: super.greet();
来源：http://hz.iojbl.cn/gtdiudcjzb.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.gzhubu.top/gtjfjszaoq.html

Ruby: super
来源：http://hz.gogol.net.cn/gtesjkbgcd.html

C#:   base.Greet();
来源：http://hz.jyoumei.cn/gtpspaalsz.html

[G08] 静态方法与属性
来源：http://hz.xziqi.cn/gttdwuhykc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhixingplan.top/gttyylzneg.html

PHP:  public static function f() {}
来源：http://hz.bjfxy.top/gtrntirthw.html

JS:   static f() {}
来源：http://hz.shanyushiyangtech.top/gtsbzhgtmz.html

TS:   static f(): void {}
来源：http://hz.nwbrower.top/gtoelzkjgj.html

Java: static void f() {}
来源：http://hz.jinqigufen.top/gtjndlvjev.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.316326.xyz/gtjxfhsuzv.html

Ruby: def self.f; end
来源：http://hz.cashguo.top/gtrfnxezsf.html

C#:   public static void F() {}
来源：http://hz.hfpthk.cn/gtjmvpmhay.html

[G09] 接口 / 抽象类
来源：http://hz.fzhhl.top/gtangttvul.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.redwolf501.top/gtbphgbmtb.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.xingfuxueyuan.xyz/gtorojemkc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.xinyue.icu/gtxrlswskw.html

TS:   interface Shape { area(): number; }
来源：http://hz.cdnleiting.top/gtgyxpnpuw.html

Java: interface Shape { double area(); }
来源：http://hz.haohaochexian.top/gtongvsuoi.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.gaohongyu789.top/gtnubawpsa.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hysaishi.cn/gttzttqvnc.html

C#:   interface IShape { double Area(); }
来源：http://hz.shuidangran.top/gtlgwzunmi.html

[G10] 访问控制
来源：http://hz.gzhubu.top/gtfexnvqcb.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.wangdashe.top/gttgwocyhf.html

PHP:  public / protected / private
来源：http://hz.wangdashe.top/gtityfszki.html

JS:   #private 字段；其余公开
来源：http://hz.cqqwz.cn/gtnitwakhu.html

TS:   public / protected / private
来源：http://hz.yj202588.top/gtdgxushot.html

Java: public / protected / private / 默认包级
来源：http://hz.iojbl.cn/gtttoiweeu.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.9152youxi.cn/gtzjigwnut.html

Ruby: public / protected / private
来源：http://hz.zhijiandao.cn/gtcryczhjr.html

C#:   public / protected / private / internal
来源：http://hz.zhiwuduotai.top/gteainscnm.html

[G11] getter / setter
来源：http://hz.xuetiantiany.cn/gtlblqzyer.html

Py:   @property 与 @x.setter
来源：http://hz.iojbl.cn/gtswjpgxer.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.tianlin.xyz/gtwnykdiim.html

JS:   get name() { return this._name; }
来源：http://hz.tian-w.cn/gthmviddtu.html

TS:   get name(): string { return this._name; }
来源：http://hz.dashuyun.cn/gtxjdkbiqf.html

Java: public String getName() { return name; }
来源：http://hz.mhx1999.top/gtzvkdajxw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.sysykeji.top/gtljlmvmtf.html

Ruby: attr_accessor :name
来源：http://hz.haohaochexian.top/gtntwzjqxb.html

C#:   public string Name { get; set; }
来源：http://hz.bjfxy.top/gtnvmsrspz.html

[G12] 对象转字符串
来源：http://hz.sysykeji.top/gtvcjbfcvt.html

Py:   def __str__(self): return self.name
来源：http://hz.bjfxy.top/gtefivqqpz.html


<!-- 参考信息 -->