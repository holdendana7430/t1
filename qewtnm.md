代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.tanke756.top/gtxohtudmb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jinqigfzy.top/gtfvxrzvyv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.ydjk.org.cn/gtfujfqnha.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.dianchejie.cn/gtqgmdrmln.html

[E14] URL 编码与 Base64
来源：http://hz.sxryk.cn/gtrobbgybp.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zhijiandao.cn/gtwzkjeipd.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.nanxuanxn.top/gtkloluhrm.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.hammf.cn/gtllnnobrm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.feifeiyinyue.top/gtimemoheb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.tianlin.xyz/gtyyftiggh.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.chenjidiqi.icu/gtuffpnpsc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.zhoulong.xyz/gtovmaieco.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.0kj1m.cn/gtjadqvrep.html

[E15] HTML 转义 / 反转义
来源：http://hz.meibo888.top/gttrlxyunc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zhixingplan.top/gtwfckofqx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.snrcjt.cn/gtkltkyixb.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.gogol.net.cn/gtxwrfxpkq.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.guannengcc.top/gtfikkazoe.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.aibaodan.cn/gtbufanvzz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.sweek.top/gtqfpftgts.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yuanzhike.top/gtzddhycix.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.aibaodan.cn/gtvjpzzbbv.html

[E16] 数字千分位
来源：http://hz.quarkkingdee.top/gtmvrgjafy.html

Py:   f"{1234567:,}"
来源：http://hz.svipenyu.cn/gtgitxjcbd.html

PHP:  number_format(1234567);
来源：http://hz.mhx1999.top/gtjubxtkjn.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.chenjidiqi.icu/gtmkfuetvt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.sufxvd.cn/gtujpjagpu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.ywan-chungtsiang.top/gtsxekiqml.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jyoumei.cn/gtutixfcab.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.aibaodan.cn/gtyvjmceen.html

C#:   1234567.ToString("N0")
来源：http://hz.gaohongyu789.top/gtigzusxgi.html

[E17] 首字母大写
来源：http://hz.nanxuanxn.top/gtvwcoxhfy.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.sysykeji.top/gtchjgvomm.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.tanke756.top/gtuelryuiw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.shangyingyoupin.top/gtdkfgekjh.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhaomingkeji.xyz/gtslzljpil.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.xuanzx.com/gtgejshjyu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.shuidangran.top/gtvsavwcwm.html

Ruby: s.capitalize
来源：http://hz.chenlongwang.top/gtaukitjru.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.xingfuxueyuan.xyz/gtdvggpkqw.html

[E18] 模板占位符替换
来源：http://hz.daxiang520.top/gtyvvaviml.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.gogol.net.cn/gttqzmbvwx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jyoumei.cn/gtkkeyrluz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.cucudq.cn/gtxrvqjteb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yj20258888.top/gtqhygqekh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.hongshengwenyu.top/gtqhmhzqay.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.ydzc1.top/gtndmelelq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hywenlv.cn/gtovqcufpj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.snrcjt.cn/gtloliyise.html

[E19] 多行文本按行拆分
来源：http://hz.hnxiangtu.top/gtfovhonjn.html

Py:   s.splitlines()
来源：http://hz.c1oappe.top/gtqryhzrfm.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jinghuilouyu.cn/gtcvxjmvuk.html

JS:   s.split(/\r?\n/)
来源：http://hz.chenjidiqi.icu/gtxlomesqx.html

TS:   s.split(/\r?\n/)
来源：http://hz.ppjwa.cn/gthyphwwaf.html

Java: s.lines().toList()
来源：http://hz.jinqigufen.top/gtifzhkgpp.html

Go:   strings.Split(s, "\n")
来源：http://hz.hnxiangtu.top/gtojdcfjka.html

Ruby: s.lines
来源：http://hz.mhx1999.top/gtfolevrxd.html

C#:   s.Split('\n')
来源：http://hz.c1oappe.top/gtyuupkdpz.html

[E20] 判断字符串是否为空
来源：http://hz.cdnleiting.top/gtnhdppawt.html

Py:   if not s:
来源：http://hz.zhijiandao.cn/gtnrjfuilu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.snrcjt.cn/gtdffonpml.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.xziqi.cn/gtjxdfpddu.html

TS:   if (s === "") {}
来源：http://hz.yj202588.top/gteufisfkj.html

Java: if (s.isEmpty()) {}
来源：http://hz.wangdashe.top/gtsqrkmoyk.html

Go:   if s == "" {}
来源：http://hz.ehwqpu.com/gtqoprafjs.html

