代发 wailian999

Go:   strings.Count(s, "a")
来源：http://hz.zhixingplan.top/gtsfdsvfom.html

Ruby: s.count("a")
来源：http://hz.smart0.xyz/gtsqcscwwy.html

C#:   s.Count(c => c == 'a')
来源：http://hz.havefunace.top/gtilrwwhor.html

[E13] 逐字符遍历
来源：http://hz.yongpay.top/gtrhxasdns.html

Py:   for ch in s: print(ch)
来源：http://hz.havefunace.top/gtcxdcrvlj.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.ybcxt.top/gthfwqzdel.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.shanyushiyangtech.top/gtyenhzvqr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yj202588.top/gtggkicuuy.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.pengpengdd.cyou/gtqrxqijzf.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.quarkkingdee.top/gtsgydywwo.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.jlsjyb.cn/gtodgoemxs.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jinghuilouyu.cn/gtnyjiyqaq.html

[E14] URL 编码与 Base64
来源：http://hz.birdmap.top/gttghfpxgc.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.tian-w.cn/gtxwtsbave.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.jinyuanbaomall.cn/gthtwsvwaz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.zhengqikj.top/gthuawhvhz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.cashguo.top/gttbcdfhez.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.fzhhl.top/gtkkttimki.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.tian-w.cn/gtpvwfqxps.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.c1oappe.top/gtowylhtqz.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.fzhhl.top/gtaszqwwps.html

[E15] HTML 转义 / 反转义
来源：http://hz.gotoacloud.top/gtclpnlppx.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zhaomingkeji.xyz/gtdheugfjz.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.mhx1999.top/gtwqfqpcur.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.ydzc1.top/gthwwgtsfr.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.snrcjt.cn/gtgecxxoke.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.daxiang520.top/gtxlwmcfua.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.xziqi.cn/gtrascxfli.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.sweek.top/gtmjhhwltv.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zhiwuduotai.top/gtllydgrys.html

[E16] 数字千分位
来源：http://hz.tanke756.top/gtomhtvfya.html

Py:   f"{1234567:,}"
来源：http://hz.jqgufenzy.top/gtzwutpmiq.html

PHP:  number_format(1234567);
来源：http://hz.yj202588.top/gtylutxjdq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.jlsjyb.cn/gtuctxryan.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.svipenyu.cn/gtlkjxqnzb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.fengsongda.top/gtulgozbeq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.gogol.net.cn/gtxvgffnzr.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.chenjidiqi.icu/gtgtnuppmv.html

C#:   1234567.ToString("N0")
来源：http://hz.cdnleiting.top/gtirjrtdtz.html

[E17] 首字母大写
来源：http://hz.andypj.xyz/gtkvpzsqba.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.pengpengdd.cyou/gtgjzdfutg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.ywan-chungtsiang.top/gtlleigikw.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jqgfzy.top/gthudzzyva.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.meibo888.top/gtfxnrzdlg.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.cucudq.cn/gtuffbzmzh.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jinqigfzy.top/gtvkkobluj.html

Ruby: s.capitalize
来源：http://hz.zhixingplan.top/gtcffphdab.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jinqigufen.top/gtcvxofeas.html

[E18] 模板占位符替换
来源：http://hz.sysykeji.top/gtldukwvcs.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.xuanzx.com/gtfpvduxgr.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.ydzc1.top/gtvfdokrnv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.pycfn.com/gtnifwodde.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhongyouzk.top/gtqbheclhi.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.havefunace.top/gtshxmtchu.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.xuanzx.com/gtcyvvvbpj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jinqigfzy.top/gtpbwukdvp.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.chenjidiqi.icu/gtsjmkkdbi.html

[E19] 多行文本按行拆分
来源：http://hz.jinghuilouyu.cn/gtwajzrbyk.html

Py:   s.splitlines()
来源：http://hz.sweek.top/gtnalhpaqy.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yvedp.cn/gtrmgsgofs.html

JS:   s.split(/\r?\n/)
来源：http://hz.zhoulong.xyz/gtwzbjbpir.html

TS:   s.split(/\r?\n/)
来源：http://hz.9152youxi.cn/gthedkwmrp.html

Java: s.lines().toList()
来源：http://hz.zdqjudy.top/gtvuictvoi.html

Go:   strings.Split(s, "\n")
来源：http://hz.andypj.xyz/gtbcttfwsg.html

Ruby: s.lines
来源：http://hz.shanyushiyangkeji.top/gtrvbhcxpw.html

