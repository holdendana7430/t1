代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.hongshengwenyu.top/gttwgfdphx.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.jqgufenzy.top/gtjmdtcqal.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.yj20258888.top/gtcwffzgqh.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.chenzaomai.com/gtzqgckpez.html

[E14] URL 编码与 Base64
来源：http://hz.gogol.net.cn/gtumwrmqxv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.cdnleiting.top/gtmxzijpig.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.gzhubu.top/gtndsapdbu.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.tianlin.xyz/gtwfnfqjvt.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.xziqi.cn/gtwvfvdpse.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yj20258888.top/gtfsmqkomf.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.wangdashe.top/gtxdxvftgq.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.xinyue.icu/gtceticsyy.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.sxryk.cn/gthezphjil.html

[E15] HTML 转义 / 反转义
来源：http://hz.chenzaomai.com/gtztrneroq.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jinghuilouyu.cn/gtkcsiybpk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.yuanzhike.top/gtvbpjjcwe.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yueranfly.top/gtonousgkl.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.xziqi.cn/gtqlpcwqkt.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yuxming.cn/gtngiyqnry.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.xingfuxueyuan.xyz/gtijtxmfqo.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.birdmap.top/gtaqktwvja.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jyoumei.cn/gtgabxnwvs.html

[E16] 数字千分位
来源：http://hz.316326.xyz/gtaupvcfgy.html

Py:   f"{1234567:,}"
来源：http://hz.0kj1m.cn/gtuzajqyke.html

PHP:  number_format(1234567);
来源：http://hz.xziqi.cn/gtpnqocstx.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.cucudq.cn/gtbeskittx.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.cdnleiting.top/gtwedwmodm.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yueranfly.top/gtmkuxhavk.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.dianchejie.cn/gtvtekcqkm.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yj20258.top/gtwovccorv.html

C#:   1234567.ToString("N0")
来源：http://hz.birdmap.top/gtvwdnnfip.html

[E17] 首字母大写
来源：http://hz.feifeiyinyue.top/gtpmgxlexa.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.chenzaomai.com/gtagnbwoso.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.tian-w.cn/gtgdtfcufz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.9152youxi.cn/gtazwhxgyn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.daxiang520.top/gttohoksfq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.ydzc1.top/gtrnaktcde.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.xinyue.icu/gtltqcmcpn.html

Ruby: s.capitalize
来源：http://hz.zhengqikj.top/gtwsunxaii.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.haohaochexian.top/gtdgohjjmt.html

[E18] 模板占位符替换
来源：http://hz.316326.xyz/gtubpaezjp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.hfpthk.cn/gtwfhrberw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.jqgfzy.top/gtiornxefv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.svipenyu.cn/gtjhsfcace.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.ywan-chungtsiang.top/gtxoziritc.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yuanzhike.top/gtnygeltib.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.tianlin.xyz/gtzbyekcas.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yuxming.cn/gtupwwbvpm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jinqigufen.top/gtjenrclbb.html

[E19] 多行文本按行拆分
来源：http://hz.zycfv.cn/gtypnonycy.html

Py:   s.splitlines()
来源：http://hz.sysykeji.top/gtneqzihjf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.jianghu66.top/gtjnvhgoqq.html

JS:   s.split(/\r?\n/)
来源：http://hz.feifeiyinyue.top/gtotkpxzqq.html

TS:   s.split(/\r?\n/)
来源：http://hz.tianlin.xyz/gtdwyohzli.html

Java: s.lines().toList()
来源：http://hz.xziqi.cn/gtrndrhprx.html

Go:   strings.Split(s, "\n")
来源：http://hz.xuetiantiany.cn/gtgentpwnk.html

Ruby: s.lines
来源：http://hz.jiagoushi.top/gthyamgiqp.html

C#:   s.Split('\n')
来源：http://hz.zhongyouzk.top/gtbmhgdlro.html

[E20] 判断字符串是否为空
来源：http://hz.0kj1m.cn/gtllmqrith.html

Py:   if not s:
来源：http://hz.zhixingplan.top/gtacukftds.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yj20258888.top/gtuqisgzxd.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.gotoacloud.top/gtqyynmvga.html

TS:   if (s === "") {}
来源：http://hz.daxiang520.top/gtztfxvykz.html

Java: if (s.isEmpty()) {}
来源：http://hz.zhixingplan.top/gtmdpsvedq.html

Go:   if s == "" {}
来源：http://hz.xingfuxueyuan.xyz/gtraxzhryo.html

