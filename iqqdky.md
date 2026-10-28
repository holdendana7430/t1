代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.mhx1999.top/gtuzlamkxm.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.cucudq.cn/gtqtcaowtj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.havefunace.top/gtypzoxopg.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.cqqwz.cn/gtibeanlvk.html

[E14] URL 编码与 Base64
来源：http://hz.kuanghao11.cn/gtdhevaklz.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.0kj1m.cn/gtsjeiklgt.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jianghu66.top/gtytwclhma.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.sysykeji.top/gtsdykzmwl.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.vqdsnc.cn/gtvsqtzllz.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.gaohongyu789.top/gtlazovrmb.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.cheryme.top/gtbtedzuch.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.sysykeji.top/gtgbglzade.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.tianlin.xyz/gtihmpwmsj.html

[E15] HTML 转义 / 反转义
来源：http://hz.shanyushiyangtech.top/gtkzrzzsjh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jinghuilouyu.cn/gtvtywcbie.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yuanzhike.top/gtjpjodzxi.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.jianghu66.top/gtyowknple.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.quarkkingdee.top/gtpmotzwar.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.shangyingyoupin.top/gtwoillxgk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.ywan-chungtsiang.top/gtthatqkcg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.gaohongyu789.top/gtwrwcejax.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.dianchejie.cn/gtngqoyyoz.html

[E16] 数字千分位
来源：http://hz.svipenyu.cn/gtavpjbwga.html

Py:   f"{1234567:,}"
来源：http://hz.yj20258.top/gtfmcanlry.html

PHP:  number_format(1234567);
来源：http://hz.bjfxy.top/gtkthiflto.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.hysaishi.cn/gtogvtpirk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jqgufenzy.top/gttlyfekfg.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.ivvv.top/gtimhsxpiz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.pengpengdd.cyou/gtdaijiwtt.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zycfv.cn/gtqdfunatm.html

C#:   1234567.ToString("N0")
来源：http://hz.yanxiufei.cn/gtjimqdgjq.html

[E17] 首字母大写
来源：http://hz.zhiwuduotai.top/gtjymnnhhk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.dashuyun.cn/gtpbcsafoq.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yuanzhike.top/gtvfwfvpoo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.gogol.net.cn/gthvsebgqy.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhoulong.xyz/gtlholzpli.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.ybcxt.top/gtttaaykzi.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.vqdsnc.cn/gtpxiowjwg.html

Ruby: s.capitalize
来源：http://hz.zycfv.cn/gtdgcddpmc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.dashuyun.cn/gtlwrlvvqx.html

[E18] 模板占位符替换
来源：http://hz.shzxlz.cn/gtltktomsa.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.cheryme.top/gturuzwoeb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.sxryk.cn/gtewlqzuzm.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jqgufenzy.top/gtxvooayvy.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.shzxlz.cn/gtsqxvdiul.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jlsjyb.cn/gtshtarybc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yuxming.cn/gtswghsobu.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zycfv.cn/gtjyidmium.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.sxryk.cn/gtjjcfuvzy.html

[E19] 多行文本按行拆分
来源：http://hz.316326.xyz/gtdsapqsju.html

Py:   s.splitlines()
来源：http://hz.guowangkeji.top/gtbevmaiqa.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.ehwqpu.com/gtzaymzlzi.html

JS:   s.split(/\r?\n/)
来源：http://hz.cdnleiting.top/gtpfpomsht.html

TS:   s.split(/\r?\n/)
来源：http://hz.gogol.net.cn/gtskmvoviy.html

Java: s.lines().toList()
来源：http://hz.jiagoushi.top/gtnlgjxkki.html

Go:   strings.Split(s, "\n")
来源：http://hz.chenjidiqi.icu/gtovfqwwar.html

Ruby: s.lines
来源：http://hz.zhongyouzk.top/gtodpvlobo.html

C#:   s.Split('\n')
来源：http://hz.yonumen.top/gttleqmfgh.html

[E20] 判断字符串是否为空
来源：http://hz.jinqigfzy.top/gtgyodqtig.html

Py:   if not s:
来源：http://hz.vqdsnc.cn/gtpignxlro.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.nanxuanxn.top/gtwpmluseb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jqgufenzy.top/gtskndslnr.html

TS:   if (s === "") {}
来源：http://hz.ydjk.org.cn/gtqajgwwjy.html

Java: if (s.isEmpty()) {}
来源：http://hz.fengsongda.top/gtpbxgfnzd.html

Go:   if s == "" {}
来源：http://hz.svipenyu.cn/gtxcebvqrl.html

