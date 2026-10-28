代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.jinghuilouyu.cn/gtuhnqlanw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.sufxvd.cn/gtyyouusrn.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jinghuilouyu.cn/gthgegpito.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.zhaomingkeji.xyz/gtuabkpqxn.html

[E14] URL 编码与 Base64
来源：http://hz.zhiwuduotai.top/gterulionk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.shanyushiyangkeji.top/gtbwqzrqek.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.chenlongwang.top/gtlwtygewf.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.zycfv.cn/gtzetqxvvc.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.daxiang520.top/gtkugoeyar.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.mhx1999.top/gtnzkirpuc.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zhiwuduotai.top/gtgjdulovv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.nanxuanxn.top/gtrthgmqve.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.cucudq.cn/gtxevwropj.html

[E15] HTML 转义 / 反转义
来源：http://hz.jyoumei.cn/gtyeiwljlp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.cqqwz.cn/gteywfwplr.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.aibaodan.cn/gtylrxpvnm.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yvedp.cn/gtlryiadby.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.havefunace.top/gtvwcatois.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.zycfv.cn/gtociuktui.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yongpay.top/gtaoqhhxpn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.9152youxi.cn/gtivfqkukx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.ybcxt.top/gtuubrhwch.html

[E16] 数字千分位
来源：http://hz.cashguo.top/gtqqasvgrn.html

Py:   f"{1234567:,}"
来源：http://hz.316326.xyz/gtslbggfks.html

PHP:  number_format(1234567);
来源：http://hz.jqgfzy.top/gtoqkejsox.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.iojbl.cn/gtsmxyzduv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.hongshengwenyu.top/gtiachsvkw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.hongshengwenyu.top/gtyrtnkkit.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yj20258.top/gtyisppquf.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.iojbl.cn/gtokwxtplr.html

C#:   1234567.ToString("N0")
来源：http://hz.wangdashe.top/gtarbzxkbc.html

[E17] 首字母大写
来源：http://hz.haohaochexian.top/gtpqbphdvl.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.wangshuangyany.cn/gtrlzzdvts.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.zhoulong.xyz/gthcubfksh.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jlsjyb.cn/gtetcattzd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hnxiangtu.top/gtkhzxfwjw.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.hnxiangtu.top/gtrbspvulu.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.0kj1m.cn/gtigqizpwn.html

Ruby: s.capitalize
来源：http://hz.birdmap.top/gtmolrripp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.sufxvd.cn/gtwalqbjdf.html

[E18] 模板占位符替换
来源：http://hz.sysykeji.top/gtghouvkqm.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.havefunace.top/gtgsypqgvb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.chenzaomai.com/gtqzdlfusi.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.gzhubu.top/gtpupvjyut.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinghuilouyu.cn/gthleftwex.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.kuanghao11.cn/gtxbdnnxbo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.ybcxt.top/gtbtkhnkbj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hnxiangtu.top/gtslbyzrms.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.hnxiangtu.top/gtrwtdcsip.html

[E19] 多行文本按行拆分
来源：http://hz.ybcxt.top/gtfvzbrkct.html

Py:   s.splitlines()
来源：http://hz.birdmap.top/gtkohymjdc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.meibo888.top/gtwrmphusz.html

JS:   s.split(/\r?\n/)
来源：http://hz.tianlin.xyz/gtxtwckvof.html

TS:   s.split(/\r?\n/)
来源：http://hz.xuanzx.com/gtxlhizhtg.html

Java: s.lines().toList()
来源：http://hz.xingfuxueyuan.xyz/gtynrcbovc.html

Go:   strings.Split(s, "\n")
来源：http://hz.zhiwuduotai.top/gtjgkjpidu.html

Ruby: s.lines
来源：http://hz.52xcode.cn/gtgjuvugxd.html

C#:   s.Split('\n')
来源：http://hz.yj202588.top/gtkxxpovob.html

[E20] 判断字符串是否为空
来源：http://hz.daxiang520.top/gtvtpopbmx.html

Py:   if not s:
来源：http://hz.gogol.net.cn/gtmzbmnrrl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.xylfe.cn/gtbrzdscxl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.wangdashe.top/gtqpqzxlrh.html

TS:   if (s === "") {}
来源：http://hz.hywenlv.cn/gthjhxgvaw.html

Java: if (s.isEmpty()) {}
来源：http://hz.zhengqikj.top/gtifamvarc.html

Go:   if s == "" {}
来源：http://hz.ybcxt.top/gtubnuufmt.html

