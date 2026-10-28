代发 wailian999

Go:   strings.Count(s, "a")
来源：http://hz.jinqigfzy.top/gtehdnanzo.html

Ruby: s.count("a")
来源：http://hz.cqqwz.cn/gtzhpeprkh.html

C#:   s.Count(c => c == 'a')
来源：http://hz.havefunace.top/gtmunismyb.html

[E13] 逐字符遍历
来源：http://hz.snrcjt.cn/gtuolidhnz.html

Py:   for ch in s: print(ch)
来源：http://hz.guannengcc.top/gtwweoopbd.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.redwolf501.top/gtaaxneqfr.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.zhixingplan.top/gtxcsjtbvt.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.dianchejie.cn/gtsofqhbpl.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.xingfuxueyuan.xyz/gtxxqmhgzb.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.ehwqpu.com/gtcokiepkf.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.shzxlz.cn/gtiauaeled.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.yangfankeji.com/gtwhjcosaw.html

[E14] URL 编码与 Base64
来源：http://hz.52xcode.cn/gtfoaxobmk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.ybcxt.top/gtawkazyfi.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.yvedp.cn/gtzsjnuupz.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.cucudq.cn/gtwltkzlnv.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.ydzc1.top/gtoqbkkkhc.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yuanzhike.top/gtpbpamqvy.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.xingfuxueyuan.xyz/gtsgaitwwz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jinyuanbaomall.cn/gtoainrdrl.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yuanzhike.top/gtqfxoeqia.html

[E15] HTML 转义 / 反转义
来源：http://hz.wangdashe.top/gtejnyhqdp.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jinyuanbaomall.cn/gtdcnycwcg.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.aizwys.cn/gtlwhydnka.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.cdnleiting.top/gtrbrcwlqm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.fengsongda.top/gtkdazezsy.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.hongshengwenyu.top/gtjipenoue.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.shangyingyoupin.top/gtpdafbdku.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jqgufenzy.top/gtyulidjqc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.shuidangran.top/gtauopwzdk.html

[E16] 数字千分位
来源：http://hz.shanyushiyangtech.top/gtymmcffyu.html

Py:   f"{1234567:,}"
来源：http://hz.gotoacloud.top/gtqxzlvgpo.html

PHP:  number_format(1234567);
来源：http://hz.zhengqikj.top/gtafttvxuo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.jinqigufen.top/gtvjnewseo.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.wangdashe.top/gtmtmwetya.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.aizwys.cn/gtsusbefev.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.cashguo.top/gtpfvwugil.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.hnqzz.top/gtbghimjje.html

C#:   1234567.ToString("N0")
来源：http://hz.yanxiufei.cn/gtpnqffezr.html

[E17] 首字母大写
来源：http://hz.xuanzx.com/gtmctnzcdp.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.aizwys.cn/gtntlmuhqb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.ybcxt.top/gtqqlncurb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hfpthk.cn/gtqsziwtwz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yj20258.top/gtrapajvrv.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yangfankeji.com/gtcyewogip.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.316326.xyz/gtenehjtpg.html

Ruby: s.capitalize
来源：http://hz.yanxiufei.cn/gtsfukaser.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.snrcjt.cn/gtwvxwxhzz.html

[E18] 模板占位符替换
来源：http://hz.shuidangran.top/gtubuelrhn.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.gzhubu.top/gtnjgoakex.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.mhx1999.top/gtxzaozirf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.shanyushiyangtech.top/gtuzetswtj.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.316326.xyz/gtfhcuebvh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.cheryme.top/gtsywiajlc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.quarkkingdee.top/gtlnpdjjdf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yanxiufei.cn/gtzbofxodn.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.sweek.top/gttdyxqzrc.html

[E19] 多行文本按行拆分
来源：http://hz.ybcxt.top/gtbiunkjkd.html

Py:   s.splitlines()
来源：http://hz.yanxiufei.cn/gtpvlvnhzi.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yuanzhike.top/gtrwamjsta.html

JS:   s.split(/\r?\n/)
来源：http://hz.jlsjyb.cn/gtbrcyyglk.html

TS:   s.split(/\r?\n/)
来源：http://hz.dianchejie.cn/gtujcxaran.html

Java: s.lines().toList()
来源：http://hz.gzhubu.top/gtbvaltfuy.html

Go:   strings.Split(s, "\n")
来源：http://hz.hfpthk.cn/gtsbhigdvl.html

Ruby: s.lines
来源：http://hz.yvedp.cn/gtngisblyz.html