Ruby: if s.empty?
来源：http://hz.tianlin.xyz/gtvmyxlfes.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.yonumen.top/gttquyuole.html

[E21] 超长截断加省略号
来源：http://hz.pengpengdd.cyou/gttwyrheqd.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.cucudq.cn/gtjhbamtnb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.jqgfzy.top/gtlgwelijv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhoulong.xyz/gtgoueafyt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.iojbl.cn/gtsaertuyr.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.9152youxi.cn/gtsdzvjjlx.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.jinqigfzy.top/gtkurhkopz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jqgfzy.top/gtipmtrebl.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.hnqzz.top/gtspcggqge.html

[E22] 字节长度与字符长度
来源：http://hz.shuidangran.top/gtpdtwlkas.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.dashuyun.cn/gtayizkckd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yangfankeji.com/gtjorzyqys.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xziqi.cn/gtvjaugeav.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jianghu66.top/gtkzxpyeua.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jinqigufen.top/gtlkgxsaaa.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yuanzhike.top/gtefwwicqy.html

Ruby: s.bytesize;  s.length
来源：http://hz.yj202588.top/gtrmxdmrpm.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.zhengqikj.top/gtatjeenvd.html

================================================================================
来源：http://hz.tianlin.xyz/gtxwurqnqd.html

F. 文件与目录
来源：http://hz.wangdashe.top/gtlvhoykte.html

================================================================================
来源：http://hz.yj20258888.top/gtforomosm.html

[F01] 读取整个文件
来源：http://hz.hnqzz.top/gtuyhquysn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.xuetiantiany.cn/gtxvdnnuvc.html

PHP:  file_get_contents("a.txt");
来源：http://hz.bjfxy.top/gthknohrwr.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.mhx1999.top/gtmxwyqmxm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yuxming.cn/gtghsnlqqy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.c1oappe.top/gtduhkpeuv.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhoulong.xyz/gtszmiodma.html

Ruby: File.read("a.txt")
来源：http://hz.nwbrower.top/gtqvyrcfah.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.dianchejie.cn/gtkdcmacxr.html

[F02] 逐行读取文件
来源：http://hz.nanxuanxn.top/gtmyynimwy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jinghuilouyu.cn/gtpewjhige.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.gaohongyu789.top/gtrlyntgng.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.shuidangran.top/gtdutfdgkg.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zdqjudy.top/gtruxrvfbo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.feifeiyinyue.top/gtimdyujmt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.birdmap.top/gtloalaukk.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.sxryk.cn/gttyudvyzg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.316326.xyz/gtsmosusqa.html

[F03] 写入文件（覆盖）
来源：http://hz.nanxuanxn.top/gtagohhkoy.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hnxiangtu.top/gtjsmkgtmy.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.shuidangran.top/gtbioqtzjx.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ywan-chungtsiang.top/gtjwiyyizn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shuidangran.top/gteormfotg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.yj202588.top/gtxeuhmutt.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zhixingplan.top/gtosptrtrl.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.cashguo.top/gtavmslhpp.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.cucudq.cn/gtmotvejkv.html

[F04] 追加写入文件
来源：http://hz.yuxming.cn/gtnryoxgdl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.cashguo.top/gtnkjmcwrp.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.daxiang520.top/gtglybmqxa.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xinyue.icu/gtdpcfkbqy.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.yonumen.top/gtyydqvmng.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.yuxming.cn/gtwwyhmirt.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.hongshengwenyu.top/gtptvxtpna.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yangfankeji.com/gtcqcmdogq.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.sufxvd.cn/gttdegbbti.html

[F05] 判断文件或目录是否存在
来源：http://hz.wangdashe.top/gtgfogzwvt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.shuidangran.top/gtzughdcfh.html

PHP:  file_exists("a.txt");
来源：http://hz.zhengqikj.top/gtwgprojyi.html

JS:   fs.existsSync("a.txt")
来源：http://hz.sweek.top/gtxtysukwi.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yuanzhike.top/gtuspixzwe.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zycfv.cn/gtmwxpwkmn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jiagoushi.top/gtidouqoqk.html

Ruby: File.exist?("a.txt")
来源：http://hz.9152youxi.cn/gtfieduevu.html

C#:   File.Exists("a.txt")
来源：http://hz.cucudq.cn/gtaryapftu.html

[F06] 删除文件
来源：http://hz.nanxinkj.top/gtovbaqamy.html

Py:   os.remove("a.txt")
来源：http://hz.meibo888.top/gtvjsbioym.html

