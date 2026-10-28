代发 wailian999

Py:   for ch in s: print(ch)
来源：http://hz.sxryk.cn/gtepalalbh.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.xylfe.cn/gtsptrkjap.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.jinqigfzy.top/gtxlpdyosq.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.redwolf501.top/gtgmxeflph.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.hongshengwenyu.top/gtpqdwhojr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jiagoushi.top/gtzmokirbd.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.hammf.cn/gtwjbgapvx.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.shanyushiyangkeji.top/gtuinbaiie.html

[E14] URL 编码与 Base64
来源：http://hz.hongshengwenyu.top/gtpbwxpgqb.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.gotoacloud.top/gtiloeqgkp.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.chenlongwang.top/gtsciawsaw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.hnqzz.top/gtobolrcse.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yanxiufei.cn/gtwedkdgsh.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jinqigfzy.top/gtiqmizvau.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.jinyuanbaomall.cn/gtdxfnponz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.jianghu66.top/gtkiclwwsn.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.chenlongwang.top/gtafhsumqk.html

[E15] HTML 转义 / 反转义
来源：http://hz.shuidangran.top/gtmxwpxfyj.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jqgfzy.top/gtflnijqsk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.andypj.xyz/gtgplwqxcp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.ydzc1.top/gtwipfeink.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.hysaishi.cn/gthdqhvgyx.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.sweek.top/gtisymemak.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.birdmap.top/gttarrkkrg.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.316326.xyz/gtefxdffzo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zycfv.cn/gtjiksdkdm.html

[E16] 数字千分位
来源：http://hz.tian-w.cn/gtkuurrrfv.html

Py:   f"{1234567:,}"
来源：http://hz.ivvv.top/gtykqbxpzt.html

PHP:  number_format(1234567);
来源：http://hz.feifeiyinyue.top/gtbljkkuor.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.9152youxi.cn/gttxoekfmv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhaomingkeji.xyz/gtvbzeruuu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jinqigfzy.top/gtizlsxjdd.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yj20258.top/gtrcrxiiww.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.svipenyu.cn/gtisvbmmat.html

C#:   1234567.ToString("N0")
来源：http://hz.iojbl.cn/gtlznxtiib.html

[E17] 首字母大写
来源：http://hz.nanxinkj.top/gtvnagorgi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.sxryk.cn/gtbkizcqza.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yonumen.top/gtjnsubrgm.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ppjwa.cn/gtjgtekzsw.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.birdmap.top/gtxsqvueyj.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.ywan-chungtsiang.top/gtmjhilemy.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yangfankeji.com/gtogswkpdh.html

Ruby: s.capitalize
来源：http://hz.daxiang520.top/gtfjffeubp.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jinghuilouyu.cn/gtnacsxxzs.html

[E18] 模板占位符替换
来源：http://hz.gogol.net.cn/gtilispzgc.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.hammf.cn/gtidbataab.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.yanxiufei.cn/gtxxhtxofo.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.dianchejie.cn/gtyqdhgpec.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.gogol.net.cn/gtnwnnpvjh.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jqgufenzy.top/gtzhhqxhim.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jyoumei.cn/gtdhyinnrf.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yvedp.cn/gthfzfwrql.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.smart0.xyz/gtdmjdhxdc.html

[E19] 多行文本按行拆分
来源：http://hz.kuanghao11.cn/gtuelbvbrz.html

Py:   s.splitlines()
来源：http://hz.smart0.xyz/gtsekqmahj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yanxiufei.cn/gthewddwhz.html

JS:   s.split(/\r?\n/)
来源：http://hz.xylfe.cn/gtgqmndlbr.html

TS:   s.split(/\r?\n/)
来源：http://hz.jyoumei.cn/gtefnnglpq.html

Java: s.lines().toList()
来源：http://hz.xuanzx.com/gtnoyslssd.html

Go:   strings.Split(s, "\n")
来源：http://hz.cheryme.top/gtcgnvvegw.html

Ruby: s.lines
来源：http://hz.daria6918.cn/gtphemqyvx.html

C#:   s.Split('\n')
来源：http://hz.jyoumei.cn/gtawrugvgg.html

[E20] 判断字符串是否为空
来源：http://hz.pycfn.com/gtkyhlstrg.html

Py:   if not s:
来源：http://hz.mhx1999.top/gtcevnkfpo.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jqgufenzy.top/gtepcvhnbl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jyoumei.cn/gtqsietmsw.html

TS:   if (s === "") {}
来源：http://hz.zdqjudy.top/gtrvfhlsbi.html

