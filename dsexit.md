代发 wailian999

[E14] URL 编码与 Base64
来源：http://hz.fzhhl.top/gtcmtkfqeu.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.ivvv.top/gtbhvfvnfs.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jqgufenzy.top/gtuxoputyd.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.hywenlv.cn/gtgrcntnnu.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.sweek.top/gtauinqixq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yanxiufei.cn/gtcwsftgve.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.hfpthk.cn/gtngpphjal.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.meibo888.top/gthynmhffw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.ivvv.top/gtchhoouss.html

[E15] HTML 转义 / 反转义
来源：http://hz.shuidangran.top/gtnxexsfpy.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jinqigfzy.top/gtcydjlzlq.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.wangdashe.top/gtgrjyjwgu.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.gotoacloud.top/gtfuxajqwj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.haohaochexian.top/gtdogpaivb.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.nanxinkj.top/gthapysbwh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.guowangkeji.top/gtwatvhzcp.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.dashuyun.cn/gtcuhuqqyk.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.xziqi.cn/gtmksnxxsc.html

[E16] 数字千分位
来源：http://hz.guannengcc.top/gtlayrkanv.html

Py:   f"{1234567:,}"
来源：http://hz.sysykeji.top/gttskldokc.html

PHP:  number_format(1234567);
来源：http://hz.chenjidiqi.icu/gtqkhafuuh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.wangshuangyany.cn/gtqfhrwbck.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.ydzc1.top/gtbxnioeei.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.haohaochexian.top/gtlicqaoos.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.hywenlv.cn/gtazrjtqob.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yangfankeji.com/gtegnixjck.html

C#:   1234567.ToString("N0")
来源：http://hz.vqdsnc.cn/gtrjbcydsy.html

[E17] 首字母大写
来源：http://hz.hongshengwenyu.top/gtltzmjoyy.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.0kj1m.cn/gtmuhzcmly.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.nanxuanxn.top/gtfvkkbfqp.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cqqwz.cn/gtdkfotwft.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.chenzaomai.com/gtrcjnhzyk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.cqqwz.cn/gtnmdckavs.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.smart0.xyz/gtvfxyzics.html

Ruby: s.capitalize
来源：http://hz.zhoulong.xyz/gtylgqzkbi.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.hysaishi.cn/gtpljnoenc.html

[E18] 模板占位符替换
来源：http://hz.cdnleiting.top/gtkqcnhxfz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.haohaochexian.top/gtoyqicuoq.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.xuetiantiany.cn/gtpvwhiqeq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yuxming.cn/gthcgmwqfq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jiagoushi.top/gtrxbrlqra.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.andypj.xyz/gtnbxocfwp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.cdnleiting.top/gtvbwkasfj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yvedp.cn/gtqqubrthe.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.snrcjt.cn/gtcowzqgbw.html

[E19] 多行文本按行拆分
来源：http://hz.0kj1m.cn/gtvbcxbydy.html

Py:   s.splitlines()
来源：http://hz.guannengcc.top/gtylgyxvis.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.tianlin.xyz/gtybilrmwx.html

JS:   s.split(/\r?\n/)
来源：http://hz.quarkkingdee.top/gtzgqpwpff.html

TS:   s.split(/\r?\n/)
来源：http://hz.hfpthk.cn/gtrseyxvmx.html

Java: s.lines().toList()
来源：http://hz.jiagoushi.top/gtegmhgcgw.html

Go:   strings.Split(s, "\n")
来源：http://hz.svipenyu.cn/gtvataqmzy.html

Ruby: s.lines
来源：http://hz.redwolf501.top/gtibsxeirh.html

C#:   s.Split('\n')
来源：http://hz.quarkkingdee.top/gtszrkpmzq.html

[E20] 判断字符串是否为空
来源：http://hz.birdmap.top/gtgqsnaviw.html

Py:   if not s:
来源：http://hz.hnxiangtu.top/gttetpqsdd.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.fzhhl.top/gtkooidzqb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yonumen.top/gtpmvyitxh.html

TS:   if (s === "") {}
来源：http://hz.sxryk.cn/gtyatmvehg.html

Java: if (s.isEmpty()) {}
来源：http://hz.aibaodan.cn/gtrveluinc.html

Go:   if s == "" {}
来源：http://hz.yvedp.cn/gtaeybpefa.html

Ruby: if s.empty?
来源：http://hz.smart0.xyz/gtinyihhog.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.daria6918.cn/gtjcukedzm.html

