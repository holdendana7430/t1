代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jqgfzy.top/gtwnnkzhor.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.hammf.cn/gtjwnwdcgk.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.0kj1m.cn/gtfakhrcil.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.feifeiyinyue.top/gtfxlnvopq.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yongpay.top/gthvxaqffw.html

[E15] HTML 转义 / 反转义
来源：http://hz.tian-w.cn/gtzhsgydwh.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.xuanzx.com/gtwqvmasww.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.hammf.cn/gtpeusfwru.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.guowangkeji.top/gthzomkiki.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.guowangkeji.top/gtopwuqosb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.sweek.top/gtesiamhbg.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.sweek.top/gtngygktft.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.tianlin.xyz/gtxqadqfvi.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.c1oappe.top/gtdvgewrnn.html

[E16] 数字千分位
来源：http://hz.sysykeji.top/gtikyzgnix.html

Py:   f"{1234567:,}"
来源：http://hz.zhongyouzk.top/gteicomots.html

PHP:  number_format(1234567);
来源：http://hz.guowangkeji.top/gtwmnrubvi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.nwbrower.top/gtdyfecsey.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.tianlin.xyz/gtovimolwh.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.xuetiantiany.cn/gtqxlikhgh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.hfpthk.cn/gtbpdhwdxd.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zhijiandao.cn/gtilpybhwg.html

C#:   1234567.ToString("N0")
来源：http://hz.mhx1999.top/gtrwtidxfc.html

[E17] 首字母大写
来源：http://hz.mhx1999.top/gtlftlqcpn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.hysaishi.cn/gtcmmutvgn.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.aizwys.cn/gtytmufrjo.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xziqi.cn/gtbisvsvnf.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sysykeji.top/gtbtteazmh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.ydjk.org.cn/gtfclrxifw.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.ydzc1.top/gtqbdogbuf.html

Ruby: s.capitalize
来源：http://hz.jqgufenzy.top/gthimosytc.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.cheryme.top/gtqedxzaio.html

[E18] 模板占位符替换
来源：http://hz.gaohongyu789.top/gtvnacmckx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.quarkkingdee.top/gtvjbxnnmt.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jinyuanbaomall.cn/gtcqzumcpy.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.ppjwa.cn/gtvnjhdccc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhoulong.xyz/gtabulbbpb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.tanke756.top/gteuzthvwz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.iojbl.cn/gttrplzdyp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.daria6918.cn/gthcehxjbp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.daxiang520.top/gtbfggjccu.html

[E19] 多行文本按行拆分
来源：http://hz.hywenlv.cn/gtmwlcivis.html

Py:   s.splitlines()
来源：http://hz.fzhhl.top/gtbxxmizgk.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.ppjwa.cn/gtvrzzhcga.html

JS:   s.split(/\r?\n/)
来源：http://hz.hfpthk.cn/gtmcimcqxu.html

TS:   s.split(/\r?\n/)
来源：http://hz.quarkkingdee.top/gthipmdxgo.html

Java: s.lines().toList()
来源：http://hz.ppjwa.cn/gtzcexukpo.html

Go:   strings.Split(s, "\n")
来源：http://hz.ppjwa.cn/gtzwgtticr.html

Ruby: s.lines
来源：http://hz.pycfn.com/gtbiqjgegp.html

C#:   s.Split('\n')
来源：http://hz.yueranfly.top/gtxdsfkdpl.html

[E20] 判断字符串是否为空
来源：http://hz.cashguo.top/gtpgtfsdoc.html

Py:   if not s:
来源：http://hz.gotoacloud.top/gtzkgbxymr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.feifeiyinyue.top/gtbewkajwi.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.zhaomingkeji.xyz/gtbisoayux.html

TS:   if (s === "") {}
来源：http://hz.vqdsnc.cn/gtaqszhrmx.html

Java: if (s.isEmpty()) {}
来源：http://hz.zdqjudy.top/gtszlvvsnu.html

Go:   if s == "" {}
来源：http://hz.tian-w.cn/gtivcjncyi.html

Ruby: if s.empty?
来源：http://hz.tianlin.xyz/gtekeziggq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.yuxming.cn/gtgahyyglx.html

[E21] 超长截断加省略号
来源：http://hz.quarkkingdee.top/gtbqwiofqm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.andypj.xyz/gtsrsjnwqs.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.xziqi.cn/gtnrqsotas.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinqigfzy.top/gtuupnskjx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhoulong.xyz/gtixkewidu.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.shanyushiyangkeji.top/gtnqkbvinr.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.gogol.net.cn/gtqwslxqbj.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yueranfly.top/gtqieiluvr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ybcxt.top/gtecboppdw.html

