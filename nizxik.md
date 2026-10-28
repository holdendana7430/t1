代发 wailian999

Go:   strings.Count(s, "a")
来源：http://hz.zhixingplan.top/gticnqywoo.html

Ruby: s.count("a")
来源：http://hz.tian-w.cn/gtboyvodfg.html

C#:   s.Count(c => c == 'a')
来源：http://hz.jlsjyb.cn/gtxsdlgovv.html

[E13] 逐字符遍历
来源：http://hz.zhoulong.xyz/gtlubyaojq.html

Py:   for ch in s: print(ch)
来源：http://hz.hnqzz.top/gtuexxitau.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.jyoumei.cn/gturzxikmr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.sweek.top/gtupkxjrcw.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.hnqzz.top/gtpitimvqw.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.cheryme.top/gtwgreagkr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.hnqzz.top/gtwqldomoi.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.iojbl.cn/gtdktqswrb.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.hongshengwenyu.top/gtqfbjglkn.html

[E14] URL 编码与 Base64
来源：http://hz.cheryme.top/gttrwqwtox.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.nwbrower.top/gtoeerzkwn.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.zdqjudy.top/gtrzpglbhw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.shanyushiyangkeji.top/gtwdwfkmhe.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.52xcode.cn/gtotrpcosu.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jianghu66.top/gtokqhofud.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.meibo888.top/gtflilfdwn.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.guowangkeji.top/gtjkrwegrw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.jinyuanbaomall.cn/gtfdgvdnni.html

[E15] HTML 转义 / 反转义
来源：http://hz.guannengcc.top/gtkazmwvlt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.iojbl.cn/gtxrehrjoo.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.aizwys.cn/gttynprcck.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.xingfuxueyuan.xyz/gtxqeayhzf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.zhengqikj.top/gtfrclxxzn.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.sufxvd.cn/gtujtvccrm.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jiagoushi.top/gtyuivyslq.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yuanzhike.top/gtzqhzdcqp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yuanzhike.top/gttrffgjog.html

[E16] 数字千分位
来源：http://hz.yuxming.cn/gtggaywtxb.html

Py:   f"{1234567:,}"
来源：http://hz.jlsjyb.cn/gtooruibie.html

PHP:  number_format(1234567);
来源：http://hz.jqgufenzy.top/gtpqoeavno.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.birdmap.top/gtlqlyomcf.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.guowangkeji.top/gtgptzuihe.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.snrcjt.cn/gtugdogxlf.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.gaohongyu789.top/gtreeinecx.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.shangyingyoupin.top/gtowbbwbau.html

C#:   1234567.ToString("N0")
来源：http://hz.yongpay.top/gtbldplzbl.html

[E17] 首字母大写
来源：http://hz.mhx1999.top/gtcyjnwain.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.dianchejie.cn/gtamxqmfxk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.havefunace.top/gtmkjuugzf.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yj20258.top/gtwdlrixre.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xuetiantiany.cn/gtsizvbugx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.ybcxt.top/gtvwiqhphm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.guannengcc.top/gtjqfeiqta.html

Ruby: s.capitalize
来源：http://hz.tian-w.cn/gtdfpbiorf.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jianghu66.top/gtfavzcdub.html

[E18] 模板占位符替换
来源：http://hz.gaohongyu789.top/gtwyvscepy.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yj20258.top/gtkghcxkrv.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jqgfzy.top/gtnfznukgo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.ppjwa.cn/gtioregqki.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.dianchejie.cn/gtvqshwpmw.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.pengpengdd.cyou/gtykbsdjfh.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.wangshuangyany.cn/gttxxtkmuq.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.shanyushiyangkeji.top/gttqciwbie.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.xziqi.cn/gthsyqylkr.html

[E19] 多行文本按行拆分
来源：http://hz.cucudq.cn/gtjusgwsba.html

Py:   s.splitlines()
来源：http://hz.yvedp.cn/gtmxvddmhi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.redwolf501.top/gtmafvrjyp.html

JS:   s.split(/\r?\n/)
来源：http://hz.smart0.xyz/gtvpaxmwnp.html

TS:   s.split(/\r?\n/)
来源：http://hz.svipenyu.cn/gtwfyrojdy.html

Java: s.lines().toList()
来源：http://hz.shuidangran.top/gtbwgzqwwa.html

Go:   strings.Split(s, "\n")
来源：http://hz.havefunace.top/gtyrupefgk.html