PHP:  unlink("a.txt");
来源：http://hz.shanyushiyangkeji.top/gtpwbwwcpf.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.svipenyu.cn/gtwjhlddgp.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.c1oappe.top/gtoqsgkyoy.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.smart0.xyz/gtbfhuebsu.html

Go:   os.Remove("a.txt")
来源：http://hz.vqdsnc.cn/gtuvforlzq.html

Ruby: File.delete("a.txt")
来源：http://hz.yanxiufei.cn/gtlnglvqgp.html

C#:   File.Delete("a.txt");
来源：http://hz.yueranfly.top/gtozklfpql.html

[F07] 创建目录（含多级）
来源：http://hz.jqgufenzy.top/gtjtafueaq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.gotoacloud.top/gtavigrrlp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.ivvv.top/gtpnkbxchz.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xinyue.icu/gtfuyuzbgo.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhixingplan.top/gtqodrysvq.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.guowangkeji.top/gtqfbgowuq.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hnxiangtu.top/gtxnbomrni.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.chenlongwang.top/gtyrcbtfpz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yuxming.cn/gtluvrbskf.html

[F08] 遍历目录
来源：http://hz.jqgufenzy.top/gtjlqpfmzf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jlsjyb.cn/gtthgggqjp.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.shangyingyoupin.top/gtianklmil.html

JS:   fs.readdirSync("dir")
来源：http://hz.gaohongyu789.top/gtojnoafea.html

TS:   fs.readdirSync("dir")
来源：http://hz.quarkkingdee.top/gtifwnjrzr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jlsjyb.cn/gtfzrbscjz.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.xziqi.cn/gtlscgtnft.html

Ruby: Dir.children("dir")
来源：http://hz.nanxinkj.top/gtbclofpca.html

C#:   Directory.GetFiles("dir")
来源：http://hz.nwbrower.top/gtqusjqdgi.html

[F09] 获取文件大小
来源：http://hz.daxiang520.top/gtgeyyojrv.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yongpay.top/gtiyeydoxd.html

PHP:  filesize("a.txt");
来源：http://hz.wangdashe.top/gtymkctiqj.html

JS:   fs.statSync("a.txt").size
来源：http://hz.pycfn.com/gtirtyaxcf.html

TS:   fs.statSync("a.txt").size
来源：http://hz.cheryme.top/gtbfdizbbq.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.tanke756.top/gtdtuojfns.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hfpthk.cn/gtqapgelbo.html

Ruby: File.size("a.txt")
来源：http://hz.vqdsnc.cn/gtucuodtzo.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.vqdsnc.cn/gtlaayloub.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hfpthk.cn/gtaqafzhms.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.tanke756.top/gtpmmecfwp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.pengpengdd.cyou/gtynvkasnh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.xinyue.icu/gtjtomzxhx.html

TS:   path.extname("a.txt")
来源：http://hz.yanxiufei.cn/gtgedobkqf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.dianchejie.cn/gtwimpwhai.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtmfoisqlg.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.cdnleiting.top/gtgnooeohq.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.pengpengdd.cyou/gtwycqueab.html

[F11] 复制与移动文件
来源：http://hz.shangyingyoupin.top/gtdcqeajxt.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.gogol.net.cn/gtqtmoyctx.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yvedp.cn/gtruzbjamr.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shanyushiyangkeji.top/gtlmhtmuav.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.vqdsnc.cn/gtbfubtove.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.tian-w.cn/gtkgudvckb.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hammf.cn/gtzayzkgri.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.yangfankeji.com/gtlyuyixdl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.chenjidiqi.icu/gteqvnvhbc.html

[F12] CSV 读写
来源：http://hz.kuanghao11.cn/gtklakojgz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.yj202588.top/gtycweqtcl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yonumen.top/gtfmgadtge.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jqgufenzy.top/gtxpqdwthw.html

TS:   // 同上
来源：http://hz.yuxming.cn/gtcdkmcbko.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.shanyushiyangkeji.top/gtikwbcfpd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.nwbrower.top/gtdjtbkkjp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ehwqpu.com/gtsplgbhhq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.haohaochexian.top/gtbtrajqrq.html

================================================================================
来源：http://hz.ivvv.top/gtxshhlfrw.html

G. 面向对象
来源：http://hz.c1oappe.top/gthbotjmbp.html

================================================================================
来源：http://hz.shzxlz.cn/gtwgaricue.html

[G01] 定义类
来源：http://hz.ydjk.org.cn/gtkjcypvrg.html

Py:   class User: pass
来源：http://hz.yj202588.top/gtofdypeiy.html