C#:   s.Split('\n')
来源：http://hz.zycfv.cn/gttpbecxbi.html

[E20] 判断字符串是否为空
来源：http://hz.hnxiangtu.top/gtgyxugcwj.html

Py:   if not s:
来源：http://hz.yangfankeji.com/gtqzucmuwx.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.dashuyun.cn/gtbjlzzsji.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yangfankeji.com/gttnwntsbg.html

TS:   if (s === "") {}
来源：http://hz.xingfuxueyuan.xyz/gtkqxhblee.html

Java: if (s.isEmpty()) {}
来源：http://hz.yueranfly.top/gtbqwldyzq.html

Go:   if s == "" {}
来源：http://hz.dashuyun.cn/gtipjoyovm.html

Ruby: if s.empty?
来源：http://hz.pycfn.com/gtdpvmxhre.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.vqdsnc.cn/gtcyuaphii.html

[E21] 超长截断加省略号
来源：http://hz.birdmap.top/gtrfjwatuy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.aibaodan.cn/gtqmptdavx.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zycfv.cn/gtcgaxwvev.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yueranfly.top/gtnecmdmst.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hnqzz.top/gtjobgtqmn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.cheryme.top/gtgkhpwozs.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.haohaochexian.top/gtiqxquocu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yuanzhike.top/gtpishkmez.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.mhx1999.top/gtldiljdbn.html

[E22] 字节长度与字符长度
来源：http://hz.hnqzz.top/gtxnqbaiqt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.guowangkeji.top/gtjkvbkhzp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shanyushiyangkeji.top/gtgyiijdxd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yonumen.top/gtnswlntpa.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jqgufenzy.top/gtuateueoo.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jianghu66.top/gtahnpjupr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.iojbl.cn/gthhyebwqu.html

Ruby: s.bytesize;  s.length
来源：http://hz.9152youxi.cn/gtsbfyvmds.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.pycfn.com/gtihdisjfm.html

================================================================================
来源：http://hz.ydzc1.top/gtdtidzyeg.html

F. 文件与目录
来源：http://hz.cheryme.top/gtsnhwangf.html

================================================================================
来源：http://hz.ehwqpu.com/gtsworpjhx.html

[F01] 读取整个文件
来源：http://hz.ywan-chungtsiang.top/gtwzftjfaq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.ybcxt.top/gtfatnnxtz.html

PHP:  file_get_contents("a.txt");
来源：http://hz.zhijiandao.cn/gtecpzwvsj.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jinqigufen.top/gtgxgtnhxa.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.xuetiantiany.cn/gtuhifmoiw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.iojbl.cn/gtzmniqxvh.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jiagoushi.top/gtnzwvgccp.html

Ruby: File.read("a.txt")
来源：http://hz.gaohongyu789.top/gtgnqdbkzq.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.smart0.xyz/gtfaltrzbq.html

[F02] 逐行读取文件
来源：http://hz.ivvv.top/gtttxfpcyf.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zhengqikj.top/gtrvceimal.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.chenjidiqi.icu/gtrddjtzng.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yanxiufei.cn/gtvvjihnkg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.guowangkeji.top/gtnvekdspu.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.daxiang520.top/gtcfjrjzmz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.ivvv.top/gtqohdeibh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.bjfxy.top/gtxstdbgvq.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.xziqi.cn/gtispivnhe.html

[F03] 写入文件（覆盖）
来源：http://hz.vqdsnc.cn/gtgjvobhhv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jqgfzy.top/gtbtjekwqn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.dashuyun.cn/gtapvzfavk.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.gaohongyu789.top/gtzvnqujun.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jyoumei.cn/gtocmjdxhv.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.tian-w.cn/gtvjgptadr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.c1oappe.top/gtqpfprrns.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.chenlongwang.top/gtkmdogeag.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.fengsongda.top/gtfebugeta.html

[F04] 追加写入文件
来源：http://hz.hammf.cn/gtifblvweg.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.pengpengdd.cyou/gtjgcfauys.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.shanyushiyangkeji.top/gtilglbaii.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.c1oappe.top/gtwksttjmg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cheryme.top/gtwjfgzvev.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yj20258.top/gtwsfagsaa.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zhongyouzk.top/gtwrtmgpqe.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.gotoacloud.top/gtzdyghgaf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.ydzc1.top/gtiuegtmfc.html

[F05] 判断文件或目录是否存在
来源：http://hz.hywenlv.cn/gtaqbuvenf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.tian-w.cn/gtpsarpaik.html

PHP:  file_exists("a.txt");
来源：http://hz.xinyue.icu/gtstxmzxki.html