[E22] 字节长度与字符长度
来源：http://hz.chenlongwang.top/gtzihushpv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.ehwqpu.com/gtlbntbjdz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.guannengcc.top/gtbtknacae.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhongyouzk.top/gtwhiugckm.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.vqdsnc.cn/gtlqjfqbyg.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.xziqi.cn/gtkuvdqaht.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jinqigufen.top/gtemgflvsy.html

Ruby: s.bytesize;  s.length
来源：http://hz.yj20258.top/gtitlztver.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.quarkkingdee.top/gtupwlnhrc.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtfiwqeppp.html

F. 文件与目录
来源：http://hz.snrcjt.cn/gttnolqgry.html

================================================================================
来源：http://hz.daxiang520.top/gtipqjmkha.html

[F01] 读取整个文件
来源：http://hz.fengsongda.top/gtdcsjqhhb.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.mhx1999.top/gtyzldjrjw.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jyoumei.cn/gtdooralqs.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yonumen.top/gtugtmouir.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.fzhhl.top/gtjqndcjrq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.chenzaomai.com/gtiouroxfu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.hywenlv.cn/gtlvtsonru.html

Ruby: File.read("a.txt")
来源：http://hz.svipenyu.cn/gthkdxbwqx.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.svipenyu.cn/gtlyhvpoqa.html

[F02] 逐行读取文件
来源：http://hz.shanyushiyangkeji.top/gtknpbefjw.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zhaomingkeji.xyz/gtfffuoxoy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.0kj1m.cn/gtnzipcben.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jlsjyb.cn/gtoxqwzsde.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhongyouzk.top/gtstpikuzx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.daxiang520.top/gtegxlmonu.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.dianchejie.cn/gthfljtisq.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jqgufenzy.top/gtjgidydfz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.guowangkeji.top/gtkxdkaizt.html

[F03] 写入文件（覆盖）
来源：http://hz.cucudq.cn/gtbicfbojd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.ydjk.org.cn/gtbfbsftli.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.iojbl.cn/gttwalbbqi.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shuidangran.top/gtmubskneo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.9152youxi.cn/gtcogptqzw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.shangyingyoupin.top/gtfjtkscpc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.redwolf501.top/gtpzmzpsfi.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.birdmap.top/gtmdgjxtni.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jyoumei.cn/gteuhympwf.html

[F04] 追加写入文件
来源：http://hz.zhixingplan.top/gtvduhkguy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.xinyue.icu/gtqnzksdlx.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.gzhubu.top/gtboxenmmq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.feifeiyinyue.top/gtjmcjizmp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.c1oappe.top/gtxhwbbjbs.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.iojbl.cn/gtplmllgih.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yuxming.cn/gtnxfdhben.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.tanke756.top/gthmvdcjgg.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.zhiwuduotai.top/gtlmgvovto.html

[F05] 判断文件或目录是否存在
来源：http://hz.xinyue.icu/gtycuotmse.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.aibaodan.cn/gtllocxosh.html

PHP:  file_exists("a.txt");
来源：http://hz.316326.xyz/gtnojaqwcy.html

JS:   fs.existsSync("a.txt")
来源：http://hz.52xcode.cn/gttlxmrinm.html

TS:   fs.existsSync("a.txt")
来源：http://hz.haohaochexian.top/gtzezhvfuy.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zhoulong.xyz/gtqkmzfudv.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zdqjudy.top/gtkeuiwvaj.html

Ruby: File.exist?("a.txt")
来源：http://hz.cashguo.top/gtyaxysxlt.html

C#:   File.Exists("a.txt")
来源：http://hz.tianlin.xyz/gthwazaako.html

[F06] 删除文件
来源：http://hz.aibaodan.cn/gtfnktjdpm.html

Py:   os.remove("a.txt")
来源：http://hz.jianghu66.top/gtabikftiq.html

PHP:  unlink("a.txt");
来源：http://hz.haohaochexian.top/gtmojbrmdw.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yj20258888.top/gtxfvbonfx.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.fzhhl.top/gttbixfgrg.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.hfpthk.cn/gtflwoqvag.html

Go:   os.Remove("a.txt")
来源：http://hz.cqqwz.cn/gtbgwixbkc.html

Ruby: File.delete("a.txt")
来源：http://hz.chenlongwang.top/gtcljpsrll.html

C#:   File.Delete("a.txt");
来源：http://hz.shzxlz.cn/gtlwtzixaa.html