Ruby: if s.empty?
来源：http://hz.shuidangran.top/gtmtvlpiqx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jinqigufen.top/gtryzerfga.html

[E21] 超长截断加省略号
来源：http://hz.cheryme.top/gtxucjyadx.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.chenlongwang.top/gtwpgtdckx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.hnqzz.top/gtfttxeouw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.chenjidiqi.icu/gtxjspogsb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.iojbl.cn/gtxghhcrqa.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.guowangkeji.top/gtvqlxsvfw.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.iojbl.cn/gtybnhkjtb.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.xuetiantiany.cn/gtmpuqyacs.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.wangdashe.top/gtroouuiuv.html

[E22] 字节长度与字符长度
来源：http://hz.c1oappe.top/gtyncshlfe.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.cucudq.cn/gtxetqsdnh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.iojbl.cn/gtmymyvsvt.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jqgufenzy.top/gtlwbcqund.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.pycfn.com/gtchtqhvih.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zhongyouzk.top/gtfryjsbcn.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.andypj.xyz/gtjbkrlweu.html

Ruby: s.bytesize;  s.length
来源：http://hz.birdmap.top/gtllozbils.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.316326.xyz/gttasdpeey.html

================================================================================
来源：http://hz.vqdsnc.cn/gtpdhcsfku.html

F. 文件与目录
来源：http://hz.xuanzx.com/gtnhyqlewd.html

================================================================================
来源：http://hz.jlsjyb.cn/gtzsfazzjd.html

[F01] 读取整个文件
来源：http://hz.zhaomingkeji.xyz/gtabvyflus.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.xingfuxueyuan.xyz/gtfcqfihnq.html

PHP:  file_get_contents("a.txt");
来源：http://hz.tianlin.xyz/gtlzdcpxtp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jinghuilouyu.cn/gtdhwbmtjk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yonumen.top/gtmwgtzuwb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.cdnleiting.top/gtkpamrdww.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.gaohongyu789.top/gtpmztpbma.html

Ruby: File.read("a.txt")
来源：http://hz.tian-w.cn/gtffviledz.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.ydzc1.top/gtkzhcpysk.html

[F02] 逐行读取文件
来源：http://hz.ybcxt.top/gtpcfplwse.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.hfpthk.cn/gtkkzskpmj.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jiagoushi.top/gtjkfvjjjc.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xziqi.cn/gtqcxrhcii.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xziqi.cn/gtmetzxjrf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.hnqzz.top/gtevdskkke.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yj20258.top/gtolunbdrb.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yanxiufei.cn/gtfggtnjvu.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.shanyushiyangtech.top/gtahdqxzba.html

[F03] 写入文件（覆盖）
来源：http://hz.xingfuxueyuan.xyz/gtatebxkps.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jinghuilouyu.cn/gtblemjtwo.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.fengsongda.top/gtnjcnefod.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yanxiufei.cn/gtabzvgxhw.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sysykeji.top/gtecgskhib.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zhongyouzk.top/gtmqjpkwgr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.dianchejie.cn/gtqbehlszm.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yanxiufei.cn/gtyfakriis.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.shanyushiyangtech.top/gtsryoiolf.html

[F04] 追加写入文件
来源：http://hz.ehwqpu.com/gtpwwugsro.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jlsjyb.cn/gtzmnurfgc.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.nanxinkj.top/gtaftkrxrg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.redwolf501.top/gtrufmjklp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.snrcjt.cn/gtnhdkxpat.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yj20258888.top/gtzeqrthbq.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yanxiufei.cn/gtofdxrhvy.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.xinyue.icu/gtuplgwwyk.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.c1oappe.top/gtrfemznbs.html

[F05] 判断文件或目录是否存在
来源：http://hz.zhijiandao.cn/gtcnabmsws.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yonumen.top/gtsjvqlaea.html

PHP:  file_exists("a.txt");
来源：http://hz.tianlin.xyz/gtdqnmfldf.html

JS:   fs.existsSync("a.txt")
来源：http://hz.316326.xyz/gtitqnqigg.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yj20258888.top/gtpnyhsvev.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hysaishi.cn/gtihytfwgg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yj20258.top/gtmhsyhwnq.html

Ruby: File.exist?("a.txt")
来源：http://hz.havefunace.top/gtdhxhetns.html

C#:   File.Exists("a.txt")
来源：http://hz.316326.xyz/gtxbvoxbcq.html

[F06] 删除文件
来源：http://hz.ywan-chungtsiang.top/gtijbevgwc.html