Ruby: s.lines
来源：http://hz.yueranfly.top/gtmaluerwe.html

C#:   s.Split('\n')
来源：http://hz.shangyingyoupin.top/gtnktavvcg.html

[E20] 判断字符串是否为空
来源：http://hz.zhixingplan.top/gtwlxaccwf.html

Py:   if not s:
来源：http://hz.shzxlz.cn/gtlnykojcw.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.svipenyu.cn/gtyqdtnjpu.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.hammf.cn/gtyrwpeymw.html

TS:   if (s === "") {}
来源：http://hz.svipenyu.cn/gtfomkwjnh.html

Java: if (s.isEmpty()) {}
来源：http://hz.daria6918.cn/gtqhtqjsra.html

Go:   if s == "" {}
来源：http://hz.ivvv.top/gtnevfnqor.html

Ruby: if s.empty?
来源：http://hz.nanxinkj.top/gtrxpdhmcd.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jiagoushi.top/gtjhiecrin.html

[E21] 超长截断加省略号
来源：http://hz.sweek.top/gtjhvwipsv.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.gogol.net.cn/gtnulfoyme.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.sweek.top/gtsthghccd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.tanke756.top/gtkdaiwjdg.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.sweek.top/gtpztebxcy.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yj20258888.top/gtqydrxzox.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.sweek.top/gtuwepbhhd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yuxming.cn/gtylqmsxvi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.fzhhl.top/gtuwafvbbt.html

[E22] 字节长度与字符长度
来源：http://hz.daxiang520.top/gtbgdyhbjs.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yj20258.top/gttjvszcao.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jlsjyb.cn/gtllejbftv.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.meibo888.top/gtbuppjafd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yonumen.top/gtpzajacoe.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.sxryk.cn/gtktqgteez.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yuanzhike.top/gtdmteqcas.html

Ruby: s.bytesize;  s.length
来源：http://hz.nanxuanxn.top/gtppxgaqgr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.haohaochexian.top/gtgdahmahr.html

================================================================================
来源：http://hz.aibaodan.cn/gtmeazgidj.html

F. 文件与目录
来源：http://hz.birdmap.top/gtbwoxywfo.html

================================================================================
来源：http://hz.sweek.top/gtzmlxgjbd.html

[F01] 读取整个文件
来源：http://hz.pengpengdd.cyou/gtuoawvxuo.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.andypj.xyz/gtwicsgzua.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zycfv.cn/gtdkvehpbq.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.sysykeji.top/gtpldjkkkv.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.chenjidiqi.icu/gtuaubueqw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.ybcxt.top/gtwbiakikn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhiwuduotai.top/gtjywplhdn.html

Ruby: File.read("a.txt")
来源：http://hz.hammf.cn/gtxxceamwd.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.svipenyu.cn/gthwexmbmz.html

[F02] 逐行读取文件
来源：http://hz.aibaodan.cn/gtdnxkhvhq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.pengpengdd.cyou/gtqmtxjndp.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.mhx1999.top/gtomzhqikb.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yuxming.cn/gtehzhknwe.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hongshengwenyu.top/gtyunskxmw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.52xcode.cn/gtznygrkqb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yanxiufei.cn/gtlrezkabh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.nwbrower.top/gtuyxhppkb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.xuanzx.com/gtusmqdjmx.html

[F03] 写入文件（覆盖）
来源：http://hz.jqgfzy.top/gtwyfsmhqy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.dianchejie.cn/gtfrnrrjhs.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yj202588.top/gtduabfrlb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.nwbrower.top/gtihyuybky.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ppjwa.cn/gtwomvfges.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.ehwqpu.com/gtwynbqlzj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.vqdsnc.cn/gtldqepzon.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yongpay.top/gtwfwvsflb.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.ybcxt.top/gtghrknmqj.html

[F04] 追加写入文件
来源：http://hz.ydjk.org.cn/gtcaxrzmpz.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.ybcxt.top/gtjrzcqdoz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.cheryme.top/gtewxyvzjp.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.nanxuanxn.top/gtlsulrafy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xuetiantiany.cn/gtitzsbreb.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.dashuyun.cn/gttepmwpys.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.mhx1999.top/gtjsdozhxn.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.xuanzx.com/gthrflsxua.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.c1oappe.top/gtwauzbuef.html

[F05] 判断文件或目录是否存在
来源：http://hz.meibo888.top/gtvrgbtmfy.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zdqjudy.top/gtavadcyak.html