Ruby: if s.empty?
来源：http://hz.yj20258.top/gtfmtiibcc.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.chenzaomai.com/gtjyvzrewh.html

[E21] 超长截断加省略号
来源：http://hz.vqdsnc.cn/gtenryjvoa.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.gaohongyu789.top/gtfdzqljps.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.shanyushiyangtech.top/gtbefsuadp.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.chenzaomai.com/gtibyiozzt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.xinyue.icu/gtbanmvemi.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jinghuilouyu.cn/gthadaofnb.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.chenjidiqi.icu/gtqeoxnuvx.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.mhx1999.top/gtnvfvkgxf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ybcxt.top/gtkzrreuac.html

[E22] 字节长度与字符长度
来源：http://hz.jianghu66.top/gtbkeiiwcp.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.zycfv.cn/gthsamlinz.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.tanke756.top/gtgnfwqxxr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hnxiangtu.top/gtfbyqhwbf.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.havefunace.top/gtfiiuiplc.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.xingfuxueyuan.xyz/gtdvxscxqo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.ppjwa.cn/gtswiyhtqo.html

Ruby: s.bytesize;  s.length
来源：http://hz.snrcjt.cn/gttzqnkiut.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.zhiwuduotai.top/gtcjkgvzjk.html

================================================================================
来源：http://hz.cucudq.cn/gtzivrwtlk.html

F. 文件与目录
来源：http://hz.tanke756.top/gtgobncfnt.html

================================================================================
来源：http://hz.sxryk.cn/gtargzzlmr.html

[F01] 读取整个文件
来源：http://hz.gaohongyu789.top/gtugdjezmu.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yvedp.cn/gtezrflnog.html

PHP:  file_get_contents("a.txt");
来源：http://hz.nanxuanxn.top/gtztgfywbx.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.xuanzx.com/gtfuaiwfnm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.quarkkingdee.top/gtokoezzps.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.kuanghao11.cn/gtsjtjaygu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhoulong.xyz/gtbdjlhqap.html

Ruby: File.read("a.txt")
来源：http://hz.tian-w.cn/gtaepjhojf.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.shzxlz.cn/gtebxgapos.html

[F02] 逐行读取文件
来源：http://hz.shangyingyoupin.top/gtaegpeipl.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.nanxuanxn.top/gtlzvwavqb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.jqgufenzy.top/gtnseaeyub.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xuanzx.com/gtqnhqnpbm.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jianghu66.top/gtmwpikari.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.tianlin.xyz/gtwehbgqwm.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.chenlongwang.top/gtfcogffhd.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.hfpthk.cn/gtqeuuswzs.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.dashuyun.cn/gtiugkcnsp.html

[F03] 写入文件（覆盖）
来源：http://hz.zhengqikj.top/gtgpjuqfph.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.9152youxi.cn/gtfelfjmhj.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.yueranfly.top/gtctpmxysk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.vqdsnc.cn/gtfricodxc.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sysykeji.top/gtfvwdljcy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.c1oappe.top/gteeikjmeq.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jinqigfzy.top/gtvnfuaovb.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.guowangkeji.top/gtgjcgolbm.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.zycfv.cn/gtkvwdacdr.html

[F04] 追加写入文件
来源：http://hz.shanyushiyangtech.top/gtdksamhvy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.ehwqpu.com/gtftrvuofq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.shangyingyoupin.top/gtljekxrye.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.tian-w.cn/gtrpusddcx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.pengpengdd.cyou/gtljoutgws.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.tian-w.cn/gtekdhnxkd.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.ppjwa.cn/gtkjeemmum.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.daria6918.cn/gtmaijfaey.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.gzhubu.top/gtbvelaxgn.html

[F05] 判断文件或目录是否存在
来源：http://hz.mhx1999.top/gtpnragoxk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.gotoacloud.top/gthmcctixr.html

PHP:  file_exists("a.txt");
来源：http://hz.shanyushiyangtech.top/gtenptypqn.html

JS:   fs.existsSync("a.txt")
来源：http://hz.birdmap.top/gtuaeomfov.html

TS:   fs.existsSync("a.txt")
来源：http://hz.jyoumei.cn/gtexkqaekp.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.ivvv.top/gtfsdhmzzs.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.quarkkingdee.top/gturdqunzr.html

Ruby: File.exist?("a.txt")
来源：http://hz.hongshengwenyu.top/gttshoavam.html

C#:   File.Exists("a.txt")
来源：http://hz.guannengcc.top/gtgeqdhvkc.html

[F06] 删除文件
来源：http://hz.fzhhl.top/gtbsambwuk.html