Java: if (s.isEmpty()) {}
来源：http://hz.nwbrower.top/gtwccdlalp.html

Go:   if s == "" {}
来源：http://hz.sxryk.cn/gtzwrpsxds.html

Ruby: if s.empty?
来源：http://hz.haohaochexian.top/gtcxzkywco.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.ydzc1.top/gtxclwyuxb.html

[E21] 超长截断加省略号
来源：http://hz.svipenyu.cn/gtbvbzalxz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.chenjidiqi.icu/gtqnljohok.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.xuetiantiany.cn/gtwkkksbcw.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.snrcjt.cn/gtuyffmckt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.chenjidiqi.icu/gthczmpdxe.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.iojbl.cn/gtstuwfggr.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yuanzhike.top/gthxwursbg.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.xylfe.cn/gtaovbehvr.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.yuxming.cn/gtloqecknr.html

[E22] 字节长度与字符长度
来源：http://hz.gaohongyu789.top/gtembnitpn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.cheryme.top/gtdvsbgszv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jqgfzy.top/gtunovbhrl.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jlsjyb.cn/gtmeuamsda.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jlsjyb.cn/gtxvatvbrz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.guannengcc.top/gtczwolzfu.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.hnqzz.top/gtjgyazwvp.html

Ruby: s.bytesize;  s.length
来源：http://hz.hongshengwenyu.top/gtpxzhglli.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.xziqi.cn/gtpiswjyby.html

================================================================================
来源：http://hz.yuxming.cn/gtcviyzvpg.html

F. 文件与目录
来源：http://hz.cheryme.top/gtvjeoqbty.html

================================================================================
来源：http://hz.ydjk.org.cn/gtbdcvtcfi.html

[F01] 读取整个文件
来源：http://hz.zhiwuduotai.top/gtdekdpdkr.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yongpay.top/gtbwtydkia.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jinghuilouyu.cn/gtzzmjstwz.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.jlsjyb.cn/gtrripuaea.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.cucudq.cn/gtgjaisyzr.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yj202588.top/gtaajbkvcj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.jqgfzy.top/gtwbbonluj.html

Ruby: File.read("a.txt")
来源：http://hz.vqdsnc.cn/gtlmabksbd.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yuanzhike.top/gtegnahwis.html

[F02] 逐行读取文件
来源：http://hz.zhiwuduotai.top/gtuvqzskjv.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zhoulong.xyz/gtekuuhwko.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.gzhubu.top/gtjasplnxe.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jinghuilouyu.cn/gtwbpepvwc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.wangshuangyany.cn/gttlxkiokv.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.haohaochexian.top/gtqwvaugak.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yvedp.cn/gtdyuzuceh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yonumen.top/gtengytvll.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.ywan-chungtsiang.top/gtrlxnlhfc.html

[F03] 写入文件（覆盖）
来源：http://hz.hnxiangtu.top/gtgycnlfvb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.nanxinkj.top/gtlcdqakpt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.sufxvd.cn/gtdwtyakrs.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.nwbrower.top/gtvgzjripo.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jyoumei.cn/gtamxkxcnn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.quarkkingdee.top/gtscfcmzkm.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.shanyushiyangtech.top/gtzygspdjw.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.chenjidiqi.icu/gtghhpbhri.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.sweek.top/gtdwbijpkv.html

[F04] 追加写入文件
来源：http://hz.shanyushiyangtech.top/gtzxffevnd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jinyuanbaomall.cn/gtvoxxktfj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.xylfe.cn/gtizjkfaxi.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhongyouzk.top/gtuqjcxzoe.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.jianghu66.top/gteunxrxxv.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.vqdsnc.cn/gtzlratmpg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zhongyouzk.top/gtukdlxnma.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zhijiandao.cn/gtkqjfptmi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.sufxvd.cn/gtzbvcyxxl.html

[F05] 判断文件或目录是否存在
来源：http://hz.cucudq.cn/gtmbomqmll.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.pycfn.com/gtwhklyogv.html

PHP:  file_exists("a.txt");
来源：http://hz.wangdashe.top/gtugofizsw.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yj20258888.top/gtdxhhhusz.html

TS:   fs.existsSync("a.txt")
来源：http://hz.hnxiangtu.top/gtgnapdzpk.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.daria6918.cn/gtwkwaavvh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.feifeiyinyue.top/gtprhzyqcy.html

Ruby: File.exist?("a.txt")
来源：http://hz.xylfe.cn/gteciybybq.html