PHP:  file_exists("a.txt");
来源：http://hz.kuanghao11.cn/gtssjwpmiw.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtjyferhdj.html

TS:   fs.existsSync("a.txt")
来源：http://hz.hnqzz.top/gtumzoyevi.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zycfv.cn/gtvbvegxsw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.wangdashe.top/gtcwpyrnqz.html

Ruby: File.exist?("a.txt")
来源：http://hz.zhongyouzk.top/gtgtynjkxa.html

C#:   File.Exists("a.txt")
来源：http://hz.shanyushiyangtech.top/gtphrjyykm.html

[F06] 删除文件
来源：http://hz.yuanzhike.top/gtvctdsnky.html

Py:   os.remove("a.txt")
来源：http://hz.yj202588.top/gtjnhzaqqq.html

PHP:  unlink("a.txt");
来源：http://hz.ppjwa.cn/gtnpzkpxvw.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.daria6918.cn/gtoljykdlg.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.0kj1m.cn/gtsfizzygo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.pycfn.com/gtgpmljlln.html

Go:   os.Remove("a.txt")
来源：http://hz.yueranfly.top/gtxczplgqq.html

Ruby: File.delete("a.txt")
来源：http://hz.quarkkingdee.top/gtjdphwcfl.html

C#:   File.Delete("a.txt");
来源：http://hz.ppjwa.cn/gtigyduovb.html

[F07] 创建目录（含多级）
来源：http://hz.jqgufenzy.top/gttdjqxnnd.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yj20258.top/gtoddzawhy.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.shuidangran.top/gthpxareya.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.0kj1m.cn/gtuarstajs.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.cashguo.top/gtxcblcjun.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.feifeiyinyue.top/gtjreejqeb.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.gaohongyu789.top/gtcnzxsaex.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.aizwys.cn/gtpeilzjeq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.vqdsnc.cn/gtqzpgoaiu.html

[F08] 遍历目录
来源：http://hz.aibaodan.cn/gtzlzywmbp.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yj202588.top/gtloehzsme.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.zhixingplan.top/gtsokbcrzr.html

JS:   fs.readdirSync("dir")
来源：http://hz.ivvv.top/gtafvfvbnd.html

TS:   fs.readdirSync("dir")
来源：http://hz.tanke756.top/gtvpwgxtsq.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.mhx1999.top/gtxjddciup.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.wangdashe.top/gtcnkftwlr.html

Ruby: Dir.children("dir")
来源：http://hz.jyoumei.cn/gtwkdfqnjp.html

C#:   Directory.GetFiles("dir")
来源：http://hz.xingfuxueyuan.xyz/gtpxbhjtli.html

[F09] 获取文件大小
来源：http://hz.jqgufenzy.top/gtclwuavdd.html

Py:   os.path.getsize("a.txt")
来源：http://hz.c1oappe.top/gtjrboehdh.html

PHP:  filesize("a.txt");
来源：http://hz.xinyue.icu/gttjxnvumz.html

JS:   fs.statSync("a.txt").size
来源：http://hz.smart0.xyz/gtqmqsinxk.html

TS:   fs.statSync("a.txt").size
来源：http://hz.gaohongyu789.top/gtrthchhfn.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.meibo888.top/gtequbclsn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.havefunace.top/gtmityyukm.html

Ruby: File.size("a.txt")
来源：http://hz.zhengqikj.top/gtynwxatep.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.fengsongda.top/gtibspbsjr.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.kuanghao11.cn/gthwxunxbv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtbrgsficr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.pengpengdd.cyou/gtifkumagn.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.xuanzx.com/gtpinpdswb.html

TS:   path.extname("a.txt")
来源：http://hz.chenjidiqi.icu/gtzhrfckop.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.nanxuanxn.top/gtipkavzcv.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.aibaodan.cn/gtnlhjufsu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.tanke756.top/gtgudtsqel.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.wangdashe.top/gtzlqhesef.html

[F11] 复制与移动文件
来源：http://hz.xziqi.cn/gtxxudazlg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.cucudq.cn/gtrkxuvbkl.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.316326.xyz/gtkcbnfhcb.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yvedp.cn/gtjzbzxdyl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xuetiantiany.cn/gtsqgfeowo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.cdnleiting.top/gttnjxtuig.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.xziqi.cn/gtprlafvis.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.cdnleiting.top/gtwzoysihk.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.havefunace.top/gtncgmpgyj.html