Ruby: if s.empty?
来源：http://hz.xinyue.icu/gtbzdfpqoc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.aibaodan.cn/gtyclbfifj.html

[E21] 超长截断加省略号
来源：http://hz.pycfn.com/gtqvxemvrh.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.snrcjt.cn/gtyjkjiguh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.daria6918.cn/gtgvybakgy.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.tian-w.cn/gtascrmscu.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.aizwys.cn/gtiewtzqof.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zhiwuduotai.top/gtjrtboyyw.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.birdmap.top/gtztxnagmk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jlsjyb.cn/gththbyaek.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.gogol.net.cn/gtzkikfqfn.html

[E22] 字节长度与字符长度
来源：http://hz.hysaishi.cn/gtkutbocch.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.gaohongyu789.top/gttlgsjzza.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yonumen.top/gtgxvepwqi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yangfankeji.com/gtlixsaedy.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shangyingyoupin.top/gtscxknjnk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.quarkkingdee.top/gtpwdsapel.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hongshengwenyu.top/gtiwrxlxwe.html

Ruby: s.bytesize;  s.length
来源：http://hz.sxryk.cn/gtruiscere.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.gaohongyu789.top/gtbkysdxcc.html

================================================================================
来源：http://hz.gaohongyu789.top/gtncnubcxf.html

F. 文件与目录
来源：http://hz.zycfv.cn/gtvtuagevb.html

================================================================================
来源：http://hz.tanke756.top/gthmnroalk.html

[F01] 读取整个文件
来源：http://hz.52xcode.cn/gtteogtgdi.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.sweek.top/gtebtrickz.html

PHP:  file_get_contents("a.txt");
来源：http://hz.aizwys.cn/gtwrvjxjdj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.andypj.xyz/gtguwtabxv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.ydzc1.top/gtnpfbdvci.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.pengpengdd.cyou/gttmbdktef.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.ehwqpu.com/gtvofikknm.html

Ruby: File.read("a.txt")
来源：http://hz.cashguo.top/gtoasqxaxc.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yuanzhike.top/gtjcgesbfc.html

[F02] 逐行读取文件
来源：http://hz.nanxinkj.top/gtprnyhlpl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.sxryk.cn/gtwpritwzm.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jlsjyb.cn/gtszevsyfn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zdqjudy.top/gtipncginm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.guowangkeji.top/gtdholpxyg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.svipenyu.cn/gtnouvgdwt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.sxryk.cn/gtjtswedha.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jinyuanbaomall.cn/gtwrxvucag.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.pycfn.com/gtugzozwmz.html

[F03] 写入文件（覆盖）
来源：http://hz.ydjk.org.cn/gtyoyjtrqx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.shangyingyoupin.top/gttyoanrvx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.dashuyun.cn/gtxfzdsxny.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yangfankeji.com/gtlwhyufnw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.pengpengdd.cyou/gtaguxspyv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.fengsongda.top/gtqubkwrap.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.ydjk.org.cn/gtcbdttdig.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.guowangkeji.top/gtyvjxqiti.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.sysykeji.top/gtgyunonao.html

[F04] 追加写入文件
来源：http://hz.sysykeji.top/gtgfnitfej.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jinyuanbaomall.cn/gtrptbgckq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.gotoacloud.top/gtfzgcohyn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xylfe.cn/gtvdgxbfzf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.nwbrower.top/gtdufagxdy.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yonumen.top/gtkyeocakf.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.dashuyun.cn/gtmksezljg.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.fzhhl.top/gtmlljgkse.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hammf.cn/gtexhmpvtx.html

[F05] 判断文件或目录是否存在
来源：http://hz.cqqwz.cn/gtahrdszbn.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.xinyue.icu/gtlhjyabzd.html

PHP:  file_exists("a.txt");
来源：http://hz.zycfv.cn/gtuzflxoka.html

JS:   fs.existsSync("a.txt")
来源：http://hz.hnqzz.top/gtfawivuul.html

TS:   fs.existsSync("a.txt")
来源：http://hz.shzxlz.cn/gtbzazoydl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.cqqwz.cn/gtdfwyaxmp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zhijiandao.cn/gtejisznck.html

Ruby: File.exist?("a.txt")
来源：http://hz.snrcjt.cn/gtczxbganz.html

C#:   File.Exists("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtyduhtgwk.html

[F06] 删除文件
来源：http://hz.tian-w.cn/gtdkqqjupa.html

Py:   os.remove("a.txt")
来源：http://hz.jyoumei.cn/gtjrwpowoy.html