Py:   os.remove("a.txt")
来源：http://hz.hongshengwenyu.top/gtgxjltjtd.html

PHP:  unlink("a.txt");
来源：http://hz.jqgufenzy.top/gtmwexylrz.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.andypj.xyz/gtscbcwjix.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jqgufenzy.top/gtanikgyxn.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.chenzaomai.com/gtlupqgcjs.html

Go:   os.Remove("a.txt")
来源：http://hz.shzxlz.cn/gtyatbozfj.html

Ruby: File.delete("a.txt")
来源：http://hz.xziqi.cn/gtdwzupvns.html

C#:   File.Delete("a.txt");
来源：http://hz.gogol.net.cn/gtwmbdazxo.html

[F07] 创建目录（含多级）
来源：http://hz.ehwqpu.com/gtfpqoxzle.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.xuanzx.com/gtrqhtzjlw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.52xcode.cn/gtfplvqhsf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ydzc1.top/gtkrofqvby.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xylfe.cn/gtywghqfdh.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.ybcxt.top/gtminokqhk.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.ydjk.org.cn/gtaiwbqtbf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.pengpengdd.cyou/gtahmfwfio.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.havefunace.top/gtomurgghc.html

[F08] 遍历目录
来源：http://hz.zhijiandao.cn/gtboejiaiq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.316326.xyz/gtqjkxmheb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.snrcjt.cn/gtzewibgtb.html

JS:   fs.readdirSync("dir")
来源：http://hz.cheryme.top/gthvvwmpax.html

TS:   fs.readdirSync("dir")
来源：http://hz.kuanghao11.cn/gtbsyewssp.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.birdmap.top/gtneokxwkt.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yuxming.cn/gtauqevjwr.html

Ruby: Dir.children("dir")
来源：http://hz.ppjwa.cn/gtiucgclnr.html

C#:   Directory.GetFiles("dir")
来源：http://hz.andypj.xyz/gtwrbsmyho.html

[F09] 获取文件大小
来源：http://hz.shuidangran.top/gtholrdakx.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yangfankeji.com/gtycsnqptu.html

PHP:  filesize("a.txt");
来源：http://hz.jinyuanbaomall.cn/gtkhkuuqap.html

JS:   fs.statSync("a.txt").size
来源：http://hz.ehwqpu.com/gtbdnmmqrp.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zhongyouzk.top/gtpswyasru.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jinghuilouyu.cn/gtxruxhgrh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.tianlin.xyz/gttiojknuv.html

Ruby: File.size("a.txt")
来源：http://hz.jyoumei.cn/gtzipiatjx.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.tian-w.cn/gtnbmdayyt.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yvedp.cn/gtbgfuqnfe.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.aizwys.cn/gtwdxxxojm.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.tianlin.xyz/gtaicqxflx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jiagoushi.top/gtzvjjvkkx.html

TS:   path.extname("a.txt")
来源：http://hz.dashuyun.cn/gtcteianuo.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.havefunace.top/gtmijcjsku.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.redwolf501.top/gttplhhqwv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.shanyushiyangtech.top/gteybcnjyj.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhongyouzk.top/gttqwsykin.html

[F11] 复制与移动文件
来源：http://hz.bjfxy.top/gtjetcwsxv.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jqgufenzy.top/gtydnakgrm.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.52xcode.cn/gtpmgwyfcv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yongpay.top/gtxuzlzkbh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ppjwa.cn/gtqgslhydu.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.hammf.cn/gtmwzmdros.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.snrcjt.cn/gtkztthcwj.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ppjwa.cn/gtivsmgxma.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hfpthk.cn/gtnfddjavj.html

[F12] CSV 读写
来源：http://hz.gogol.net.cn/gtwgatxdsz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.tian-w.cn/gtcnqxgkxq.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hammf.cn/gtgrvouppo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.xinyue.icu/gtfoesthjp.html

TS:   // 同上
来源：http://hz.52xcode.cn/gtyrguahbp.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.0kj1m.cn/gtdonktyvn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.ywan-chungtsiang.top/gtulkegbvr.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.shzxlz.cn/gtrscnfnxy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.smart0.xyz/gtdijckutt.html

================================================================================
来源：http://hz.daxiang520.top/gtyquzrwsm.html

G. 面向对象
来源：http://hz.zhengqikj.top/gtlpboswuq.html

================================================================================
来源：http://hz.yuxming.cn/gthjhktfim.html

[G01] 定义类
来源：http://hz.cashguo.top/gtvjeacqgn.html