[F12] CSV 读写
来源：http://hz.zhongyouzk.top/gtwtqbkbxy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.chenlongwang.top/gtcksmaqlt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.cucudq.cn/gtsxtxugez.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhengqikj.top/gtrptvxael.html

TS:   // 同上
来源：http://hz.cashguo.top/gtfkqcpswm.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.cucudq.cn/gthmqoemrw.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhixingplan.top/gtbwryhhwf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ybcxt.top/gtukysnyfa.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.ehwqpu.com/gtkzmagfuu.html

================================================================================
来源：http://hz.dianchejie.cn/gtadtxifiv.html

G. 面向对象
来源：http://hz.nanxuanxn.top/gtobljntkd.html

================================================================================
来源：http://hz.cqqwz.cn/gtsihvvrhj.html

[G01] 定义类
来源：http://hz.chenlongwang.top/gtiemuxxfm.html

Py:   class User: pass
来源：http://hz.guannengcc.top/gtnhoyjkgt.html

PHP:  class User {}
来源：http://hz.haohaochexian.top/gtyufodzgf.html

JS:   class User {}
来源：http://hz.cheryme.top/gtiiiiipvm.html

TS:   class User { name: string = ""; }
来源：http://hz.yonumen.top/gtwksdwzco.html

Java: class User {}
来源：http://hz.52xcode.cn/gtqdijhipe.html

Go:   type User struct { Name string }
来源：http://hz.jqgufenzy.top/gtfvsprqnp.html

Ruby: class User; end
来源：http://hz.yueranfly.top/gthxluhwhh.html

C#:   class User {}
来源：http://hz.wangdashe.top/gtfhfnexnr.html

[G02] 构造函数
来源：http://hz.wangdashe.top/gttqkwlmbm.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.gotoacloud.top/gtbhdcapjo.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.0kj1m.cn/gtfwyunkkm.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.nanxinkj.top/gtbuypvozy.html

TS:   constructor(public name: string) {}
来源：http://hz.guannengcc.top/gtfzgyftwl.html

Java: User(String name) { this.name = name; }
来源：http://hz.birdmap.top/gtettwmxxq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.ybcxt.top/gtlbehlymn.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.zycfv.cn/gtxqrckyff.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhijiandao.cn/gtcjpinoul.html

[G03] 实例属性
来源：http://hz.c1oappe.top/gtsavpnwwq.html

Py:   self.name = "x"
来源：http://hz.9152youxi.cn/gtkpmbkjem.html

PHP:  public string $name = "x";
来源：http://hz.yuxming.cn/gtvwzrylxk.html

JS:   this.name = "x";
来源：http://hz.cashguo.top/gtnbqtaiuz.html

TS:   name: string = "x";
来源：http://hz.svipenyu.cn/gtxgkkxmde.html

Java: private String name;
来源：http://hz.yueranfly.top/gtowuzvvkg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.gzhubu.top/gtpmztnher.html

Ruby: @name = "x"
来源：http://hz.haohaochexian.top/gthgzqymcz.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jqgufenzy.top/gtfmfeqegw.html

[G04] 定义方法
来源：http://hz.wangdashe.top/gturrtcemf.html

Py:   def greet(self): return self.name
来源：http://hz.jqgfzy.top/gtxrqljncp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhiwuduotai.top/gtirvagyel.html

JS:   greet() { return this.name; }
来源：http://hz.jlsjyb.cn/gtekqkvhws.html

TS:   greet(): string { return this.name; }
来源：http://hz.dianchejie.cn/gtpsyphrum.html

Java: String greet() { return name; }
来源：http://hz.zhixingplan.top/gtzzomxnhw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ydjk.org.cn/gtrtexivsg.html

Ruby: def greet; @name; end
来源：http://hz.snrcjt.cn/gtuxatfuto.html

C#:   public string Greet() => Name;
来源：http://hz.svipenyu.cn/gtbsreafad.html

[G05] 继承
来源：http://hz.zhengqikj.top/gtsmnmozfv.html

Py:   class Admin(User): pass
来源：http://hz.jianghu66.top/gtpxzylvwu.html

PHP:  class Admin extends User {}
来源：http://hz.zhongyouzk.top/gtsbqydfkg.html

JS:   class Admin extends User {}
来源：http://hz.aizwys.cn/gtarampnyx.html

TS:   class Admin extends User {}
来源：http://hz.hammf.cn/gtevvqhhgw.html

Java: class Admin extends User {}
来源：http://hz.jiagoushi.top/gtvtxzqwxv.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.c1oappe.top/gtatyqrzbx.html