C#:   File.Exists("a.txt")
来源：http://hz.smart0.xyz/gtpdvczonc.html

[F06] 删除文件
来源：http://hz.vqdsnc.cn/gteqsysave.html

Py:   os.remove("a.txt")
来源：http://hz.c1oappe.top/gtrzkscvjo.html

PHP:  unlink("a.txt");
来源：http://hz.yvedp.cn/gtshzmexwk.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yonumen.top/gtflwxacdy.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.chenlongwang.top/gtwqivexca.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.haohaochexian.top/gtstxykaox.html

Go:   os.Remove("a.txt")
来源：http://hz.aibaodan.cn/gtmxeksxnj.html

Ruby: File.delete("a.txt")
来源：http://hz.0kj1m.cn/gtjrtmpldd.html

C#:   File.Delete("a.txt");
来源：http://hz.pycfn.com/gtzyyjgmbw.html

[F07] 创建目录（含多级）
来源：http://hz.yj20258888.top/gtpkvgiykn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.cqqwz.cn/gtzojxqiio.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.xylfe.cn/gtrszmerlg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.nanxinkj.top/gtmrqfojip.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.pengpengdd.cyou/gtepbsuedb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yj20258.top/gtwadmhqky.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jqgufenzy.top/gtvhpkomme.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.birdmap.top/gtkbsykvsa.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.wangshuangyany.cn/gtwfciypgx.html

[F08] 遍历目录
来源：http://hz.svipenyu.cn/gtmlapdlyk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.cqqwz.cn/gtulmaxwvv.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.quarkkingdee.top/gtzdmpiypt.html

JS:   fs.readdirSync("dir")
来源：http://hz.shuidangran.top/gtswtafadf.html

TS:   fs.readdirSync("dir")
来源：http://hz.birdmap.top/gtbiviknoa.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.sufxvd.cn/gtmmdytmbl.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.ywan-chungtsiang.top/gtnlychqrk.html

Ruby: Dir.children("dir")
来源：http://hz.guannengcc.top/gtwaodshxt.html

C#:   Directory.GetFiles("dir")
来源：http://hz.fengsongda.top/gthnvxhiph.html

[F09] 获取文件大小
来源：http://hz.sysykeji.top/gtbunyhapf.html

Py:   os.path.getsize("a.txt")
来源：http://hz.sxryk.cn/gtchgzszej.html

PHP:  filesize("a.txt");
来源：http://hz.jqgufenzy.top/gtiwxofgdo.html

JS:   fs.statSync("a.txt").size
来源：http://hz.nanxinkj.top/gtmrrgsfhx.html

TS:   fs.statSync("a.txt").size
来源：http://hz.wangdashe.top/gttgihphjc.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.hysaishi.cn/gttgqztfjc.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.xuetiantiany.cn/gtbzjfqgnp.html

Ruby: File.size("a.txt")
来源：http://hz.jinghuilouyu.cn/gtakcbouwk.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yvedp.cn/gtcvwgoiez.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hnqzz.top/gtslxltvhw.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jinqigfzy.top/gtcmiedica.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.andypj.xyz/gttzmyizug.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jiagoushi.top/gtnwhoihfl.html

TS:   path.extname("a.txt")
来源：http://hz.dashuyun.cn/gtrshelpmu.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.shanyushiyangkeji.top/gtyyygwfwq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhoulong.xyz/gtmnwopnzv.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.mhx1999.top/gtuzclglpw.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.shanyushiyangkeji.top/gtrpuofdyi.html

[F11] 复制与移动文件
来源：http://hz.sxryk.cn/gtqlicujfr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.gaohongyu789.top/gtcxfspijz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.cdnleiting.top/gtntozbaxu.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.redwolf501.top/gtvsnfchnf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.9152youxi.cn/gtlgtgyxka.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.sweek.top/gtzvesszyl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.sweek.top/gtcykuuixr.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.chenjidiqi.icu/gtsovuordc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.zhijiandao.cn/gtujuozaza.html

[F12] CSV 读写
来源：http://hz.mhx1999.top/gtqjdhuhpc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.chenzaomai.com/gtxlvijhot.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yongpay.top/gtzqpkmkoj.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.dashuyun.cn/gtryqapqik.html

TS:   // 同上
来源：http://hz.hnqzz.top/gtinnmmjtw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.ybcxt.top/gtakcqxvae.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.zhixingplan.top/gtxbgyvmbq.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jyoumei.cn/gtfsfsvdlu.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.aibaodan.cn/gtdlrgvunm.html