[E21] 超长截断加省略号
来源：http://hz.zycfv.cn/gtpyqjxnbm.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yanxiufei.cn/gtaanplwtg.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.hnxiangtu.top/gtzwqejtqf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.chenlongwang.top/gtvyofebxx.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hysaishi.cn/gtblhjnsge.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.xuetiantiany.cn/gtdfomjevp.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.gotoacloud.top/gthtxzptcv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.tanke756.top/gtwcazypmb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.nwbrower.top/gtthxsorbl.html

[E22] 字节长度与字符长度
来源：http://hz.yuanzhike.top/gtjohnitah.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yj202588.top/gtsmunzdvn.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.9152youxi.cn/gtvlcnegdu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.52xcode.cn/gtokeclsbu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ydjk.org.cn/gtnjklygdh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.cdnleiting.top/gtjshuemzx.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.ywan-chungtsiang.top/gtkhjoygru.html

Ruby: s.bytesize;  s.length
来源：http://hz.hammf.cn/gtfwguuito.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.316326.xyz/gtkhewkzgu.html

================================================================================
来源：http://hz.xinyue.icu/gttymbypmy.html

F. 文件与目录
来源：http://hz.daria6918.cn/gtnutdvsxj.html

================================================================================
来源：http://hz.hfpthk.cn/gtqfucuwgg.html

[F01] 读取整个文件
来源：http://hz.cheryme.top/gtehzxdrvy.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.ybcxt.top/gthllchmey.html

PHP:  file_get_contents("a.txt");
来源：http://hz.gogol.net.cn/gtxoftdcan.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.gotoacloud.top/gtueyqyhok.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhongyouzk.top/gtxecguvdw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yongpay.top/gtzvwsqjqs.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.cdnleiting.top/gtgujdufzr.html

Ruby: File.read("a.txt")
来源：http://hz.nanxuanxn.top/gtyrwbnzkg.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.havefunace.top/gtmcvjrcci.html

[F02] 逐行读取文件
来源：http://hz.zycfv.cn/gtetrxkctc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.pycfn.com/gtpsxusgfb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yanxiufei.cn/gtifrrvtbo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xingfuxueyuan.xyz/gtvmyawvlr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhiwuduotai.top/gtudufrbvg.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.daxiang520.top/gtmtdyuxad.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.0kj1m.cn/gtwfgfkzvj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.ehwqpu.com/gteddctben.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.gogol.net.cn/gtipluihoq.html

[F03] 写入文件（覆盖）
来源：http://hz.zhixingplan.top/gtuxduwrnl.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hongshengwenyu.top/gtuplopdvl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.gzhubu.top/gtznvvpouh.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.redwolf501.top/gtfeqplkzu.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jiagoushi.top/gtjnhrgtad.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jiagoushi.top/gtivvdvclw.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yj20258888.top/gtxwguhqyt.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.chenjidiqi.icu/gtatardmhm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.hfpthk.cn/gtkzrzspgb.html

[F04] 追加写入文件
来源：http://hz.yonumen.top/gtfiqdgflc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.9152youxi.cn/gtohgyoext.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.hywenlv.cn/gtyrtlbvjv.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.nanxinkj.top/gtoufqymjo.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.wangdashe.top/gtvpdbopfr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.iojbl.cn/gtplwphldb.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yonumen.top/gtvuntzmfo.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.ydjk.org.cn/gtzlfwplup.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ybcxt.top/gtucvxsxzs.html

[F05] 判断文件或目录是否存在
来源：http://hz.jlsjyb.cn/gtfjsbybtl.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.shanyushiyangkeji.top/gtccrxusfy.html

PHP:  file_exists("a.txt");
来源：http://hz.daria6918.cn/gtlafovujl.html

JS:   fs.existsSync("a.txt")
来源：http://hz.hnqzz.top/gtxwcetxcz.html

TS:   fs.existsSync("a.txt")
来源：http://hz.gzhubu.top/gtzbwkyplj.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.xylfe.cn/gtugfzljbg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.c1oappe.top/gtgtbjxyyd.html

Ruby: File.exist?("a.txt")
来源：http://hz.zhongyouzk.top/gtnnbsvbdh.html

C#:   File.Exists("a.txt")
来源：http://hz.andypj.xyz/gteahtxhiy.html

[F06] 删除文件
来源：http://hz.vqdsnc.cn/gtbjawpayx.html

Py:   os.remove("a.txt")
来源：http://hz.52xcode.cn/gtnqlhztfs.html

PHP:  unlink("a.txt");
来源：http://hz.dashuyun.cn/gtxdketqea.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.sufxvd.cn/gtyiyihfhf.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.mhx1999.top/gtubfgihdw.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.vqdsnc.cn/gtbljyjhym.html