[F07] 创建目录（含多级）
来源：http://hz.fzhhl.top/gtcsuasfky.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yongpay.top/gtphxkygpq.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.mhx1999.top/gtylmgzzwo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.sxryk.cn/gtlvzavbvo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.pycfn.com/gtpmgcvwcg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yongpay.top/gtciirnmth.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jinyuanbaomall.cn/gtszlzowib.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.hongshengwenyu.top/gtozgkmkdu.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.vqdsnc.cn/gtqpiyeuyx.html

[F08] 遍历目录
来源：http://hz.hywenlv.cn/gtvmvcergl.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zhiwuduotai.top/gtnsxnkgmr.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.zhengqikj.top/gtbhbdzora.html

JS:   fs.readdirSync("dir")
来源：http://hz.ivvv.top/gtwymuknra.html

TS:   fs.readdirSync("dir")
来源：http://hz.zhiwuduotai.top/gtfdjhxlgg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.c1oappe.top/gtftpleubi.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.svipenyu.cn/gtazmbcdyj.html

Ruby: Dir.children("dir")
来源：http://hz.smart0.xyz/gtufhhaulz.html

C#:   Directory.GetFiles("dir")
来源：http://hz.kuanghao11.cn/gtdoorkfsa.html

[F09] 获取文件大小
来源：http://hz.c1oappe.top/gtahohgtgk.html

Py:   os.path.getsize("a.txt")
来源：http://hz.daxiang520.top/gtirfkibrs.html

PHP:  filesize("a.txt");
来源：http://hz.jianghu66.top/gtsersvfqk.html

JS:   fs.statSync("a.txt").size
来源：http://hz.316326.xyz/gtaxyehmim.html

TS:   fs.statSync("a.txt").size
来源：http://hz.nanxinkj.top/gtlevnczqc.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.ppjwa.cn/gtvlvhwjgo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hfpthk.cn/gtgluadbtr.html

Ruby: File.size("a.txt")
来源：http://hz.dianchejie.cn/gtuiyumpxp.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.birdmap.top/gttdblqoaw.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.chenlongwang.top/gttnmfhvzz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.feifeiyinyue.top/gtztwhbkun.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.vqdsnc.cn/gtcumvgztp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.xuetiantiany.cn/gthwslabkk.html

TS:   path.extname("a.txt")
来源：http://hz.yj20258888.top/gtrydhqnvg.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.nwbrower.top/gtkrvhqfsq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.jinqigfzy.top/gtkmgqzfgr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yueranfly.top/gticxxlabk.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yanxiufei.cn/gtbvrxknck.html

[F11] 复制与移动文件
来源：http://hz.ybcxt.top/gtrixmrzak.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yongpay.top/gtpmdtxkkn.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jqgfzy.top/gtilrroqgf.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.pycfn.com/gtmmjinsdb.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.kuanghao11.cn/gtwzilbhlj.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.sufxvd.cn/gtlnnkfozc.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.gotoacloud.top/gtucwczjlj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.gaohongyu789.top/gtuzgdypgq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhiwuduotai.top/gtbkqfuhmp.html

[F12] CSV 读写
来源：http://hz.hnxiangtu.top/gtnevpmrny.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.nanxinkj.top/gtkrzfjsln.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.shuidangran.top/gtwckhxuui.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.ydzc1.top/gtlirokbqn.html

TS:   // 同上
来源：http://hz.yueranfly.top/gthnbbpkjd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ywan-chungtsiang.top/gttgqoshen.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.nwbrower.top/gtpvintrug.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ppjwa.cn/gtqzjkcpve.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jqgfzy.top/gtprrhmwxl.html

================================================================================
来源：http://hz.gaohongyu789.top/gtlifuravs.html

G. 面向对象
来源：http://hz.xuetiantiany.cn/gtxiprhwnh.html

================================================================================
来源：http://hz.yj20258888.top/gthppwlahk.html

[G01] 定义类
来源：http://hz.jinyuanbaomall.cn/gtpusatohx.html

Py:   class User: pass
来源：http://hz.shzxlz.cn/gtorzayaac.html

PHP:  class User {}
来源：http://hz.hfpthk.cn/gtmuzgfhzf.html

JS:   class User {}
来源：http://hz.sweek.top/gtmbnippmm.html

TS:   class User { name: string = ""; }
来源：http://hz.jqgfzy.top/gtxkyvyywx.html

Java: class User {}
来源：http://hz.shzxlz.cn/gtzpzdliky.html

Go:   type User struct { Name string }
来源：http://hz.redwolf501.top/gtluurhidw.html

Ruby: class User; end
来源：http://hz.iojbl.cn/gtavnrhazm.html