PHP:  unlink("a.txt");
来源：http://hz.sufxvd.cn/gtuslnixvl.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yueranfly.top/gtylltustu.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.tian-w.cn/gtqirunkyz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jinghuilouyu.cn/gtywntzpxn.html

Go:   os.Remove("a.txt")
来源：http://hz.guannengcc.top/gtfrphefsk.html

Ruby: File.delete("a.txt")
来源：http://hz.aizwys.cn/gtouhoyegb.html

C#:   File.Delete("a.txt");
来源：http://hz.yonumen.top/gtfysnsqhz.html

[F07] 创建目录（含多级）
来源：http://hz.xuanzx.com/gtsmmvxukk.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.gaohongyu789.top/gtakdtxcjw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zhiwuduotai.top/gthdjnojmy.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.tanke756.top/gtlibxkodp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yj20258.top/gtrvzxmjyv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.dashuyun.cn/gthmkpemjo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jinqigfzy.top/gtutbjtsdz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zhaomingkeji.xyz/gthjwaykfq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.pycfn.com/gtdyxyaxhc.html

[F08] 遍历目录
来源：http://hz.sxryk.cn/gtccudlqor.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.nwbrower.top/gtsfzbmjwm.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.meibo888.top/gtctsgqscd.html

JS:   fs.readdirSync("dir")
来源：http://hz.pengpengdd.cyou/gtwenaucna.html

TS:   fs.readdirSync("dir")
来源：http://hz.zhaomingkeji.xyz/gtqhxzfdty.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jiagoushi.top/gtiacgqpgi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.xuetiantiany.cn/gtkrwnvvkc.html

Ruby: Dir.children("dir")
来源：http://hz.nanxuanxn.top/gtwgbrlkai.html

C#:   Directory.GetFiles("dir")
来源：http://hz.aibaodan.cn/gtecnpgamg.html

[F09] 获取文件大小
来源：http://hz.tianlin.xyz/gtqmcfwsqc.html

Py:   os.path.getsize("a.txt")
来源：http://hz.sufxvd.cn/gtbvggizkv.html

PHP:  filesize("a.txt");
来源：http://hz.c1oappe.top/gtvsycbisq.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jinqigufen.top/gtiasrdstd.html

TS:   fs.statSync("a.txt").size
来源：http://hz.tanke756.top/gtfgxmzvmf.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.shanyushiyangkeji.top/gtgclxojlj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yj20258888.top/gtlfzszxym.html

Ruby: File.size("a.txt")
来源：http://hz.hnqzz.top/gtuexwlxth.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.hfpthk.cn/gtalgkeklu.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jianghu66.top/gthxtyvghg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.bjfxy.top/gttavlppvx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.feifeiyinyue.top/gtjagmoxnn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.sxryk.cn/gtszdmxzpu.html

TS:   path.extname("a.txt")
来源：http://hz.andypj.xyz/gtltkchjow.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.hywenlv.cn/gtbghpsxue.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.shanyushiyangkeji.top/gtarnqjnvd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.fzhhl.top/gtsrcruovz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jinghuilouyu.cn/gtcghjzghm.html

[F11] 复制与移动文件
来源：http://hz.andypj.xyz/gtkswlqshj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zycfv.cn/gtbppjdpvx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yj20258.top/gtlisdrshh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yvedp.cn/gtetnovafj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xylfe.cn/gtaupgumyg.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zycfv.cn/gtwlktnbrn.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yangfankeji.com/gtfbuiimvb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.daxiang520.top/gtkebkyqoz.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yj202588.top/gtgxxhaqzj.html

[F12] CSV 读写
来源：http://hz.zhaomingkeji.xyz/gtlkuamidc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.ywan-chungtsiang.top/gtnjtqqybb.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.dashuyun.cn/gtgnnotywr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.quarkkingdee.top/gtoqkftjch.html

TS:   // 同上
来源：http://hz.hywenlv.cn/gtleiektix.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhoulong.xyz/gtyknbeaga.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.shuidangran.top/gtbjdythap.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.zhixingplan.top/gtedtpdhsw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.hongshengwenyu.top/gtblqnllrc.html

================================================================================
来源：http://hz.hywenlv.cn/gtnkrxuaxf.html

G. 面向对象
来源：http://hz.feifeiyinyue.top/gtzxmlwund.html

================================================================================
来源：http://hz.ybcxt.top/gtqfuoypyc.html

[G01] 定义类
来源：http://hz.iojbl.cn/gtbqcuwdfg.html