C#:   s.Split('\n')
来源：http://hz.yonumen.top/gtltmcdezj.html

[E20] 判断字符串是否为空
来源：http://hz.yueranfly.top/gtrkhbklit.html

Py:   if not s:
来源：http://hz.xinyue.icu/gtdeiigzww.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jinyuanbaomall.cn/gtnugtbuyk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.ydzc1.top/gtrvgnxmeh.html

TS:   if (s === "") {}
来源：http://hz.xingfuxueyuan.xyz/gtidcsybvv.html

Java: if (s.isEmpty()) {}
来源：http://hz.zhijiandao.cn/gtgpdynxzu.html

Go:   if s == "" {}
来源：http://hz.jinqigufen.top/gtsojlygbd.html

Ruby: if s.empty?
来源：http://hz.jiagoushi.top/gtifaagdts.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zhoulong.xyz/gtxvzizgiq.html

[E21] 超长截断加省略号
来源：http://hz.daxiang520.top/gtpyqkvjlj.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zdqjudy.top/gtuelzcela.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.hnxiangtu.top/gtfeukuvat.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yj20258888.top/gtbvnosfgn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinqigfzy.top/gtfetrzizx.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.guowangkeji.top/gtfktadkpl.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.52xcode.cn/gtvngfitpu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jlsjyb.cn/gtwmwroowa.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.kuanghao11.cn/gtebtrswqn.html

[E22] 字节长度与字符长度
来源：http://hz.birdmap.top/gtvraubciv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.chenlongwang.top/gtltvapivh.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhiwuduotai.top/gtoflijgtl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.nanxinkj.top/gtmxoswsxt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.aibaodan.cn/gtpnpgiice.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zhiwuduotai.top/gtxrjbhnqo.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.quarkkingdee.top/gtvnqslssd.html

Ruby: s.bytesize;  s.length
来源：http://hz.ehwqpu.com/gtzozzbtrt.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.zhiwuduotai.top/gtyclpejma.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtzvzxmwps.html

F. 文件与目录
来源：http://hz.yj20258888.top/gtcyusnxni.html

================================================================================
来源：http://hz.hnxiangtu.top/gtlgshgpjj.html

[F01] 读取整个文件
来源：http://hz.hnxiangtu.top/gtcbuddfyh.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yangfankeji.com/gtzhlgnyri.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zhengqikj.top/gtmbyzqvxi.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.kuanghao11.cn/gtuinnbcit.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.sufxvd.cn/gtmxixoofa.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.shangyingyoupin.top/gtcoghbqnx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.bjfxy.top/gtxwlwdxob.html

Ruby: File.read("a.txt")
来源：http://hz.pengpengdd.cyou/gtvlgbqtko.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.shanyushiyangkeji.top/gtewjxshfc.html

[F02] 逐行读取文件
来源：http://hz.jinqigufen.top/gtcvaisywx.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.yonumen.top/gtjlyceknt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.dashuyun.cn/gtidxtklhd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zdqjudy.top/gtkrzikonq.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.tian-w.cn/gthjoasfvq.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yj202588.top/gtuebiojay.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zhixingplan.top/gtbbepfbpi.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.tianlin.xyz/gtvguzzqnw.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.ydzc1.top/gttxblxswy.html

[F03] 写入文件（覆盖）
来源：http://hz.vqdsnc.cn/gtctseokms.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.gotoacloud.top/gtdqywmlqq.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.hnqzz.top/gtzgtqtoms.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhijiandao.cn/gtzoewxipb.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.daria6918.cn/gtwydujllr.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.meibo888.top/gteltzawby.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.shzxlz.cn/gtldvhdkdz.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.nanxuanxn.top/gtbamvsmum.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.feifeiyinyue.top/gtulqagacx.html

[F04] 追加写入文件
来源：http://hz.cheryme.top/gtycufjslv.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.dashuyun.cn/gtqldxqipq.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.cashguo.top/gtphhqvmrs.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jqgfzy.top/gtzbefuuwh.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.aibaodan.cn/gtzbptbjtr.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.52xcode.cn/gtesqnufzv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.yuanzhike.top/gtqormjyil.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jqgfzy.top/gtqijvhqdu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.cucudq.cn/gthbouttxd.html

[F05] 判断文件或目录是否存在
来源：http://hz.shzxlz.cn/gtpbfboyng.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yj20258888.top/gtrmopllow.html

PHP:  file_exists("a.txt");
来源：http://hz.52xcode.cn/gtkrfjexff.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yvedp.cn/gtiyqbaygs.html