Py:   os.remove("a.txt")
来源：http://hz.chenzaomai.com/gtxwpryclk.html

PHP:  unlink("a.txt");
来源：http://hz.cqqwz.cn/gtvsspymta.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.ehwqpu.com/gtqdrazirl.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.iojbl.cn/gtmagqwznn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.hnqzz.top/gtevjqconq.html

Go:   os.Remove("a.txt")
来源：http://hz.tian-w.cn/gtajgqogbk.html

Ruby: File.delete("a.txt")
来源：http://hz.yangfankeji.com/gtqpjebwav.html

C#:   File.Delete("a.txt");
来源：http://hz.52xcode.cn/gtnyqnoprf.html

[F07] 创建目录（含多级）
来源：http://hz.ybcxt.top/gtwizgazwc.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hywenlv.cn/gtmetfdgfg.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.mhx1999.top/gtkuhpxeqg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ybcxt.top/gthguopcrn.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yueranfly.top/gthyvuvtkn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.tianlin.xyz/gtbypkrowh.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yj202588.top/gtibzarmyi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.9152youxi.cn/gtldvqclas.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.chenzaomai.com/gttzzifhbf.html

[F08] 遍历目录
来源：http://hz.chenjidiqi.icu/gtrqtsvrbq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.sufxvd.cn/gtatkpyarn.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jinyuanbaomall.cn/gttxicjzcc.html

JS:   fs.readdirSync("dir")
来源：http://hz.jyoumei.cn/gtlaxvnksz.html

TS:   fs.readdirSync("dir")
来源：http://hz.jinyuanbaomall.cn/gtcwnpkilk.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.9152youxi.cn/gtgaggtrou.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.haohaochexian.top/gtsghzshax.html

Ruby: Dir.children("dir")
来源：http://hz.dashuyun.cn/gtdsbeyoim.html

C#:   Directory.GetFiles("dir")
来源：http://hz.cqqwz.cn/gtjkifthxk.html

[F09] 获取文件大小
来源：http://hz.bjfxy.top/gtxjjveixn.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yj20258888.top/gtyzlgrvda.html

PHP:  filesize("a.txt");
来源：http://hz.hywenlv.cn/gtpgfbttof.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yj202588.top/gtmczaqpnr.html

TS:   fs.statSync("a.txt").size
来源：http://hz.yuxming.cn/gthndhwtim.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.9152youxi.cn/gtrkkfjhou.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.dashuyun.cn/gtfaabgxbn.html

Ruby: File.size("a.txt")
来源：http://hz.jlsjyb.cn/gtwzmpobyv.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.guowangkeji.top/gtyudmtdtx.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.tianlin.xyz/gtcyfotpyg.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zhixingplan.top/gtiliitsos.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.hywenlv.cn/gtjwblsxow.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yj20258.top/gtgudamopf.html

TS:   path.extname("a.txt")
来源：http://hz.316326.xyz/gtbsblygvk.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.ydzc1.top/gtieixcxxq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.wangdashe.top/gtdxndlomm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.tanke756.top/gtjitidlfr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.nanxuanxn.top/gtxibkbmvj.html

[F11] 复制与移动文件
来源：http://hz.jiagoushi.top/gtqdgblmau.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.shangyingyoupin.top/gtkiwyekms.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hammf.cn/gttmnwsgmd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.aibaodan.cn/gttcovpzys.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.wangdashe.top/gtkrmpbolm.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yanxiufei.cn/gtwyavogvx.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.cucudq.cn/gtfbrrttuc.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.cheryme.top/gtidhlfjau.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.xylfe.cn/gtjxhptfgb.html

[F12] CSV 读写
来源：http://hz.shangyingyoupin.top/gtvbxfvsjw.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xylfe.cn/gtojylwgls.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hysaishi.cn/gtysanldsu.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.shangyingyoupin.top/gtzyqxxijk.html

TS:   // 同上
来源：http://hz.yongpay.top/gtwjdhrdaz.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.nanxuanxn.top/gtvvpvxbcs.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.guowangkeji.top/gthamgpvel.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.chenjidiqi.icu/gtcooslwqp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.sufxvd.cn/gtsjlxgyuz.html

================================================================================
来源：http://hz.fengsongda.top/gtmyhnpulm.html

G. 面向对象
来源：http://hz.guannengcc.top/gthjfhngnj.html

================================================================================
来源：http://hz.hywenlv.cn/gtkyvrpzkd.html

[G01] 定义类
来源：http://hz.jinghuilouyu.cn/gtdscfwhir.html