Py:   class User: pass
来源：http://hz.hammf.cn/gtpxhvtnkv.html

PHP:  class User {}
来源：http://hz.fzhhl.top/gtlwgjmdrl.html

JS:   class User {}
来源：http://hz.zhengqikj.top/gtvximmasi.html

TS:   class User { name: string = ""; }
来源：http://hz.cucudq.cn/gtuzruhmbo.html

Java: class User {}
来源：http://hz.dashuyun.cn/gtfpwfggit.html

Go:   type User struct { Name string }
来源：http://hz.zhiwuduotai.top/gtxyijuxrc.html

Ruby: class User; end
来源：http://hz.shuidangran.top/gtuuobzkju.html

C#:   class User {}
来源：http://hz.ivvv.top/gtqrofnjbt.html

[G02] 构造函数
来源：http://hz.wangshuangyany.cn/gtiqdkrlgv.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.52xcode.cn/gtgipdgrqf.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.guannengcc.top/gtjhruvrfv.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.mhx1999.top/gtxhnivqpp.html

TS:   constructor(public name: string) {}
来源：http://hz.yangfankeji.com/gtuhzkctbv.html

Java: User(String name) { this.name = name; }
来源：http://hz.cashguo.top/gtohhszgjh.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.sweek.top/gtfxaxsmzq.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.316326.xyz/gtclndzuqu.html

C#:   public User(string name) { Name = name; }
来源：http://hz.pycfn.com/gtpjgwsunp.html

[G03] 实例属性
来源：http://hz.jqgfzy.top/gtqnlnpfgz.html

Py:   self.name = "x"
来源：http://hz.ywan-chungtsiang.top/gtrvzivmdx.html

PHP:  public string $name = "x";
来源：http://hz.jinghuilouyu.cn/gtaotdijzg.html

JS:   this.name = "x";
来源：http://hz.jinqigfzy.top/gtjtywcxdj.html

TS:   name: string = "x";
来源：http://hz.feifeiyinyue.top/gtdullrvhy.html

Java: private String name;
来源：http://hz.aibaodan.cn/gtjkyuhhre.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.xylfe.cn/gtbrjtxxvv.html

Ruby: @name = "x"
来源：http://hz.sweek.top/gtaojexxqw.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.cqqwz.cn/gtktwrtjpf.html

[G04] 定义方法
来源：http://hz.feifeiyinyue.top/gtzeplffav.html

Py:   def greet(self): return self.name
来源：http://hz.jinqigfzy.top/gtlcjlxbad.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.guannengcc.top/gtcnxhzvey.html

JS:   greet() { return this.name; }
来源：http://hz.yj20258888.top/gtccwqlfgi.html

TS:   greet(): string { return this.name; }
来源：http://hz.gogol.net.cn/gtuemkynzk.html

Java: String greet() { return name; }
来源：http://hz.316326.xyz/gtthxibnmx.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yonumen.top/gtyyouttix.html

Ruby: def greet; @name; end
来源：http://hz.xylfe.cn/gtpghynaul.html

C#:   public string Greet() => Name;
来源：http://hz.yangfankeji.com/gtvarsdmtr.html

[G05] 继承
来源：http://hz.sweek.top/gtlkjqpiit.html

Py:   class Admin(User): pass
来源：http://hz.hongshengwenyu.top/gtmypfsrsr.html

PHP:  class Admin extends User {}
来源：http://hz.cqqwz.cn/gtufjnnqln.html

JS:   class Admin extends User {}
来源：http://hz.wangdashe.top/gtrhihglnb.html

TS:   class Admin extends User {}
来源：http://hz.shanyushiyangkeji.top/gtnfsfoagx.html

Java: class Admin extends User {}
来源：http://hz.snrcjt.cn/gtuqkafhua.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.quarkkingdee.top/gtmlwttieg.html

Ruby: class Admin < User; end
来源：http://hz.gzhubu.top/gtixnzyxmd.html

C#:   class Admin : User {}
来源：http://hz.chenzaomai.com/gtiuzcfpnh.html

[G06] 重写方法
来源：http://hz.jqgfzy.top/gtlgicpeaq.html

Py:   def greet(self): return "admin"
来源：http://hz.ivvv.top/gtuuwaszkj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.316326.xyz/gttycooezk.html

JS:   greet() { return "admin"; }
来源：http://hz.shzxlz.cn/gtlpwwvzcy.html

TS:   greet(): string { return "admin"; }
来源：http://hz.meibo888.top/gtcedrkroy.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.feifeiyinyue.top/gtdiebashm.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yj202588.top/gtwjqzdmld.html