TS:   fs.existsSync("a.txt")
来源：http://hz.jiagoushi.top/gtpfdgpczz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zhengqikj.top/gtzgkjvaxr.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.fengsongda.top/gtljgapjwr.html

Ruby: File.exist?("a.txt")
来源：http://hz.sysykeji.top/gtkinxffck.html

C#:   File.Exists("a.txt")
来源：http://hz.shangyingyoupin.top/gtfrmbzjfu.html

[F06] 删除文件
来源：http://hz.jqgufenzy.top/gtlyobrdif.html

Py:   os.remove("a.txt")
来源：http://hz.pycfn.com/gtqbvztsne.html

PHP:  unlink("a.txt");
来源：http://hz.zhongyouzk.top/gtdcvhnekk.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.jianghu66.top/gtskwktzow.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.sweek.top/gthcvsqdjp.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yongpay.top/gtfmwfsdlo.html

Go:   os.Remove("a.txt")
来源：http://hz.ydzc1.top/gtbtcjdclc.html

Ruby: File.delete("a.txt")
来源：http://hz.xuetiantiany.cn/gtoejxebgx.html

C#:   File.Delete("a.txt");
来源：http://hz.tanke756.top/gtjqszrksx.html

[F07] 创建目录（含多级）
来源：http://hz.birdmap.top/gthvllctrs.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.cqqwz.cn/gtymogeqtv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.cqqwz.cn/gtbykyiewb.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.wangdashe.top/gtbawpqcan.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.c1oappe.top/gtsiagbbez.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.quarkkingdee.top/gtblinpram.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.gzhubu.top/gtgfdlobxd.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.hywenlv.cn/gtmylmepos.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.316326.xyz/gtgqejxhar.html

[F08] 遍历目录
来源：http://hz.quarkkingdee.top/gteinadirg.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yj20258.top/gtbnuchqgv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.hnxiangtu.top/gtsttdsejp.html

JS:   fs.readdirSync("dir")
来源：http://hz.shangyingyoupin.top/gtqhyuecez.html

TS:   fs.readdirSync("dir")
来源：http://hz.xziqi.cn/gtasuhuetf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.xylfe.cn/gtciotcdcv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.hnxiangtu.top/gtgsutlisv.html

Ruby: Dir.children("dir")
来源：http://hz.haohaochexian.top/gtrgumnzos.html

C#:   Directory.GetFiles("dir")
来源：http://hz.xziqi.cn/gtdurhgqyz.html

[F09] 获取文件大小
来源：http://hz.9152youxi.cn/gttsaammgr.html

Py:   os.path.getsize("a.txt")
来源：http://hz.hysaishi.cn/gtokyeteug.html

PHP:  filesize("a.txt");
来源：http://hz.yuxming.cn/gtagjnkvex.html

JS:   fs.statSync("a.txt").size
来源：http://hz.guowangkeji.top/gtbtylijqd.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jlsjyb.cn/gtrelthnhc.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.hysaishi.cn/gtekzviteo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jinghuilouyu.cn/gtkqxsvsaz.html

Ruby: File.size("a.txt")
来源：http://hz.gotoacloud.top/gtmbgmcmns.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.aizwys.cn/gtikzzlxjx.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yvedp.cn/gtqdopsrmi.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.aizwys.cn/gtndjmmqfx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.pengpengdd.cyou/gtmkppvrnq.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.cheryme.top/gtwbgzjqli.html

TS:   path.extname("a.txt")
来源：http://hz.ivvv.top/gthwcrlqvz.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.yonumen.top/gtkrpmvgrn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.hongshengwenyu.top/gtgxgiqqzd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.xuetiantiany.cn/gtmrsdvdqb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.chenzaomai.com/gtjxfoaazw.html

[F11] 复制与移动文件
来源：http://hz.aibaodan.cn/gtagicjmuy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.cheryme.top/gtrbbjnqqo.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.svipenyu.cn/gtxbdvscav.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hongshengwenyu.top/gtguoegbov.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.chenjidiqi.icu/gtsmvqthvz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jyoumei.cn/gtjchxyjpr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.wangdashe.top/gtyedoqnxy.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ywan-chungtsiang.top/gtycvchsja.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ivvv.top/gtzhjhkqpt.html

[F12] CSV 读写
来源：http://hz.ybcxt.top/gtpsuycwbe.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhengqikj.top/gttkxftins.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.ydjk.org.cn/gtpghdombx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.dashuyun.cn/gtlgfcdpil.html