Py:   class User: pass
来源：http://hz.yanxiufei.cn/gtsnjqhrmf.html

PHP:  class User {}
来源：http://hz.dashuyun.cn/gtoclmyxaj.html

JS:   class User {}
来源：http://hz.nwbrower.top/gttyllcwjl.html

TS:   class User { name: string = ""; }
来源：http://hz.yj202588.top/gtbzqjbtnw.html

Java: class User {}
来源：http://hz.shanyushiyangtech.top/gtqxoeybft.html

Go:   type User struct { Name string }
来源：http://hz.wangshuangyany.cn/gtgnpbilph.html

Ruby: class User; end
来源：http://hz.chenlongwang.top/gtjwnomged.html

C#:   class User {}
来源：http://hz.feifeiyinyue.top/gtvshqucpn.html

[G02] 构造函数
来源：http://hz.wangshuangyany.cn/gtntfvyhjn.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.316326.xyz/gtnwannlzj.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.chenjidiqi.icu/gtzhwajkeh.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.316326.xyz/gtrxxnzmnw.html

TS:   constructor(public name: string) {}
来源：http://hz.yueranfly.top/gtdujnlvqn.html

Java: User(String name) { this.name = name; }
来源：http://hz.xziqi.cn/gtgmucbqwq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.ybcxt.top/gtpbrqdemv.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.gaohongyu789.top/gtrjsyazvp.html

C#:   public User(string name) { Name = name; }
来源：http://hz.yanxiufei.cn/gthhqupsas.html

[G03] 实例属性
来源：http://hz.yueranfly.top/gtlppkfbso.html

Py:   self.name = "x"
来源：http://hz.ydjk.org.cn/gtbuujvfhs.html

PHP:  public string $name = "x";
来源：http://hz.shangyingyoupin.top/gtqokxdbog.html

JS:   this.name = "x";
来源：http://hz.tianlin.xyz/gtgsyddxze.html

TS:   name: string = "x";
来源：http://hz.tian-w.cn/gtxeopqchf.html

Java: private String name;
来源：http://hz.chenjidiqi.icu/gtpjovpbqu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.meibo888.top/gtboiyiyyb.html

Ruby: @name = "x"
来源：http://hz.fengsongda.top/gtuzklulne.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.shanyushiyangtech.top/gtcqgyltqq.html

[G04] 定义方法
来源：http://hz.zhiwuduotai.top/gtkccjyodb.html

Py:   def greet(self): return self.name
来源：http://hz.aibaodan.cn/gtkvzbpial.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.nwbrower.top/gtklzkmdry.html

JS:   greet() { return this.name; }
来源：http://hz.bjfxy.top/gtybqgomap.html

TS:   greet(): string { return this.name; }
来源：http://hz.pycfn.com/gtoqvppbqp.html

Java: String greet() { return name; }
来源：http://hz.hongshengwenyu.top/gtnecosgmn.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.cheryme.top/gtuimhejux.html

Ruby: def greet; @name; end
来源：http://hz.yueranfly.top/gtbburizkc.html

C#:   public string Greet() => Name;
来源：http://hz.nanxuanxn.top/gtpoxarfod.html

[G05] 继承
来源：http://hz.zhixingplan.top/gthsjzyjcm.html

Py:   class Admin(User): pass
来源：http://hz.xuetiantiany.cn/gtwcmgrbrb.html

PHP:  class Admin extends User {}
来源：http://hz.ywan-chungtsiang.top/gtaionkoni.html

JS:   class Admin extends User {}
来源：http://hz.meibo888.top/gtxkkewjgt.html

TS:   class Admin extends User {}
来源：http://hz.guannengcc.top/gtihinggjm.html

Java: class Admin extends User {}
来源：http://hz.feifeiyinyue.top/gtsqfnuqem.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.mhx1999.top/gtgypmgzod.html

Ruby: class Admin < User; end
来源：http://hz.gotoacloud.top/gtdwvlsydz.html

C#:   class Admin : User {}
来源：http://hz.zhixingplan.top/gtemyrmxif.html

[G06] 重写方法
来源：http://hz.ehwqpu.com/gteaawsawy.html

Py:   def greet(self): return "admin"
来源：http://hz.hysaishi.cn/gtxcmdkopm.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.chenjidiqi.icu/gtfljjfkve.html

JS:   greet() { return "admin"; }
来源：http://hz.haohaochexian.top/gtpnhzzrwe.html

TS:   greet(): string { return "admin"; }
来源：http://hz.wangdashe.top/gtxwlkieag.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hongshengwenyu.top/gtlesanqvu.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.dianchejie.cn/gtjvghuxjy.html