JS:   fs.existsSync("a.txt")
来源：http://hz.tanke756.top/gtahqajutq.html

TS:   fs.existsSync("a.txt")
来源：http://hz.0kj1m.cn/gtgyznmddn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zhongyouzk.top/gtniudqdym.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ppjwa.cn/gtbntadzuj.html

Ruby: File.exist?("a.txt")
来源：http://hz.hammf.cn/gtabiwdwxw.html

C#:   File.Exists("a.txt")
来源：http://hz.bjfxy.top/gtmxbecrcu.html

[F06] 删除文件
来源：http://hz.hfpthk.cn/gtlxpviatz.html

Py:   os.remove("a.txt")
来源：http://hz.cashguo.top/gtfhsiremy.html

PHP:  unlink("a.txt");
来源：http://hz.c1oappe.top/gtfwhdfkcy.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.nanxuanxn.top/gtkeyculuv.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.shangyingyoupin.top/gtzblforlv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.0kj1m.cn/gtrsubqjmy.html

Go:   os.Remove("a.txt")
来源：http://hz.chenjidiqi.icu/gtxgbudajc.html

Ruby: File.delete("a.txt")
来源：http://hz.52xcode.cn/gtbgaqwcxg.html

C#:   File.Delete("a.txt");
来源：http://hz.jinqigufen.top/gtizqdohwq.html

[F07] 创建目录（含多级）
来源：http://hz.bjfxy.top/gtkspfqtfa.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.wangshuangyany.cn/gtckrgrlve.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.chenzaomai.com/gttfvafetv.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.316326.xyz/gtyxprgalc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shuidangran.top/gtakonmbam.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.pycfn.com/gtkoaqxhbp.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.bjfxy.top/gtxaoyholi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.gzhubu.top/gtnjtcdgcq.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.guowangkeji.top/gtejpyqukg.html

[F08] 遍历目录
来源：http://hz.jqgufenzy.top/gtqlwinyax.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.tian-w.cn/gtkhtuoksv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.zhengqikj.top/gtcijqfnsj.html

JS:   fs.readdirSync("dir")
来源：http://hz.yj20258888.top/gthbvagkox.html

TS:   fs.readdirSync("dir")
来源：http://hz.hnqzz.top/gtqanfbetm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.dashuyun.cn/gtmxyikwsu.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yanxiufei.cn/gtwseamhbl.html

Ruby: Dir.children("dir")
来源：http://hz.chenzaomai.com/gtqrwevmfg.html

C#:   Directory.GetFiles("dir")
来源：http://hz.wangshuangyany.cn/gtlxrokmrh.html

[F09] 获取文件大小
来源：http://hz.cucudq.cn/gttxhqiiju.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jqgufenzy.top/gtdovvbior.html

PHP:  filesize("a.txt");
来源：http://hz.ydjk.org.cn/gthijnrnav.html

JS:   fs.statSync("a.txt").size
来源：http://hz.sxryk.cn/gtbxfzslyy.html

TS:   fs.statSync("a.txt").size
来源：http://hz.shangyingyoupin.top/gtyveadeur.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.xuetiantiany.cn/gtjcjnjssd.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.tianlin.xyz/gtvhvqpbjt.html

Ruby: File.size("a.txt")
来源：http://hz.yj20258.top/gtrjzhoohf.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yongpay.top/gtqudajfdc.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.jqgufenzy.top/gtgutrghsk.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.fzhhl.top/gtcyirpgfq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.yonumen.top/gtgsrvmqgm.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.cheryme.top/gtoaggxhhn.html

TS:   path.extname("a.txt")
来源：http://hz.jianghu66.top/gtoocmscnx.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.hfpthk.cn/gtebgwnexg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.kuanghao11.cn/gtilxpsupy.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.shanyushiyangkeji.top/gtgfaidnpc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.gaohongyu789.top/gtppxpamry.html

[F11] 复制与移动文件
来源：http://hz.ivvv.top/gtrsbksvzw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.c1oappe.top/gtrhrskmde.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.quarkkingdee.top/gttadiawtu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hfpthk.cn/gtjlissxsl.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cheryme.top/gtenbbnmle.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jlsjyb.cn/gtvmrzqdpm.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.nanxuanxn.top/gtbugadhth.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.aibaodan.cn/gtxhvgwvce.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.shzxlz.cn/gtgowxyazx.html

[F12] CSV 读写
来源：http://hz.guannengcc.top/gttkdwszro.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.hammf.cn/gtyofwkxei.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.fzhhl.top/gtcptuaeoh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.haohaochexian.top/gtpaimlwke.html