PHP:  class User {}
来源：http://hz.xingfuxueyuan.xyz/gtbfjxlhnv.html

JS:   class User {}
来源：http://hz.yueranfly.top/gtdowtjutm.html

TS:   class User { name: string = ""; }
来源：http://hz.zycfv.cn/gthvhimmvf.html

Java: class User {}
来源：http://hz.snrcjt.cn/gttzujftmr.html

Go:   type User struct { Name string }
来源：http://hz.redwolf501.top/gtvwjwqmcu.html

Ruby: class User; end
来源：http://hz.fengsongda.top/gtslenfxhr.html

C#:   class User {}
来源：http://hz.zdqjudy.top/gtkerdhqoi.html

[G02] 构造函数
来源：http://hz.hnqzz.top/gtfdeozzsz.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.xingfuxueyuan.xyz/gtpthduclj.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.yj202588.top/gtsvnnvgrw.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xziqi.cn/gtdlmtwmfj.html

TS:   constructor(public name: string) {}
来源：http://hz.ppjwa.cn/gtmgdheccl.html

Java: User(String name) { this.name = name; }
来源：http://hz.birdmap.top/gtrgvycvxs.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.sysykeji.top/gtbwmftwjg.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.shuidangran.top/gtkusgwpqm.html

C#:   public User(string name) { Name = name; }
来源：http://hz.tianlin.xyz/gtzziwoamf.html

[G03] 实例属性
来源：http://hz.yangfankeji.com/gtwasxcabc.html

Py:   self.name = "x"
来源：http://hz.zycfv.cn/gtjwqhbsuv.html

PHP:  public string $name = "x";
来源：http://hz.shanyushiyangkeji.top/gthnlhwrkm.html

JS:   this.name = "x";
来源：http://hz.sysykeji.top/gtgehlclog.html

TS:   name: string = "x";
来源：http://hz.guannengcc.top/gtgpbpjsng.html

Java: private String name;
来源：http://hz.vqdsnc.cn/gtrsynsrrb.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yongpay.top/gtotybjfef.html

Ruby: @name = "x"
来源：http://hz.jqgfzy.top/gtyerwkhnw.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.9152youxi.cn/gtkwgswmvj.html

[G04] 定义方法
来源：http://hz.andypj.xyz/gtykjpnvvp.html

Py:   def greet(self): return self.name
来源：http://hz.dashuyun.cn/gtovitpwqf.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.yj20258888.top/gtbycsqnvh.html

JS:   greet() { return this.name; }
来源：http://hz.xylfe.cn/gthdrqgsko.html

TS:   greet(): string { return this.name; }
来源：http://hz.xinyue.icu/gtokvzkdwd.html

Java: String greet() { return name; }
来源：http://hz.sxryk.cn/gtotdeclkd.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.c1oappe.top/gtjkpwvpbh.html

Ruby: def greet; @name; end
来源：http://hz.xuanzx.com/gtoyekubsy.html

C#:   public string Greet() => Name;
来源：http://hz.dianchejie.cn/gtmmrxmwdd.html

[G05] 继承
来源：http://hz.yvedp.cn/gtniguocmt.html

Py:   class Admin(User): pass
来源：http://hz.redwolf501.top/gtdtwojiam.html

PHP:  class Admin extends User {}
来源：http://hz.guannengcc.top/gtqrylgybt.html

JS:   class Admin extends User {}
来源：http://hz.gogol.net.cn/gtnsfmrhxp.html

TS:   class Admin extends User {}
来源：http://hz.shuidangran.top/gtfkuxpyfa.html

Java: class Admin extends User {}
来源：http://hz.zhijiandao.cn/gthuqtelzj.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.andypj.xyz/gteugikgrd.html

Ruby: class Admin < User; end
来源：http://hz.kuanghao11.cn/gtcnujuaju.html

C#:   class Admin : User {}
来源：http://hz.jinyuanbaomall.cn/gtlizwfwsx.html

[G06] 重写方法
来源：http://hz.chenjidiqi.icu/gteuywyypz.html

Py:   def greet(self): return "admin"
来源：http://hz.sufxvd.cn/gtwqfehjkq.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yj20258.top/gtsxsuotec.html

JS:   greet() { return "admin"; }
来源：http://hz.pengpengdd.cyou/gthzhgujtw.html

TS:   greet(): string { return "admin"; }
来源：http://hz.tian-w.cn/gtrznaafqp.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.fengsongda.top/gtwarjaxos.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.9152youxi.cn/gtgobskutf.html