================================================================================
来源：http://hz.0kj1m.cn/gtlclpjqnt.html

G. 面向对象
来源：http://hz.yangfankeji.com/gtkfpxlysj.html

================================================================================
来源：http://hz.daxiang520.top/gtjgtlyvuz.html

[G01] 定义类
来源：http://hz.yangfankeji.com/gtnkgzpdwr.html

Py:   class User: pass
来源：http://hz.jinqigfzy.top/gtqftfvxjo.html

PHP:  class User {}
来源：http://hz.cqqwz.cn/gttleenoaa.html

JS:   class User {}
来源：http://hz.birdmap.top/gtqznkxabr.html

TS:   class User { name: string = ""; }
来源：http://hz.xuetiantiany.cn/gtsmnkrcvy.html

Java: class User {}
来源：http://hz.shangyingyoupin.top/gtvwektyid.html

Go:   type User struct { Name string }
来源：http://hz.hywenlv.cn/gtkgqatqas.html

Ruby: class User; end
来源：http://hz.shzxlz.cn/gtznemocnc.html

C#:   class User {}
来源：http://hz.jyoumei.cn/gtkisfdtlv.html

[G02] 构造函数
来源：http://hz.zhixingplan.top/gtvolxhfik.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.gaohongyu789.top/gtwcdxojqd.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yueranfly.top/gtdsgbmwiv.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.316326.xyz/gtypkenxac.html

TS:   constructor(public name: string) {}
来源：http://hz.vqdsnc.cn/gtxabchjzb.html

Java: User(String name) { this.name = name; }
来源：http://hz.jlsjyb.cn/gtjphjuoys.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.nwbrower.top/gtjnmzuxjj.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.yuanzhike.top/gtixiocjdo.html

C#:   public User(string name) { Name = name; }
来源：http://hz.andypj.xyz/gtvuljswut.html

[G03] 实例属性
来源：http://hz.zhijiandao.cn/gttvhrzxzs.html

Py:   self.name = "x"
来源：http://hz.xinyue.icu/gtaceqnvtp.html

PHP:  public string $name = "x";
来源：http://hz.guannengcc.top/gtpqymcldo.html

JS:   this.name = "x";
来源：http://hz.birdmap.top/gtrhwrhutu.html

TS:   name: string = "x";
来源：http://hz.ywan-chungtsiang.top/gtmuibzsdw.html

Java: private String name;
来源：http://hz.ivvv.top/gtiajxlnrj.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.smart0.xyz/gtzwvifejn.html

Ruby: @name = "x"
来源：http://hz.0kj1m.cn/gtfcljuvat.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.hammf.cn/gtcbshalbl.html

[G04] 定义方法
来源：http://hz.daria6918.cn/gtpdyqqnrv.html

Py:   def greet(self): return self.name
来源：http://hz.chenjidiqi.icu/gtpeguxqtq.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.shzxlz.cn/gtfaftqfqe.html

JS:   greet() { return this.name; }
来源：http://hz.shzxlz.cn/gtuickrjke.html

TS:   greet(): string { return this.name; }
来源：http://hz.hywenlv.cn/gtneruxtra.html

Java: String greet() { return name; }
来源：http://hz.zhoulong.xyz/gtrljgavky.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.andypj.xyz/gtjnkdolmn.html

Ruby: def greet; @name; end
来源：http://hz.yangfankeji.com/gtskhiyvja.html

C#:   public string Greet() => Name;
来源：http://hz.nanxuanxn.top/gtkgfqydaw.html

[G05] 继承
来源：http://hz.zhiwuduotai.top/gttuqmehbq.html

Py:   class Admin(User): pass
来源：http://hz.zhiwuduotai.top/gtjtrvaqzo.html

PHP:  class Admin extends User {}
来源：http://hz.sysykeji.top/gtxfiedjaj.html

JS:   class Admin extends User {}
来源：http://hz.yangfankeji.com/gtfdgihcnj.html

TS:   class Admin extends User {}
来源：http://hz.zycfv.cn/gtwkiarvvx.html

Java: class Admin extends User {}
来源：http://hz.c1oappe.top/gtdbwwpuso.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.snrcjt.cn/gtcusrkvkw.html

Ruby: class Admin < User; end
来源：http://hz.zhoulong.xyz/gtptghdegt.html

C#:   class Admin : User {}
来源：http://hz.xingfuxueyuan.xyz/gtxlszbdmo.html

[G06] 重写方法
来源：http://hz.aizwys.cn/gtrzizqurs.html