TS:   // 同上
来源：http://hz.zhoulong.xyz/gtmbcsaoiw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.xingfuxueyuan.xyz/gtchxdrqcz.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.gzhubu.top/gtdnyvsgki.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.daria6918.cn/gtcopujgch.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.nwbrower.top/gtmuouzxut.html

================================================================================
来源：http://hz.redwolf501.top/gttkxfxxsz.html

G. 面向对象
来源：http://hz.aibaodan.cn/gtnusbciqc.html

================================================================================
来源：http://hz.yuanzhike.top/gtjhbfvzcg.html

[G01] 定义类
来源：http://hz.kuanghao11.cn/gtdyirqsfd.html

Py:   class User: pass
来源：http://hz.shzxlz.cn/gtqjbwytut.html

PHP:  class User {}
来源：http://hz.ywan-chungtsiang.top/gtgtcyrlhp.html

JS:   class User {}
来源：http://hz.yanxiufei.cn/gtglbhzkki.html

TS:   class User { name: string = ""; }
来源：http://hz.tianlin.xyz/gtsbxgpuvn.html

Java: class User {}
来源：http://hz.ybcxt.top/gtdtwyrmtx.html

Go:   type User struct { Name string }
来源：http://hz.gzhubu.top/gtvomlyuzy.html

Ruby: class User; end
来源：http://hz.zhaomingkeji.xyz/gtgdgmxkcm.html

C#:   class User {}
来源：http://hz.jinyuanbaomall.cn/gtzpwrafqh.html

[G02] 构造函数
来源：http://hz.jinghuilouyu.cn/gttjqjiaah.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.sxryk.cn/gtjptcipxh.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yuxming.cn/gtvjsyzemd.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.nwbrower.top/gtmcuctuqn.html

TS:   constructor(public name: string) {}
来源：http://hz.aizwys.cn/gtrbgunfnn.html

Java: User(String name) { this.name = name; }
来源：http://hz.xingfuxueyuan.xyz/gtlavxncmd.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.jinqigfzy.top/gttjiwqefz.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.cheryme.top/gtfsvftdfo.html

C#:   public User(string name) { Name = name; }
来源：http://hz.ybcxt.top/gtisrzyfhb.html

[G03] 实例属性
来源：http://hz.pycfn.com/gtnokkycoh.html

Py:   self.name = "x"
来源：http://hz.yanxiufei.cn/gtuoqngdff.html

PHP:  public string $name = "x";
来源：http://hz.ybcxt.top/gtwjljgjuz.html

JS:   this.name = "x";
来源：http://hz.wangdashe.top/gtwlhbousc.html

TS:   name: string = "x";
来源：http://hz.jinyuanbaomall.cn/gtwacmjeqy.html

Java: private String name;
来源：http://hz.shangyingyoupin.top/gtgnjpryog.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jinqigfzy.top/gtqsbxucgw.html

Ruby: @name = "x"
来源：http://hz.cdnleiting.top/gtdsdazhlf.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.xingfuxueyuan.xyz/gttvicyouh.html

[G04] 定义方法
来源：http://hz.yj20258.top/gtjlokfiff.html

Py:   def greet(self): return self.name
来源：http://hz.c1oappe.top/gtezfeatag.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.mhx1999.top/gtfhvsdccu.html

JS:   greet() { return this.name; }
来源：http://hz.zhiwuduotai.top/gtjbumdonl.html

TS:   greet(): string { return this.name; }
来源：http://hz.ppjwa.cn/gtpjzunpzo.html

Java: String greet() { return name; }
来源：http://hz.xylfe.cn/gtzjrsendb.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ivvv.top/gtjleryswc.html

Ruby: def greet; @name; end
来源：http://hz.fengsongda.top/gtxgxtowgo.html

C#:   public string Greet() => Name;
来源：http://hz.shuidangran.top/gtqrehtrdl.html

[G05] 继承
来源：http://hz.shangyingyoupin.top/gtpxymmugz.html

Py:   class Admin(User): pass
来源：http://hz.vqdsnc.cn/gtiamfspis.html

PHP:  class Admin extends User {}
来源：http://hz.yanxiufei.cn/gttwaqtmpu.html

JS:   class Admin extends User {}
来源：http://hz.fengsongda.top/gtqnwqucuw.html

TS:   class Admin extends User {}
来源：http://hz.hammf.cn/gtvnlicxog.html