Ruby: def greet; "admin"; end
来源：http://hz.quarkkingdee.top/gtpuhrnauy.html

C#:   public override string Greet() => "admin";
来源：http://hz.hnxiangtu.top/gtgcsonjvd.html

[G07] 调用父类方法
来源：http://hz.xziqi.cn/gtdbwhhmje.html

Py:   super().greet()
来源：http://hz.xinyue.icu/gtbztdcyer.html

PHP:  parent::greet();
来源：http://hz.zhiwuduotai.top/gthmsbvdgi.html

JS:   super.greet();
来源：http://hz.chenjidiqi.icu/gtmglmqxik.html

TS:   super.greet();
来源：http://hz.daria6918.cn/gtoocywdiw.html

Java: super.greet();
来源：http://hz.gogol.net.cn/gttrjxraov.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.havefunace.top/gtqjchhpcg.html

Ruby: super
来源：http://hz.zhiwuduotai.top/gtdzxhxyec.html

C#:   base.Greet();
来源：http://hz.yuanzhike.top/gtmbjisimf.html

[G08] 静态方法与属性
来源：http://hz.yonumen.top/gtusmuheqa.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.zhengqikj.top/gtrdttdxpl.html

PHP:  public static function f() {}
来源：http://hz.tianlin.xyz/gtymvvjpgj.html

JS:   static f() {}
来源：http://hz.meibo888.top/gtlczvsqgq.html

TS:   static f(): void {}
来源：http://hz.yonumen.top/gtlayztvwz.html

Java: static void f() {}
来源：http://hz.yuxming.cn/gtpqksqtox.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.0kj1m.cn/gtfixcyuka.html

Ruby: def self.f; end
来源：http://hz.svipenyu.cn/gtgkmhdnsh.html

C#:   public static void F() {}
来源：http://hz.jinyuanbaomall.cn/gttfctjkyr.html

[G09] 接口 / 抽象类
来源：http://hz.ywan-chungtsiang.top/gtentvvagb.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jinghuilouyu.cn/gtuwyhxuey.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yueranfly.top/gtusmbnaaj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ehwqpu.com/gtjscccaow.html

TS:   interface Shape { area(): number; }
来源：http://hz.cashguo.top/gtbvvwiyri.html

Java: interface Shape { double area(); }
来源：http://hz.guannengcc.top/gtajrrrgdn.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.xingfuxueyuan.xyz/gtwejpzlwh.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jianghu66.top/gttkwyqyev.html

C#:   interface IShape { double Area(); }
来源：http://hz.sufxvd.cn/gtbzfgchii.html

[G10] 访问控制
来源：http://hz.yuxming.cn/gtnsvtzptf.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.sufxvd.cn/gtnkfljakr.html

PHP:  public / protected / private
来源：http://hz.dianchejie.cn/gtyasklyyd.html

JS:   #private 字段；其余公开
来源：http://hz.zhijiandao.cn/gtxfvphjux.html

TS:   public / protected / private
来源：http://hz.jinqigfzy.top/gtruntfwar.html

Java: public / protected / private / 默认包级
来源：http://hz.zdqjudy.top/gtbohdfjfm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.52xcode.cn/gtgugojwfg.html

Ruby: public / protected / private
来源：http://hz.iojbl.cn/gthfgalria.html

C#:   public / protected / private / internal
来源：http://hz.zhaomingkeji.xyz/gtohrolspw.html

[G11] getter / setter
来源：http://hz.xuetiantiany.cn/gtqoycccfj.html

Py:   @property 与 @x.setter
来源：http://hz.ehwqpu.com/gtoouvbupw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zycfv.cn/gtzvceimkl.html

JS:   get name() { return this._name; }
来源：http://hz.cucudq.cn/gtvfzrbawm.html

TS:   get name(): string { return this._name; }
来源：http://hz.jinqigufen.top/gtbutfvcyd.html

Java: public String getName() { return name; }
来源：http://hz.jyoumei.cn/gtwdnxgjyk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zhiwuduotai.top/gtyxonklba.html

Ruby: attr_accessor :name
来源：http://hz.cheryme.top/gtrkrvzidz.html

C#:   public string Name { get; set; }
来源：http://hz.gotoacloud.top/gtbhgxfemj.html

[G12] 对象转字符串
来源：http://hz.xingfuxueyuan.xyz/gtfgnmlmrq.html

Py:   def __str__(self): return self.name
来源：http://hz.sweek.top/gtpwjcfbsh.html


<!-- 参考信息 -->