Py:   def greet(self): return "admin"
来源：http://hz.0kj1m.cn/gtldslfbmj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.snrcjt.cn/gtjxlvbhyx.html

JS:   greet() { return "admin"; }
来源：http://hz.ehwqpu.com/gtdyxgsotb.html

TS:   greet(): string { return "admin"; }
来源：http://hz.cashguo.top/gtyeqbzcfi.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhengqikj.top/gtddqcptjc.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.andypj.xyz/gtpbgwwbyd.html

Ruby: def greet; "admin"; end
来源：http://hz.sxryk.cn/gtfjleiych.html

C#:   public override string Greet() => "admin";
来源：http://hz.xylfe.cn/gtjdpoaoer.html

[G07] 调用父类方法
来源：http://hz.kuanghao11.cn/gtkyxumjaz.html

Py:   super().greet()
来源：http://hz.bjfxy.top/gtzddztxsi.html

PHP:  parent::greet();
来源：http://hz.cashguo.top/gtvosvihmp.html

JS:   super.greet();
来源：http://hz.tian-w.cn/gtsdalxsbz.html

TS:   super.greet();
来源：http://hz.zycfv.cn/gtztefcpdo.html

Java: super.greet();
来源：http://hz.bjfxy.top/gtvkdxwzdx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.nanxinkj.top/gtwlcfduzw.html

Ruby: super
来源：http://hz.shanyushiyangkeji.top/gtvwzjequr.html

C#:   base.Greet();
来源：http://hz.hnxiangtu.top/gtlvazotxn.html

[G08] 静态方法与属性
来源：http://hz.tanke756.top/gtynmsqaze.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jqgufenzy.top/gttmahuzuu.html

PHP:  public static function f() {}
来源：http://hz.iojbl.cn/gtaoupcysj.html

JS:   static f() {}
来源：http://hz.xylfe.cn/gtbejjjlco.html

TS:   static f(): void {}
来源：http://hz.xuanzx.com/gtpxpgysep.html

Java: static void f() {}
来源：http://hz.zhengqikj.top/gtkoyhybzn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.0kj1m.cn/gtdcgtocxu.html

Ruby: def self.f; end
来源：http://hz.jqgfzy.top/gtofetptgy.html

C#:   public static void F() {}
来源：http://hz.zhaomingkeji.xyz/gtrvtliutv.html

[G09] 接口 / 抽象类
来源：http://hz.iojbl.cn/gtcvusazjr.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.chenzaomai.com/gtzfhqmswr.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.sxryk.cn/gtidamhkyn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.pengpengdd.cyou/gtlsgirsvi.html

TS:   interface Shape { area(): number; }
来源：http://hz.52xcode.cn/gttpbyjolo.html

Java: interface Shape { double area(); }
来源：http://hz.xziqi.cn/gtcsclgibl.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.sufxvd.cn/gtgotymahe.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zhaomingkeji.xyz/gtetxppyvt.html

C#:   interface IShape { double Area(); }
来源：http://hz.dianchejie.cn/gtyqcmjefu.html

[G10] 访问控制
来源：http://hz.yuxming.cn/gtykulnvpm.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhijiandao.cn/gtqqxvzelt.html

PHP:  public / protected / private
来源：http://hz.nanxinkj.top/gturacvtgr.html

JS:   #private 字段；其余公开
来源：http://hz.yangfankeji.com/gtqeojvyla.html

TS:   public / protected / private
来源：http://hz.yj20258888.top/gtfrvlyath.html

Java: public / protected / private / 默认包级
来源：http://hz.shanyushiyangtech.top/gtmbylvqbr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.sufxvd.cn/gtcsyqfkly.html

Ruby: public / protected / private
来源：http://hz.hysaishi.cn/gtyecvicvo.html

C#:   public / protected / private / internal
来源：http://hz.yj20258888.top/gtggtwepbg.html

[G11] getter / setter
来源：http://hz.shanyushiyangkeji.top/gtvdvkddgd.html

Py:   @property 与 @x.setter
来源：http://hz.ehwqpu.com/gtllgvgopm.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.cdnleiting.top/gtsoxsmomg.html

JS:   get name() { return this._name; }
来源：http://hz.nanxinkj.top/gtvgokvfda.html

TS:   get name(): string { return this._name; }
来源：http://hz.ybcxt.top/gtjzajtbtb.html

Java: public String getName() { return name; }
来源：http://hz.hywenlv.cn/gtbdhfqlyz.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zhoulong.xyz/gtuctjsbvc.html


<!-- 参考信息 -->