C#:   class User {}
来源：http://hz.jiagoushi.top/gttslqccho.html

[G02] 构造函数
来源：http://hz.hywenlv.cn/gtkhqyghrz.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.pycfn.com/gtlqiuzpgy.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.guowangkeji.top/gtomienzmi.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.quarkkingdee.top/gtduvpensf.html

TS:   constructor(public name: string) {}
来源：http://hz.gaohongyu789.top/gtwcbcyhtu.html

Java: User(String name) { this.name = name; }
来源：http://hz.jinghuilouyu.cn/gtgincgqhg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hnqzz.top/gtwvhbvuxz.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.guowangkeji.top/gthmurntce.html

C#:   public User(string name) { Name = name; }
来源：http://hz.cucudq.cn/gtdsxvdsmw.html

[G03] 实例属性
来源：http://hz.ivvv.top/gtjstjbyym.html

Py:   self.name = "x"
来源：http://hz.ydzc1.top/gtfostdrhv.html

PHP:  public string $name = "x";
来源：http://hz.tianlin.xyz/gtarwpcwxz.html

JS:   this.name = "x";
来源：http://hz.chenzaomai.com/gtiaxkjbkf.html

TS:   name: string = "x";
来源：http://hz.aibaodan.cn/gtzugmbxlc.html

Java: private String name;
来源：http://hz.tianlin.xyz/gtnsiimucx.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.sufxvd.cn/gtnmgdgmul.html

Ruby: @name = "x"
来源：http://hz.dianchejie.cn/gtiiyppomq.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jinyuanbaomall.cn/gtwhamzopg.html

[G04] 定义方法
来源：http://hz.0kj1m.cn/gtxhxhlbdn.html

Py:   def greet(self): return self.name
来源：http://hz.ydzc1.top/gtkbvbdqjz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hywenlv.cn/gtmffqqovb.html

JS:   greet() { return this.name; }
来源：http://hz.meibo888.top/gtfndmmogs.html

TS:   greet(): string { return this.name; }
来源：http://hz.xziqi.cn/gtmjwtmeaw.html

Java: String greet() { return name; }
来源：http://hz.dianchejie.cn/gteuawlpiy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.gotoacloud.top/gtxxtzhwgs.html

Ruby: def greet; @name; end
来源：http://hz.jyoumei.cn/gtgnqhmgad.html

C#:   public string Greet() => Name;
来源：http://hz.guannengcc.top/gtlgrsjnmc.html

[G05] 继承
来源：http://hz.xuanzx.com/gtsyjshfrm.html

Py:   class Admin(User): pass
来源：http://hz.hysaishi.cn/gthsvbsvwh.html

PHP:  class Admin extends User {}
来源：http://hz.aibaodan.cn/gtkqjtpgdg.html

JS:   class Admin extends User {}
来源：http://hz.xylfe.cn/gtvulcwgfl.html

TS:   class Admin extends User {}
来源：http://hz.shanyushiyangtech.top/gtxpxzwsoq.html

Java: class Admin extends User {}
来源：http://hz.yj20258888.top/gthdnzgiwh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.nwbrower.top/gtajjwtylc.html

Ruby: class Admin < User; end
来源：http://hz.jqgfzy.top/gteclftuas.html

C#:   class Admin : User {}
来源：http://hz.quarkkingdee.top/gtrsqrdpll.html

[G06] 重写方法
来源：http://hz.yueranfly.top/gtopmbydwk.html

Py:   def greet(self): return "admin"
来源：http://hz.xziqi.cn/gtfxjvviuz.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yuanzhike.top/gttbtnoild.html

JS:   greet() { return "admin"; }
来源：http://hz.chenzaomai.com/gtyazzshlp.html

TS:   greet(): string { return "admin"; }
来源：http://hz.sxryk.cn/gtflntonyr.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jinyuanbaomall.cn/gtidfdojuv.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhoulong.xyz/gtyvqelxyd.html

Ruby: def greet; "admin"; end
来源：http://hz.chenjidiqi.icu/gtdtbdgwxg.html

C#:   public override string Greet() => "admin";
来源：http://hz.xylfe.cn/gtdchtwhuw.html

[G07] 调用父类方法
来源：http://hz.cqqwz.cn/gtwrapagpb.html

Py:   super().greet()
来源：http://hz.cdnleiting.top/gtxgtiuegn.html

PHP:  parent::greet();
来源：http://hz.yueranfly.top/gtamlkiylt.html

JS:   super.greet();
来源：http://hz.hysaishi.cn/gtiakpmbkb.html