Go:   os.Remove("a.txt")
来源：http://hz.sufxvd.cn/gtnqvxstvj.html

Ruby: File.delete("a.txt")
来源：http://hz.gotoacloud.top/gtanyuktiz.html

C#:   File.Delete("a.txt");
来源：http://hz.ivvv.top/gtajgbzbdq.html

[F07] 创建目录（含多级）
来源：http://hz.xziqi.cn/gtnctwmwem.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.daxiang520.top/gtrtcevsoi.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.316326.xyz/gtohiqhwen.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jyoumei.cn/gticuoejhq.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jinqigufen.top/gtirvhukqb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yanxiufei.cn/gtinsbawvo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.sxryk.cn/gtevtmvwvh.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.yj202588.top/gtfrwrrgtp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.gzhubu.top/gtgqrauqmv.html

[F08] 遍历目录
来源：http://hz.gogol.net.cn/gtyvunisvt.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yuanzhike.top/gtvzgmxuhe.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jinyuanbaomall.cn/gtffedwebi.html

JS:   fs.readdirSync("dir")
来源：http://hz.cucudq.cn/gtsyoecibk.html

TS:   fs.readdirSync("dir")
来源：http://hz.yvedp.cn/gtbdvyzurt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.havefunace.top/gthkxjgbmz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zhengqikj.top/gtjvkerchr.html

Ruby: Dir.children("dir")
来源：http://hz.xuanzx.com/gtahfgtnow.html

C#:   Directory.GetFiles("dir")
来源：http://hz.hywenlv.cn/gtoionnfrn.html

[F09] 获取文件大小
来源：http://hz.meibo888.top/gtponmelvw.html

Py:   os.path.getsize("a.txt")
来源：http://hz.kuanghao11.cn/gtmkmaguvd.html

PHP:  filesize("a.txt");
来源：http://hz.52xcode.cn/gtlcpxwypu.html

JS:   fs.statSync("a.txt").size
来源：http://hz.kuanghao11.cn/gtmynxlalr.html

TS:   fs.statSync("a.txt").size
来源：http://hz.andypj.xyz/gtonkrwzbt.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.nanxinkj.top/gtxhclyheb.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.c1oappe.top/gtasxpjhgm.html

Ruby: File.size("a.txt")
来源：http://hz.havefunace.top/gtypxjkmut.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.fzhhl.top/gtofwjxcav.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.xinyue.icu/gtzllostae.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.sysykeji.top/gtddpfhbmf.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.chenzaomai.com/gtszudvbgd.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.chenjidiqi.icu/gtmghzcwft.html

TS:   path.extname("a.txt")
来源：http://hz.guowangkeji.top/gtqyviscum.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.aizwys.cn/gtovzhlvbo.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.nanxinkj.top/gteyqsjplf.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.ydzc1.top/gtgdxdnjvb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.wangdashe.top/gtfvdhjdie.html

[F11] 复制与移动文件
来源：http://hz.ydzc1.top/gtqbxpmgpc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.kuanghao11.cn/gtpkhbuxyw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.gaohongyu789.top/gtmxvsdsot.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.fengsongda.top/gtjywwgyct.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.aizwys.cn/gtkmgvvekl.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.cashguo.top/gteowwvqlm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.zhijiandao.cn/gthikkavmo.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yanxiufei.cn/gtqxvboznk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.chenlongwang.top/gteklhhiyx.html

[F12] CSV 读写
来源：http://hz.xingfuxueyuan.xyz/gtxxfcxaxg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jiagoushi.top/gtybgllbpt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.xziqi.cn/gtxxrgezgy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.kuanghao11.cn/gtzwxnjvfo.html

TS:   // 同上
来源：http://hz.zhiwuduotai.top/gtwfvfadyc.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jinqigfzy.top/gthdjffunz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jianghu66.top/gtrlizoaoh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jinghuilouyu.cn/gtuijfjgll.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jqgfzy.top/gtqltaedfz.html

================================================================================
来源：http://hz.yj202588.top/gtrsnrzoqm.html

G. 面向对象
来源：http://hz.xuanzx.com/gtlsxmqwil.html

================================================================================
来源：http://hz.52xcode.cn/gtwhollohy.html

[G01] 定义类
来源：http://hz.gzhubu.top/gtyjxxmvhg.html

Py:   class User: pass
来源：http://hz.zhongyouzk.top/gtpgkdqotv.html

PHP:  class User {}
来源：http://hz.svipenyu.cn/gtjzhpsmhb.html

JS:   class User {}
来源：http://hz.aizwys.cn/gtrqikwetq.html