Py:   class User: pass
来源：http://hz.redwolf501.top/gtadmwpcow.html

PHP:  class User {}
来源：http://hz.shuidangran.top/gtuttnstny.html

JS:   class User {}
来源：http://hz.daxiang520.top/gtvlivwzyv.html

TS:   class User { name: string = ""; }
来源：http://hz.gzhubu.top/gttrruobfc.html

Java: class User {}
来源：http://hz.yj20258888.top/gtkoeimsvo.html

Go:   type User struct { Name string }
来源：http://hz.hnqzz.top/gtwtbqkwdm.html

Ruby: class User; end
来源：http://hz.9152youxi.cn/gttxuawrly.html

C#:   class User {}
来源：http://hz.52xcode.cn/gtgbrlkajc.html

[G02] 构造函数
来源：http://hz.yongpay.top/gtjpqfftzv.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhongyouzk.top/gtscwjyoec.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jqgufenzy.top/gtptosnxua.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yvedp.cn/gtscxyamdh.html

TS:   constructor(public name: string) {}
来源：http://hz.yj202588.top/gtmsdtkgmh.html

Java: User(String name) { this.name = name; }
来源：http://hz.nanxinkj.top/gtfiafzyhb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hfpthk.cn/gtzrpzzjmw.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.fzhhl.top/gtbukgoqqx.html

C#:   public User(string name) { Name = name; }
来源：http://hz.meibo888.top/gttxdlvnrt.html

[G03] 实例属性
来源：http://hz.daria6918.cn/gtlzpvysxa.html

Py:   self.name = "x"
来源：http://hz.bjfxy.top/gtenncjapn.html

PHP:  public string $name = "x";
来源：http://hz.jlsjyb.cn/gtrbpucfjp.html

JS:   this.name = "x";
来源：http://hz.hongshengwenyu.top/gtmmpcobub.html

TS:   name: string = "x";
来源：http://hz.zdqjudy.top/gtrnvfzpsr.html

Java: private String name;
来源：http://hz.redwolf501.top/gtendgdkwv.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yonumen.top/gtkhoqgvnc.html

Ruby: @name = "x"
来源：http://hz.vqdsnc.cn/gtlcmrhowq.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.svipenyu.cn/gtqebkqcrb.html

[G04] 定义方法
来源：http://hz.hfpthk.cn/gtgcnhwews.html

Py:   def greet(self): return self.name
来源：http://hz.zhongyouzk.top/gtboayxgob.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yanxiufei.cn/gthrfrpcbl.html

JS:   greet() { return this.name; }
来源：http://hz.jinqigfzy.top/gtauelxtjp.html

TS:   greet(): string { return this.name; }
来源：http://hz.zycfv.cn/gthrjwlbhh.html

Java: String greet() { return name; }
来源：http://hz.cucudq.cn/gtepjbqfbv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.sufxvd.cn/gtykfszzjk.html

Ruby: def greet; @name; end
来源：http://hz.dashuyun.cn/gtoikngwqg.html

C#:   public string Greet() => Name;
来源：http://hz.guannengcc.top/gtzmszvjhh.html

[G05] 继承
来源：http://hz.dashuyun.cn/gtdtqourjk.html

Py:   class Admin(User): pass
来源：http://hz.chenjidiqi.icu/gttkcyicff.html

PHP:  class Admin extends User {}
来源：http://hz.nanxuanxn.top/gtbaymhlqy.html

JS:   class Admin extends User {}
来源：http://hz.pengpengdd.cyou/gtfdkolnho.html

TS:   class Admin extends User {}
来源：http://hz.feifeiyinyue.top/gtmyhuozlr.html

Java: class Admin extends User {}
来源：http://hz.daria6918.cn/gtzpgdnzhm.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.sysykeji.top/gtiididkcy.html

Ruby: class Admin < User; end
来源：http://hz.jlsjyb.cn/gtrmbpsbxh.html

C#:   class Admin : User {}
来源：http://hz.zhoulong.xyz/gtxvycdiav.html

[G06] 重写方法
来源：http://hz.ywan-chungtsiang.top/gtpakajwxq.html

Py:   def greet(self): return "admin"
来源：http://hz.sysykeji.top/gtvbggvntj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.daria6918.cn/gtbzhzlpei.html

JS:   greet() { return "admin"; }
来源：http://hz.yanxiufei.cn/gtakielizy.html

TS:   greet(): string { return "admin"; }
来源：http://hz.hywenlv.cn/gtpidjfpnz.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.iojbl.cn/gtphsxhijn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.jinqigufen.top/gtnggjiage.html