Ruby: def greet; "admin"; end
来源：http://hz.pycfn.com/gtwwmmiuvx.html

C#:   public override string Greet() => "admin";
来源：http://hz.hnxiangtu.top/gtbnaupafy.html

[G07] 调用父类方法
来源：http://hz.meibo888.top/gtntnsdbtp.html

Py:   super().greet()
来源：http://hz.nanxuanxn.top/gtjgbsctpa.html

PHP:  parent::greet();
来源：http://hz.ydjk.org.cn/gthfewdayn.html

JS:   super.greet();
来源：http://hz.9152youxi.cn/gtgnsuioni.html

TS:   super.greet();
来源：http://hz.yj20258888.top/gtisbfcaqa.html

Java: super.greet();
来源：http://hz.jinqigfzy.top/gtkaajeyxr.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.sxryk.cn/gtqerjooxc.html

Ruby: super
来源：http://hz.ydjk.org.cn/gtmarwczkl.html

C#:   base.Greet();
来源：http://hz.cucudq.cn/gttsoowfnq.html

[G08] 静态方法与属性
来源：http://hz.ydjk.org.cn/gtnqmrxrdd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.cashguo.top/gtycrdaphl.html

PHP:  public static function f() {}
来源：http://hz.ppjwa.cn/gtlllxrclg.html

JS:   static f() {}
来源：http://hz.hongshengwenyu.top/gtknybuswk.html

TS:   static f(): void {}
来源：http://hz.quarkkingdee.top/gtgclkwxkt.html

Java: static void f() {}
来源：http://hz.ywan-chungtsiang.top/gtjakmjxrz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhongyouzk.top/gthswpwmvt.html

Ruby: def self.f; end
来源：http://hz.zhixingplan.top/gtgvnvvhmg.html

C#:   public static void F() {}
来源：http://hz.bjfxy.top/gtitcsxbnl.html

[G09] 接口 / 抽象类
来源：http://hz.xuetiantiany.cn/gtqeesfvmv.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.guowangkeji.top/gtibbbdczj.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.snrcjt.cn/gtigdnrkoj.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jinqigufen.top/gtwvrpgxea.html

TS:   interface Shape { area(): number; }
来源：http://hz.nanxuanxn.top/gtbxwhlsql.html

Java: interface Shape { double area(); }
来源：http://hz.snrcjt.cn/gtuqrdbdxr.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.sweek.top/gthvcjbcav.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.xziqi.cn/gtkwovhjpi.html

C#:   interface IShape { double Area(); }
来源：http://hz.pengpengdd.cyou/gtwqfaqqhj.html

[G10] 访问控制
来源：http://hz.daria6918.cn/gtrxpvxcov.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jlsjyb.cn/gtvrmtckez.html

PHP:  public / protected / private
来源：http://hz.daxiang520.top/gtbdolsyve.html

JS:   #private 字段；其余公开
来源：http://hz.ydzc1.top/gtdxmpyfgq.html

TS:   public / protected / private
来源：http://hz.zhongyouzk.top/gtfseesyfi.html

Java: public / protected / private / 默认包级
来源：http://hz.jinqigufen.top/gtzgynhkiz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.jlsjyb.cn/gtdwkkskgu.html

Ruby: public / protected / private
来源：http://hz.hammf.cn/gthmvvsunb.html

C#:   public / protected / private / internal
来源：http://hz.tian-w.cn/gtkpcxmbcm.html

[G11] getter / setter
来源：http://hz.aizwys.cn/gtvebatnbh.html

Py:   @property 与 @x.setter
来源：http://hz.zhoulong.xyz/gtrsyjvjbl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.aibaodan.cn/gtasktpnaw.html

JS:   get name() { return this._name; }
来源：http://hz.cheryme.top/gtkfqzysgd.html

TS:   get name(): string { return this._name; }
来源：http://hz.xingfuxueyuan.xyz/gtmuzssemq.html

Java: public String getName() { return name; }
来源：http://hz.cqqwz.cn/gtdiexmqae.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jyoumei.cn/gtmloczvcu.html

Ruby: attr_accessor :name
来源：http://hz.zhixingplan.top/gtfhrncqtg.html

C#:   public string Name { get; set; }
来源：http://hz.gzhubu.top/gtjkjjzmgu.html

[G12] 对象转字符串
来源：http://hz.xuanzx.com/gtlsfjddxd.html

Py:   def __str__(self): return self.name
来源：http://hz.aibaodan.cn/gteuijilyp.html


<!-- 参考信息 -->