TS:   class User { name: string = ""; }
来源：http://hz.tanke756.top/gtjnszwpcl.html

Java: class User {}
来源：http://hz.tianlin.xyz/gtggfaiokt.html

Go:   type User struct { Name string }
来源：http://hz.nanxinkj.top/gtpjrdnllh.html

Ruby: class User; end
来源：http://hz.wangdashe.top/gtxtlondxy.html

C#:   class User {}
来源：http://hz.svipenyu.cn/gtwgtybqjm.html

[G02] 构造函数
来源：http://hz.yvedp.cn/gthcgrhdxf.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.kuanghao11.cn/gtidwmhced.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.gogol.net.cn/gtiivxmaqy.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.nanxinkj.top/gtgipbtkah.html

TS:   constructor(public name: string) {}
来源：http://hz.gzhubu.top/gtmsdpefvw.html

Java: User(String name) { this.name = name; }
来源：http://hz.sweek.top/gtrhbjucwo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.redwolf501.top/gtnfqhohav.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.ehwqpu.com/gtuxlnbnvt.html

C#:   public User(string name) { Name = name; }
来源：http://hz.jqgufenzy.top/gtsrnrssnp.html

[G03] 实例属性
来源：http://hz.guowangkeji.top/gtwptldlvl.html

Py:   self.name = "x"
来源：http://hz.birdmap.top/gtawvfnsia.html

PHP:  public string $name = "x";
来源：http://hz.ydzc1.top/gtbebtfrfz.html

JS:   this.name = "x";
来源：http://hz.wangdashe.top/gtswbzjavi.html

TS:   name: string = "x";
来源：http://hz.cdnleiting.top/gtydaljdkh.html

Java: private String name;
来源：http://hz.shzxlz.cn/gtfvfpmcra.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.cheryme.top/gtrwarbcce.html

Ruby: @name = "x"
来源：http://hz.shzxlz.cn/gtfdhiifco.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.52xcode.cn/gtenqxrrrt.html

[G04] 定义方法
来源：http://hz.aibaodan.cn/gtbizigkli.html

Py:   def greet(self): return self.name
来源：http://hz.feifeiyinyue.top/gtlucqfztj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.feifeiyinyue.top/gtmakmcrfi.html

JS:   greet() { return this.name; }
来源：http://hz.zhaomingkeji.xyz/gtoulkodca.html

TS:   greet(): string { return this.name; }
来源：http://hz.zdqjudy.top/gtcwbkzyox.html

Java: String greet() { return name; }
来源：http://hz.shuidangran.top/gttwtwthbr.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jlsjyb.cn/gtesbxmzpq.html

Ruby: def greet; @name; end
来源：http://hz.birdmap.top/gtexcvlfbw.html

C#:   public string Greet() => Name;
来源：http://hz.ivvv.top/gtjfkitdgs.html

[G05] 继承
来源：http://hz.ppjwa.cn/gtluoyayil.html

Py:   class Admin(User): pass
来源：http://hz.dianchejie.cn/gtgzayxltu.html

PHP:  class Admin extends User {}
来源：http://hz.xuetiantiany.cn/gtqctqqtxs.html

JS:   class Admin extends User {}
来源：http://hz.feifeiyinyue.top/gtwbxcihwp.html

TS:   class Admin extends User {}
来源：http://hz.aibaodan.cn/gtjnbsmumf.html

Java: class Admin extends User {}
来源：http://hz.guannengcc.top/gthmvxnhgb.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.nanxinkj.top/gtnzofmbqv.html

Ruby: class Admin < User; end
来源：http://hz.yueranfly.top/gtpupdvjvb.html

C#:   class Admin : User {}
来源：http://hz.xziqi.cn/gtvsutieqx.html

[G06] 重写方法
来源：http://hz.gogol.net.cn/gtvrikctau.html

Py:   def greet(self): return "admin"
来源：http://hz.nanxinkj.top/gtamuulbws.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yj20258888.top/gtyziotesv.html

JS:   greet() { return "admin"; }
来源：http://hz.ybcxt.top/gtrhptymbe.html

TS:   greet(): string { return "admin"; }
来源：http://hz.ywan-chungtsiang.top/gtdlhrmqpu.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.hnqzz.top/gtwlgrhmhh.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.sxryk.cn/gtjoksxkit.html

Ruby: def greet; "admin"; end
来源：http://hz.pengpengdd.cyou/gttozkjuuc.html

C#:   public override string Greet() => "admin";
来源：http://hz.yongpay.top/gthsspfnqa.html