Ruby: def greet; "admin"; end
来源：http://hz.zhongyouzk.top/gtpspvuuud.html

C#:   public override string Greet() => "admin";
来源：http://hz.ybcxt.top/gtmslxwkcr.html

[G07] 调用父类方法
来源：http://hz.aibaodan.cn/gtaxdjxjsk.html

Py:   super().greet()
来源：http://hz.zhengqikj.top/gtnfquvuwo.html

PHP:  parent::greet();
来源：http://hz.smart0.xyz/gtkdamzshc.html

JS:   super.greet();
来源：http://hz.hnxiangtu.top/gtncncornz.html

TS:   super.greet();
来源：http://hz.nwbrower.top/gtfbjpjwei.html

Java: super.greet();
来源：http://hz.hfpthk.cn/gtyiwgsmdv.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hnxiangtu.top/gtpxgsxnpe.html

Ruby: super
来源：http://hz.shanyushiyangtech.top/gttmottbvn.html

C#:   base.Greet();
来源：http://hz.zhixingplan.top/gtlnuhqfdh.html

[G08] 静态方法与属性
来源：http://hz.cdnleiting.top/gtvcmtuuif.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.ydjk.org.cn/gtwgbnvtyi.html

PHP:  public static function f() {}
来源：http://hz.feifeiyinyue.top/gtpqeottwn.html

JS:   static f() {}
来源：http://hz.yonumen.top/gtmigigcpl.html

TS:   static f(): void {}
来源：http://hz.zhoulong.xyz/gtxrztazyl.html

Java: static void f() {}
来源：http://hz.hnqzz.top/gthtzycpcr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jinqigufen.top/gtifvwjrip.html

Ruby: def self.f; end
来源：http://hz.pycfn.com/gtugxrhsfj.html

C#:   public static void F() {}
来源：http://hz.xylfe.cn/gttpcwpnlt.html

[G09] 接口 / 抽象类
来源：http://hz.hongshengwenyu.top/gtbjdzlfpa.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.pycfn.com/gtnggctpym.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.zycfv.cn/gtjxfhkjer.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yangfankeji.com/gtmfbpansk.html

TS:   interface Shape { area(): number; }
来源：http://hz.havefunace.top/gtkzhemcxm.html

Java: interface Shape { double area(); }
来源：http://hz.sysykeji.top/gtotzdhekk.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.feifeiyinyue.top/gtabiaxjad.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhiwuduotai.top/gtlcjlhuey.html

C#:   interface IShape { double Area(); }
来源：http://hz.52xcode.cn/gtfbvdgmye.html

[G10] 访问控制
来源：http://hz.sysykeji.top/gtxrkqasea.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.dianchejie.cn/gtmhrlwdnj.html

PHP:  public / protected / private
来源：http://hz.jinyuanbaomall.cn/gtqplmtxil.html

JS:   #private 字段；其余公开
来源：http://hz.nanxinkj.top/gtwisikspx.html

TS:   public / protected / private
来源：http://hz.ywan-chungtsiang.top/gtwfprtibr.html

Java: public / protected / private / 默认包级
来源：http://hz.dashuyun.cn/gtajysqyfw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.cqqwz.cn/gtqcvsquth.html

Ruby: public / protected / private
来源：http://hz.wangshuangyany.cn/gtyjubgihm.html

C#:   public / protected / private / internal
来源：http://hz.yj20258888.top/gtfovfzqzq.html

[G11] getter / setter
来源：http://hz.mhx1999.top/gtfqtshzts.html

Py:   @property 与 @x.setter
来源：http://hz.zycfv.cn/gtlwmsrtdn.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.316326.xyz/gtgvlubzxo.html

JS:   get name() { return this._name; }
来源：http://hz.316326.xyz/gtatvlhxht.html

TS:   get name(): string { return this._name; }
来源：http://hz.gogol.net.cn/gttmsfowgf.html

Java: public String getName() { return name; }
来源：http://hz.hnxiangtu.top/gtuixofckw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.gaohongyu789.top/gtytxoxqcx.html

Ruby: attr_accessor :name
来源：http://hz.ehwqpu.com/gtwwsymfpp.html

C#:   public string Name { get; set; }
来源：http://hz.yueranfly.top/gtywksgqen.html

[G12] 对象转字符串
来源：http://hz.yueranfly.top/gtqemeotmo.html

Py:   def __str__(self): return self.name
来源：http://hz.yanxiufei.cn/gtxgtgcdsb.html


<!-- 参考信息 -->