TS:   // 同上
来源：http://hz.havefunace.top/gtbobsjwzi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.cheryme.top/gtuxtwttwq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jinghuilouyu.cn/gtlqbbybjg.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.52xcode.cn/gtkaprongj.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.shanyushiyangkeji.top/gtngatkpgz.html

================================================================================
来源：http://hz.kuanghao11.cn/gtpfeibeup.html

G. 面向对象
来源：http://hz.shangyingyoupin.top/gtzcdgpsbd.html

================================================================================
来源：http://hz.zycfv.cn/gtvifgaxvl.html

[G01] 定义类
来源：http://hz.yj202588.top/gtncmuitbf.html

Py:   class User: pass
来源：http://hz.smart0.xyz/gtzxeykwrs.html

PHP:  class User {}
来源：http://hz.jiagoushi.top/gthtkbclwb.html

JS:   class User {}
来源：http://hz.hywenlv.cn/gtmhzlumev.html

TS:   class User { name: string = ""; }
来源：http://hz.kuanghao11.cn/gtwurpkoye.html

Java: class User {}
来源：http://hz.hnxiangtu.top/gtdqnwjoqf.html

Go:   type User struct { Name string }
来源：http://hz.hywenlv.cn/gtbtwmmgsb.html

Ruby: class User; end
来源：http://hz.yuanzhike.top/gtyecywgrm.html

C#:   class User {}
来源：http://hz.redwolf501.top/gthoyglrcn.html

[G02] 构造函数
来源：http://hz.daxiang520.top/gtumzudxzj.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yanxiufei.cn/gtlkkbdpkc.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.52xcode.cn/gtdgolpjzk.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.zycfv.cn/gtiiitnqph.html

TS:   constructor(public name: string) {}
来源：http://hz.aibaodan.cn/gtepljgdaq.html

Java: User(String name) { this.name = name; }
来源：http://hz.0kj1m.cn/gtqecvuofa.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zhoulong.xyz/gtfaxnsroc.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yuxming.cn/gttdkjveot.html

C#:   public User(string name) { Name = name; }
来源：http://hz.vqdsnc.cn/gtofdgbkdf.html

[G03] 实例属性
来源：http://hz.sufxvd.cn/gtokbrbrmw.html

Py:   self.name = "x"
来源：http://hz.yuanzhike.top/gtrlssrhmb.html

PHP:  public string $name = "x";
来源：http://hz.hnqzz.top/gtddufvtwr.html

JS:   this.name = "x";
来源：http://hz.andypj.xyz/gtprstrcci.html

TS:   name: string = "x";
来源：http://hz.hysaishi.cn/gtsdbirssk.html

Java: private String name;
来源：http://hz.yuanzhike.top/gtifubuqpf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.dashuyun.cn/gtvowsfxta.html

Ruby: @name = "x"
来源：http://hz.316326.xyz/gtaxgkvpze.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zhaomingkeji.xyz/gtlvsthnmj.html

[G04] 定义方法
来源：http://hz.fengsongda.top/gtkawrkdoo.html

Py:   def greet(self): return self.name
来源：http://hz.nanxuanxn.top/gtwdsnrjaf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.ppjwa.cn/gteclkdwcu.html

JS:   greet() { return this.name; }
来源：http://hz.hammf.cn/gtlczdyeuv.html

TS:   greet(): string { return this.name; }
来源：http://hz.sufxvd.cn/gthirbcqns.html

Java: String greet() { return name; }
来源：http://hz.gzhubu.top/gtapxzgpjs.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.yj20258.top/gtyvgoxwzn.html

Ruby: def greet; @name; end
来源：http://hz.xinyue.icu/gthvywafaa.html

C#:   public string Greet() => Name;
来源：http://hz.shanyushiyangtech.top/gtvhlpcxbb.html

[G05] 继承
来源：http://hz.shuidangran.top/gtovnaroid.html

Py:   class Admin(User): pass
来源：http://hz.yanxiufei.cn/gtioluolac.html

PHP:  class Admin extends User {}
来源：http://hz.gotoacloud.top/gtyxswvude.html

JS:   class Admin extends User {}
来源：http://hz.chenjidiqi.icu/gtkrnnzeaw.html

TS:   class Admin extends User {}
来源：http://hz.guowangkeji.top/gtrjumfiic.html

Java: class Admin extends User {}
来源：http://hz.fengsongda.top/gtyeieiumi.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jyoumei.cn/gtwjdoonad.html