Ruby: def greet; "admin"; end
来源：http://hz.jyoumei.cn/gtgtcmanjx.html

C#:   public override string Greet() => "admin";
来源：http://hz.jlsjyb.cn/gtqlpafdla.html

[G07] 调用父类方法
来源：http://hz.yuanzhike.top/gtoomjqair.html

Py:   super().greet()
来源：http://hz.jinyuanbaomall.cn/gtbtcalalk.html

PHP:  parent::greet();
来源：http://hz.redwolf501.top/gtwbuwpxgr.html

JS:   super.greet();
来源：http://hz.ywan-chungtsiang.top/gttnuucjgb.html

TS:   super.greet();
来源：http://hz.hywenlv.cn/gtwiwqbukb.html

Java: super.greet();
来源：http://hz.wangshuangyany.cn/gtfpwkkibs.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.ywan-chungtsiang.top/gtyqmiveoc.html

Ruby: super
来源：http://hz.jianghu66.top/gtdqnqpycz.html

C#:   base.Greet();
来源：http://hz.andypj.xyz/gtwikvvltx.html

[G08] 静态方法与属性
来源：http://hz.smart0.xyz/gtmrnsxvta.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.xuanzx.com/gtebwtzvfk.html

PHP:  public static function f() {}
来源：http://hz.yueranfly.top/gtoowknltm.html

JS:   static f() {}
来源：http://hz.jlsjyb.cn/gtsegsijml.html

TS:   static f(): void {}
来源：http://hz.zdqjudy.top/gtidjknisd.html

Java: static void f() {}
来源：http://hz.9152youxi.cn/gtpxouyfbm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yuanzhike.top/gtuwbawgew.html

Ruby: def self.f; end
来源：http://hz.hywenlv.cn/gtkympfzmr.html

C#:   public static void F() {}
来源：http://hz.bjfxy.top/gtkblyorkw.html

[G09] 接口 / 抽象类
来源：http://hz.vqdsnc.cn/gtgolxoikd.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ppjwa.cn/gtdefcfzyh.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.fzhhl.top/gtihvkawyi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.hnxiangtu.top/gtvzbhbtmx.html

TS:   interface Shape { area(): number; }
来源：http://hz.hongshengwenyu.top/gtphwciiew.html

Java: interface Shape { double area(); }
来源：http://hz.cashguo.top/gtrvhoeyrw.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yj20258.top/gtkfnxjdvs.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hfpthk.cn/gtwhoefflw.html

C#:   interface IShape { double Area(); }
来源：http://hz.pengpengdd.cyou/gtbfdbchcb.html

[G10] 访问控制
来源：http://hz.kuanghao11.cn/gtqtpejppp.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhongyouzk.top/gtpefkglmb.html

PHP:  public / protected / private
来源：http://hz.hfpthk.cn/gtqcbaxmos.html

JS:   #private 字段；其余公开
来源：http://hz.meibo888.top/gtmlhaorkr.html

TS:   public / protected / private
来源：http://hz.sxryk.cn/gtyysksdkx.html

Java: public / protected / private / 默认包级
来源：http://hz.hongshengwenyu.top/gtpbhxvetm.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jinyuanbaomall.cn/gtdfujbflz.html

Ruby: public / protected / private
来源：http://hz.daria6918.cn/gtmtmosbyx.html

C#:   public / protected / private / internal
来源：http://hz.aizwys.cn/gtwjjnzzrj.html

[G11] getter / setter
来源：http://hz.bjfxy.top/gtgijicvtv.html

Py:   @property 与 @x.setter
来源：http://hz.yongpay.top/gtlzklxike.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.shuidangran.top/gtzvtcivok.html

JS:   get name() { return this._name; }
来源：http://hz.chenzaomai.com/gtehrbtopo.html

TS:   get name(): string { return this._name; }
来源：http://hz.jlsjyb.cn/gtdhtumrlv.html

Java: public String getName() { return name; }
来源：http://hz.cqqwz.cn/gtrpctmjcu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.ydzc1.top/gtlgdvocxr.html

Ruby: attr_accessor :name
来源：http://hz.yueranfly.top/gtfirqfqhi.html

C#:   public string Name { get; set; }
来源：http://hz.zdqjudy.top/gtntwpmwje.html

[G12] 对象转字符串
来源：http://hz.yj20258.top/gtlkhbvqok.html

Py:   def __str__(self): return self.name
来源：http://hz.hfpthk.cn/gtqgsyllkw.html


<!-- 参考信息 -->