[G07] 调用父类方法
来源：http://hz.yueranfly.top/gthpiywbsa.html

Py:   super().greet()
来源：http://hz.dashuyun.cn/gtoddtignt.html

PHP:  parent::greet();
来源：http://hz.gzhubu.top/gtibqptyqc.html

JS:   super.greet();
来源：http://hz.shanyushiyangtech.top/gtsreacgij.html

TS:   super.greet();
来源：http://hz.yueranfly.top/gtziyvlikv.html

Java: super.greet();
来源：http://hz.xuetiantiany.cn/gtqnfkfujz.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.yueranfly.top/gtxdifrcbr.html

Ruby: super
来源：http://hz.xuanzx.com/gtwyxcxzkv.html

C#:   base.Greet();
来源：http://hz.pengpengdd.cyou/gtkcsktqgw.html

[G08] 静态方法与属性
来源：http://hz.guowangkeji.top/gttxfqvccl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.meibo888.top/gtakzcongw.html

PHP:  public static function f() {}
来源：http://hz.hongshengwenyu.top/gtmgpjavcb.html

JS:   static f() {}
来源：http://hz.daxiang520.top/gttgxhitxg.html

TS:   static f(): void {}
来源：http://hz.daxiang520.top/gtfhgwrzlt.html

Java: static void f() {}
来源：http://hz.shuidangran.top/gtrzhkfylf.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yonumen.top/gtrfypzlpj.html

Ruby: def self.f; end
来源：http://hz.jinqigfzy.top/gtkitgovhs.html

C#:   public static void F() {}
来源：http://hz.havefunace.top/gtwzyuxtgl.html

[G09] 接口 / 抽象类
来源：http://hz.ppjwa.cn/gttwxeyasq.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zdqjudy.top/gtqawmvjer.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.snrcjt.cn/gttlpjstqw.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yuanzhike.top/gtksmjomrj.html

TS:   interface Shape { area(): number; }
来源：http://hz.gzhubu.top/gtdfbdihho.html

Java: interface Shape { double area(); }
来源：http://hz.ehwqpu.com/gtxrweikxr.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yongpay.top/gthusdwtlb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.iojbl.cn/gtqeuvzixb.html

C#:   interface IShape { double Area(); }
来源：http://hz.yongpay.top/gtrlcuepmi.html

[G10] 访问控制
来源：http://hz.xziqi.cn/gtgacxadwy.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jiagoushi.top/gtgcyksfyi.html

PHP:  public / protected / private
来源：http://hz.chenlongwang.top/gtajptqnnq.html

JS:   #private 字段；其余公开
来源：http://hz.andypj.xyz/gtmnbpwoun.html

TS:   public / protected / private
来源：http://hz.sweek.top/gtcwdoxqsm.html

Java: public / protected / private / 默认包级
来源：http://hz.hnqzz.top/gtvferwcyw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jinyuanbaomall.cn/gtnlakvfhq.html

Ruby: public / protected / private
来源：http://hz.aibaodan.cn/gtgvkcfhwf.html

C#:   public / protected / private / internal
来源：http://hz.chenjidiqi.icu/gtrbsiipod.html

[G11] getter / setter
来源：http://hz.zhengqikj.top/gtrtgbkxbm.html

Py:   @property 与 @x.setter
来源：http://hz.yj20258888.top/gtwfwnmydu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.cqqwz.cn/gtqiqergju.html

JS:   get name() { return this._name; }
来源：http://hz.yanxiufei.cn/gtfqciyeqr.html

TS:   get name(): string { return this._name; }
来源：http://hz.fzhhl.top/gtsbcnjafv.html

Java: public String getName() { return name; }
来源：http://hz.tanke756.top/gtljmjzckz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.hfpthk.cn/gtyaqctkwo.html

Ruby: attr_accessor :name
来源：http://hz.tianlin.xyz/gtggcsqjtb.html

C#:   public string Name { get; set; }
来源：http://hz.hongshengwenyu.top/gtznhemyuo.html

[G12] 对象转字符串
来源：http://hz.yongpay.top/gtatfexzpi.html

Py:   def __str__(self): return self.name
来源：http://hz.jlsjyb.cn/gtzhuadqjz.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.feifeiyinyue.top/gtyalltlmg.html

JS:   toString() { return this.name; }
来源：http://hz.yangfankeji.com/gtciwlkpnb.html

TS:   toString(): string { return this.name; }
来源：http://hz.birdmap.top/gtkjvvmsju.html

Java: @Override public String toString() { return name; }
来源：http://hz.nwbrower.top/gtzcsskpbv.html


<!-- 参考信息 -->