Ruby: class Admin < User; end
来源：http://hz.smart0.xyz/gtlpmrxtkx.html

C#:   class Admin : User {}
来源：http://hz.kuanghao11.cn/gtwkhjoqpa.html

[G06] 重写方法
来源：http://hz.hywenlv.cn/gtcayxacaf.html

Py:   def greet(self): return "admin"
来源：http://hz.sysykeji.top/gtngylzzlj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jinghuilouyu.cn/gtenpcnzzw.html

JS:   greet() { return "admin"; }
来源：http://hz.feifeiyinyue.top/gtbyfqgajp.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jinghuilouyu.cn/gtvriqqyah.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.nanxinkj.top/gtkrnmqcyc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.guannengcc.top/gtzvtcxqid.html

Ruby: def greet; "admin"; end
来源：http://hz.c1oappe.top/gtbkcxdhcr.html

C#:   public override string Greet() => "admin";
来源：http://hz.yanxiufei.cn/gtfgndjsas.html

[G07] 调用父类方法
来源：http://hz.zycfv.cn/gtimnsqvpu.html

Py:   super().greet()
来源：http://hz.xingfuxueyuan.xyz/gteqnsrxeh.html

PHP:  parent::greet();
来源：http://hz.havefunace.top/gtgntoxows.html

JS:   super.greet();
来源：http://hz.smart0.xyz/gtpxtmqrig.html

TS:   super.greet();
来源：http://hz.jqgfzy.top/gtjjhfdbuo.html

Java: super.greet();
来源：http://hz.iojbl.cn/gtjrexfzmi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.iojbl.cn/gtghklslyy.html

Ruby: super
来源：http://hz.dianchejie.cn/gtbldijixt.html

C#:   base.Greet();
来源：http://hz.bjfxy.top/gtzekjjaqh.html

[G08] 静态方法与属性
来源：http://hz.jinqigfzy.top/gtokenhzyc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jqgfzy.top/gtdzzgcmjg.html

PHP:  public static function f() {}
来源：http://hz.hfpthk.cn/gtsmbenoxm.html

JS:   static f() {}
来源：http://hz.shangyingyoupin.top/gtlaeitamy.html

TS:   static f(): void {}
来源：http://hz.tanke756.top/gtrutptxev.html

Java: static void f() {}
来源：http://hz.xziqi.cn/gtuixapdsd.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yj20258.top/gtrdkzyqys.html

Ruby: def self.f; end
来源：http://hz.xuetiantiany.cn/gtypvuwozr.html

C#:   public static void F() {}
来源：http://hz.hfpthk.cn/gtlrleavwb.html

[G09] 接口 / 抽象类
来源：http://hz.jianghu66.top/gtccooiana.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.shzxlz.cn/gtvwnzgkun.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yj20258.top/gtuovleaqc.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.guannengcc.top/gtxalnrevb.html

TS:   interface Shape { area(): number; }
来源：http://hz.xuanzx.com/gthfmhxcam.html

Java: interface Shape { double area(); }
来源：http://hz.chenzaomai.com/gtwrqvcjaa.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.shzxlz.cn/gtqprclqld.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jianghu66.top/gtrtnrzddy.html

C#:   interface IShape { double Area(); }
来源：http://hz.jinghuilouyu.cn/gtzogncjyx.html

[G10] 访问控制
来源：http://hz.dianchejie.cn/gtimfdbhsg.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.vqdsnc.cn/gtqqwftjar.html

PHP:  public / protected / private
来源：http://hz.smart0.xyz/gtgcztdvws.html

JS:   #private 字段；其余公开
来源：http://hz.fzhhl.top/gtmjvqxxaj.html

TS:   public / protected / private
来源：http://hz.nanxinkj.top/gtfdkbnlvg.html

Java: public / protected / private / 默认包级
来源：http://hz.c1oappe.top/gtrwlkbmhl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.svipenyu.cn/gtscrqmrgr.html

Ruby: public / protected / private
来源：http://hz.zhaomingkeji.xyz/gthrequzbr.html

C#:   public / protected / private / internal
来源：http://hz.hnqzz.top/gtjwrrvqtd.html

[G11] getter / setter
来源：http://hz.yongpay.top/gticnipuih.html

Py:   @property 与 @x.setter
来源：http://hz.jinqigufen.top/gtiifjcwkm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.snrcjt.cn/gtrmfermdh.html


<!-- 参考信息 -->