Java: class Admin extends User {}
来源：http://hz.xylfe.cn/gtwbzaiweq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.jianghu66.top/gtaxqctvzx.html

Ruby: class Admin < User; end
来源：http://hz.jlsjyb.cn/gtpsfwwhtb.html

C#:   class Admin : User {}
来源：http://hz.yj20258.top/gtgzmqnykx.html

[G06] 重写方法
来源：http://hz.pengpengdd.cyou/gtzqfqllpe.html

Py:   def greet(self): return "admin"
来源：http://hz.cucudq.cn/gteehtuffe.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.pycfn.com/gtfjlgakfd.html

JS:   greet() { return "admin"; }
来源：http://hz.52xcode.cn/gtygnsifop.html

TS:   greet(): string { return "admin"; }
来源：http://hz.bjfxy.top/gtmnirfuhj.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xuanzx.com/gtydzxmjzp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.chenlongwang.top/gtswbsebqf.html

Ruby: def greet; "admin"; end
来源：http://hz.hammf.cn/gtragbemlh.html

C#:   public override string Greet() => "admin";
来源：http://hz.hywenlv.cn/gtwmannclo.html

[G07] 调用父类方法
来源：http://hz.cashguo.top/gtumtcjkpx.html

Py:   super().greet()
来源：http://hz.yuxming.cn/gtpifknkbf.html

PHP:  parent::greet();
来源：http://hz.vqdsnc.cn/gtscqpmeww.html

JS:   super.greet();
来源：http://hz.zycfv.cn/gtuidsmpvk.html

TS:   super.greet();
来源：http://hz.redwolf501.top/gtajaghupl.html

Java: super.greet();
来源：http://hz.redwolf501.top/gtvtzeinvp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.wangshuangyany.cn/gtmktxbbpu.html

Ruby: super
来源：http://hz.shanyushiyangtech.top/gtippgchsi.html

C#:   base.Greet();
来源：http://hz.chenzaomai.com/gtuegtpdjv.html

[G08] 静态方法与属性
来源：http://hz.jianghu66.top/gtzffppfdq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jinqigufen.top/gtjehdubov.html

PHP:  public static function f() {}
来源：http://hz.xinyue.icu/gtajmnevgr.html

JS:   static f() {}
来源：http://hz.tanke756.top/gtrqgsnbew.html

TS:   static f(): void {}
来源：http://hz.hnxiangtu.top/gttdctxuku.html

Java: static void f() {}
来源：http://hz.pycfn.com/gtqbdgpnlw.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhoulong.xyz/gtirrbfbjj.html

Ruby: def self.f; end
来源：http://hz.zycfv.cn/gtszhkjccl.html

C#:   public static void F() {}
来源：http://hz.yuanzhike.top/gtdgpvzdfs.html

[G09] 接口 / 抽象类
来源：http://hz.zhixingplan.top/gtiokdewwv.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.wangdashe.top/gtggahnxke.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.tanke756.top/gtcdrcethe.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.hnxiangtu.top/gtlkvunfja.html

TS:   interface Shape { area(): number; }
来源：http://hz.fengsongda.top/gtoyufbfua.html

Java: interface Shape { double area(); }
来源：http://hz.pengpengdd.cyou/gtjlrnbkud.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zhoulong.xyz/gteljkzjsv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.hongshengwenyu.top/gtvdqxjnjv.html

C#:   interface IShape { double Area(); }
来源：http://hz.hongshengwenyu.top/gtkcxhknxr.html

[G10] 访问控制
来源：http://hz.zhaomingkeji.xyz/gtcgnrhief.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.mhx1999.top/gtkmrcmaeu.html

PHP:  public / protected / private
来源：http://hz.xylfe.cn/gturaeymkz.html

JS:   #private 字段；其余公开
来源：http://hz.zhoulong.xyz/gtcbixwioj.html

TS:   public / protected / private
来源：http://hz.zdqjudy.top/gtaoxosqpb.html

Java: public / protected / private / 默认包级
来源：http://hz.zhongyouzk.top/gtbxiutjfl.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.birdmap.top/gtcygcgaua.html

Ruby: public / protected / private
来源：http://hz.pycfn.com/gtrppqxbnt.html

C#:   public / protected / private / internal
来源：http://hz.ybcxt.top/gtpxkmmjnt.html

[G11] getter / setter
来源：http://hz.hnxiangtu.top/gtvaiuzxlc.html

Py:   @property 与 @x.setter
来源：http://hz.sweek.top/gtuniakycv.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yuxming.cn/gtrynpnjkn.html


<!-- 参考信息 -->