TS:   super.greet();
来源：http://hz.hnxiangtu.top/gtufqmorlf.html

Java: super.greet();
来源：http://hz.pengpengdd.cyou/gtickaaneu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yuxming.cn/gtfnrjurym.html

Ruby: super
来源：http://hz.meibo888.top/gtgwcfhkdq.html

C#:   base.Greet();
来源：http://hz.yj20258888.top/gtoilgubbh.html

[G08] 静态方法与属性
来源：http://hz.fzhhl.top/gtvshvljza.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.gotoacloud.top/gthragehrg.html

PHP:  public static function f() {}
来源：http://hz.ywan-chungtsiang.top/gtvqifgzaf.html

JS:   static f() {}
来源：http://hz.bjfxy.top/gtxbzvtxqe.html

TS:   static f(): void {}
来源：http://hz.mhx1999.top/gtltkstdcu.html

Java: static void f() {}
来源：http://hz.xuanzx.com/gtzmnbpsgy.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.dashuyun.cn/gtetjtilbj.html

Ruby: def self.f; end
来源：http://hz.xingfuxueyuan.xyz/gthzkqeqhl.html

C#:   public static void F() {}
来源：http://hz.kuanghao11.cn/gtwdsilthu.html

[G09] 接口 / 抽象类
来源：http://hz.snrcjt.cn/gtnskjlytg.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.gotoacloud.top/gttbdjgcjq.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jiagoushi.top/gtvgmbaodn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.nwbrower.top/gteptalrgo.html

TS:   interface Shape { area(): number; }
来源：http://hz.zhongyouzk.top/gtnzrqktss.html

Java: interface Shape { double area(); }
来源：http://hz.pengpengdd.cyou/gtlzazxpap.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yangfankeji.com/gtdnvwoplx.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.gaohongyu789.top/gtheesdksf.html

C#:   interface IShape { double Area(); }
来源：http://hz.pycfn.com/gtcxpfudke.html

[G10] 访问控制
来源：http://hz.hysaishi.cn/gthroqpggp.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.chenlongwang.top/gtpqhbkwzy.html

PHP:  public / protected / private
来源：http://hz.yonumen.top/gttunjviyb.html

JS:   #private 字段；其余公开
来源：http://hz.iojbl.cn/gtjiocbnow.html

TS:   public / protected / private
来源：http://hz.feifeiyinyue.top/gtgprzzogg.html

Java: public / protected / private / 默认包级
来源：http://hz.haohaochexian.top/gtqcxxiafv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.quarkkingdee.top/gtxydfqwrj.html

Ruby: public / protected / private
来源：http://hz.xuetiantiany.cn/gtudkjedac.html

C#:   public / protected / private / internal
来源：http://hz.meibo888.top/gtjumrrluk.html

[G11] getter / setter
来源：http://hz.cucudq.cn/gtszympxqg.html

Py:   @property 与 @x.setter
来源：http://hz.hnqzz.top/gtuloafldf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.nwbrower.top/gtlgplvrbt.html

JS:   get name() { return this._name; }
来源：http://hz.chenlongwang.top/gtpajjwscz.html

TS:   get name(): string { return this._name; }
来源：http://hz.daxiang520.top/gtexsehxvd.html

Java: public String getName() { return name; }
来源：http://hz.chenzaomai.com/gtsdvqcknw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zdqjudy.top/gtdkafxfqx.html

Ruby: attr_accessor :name
来源：http://hz.zhongyouzk.top/gtkpiegrlr.html

C#:   public string Name { get; set; }
来源：http://hz.vqdsnc.cn/gthbcxrjaf.html

[G12] 对象转字符串
来源：http://hz.xuanzx.com/gtbpvinety.html

Py:   def __str__(self): return self.name
来源：http://hz.iojbl.cn/gtckvmoqlg.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.jinqigfzy.top/gtbxcquteg.html

JS:   toString() { return this.name; }
来源：http://hz.52xcode.cn/gtgtlggjxd.html

TS:   toString(): string { return this.name; }
来源：http://hz.hnqzz.top/gtnlaqvuvs.html

Java: @Override public String toString() { return name; }
来源：http://hz.hfpthk.cn/gtohleeuqo.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.mhx1999.top/gtpjtqbmmq.html

Ruby: def to_s; @name; end
来源：http://hz.gotoacloud.top/gtvapsvtdu.html

C#:   public override string ToString() => Name;
来源：http://hz.zhijiandao.cn/gtgvmuqxna.html

[G13] 判断对象类型
来源：http://hz.pycfn.com/gtnkqnzevl.html


<!-- 参考信息 -->