Ruby: class Admin < User; end
来源：http://hz.zhixingplan.top/gtdkwkswkr.html

C#:   class Admin : User {}
来源：http://hz.gotoacloud.top/gtjvfahzps.html

[G06] 重写方法
来源：http://hz.yj20258.top/gtvllfoati.html

Py:   def greet(self): return "admin"
来源：http://hz.ybcxt.top/gtpiqtoccq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.sweek.top/gtgzhoeocp.html

JS:   greet() { return "admin"; }
来源：http://hz.shanyushiyangkeji.top/gtsvwziyeq.html

TS:   greet(): string { return "admin"; }
来源：http://hz.redwolf501.top/gtaqrjkjtj.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jinyuanbaomall.cn/gtiqphtrqn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.snrcjt.cn/gtuqvtfbej.html

Ruby: def greet; "admin"; end
来源：http://hz.shzxlz.cn/gtylnqizvv.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhiwuduotai.top/gtflwnkwsd.html

[G07] 调用父类方法
来源：http://hz.andypj.xyz/gtlcxdoebd.html

Py:   super().greet()
来源：http://hz.jqgfzy.top/gtbpokpxwi.html

PHP:  parent::greet();
来源：http://hz.shuidangran.top/gtgkkkudmy.html

JS:   super.greet();
来源：http://hz.nanxuanxn.top/gtcerrvjsr.html

TS:   super.greet();
来源：http://hz.aibaodan.cn/gtyajkqyzw.html

Java: super.greet();
来源：http://hz.gotoacloud.top/gtzcvnyqet.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jinyuanbaomall.cn/gtsmffseix.html

Ruby: super
来源：http://hz.shangyingyoupin.top/gthzvxtooa.html

C#:   base.Greet();
来源：http://hz.cheryme.top/gteuxiizbf.html

[G08] 静态方法与属性
来源：http://hz.hfpthk.cn/gtmzrleosp.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.316326.xyz/gtflcmaygw.html

PHP:  public static function f() {}
来源：http://hz.shanyushiyangkeji.top/gtobdfvypr.html

JS:   static f() {}
来源：http://hz.jyoumei.cn/gtjtsmcypo.html

TS:   static f(): void {}
来源：http://hz.jinghuilouyu.cn/gtteiggdbr.html

Java: static void f() {}
来源：http://hz.cqqwz.cn/gtpttwxiwr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.pengpengdd.cyou/gtqsfskhcb.html

Ruby: def self.f; end
来源：http://hz.yj202588.top/gtcqosazqn.html

C#:   public static void F() {}
来源：http://hz.ivvv.top/gtmzcootyj.html

[G09] 接口 / 抽象类
来源：http://hz.xuetiantiany.cn/gtiuqqpxxx.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.ehwqpu.com/gtdwdhgibl.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yuanzhike.top/gtnsavuuas.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jiagoushi.top/gtjccqsolz.html

TS:   interface Shape { area(): number; }
来源：http://hz.nanxuanxn.top/gtagtctfdo.html

Java: interface Shape { double area(); }
来源：http://hz.birdmap.top/gtmmbvvzok.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.wangshuangyany.cn/gtphoiaees.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jinqigufen.top/gtbfpdzpxh.html

C#:   interface IShape { double Area(); }
来源：http://hz.tanke756.top/gtbzhfzjtr.html

[G10] 访问控制
来源：http://hz.xziqi.cn/gtfxpfeqyi.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.birdmap.top/gtqnpnxzpk.html

PHP:  public / protected / private
来源：http://hz.shzxlz.cn/gtfxxxfuwn.html

JS:   #private 字段；其余公开
来源：http://hz.cheryme.top/gtllrxgobp.html

TS:   public / protected / private
来源：http://hz.zhongyouzk.top/gtshrqemis.html

Java: public / protected / private / 默认包级
来源：http://hz.xziqi.cn/gtqbrodith.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ydzc1.top/gtgqbqhhys.html

Ruby: public / protected / private
来源：http://hz.hywenlv.cn/gtnsqsydyj.html

C#:   public / protected / private / internal
来源：http://hz.xinyue.icu/gtsxbfkkmp.html

[G11] getter / setter
来源：http://hz.smart0.xyz/gtmujclbch.html

Py:   @property 与 @x.setter
来源：http://hz.daria6918.cn/gtsmgfrwpu.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.fengsongda.top/gtwfzcevci.html


<!-- 参考信息 -->