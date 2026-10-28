代发 wailian999

Go:   strings.Count(s, "a")
来源：http://hz.vqdsnc.cn/gtfxbndytw.html

Ruby: s.count("a")
来源：http://hz.tian-w.cn/gtibegbndn.html

C#:   s.Count(c => c == 'a')
来源：http://hz.zhiwuduotai.top/gtqgwneqvz.html

[E13] 逐字符遍历
来源：http://hz.jinyuanbaomall.cn/gtpyzrlvhk.html

Py:   for ch in s: print(ch)
来源：http://hz.guowangkeji.top/gthlauavkl.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.zhongyouzk.top/gtpaotrsht.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.xziqi.cn/gtgztbvjxi.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yangfankeji.com/gtkcasfvhz.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.zycfv.cn/gtxxodcuzw.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.ybcxt.top/gtwmwacgzj.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.cashguo.top/gtmgwggjca.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.cashguo.top/gtiplqaaby.html

[E14] URL 编码与 Base64
来源：http://hz.hfpthk.cn/gtbcznmako.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.aizwys.cn/gthvbmaovm.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.dashuyun.cn/gtdxhvutrw.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yanxiufei.cn/gtvrdcuqrt.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.zhongyouzk.top/gtozmrexou.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.yongpay.top/gttcznvbiw.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yongpay.top/gttibscedj.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.feifeiyinyue.top/gtdgmxyscu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.daxiang520.top/gtroehcuec.html

[E15] HTML 转义 / 反转义
来源：http://hz.zhixingplan.top/gtsagyiqpz.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.xingfuxueyuan.xyz/gtutpsdmtw.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.xuanzx.com/gtvpiaucdg.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.wangdashe.top/gtxkrmwlvi.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.svipenyu.cn/gtzsahstck.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.ybcxt.top/gtgnlpczfs.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.hongshengwenyu.top/gtlvfbcyty.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.52xcode.cn/gtnprhygqo.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.smart0.xyz/gtealpfyhg.html

[E16] 数字千分位
来源：http://hz.c1oappe.top/gtaogquqpy.html

Py:   f"{1234567:,}"
来源：http://hz.c1oappe.top/gtodqruiiz.html

PHP:  number_format(1234567);
来源：http://hz.hfpthk.cn/gtovxhxhmi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.daria6918.cn/gtrygfrnjd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.daxiang520.top/gtjzrixgey.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.daxiang520.top/gtzyizvpjr.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jianghu66.top/gtrubyeowy.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.smart0.xyz/gttnwrvvmm.html

C#:   1234567.ToString("N0")
来源：http://hz.jinqigfzy.top/gtxiogzkaz.html

[E17] 首字母大写
来源：http://hz.hfpthk.cn/gtahzkhdyy.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.sweek.top/gtpylhijdu.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.mhx1999.top/gtaxzmcuis.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cucudq.cn/gtqthmsrcr.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.xziqi.cn/gtmagoeuvk.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.daria6918.cn/gtnqwadgdo.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.dashuyun.cn/gtgbpjlzyg.html

Ruby: s.capitalize
来源：http://hz.xuanzx.com/gtxxfqgoyu.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.dashuyun.cn/gtlwzzsdfp.html

[E18] 模板占位符替换
来源：http://hz.zdqjudy.top/gtmtromkeg.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.ydjk.org.cn/gttzaljrhx.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.hnxiangtu.top/gttechfwhd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.gaohongyu789.top/gtsdqtrqjm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinghuilouyu.cn/gtivgwbdog.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.yj202588.top/gtfdambjmx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yueranfly.top/gtsbfzswpx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zhaomingkeji.xyz/gtrkegasmj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zhaomingkeji.xyz/gttekdpqjy.html

[E19] 多行文本按行拆分
来源：http://hz.ehwqpu.com/gtjzsrrpqh.html

Py:   s.splitlines()
来源：http://hz.xingfuxueyuan.xyz/gtiblzeeuf.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.pengpengdd.cyou/gtypcvpjqk.html

JS:   s.split(/\r?\n/)
来源：http://hz.ydzc1.top/gthjpocueo.html

TS:   s.split(/\r?\n/)
来源：http://hz.zhongyouzk.top/gtkiiiiwlq.html

Java: s.lines().toList()
来源：http://hz.gogol.net.cn/gtuwfbneqn.html

Go:   strings.Split(s, "\n")
来源：http://hz.xziqi.cn/gtfjschswj.html

Ruby: s.lines
来源：http://hz.cheryme.top/gtochrpllg.html

C#:   s.Split('\n')
来源：http://hz.nwbrower.top/gtvahbfvtq.html

[E20] 判断字符串是否为空
来源：http://hz.yuanzhike.top/gtlbxdamxz.html

Py:   if not s:
来源：http://hz.shanyushiyangtech.top/gtnsnhhmjh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.svipenyu.cn/gtyytgpnjo.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.xuetiantiany.cn/gturiyhwvz.html

TS:   if (s === "") {}
来源：http://hz.shanyushiyangkeji.top/gtixndptdw.html

Java: if (s.isEmpty()) {}
来源：http://hz.gotoacloud.top/gtoniwylug.html

Go:   if s == "" {}
来源：http://hz.shanyushiyangkeji.top/gtzvrlmekc.html

Ruby: if s.empty?
来源：http://hz.yj202588.top/gtronixlyo.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.birdmap.top/gtjhwjnifb.html

[E21] 超长截断加省略号
来源：http://hz.yj20258888.top/gtalqhbfky.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.ppjwa.cn/gtgjruovvo.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.fzhhl.top/gtymyxnqst.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jqgufenzy.top/gttesfmtsn.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.havefunace.top/gtgrwlnogn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jinqigufen.top/gtupzcjpfs.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.daria6918.cn/gtkxjwcomd.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.shzxlz.cn/gtevpfspyo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.hongshengwenyu.top/gtafjymlek.html

[E22] 字节长度与字符长度
来源：http://hz.9152youxi.cn/gtodlegbda.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jyoumei.cn/gtimafwkti.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.chenlongwang.top/gtvqgvrzms.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shangyingyoupin.top/gtuezggrjt.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.316326.xyz/gtahrqizzx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.zdqjudy.top/gtatsjaqqy.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.nanxuanxn.top/gtnwivekkf.html

Ruby: s.bytesize;  s.length
来源：http://hz.smart0.xyz/gtmlqmxrru.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yanxiufei.cn/gtidbutxlq.html

================================================================================
来源：http://hz.yongpay.top/gtbxdrdgsz.html

F. 文件与目录
来源：http://hz.zdqjudy.top/gtpxavbygk.html

================================================================================
来源：http://hz.daria6918.cn/gtzltazzmr.html

[F01] 读取整个文件
来源：http://hz.yangfankeji.com/gtoqiprulf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.smart0.xyz/gtvzxcmxqh.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jqgufenzy.top/gtwakzespd.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.ivvv.top/gteeqfnuty.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jiagoushi.top/gtbobxnrsj.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.nanxuanxn.top/gtgdyzwuif.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.haohaochexian.top/gtvudwjbrc.html

Ruby: File.read("a.txt")
来源：http://hz.yuxming.cn/gtkogkljpv.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.ydjk.org.cn/gtpfkgssqc.html

[F02] 逐行读取文件
来源：http://hz.gotoacloud.top/gtqfjffkrm.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.cashguo.top/gtfbwhvrmo.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.shangyingyoupin.top/gtizamvwpo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hnxiangtu.top/gtokfirmbv.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xingfuxueyuan.xyz/gtpantuevc.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.aibaodan.cn/gtadzjcdve.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.hfpthk.cn/gtzleudmft.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.xylfe.cn/gttdkbuhfr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.chenzaomai.com/gthnxmdfwz.html

[F03] 写入文件（覆盖）
来源：http://hz.xingfuxueyuan.xyz/gtbkqeeqdj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhaomingkeji.xyz/gtimvtuqpu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.smart0.xyz/gtspwhkfqy.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.havefunace.top/gttrjpukwx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.chenzaomai.com/gtechqjqsm.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.yj20258.top/gtotfyaivy.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.9152youxi.cn/gtoskpoaeg.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.birdmap.top/gtojxyqpmc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.cqqwz.cn/gtgjnskhdo.html

[F04] 追加写入文件
来源：http://hz.shuidangran.top/gtknrxpehw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.c1oappe.top/gttkpbljjt.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zhoulong.xyz/gtafekphqy.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.hnxiangtu.top/gtbggvzuuz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhiwuduotai.top/gtdoywurfl.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zhixingplan.top/gthchcazap.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.tian-w.cn/gttwdywvsu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jinghuilouyu.cn/gtopqdqrgj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.zhengqikj.top/gtvrsmfjia.html

[F05] 判断文件或目录是否存在
来源：http://hz.shanyushiyangkeji.top/gtcvonqjdp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.ydzc1.top/gtjqyeqgof.html

PHP:  file_exists("a.txt");
来源：http://hz.xziqi.cn/gtjfptcngz.html

JS:   fs.existsSync("a.txt")
来源：http://hz.9152youxi.cn/gtwwipimhu.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zhaomingkeji.xyz/gtorcrrmca.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.dashuyun.cn/gtdbqhawkp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.9152youxi.cn/gtrqyxrhcj.html

Ruby: File.exist?("a.txt")
来源：http://hz.ehwqpu.com/gtkvfrtkxt.html

C#:   File.Exists("a.txt")
来源：http://hz.fzhhl.top/gtfvdzsdmt.html

[F06] 删除文件
来源：http://hz.shuidangran.top/gtwglldcpc.html

Py:   os.remove("a.txt")
来源：http://hz.wangshuangyany.cn/gthuzosqla.html

PHP:  unlink("a.txt");
来源：http://hz.jinqigufen.top/gtkolondeq.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.cdnleiting.top/gtxsymskab.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.tianlin.xyz/gtxdnlifdc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.xuetiantiany.cn/gttcmeoeai.html

Go:   os.Remove("a.txt")
来源：http://hz.hywenlv.cn/gtjxjvgxjf.html

Ruby: File.delete("a.txt")
来源：http://hz.ehwqpu.com/gtyuthqhab.html

C#:   File.Delete("a.txt");
来源：http://hz.ywan-chungtsiang.top/gteiouydxa.html

[F07] 创建目录（含多级）
来源：http://hz.pengpengdd.cyou/gthobshkxb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.xingfuxueyuan.xyz/gtyncfnjjk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.hywenlv.cn/gthbdvikpw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yj202588.top/gtevrvzjtd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xinyue.icu/gtpnlbnrct.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.aizwys.cn/gtmkpvjttz.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.ydzc1.top/gtkzgynlaa.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jinqigufen.top/gtilbbbcew.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.sufxvd.cn/gtvkcpspfp.html

[F08] 遍历目录
来源：http://hz.gzhubu.top/gtzgxuidym.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.chenjidiqi.icu/gtretdgzip.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.yongpay.top/gtmmcfmqhd.html

JS:   fs.readdirSync("dir")
来源：http://hz.ydjk.org.cn/gtfplbxnws.html

TS:   fs.readdirSync("dir")
来源：http://hz.dianchejie.cn/gtiuglgtdi.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.daria6918.cn/gtownxhvva.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.gogol.net.cn/gtzffklnhy.html

Ruby: Dir.children("dir")
来源：http://hz.nanxuanxn.top/gtchzjpxdg.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jqgfzy.top/gtbinnkcga.html

[F09] 获取文件大小
来源：http://hz.316326.xyz/gtkjlngbsu.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yvedp.cn/gtqwhpdfaa.html

PHP:  filesize("a.txt");
来源：http://hz.pycfn.com/gtbolwslvc.html

JS:   fs.statSync("a.txt").size
来源：http://hz.gzhubu.top/gtjtxcqlco.html

TS:   fs.statSync("a.txt").size
来源：http://hz.aibaodan.cn/gtxqesdcrm.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.andypj.xyz/gtobjybhxr.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.sweek.top/gtpkxcwoal.html

Ruby: File.size("a.txt")
来源：http://hz.xinyue.icu/gtryfxnedy.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jlsjyb.cn/gtbporiucm.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.wangdashe.top/gtloexmbkm.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.hysaishi.cn/gtbguubfja.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.gzhubu.top/gtabdzgofp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.fzhhl.top/gtdblehmpd.html

TS:   path.extname("a.txt")
来源：http://hz.nanxinkj.top/gtidsluttm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.cashguo.top/gtjxjfithe.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.fzhhl.top/gtzwwypsxn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jqgufenzy.top/gtwojlhtgo.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhongyouzk.top/gtfmkuaazq.html

[F11] 复制与移动文件
来源：http://hz.cashguo.top/gtgxugruoj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.xuanzx.com/gteajrhoyg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.haohaochexian.top/gtrabnskxz.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cqqwz.cn/gthdcwreuf.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinqigufen.top/gtxeyrrhxo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.bjfxy.top/gtujmnigkt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jinghuilouyu.cn/gtgzgarkbb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.zdqjudy.top/gtmtrngwaf.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.yonumen.top/gtnlnxnvnk.html

[F12] CSV 读写
来源：http://hz.jiagoushi.top/gtgwbqvtly.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.c1oappe.top/gtinghpkio.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jqgufenzy.top/gthbvwxbie.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.316326.xyz/gtyuswemjq.html

TS:   // 同上
来源：http://hz.hysaishi.cn/gtmazbbjde.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.shanyushiyangkeji.top/gtxiiyypwa.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.bjfxy.top/gtyonqdgro.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jqgufenzy.top/gtyzotpsic.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.havefunace.top/gtwbrtdhel.html

================================================================================
来源：http://hz.wangdashe.top/gtzeeybjyj.html

G. 面向对象
来源：http://hz.gotoacloud.top/gtcgwvufmg.html

================================================================================
来源：http://hz.316326.xyz/gtlfiberus.html

[G01] 定义类
来源：http://hz.smart0.xyz/gtulyyighj.html

Py:   class User: pass
来源：http://hz.sysykeji.top/gtmxswcorn.html

PHP:  class User {}
来源：http://hz.yvedp.cn/gtxmcirprd.html

JS:   class User {}
来源：http://hz.xingfuxueyuan.xyz/gtslluzpki.html

TS:   class User { name: string = ""; }
来源：http://hz.cdnleiting.top/gtuhgevilc.html

Java: class User {}
来源：http://hz.zhixingplan.top/gtfexuhjzy.html

Go:   type User struct { Name string }
来源：http://hz.gogol.net.cn/gtcxrmuynq.html

Ruby: class User; end
来源：http://hz.zhongyouzk.top/gteqsdzmxc.html

C#:   class User {}
来源：http://hz.andypj.xyz/gthehwjbfs.html

[G02] 构造函数
来源：http://hz.kuanghao11.cn/gtybfxopip.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jiagoushi.top/gtdulnwngq.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.wangshuangyany.cn/gtxmvdohzi.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.ppjwa.cn/gtkjymzvll.html

TS:   constructor(public name: string) {}
来源：http://hz.snrcjt.cn/gttpuradxm.html

Java: User(String name) { this.name = name; }
来源：http://hz.birdmap.top/gtnoeuaieo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.gaohongyu789.top/gtbvfbutcw.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.nanxinkj.top/gtleetpggc.html

C#:   public User(string name) { Name = name; }
来源：http://hz.haohaochexian.top/gttlxtejlh.html

[G03] 实例属性
来源：http://hz.cqqwz.cn/gtjomlirti.html

Py:   self.name = "x"
来源：http://hz.birdmap.top/gteuwpuvoy.html

PHP:  public string $name = "x";
来源：http://hz.guannengcc.top/gtvhpyseue.html

JS:   this.name = "x";
来源：http://hz.wangshuangyany.cn/gtsrncosjn.html

TS:   name: string = "x";
来源：http://hz.svipenyu.cn/gtncoooftq.html

Java: private String name;
来源：http://hz.kuanghao11.cn/gtxemjnrev.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hywenlv.cn/gtitverwwp.html

Ruby: @name = "x"
来源：http://hz.quarkkingdee.top/gtveyywhkn.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.iojbl.cn/gtuavxpfbi.html

[G04] 定义方法
来源：http://hz.sweek.top/gtahjkeaso.html

Py:   def greet(self): return self.name
来源：http://hz.redwolf501.top/gtjuwhjhrn.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.haohaochexian.top/gtizewmqfv.html

JS:   greet() { return this.name; }
来源：http://hz.jinqigfzy.top/gthldqyeeo.html

TS:   greet(): string { return this.name; }
来源：http://hz.ppjwa.cn/gtruxdzrug.html

Java: String greet() { return name; }
来源：http://hz.jqgufenzy.top/gtsdvipvaw.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hysaishi.cn/gtlpdnwofy.html

Ruby: def greet; @name; end
来源：http://hz.guowangkeji.top/gtnsdbeabr.html

C#:   public string Greet() => Name;
来源：http://hz.gaohongyu789.top/gtnpeyjzkg.html

[G05] 继承
来源：http://hz.shuidangran.top/gtahapikzl.html

Py:   class Admin(User): pass
来源：http://hz.nanxuanxn.top/gtvjjtnsdo.html

PHP:  class Admin extends User {}
来源：http://hz.zhoulong.xyz/gtaweffjna.html

JS:   class Admin extends User {}
来源：http://hz.guowangkeji.top/gttfqanatj.html

TS:   class Admin extends User {}
来源：http://hz.nwbrower.top/gtdxszgsau.html

Java: class Admin extends User {}
来源：http://hz.pycfn.com/gtfcjokujc.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.gogol.net.cn/gtayhlvccd.html

Ruby: class Admin < User; end
来源：http://hz.ywan-chungtsiang.top/gtwkhjncus.html

C#:   class Admin : User {}
来源：http://hz.shzxlz.cn/gtkkrkcaej.html

[G06] 重写方法
来源：http://hz.wangdashe.top/gtcfbwlljo.html

Py:   def greet(self): return "admin"
来源：http://hz.jinghuilouyu.cn/gterlepqzw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.shzxlz.cn/gtcewfyfjd.html

JS:   greet() { return "admin"; }
来源：http://hz.shzxlz.cn/gtszitnhjb.html

TS:   greet(): string { return "admin"; }
来源：http://hz.pycfn.com/gtiqlizcng.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.ydzc1.top/gtdjlzczph.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.hnqzz.top/gtsdiyaeds.html

Ruby: def greet; "admin"; end
来源：http://hz.mhx1999.top/gtznikxsev.html

C#:   public override string Greet() => "admin";
来源：http://hz.sysykeji.top/gtrvovuwst.html

[G07] 调用父类方法
来源：http://hz.zhiwuduotai.top/gtoonbehru.html

Py:   super().greet()
来源：http://hz.bjfxy.top/gtqsuloqpz.html

PHP:  parent::greet();
来源：http://hz.ybcxt.top/gtugwlfdtq.html

JS:   super.greet();
来源：http://hz.sweek.top/gthqomywkt.html

TS:   super.greet();
来源：http://hz.aibaodan.cn/gtqiqelydk.html

Java: super.greet();
来源：http://hz.jinqigfzy.top/gtoxbvvdxc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.wangshuangyany.cn/gtuhpomvvq.html

Ruby: super
来源：http://hz.zhengqikj.top/gtumsehtpu.html

C#:   base.Greet();
来源：http://hz.tian-w.cn/gtxpfzbstd.html

[G08] 静态方法与属性
来源：http://hz.snrcjt.cn/gthitfwxkr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.wangdashe.top/gtwglkohgn.html

PHP:  public static function f() {}
来源：http://hz.kuanghao11.cn/gtrivmwlcw.html

JS:   static f() {}
来源：http://hz.hammf.cn/gtdzdooexy.html

TS:   static f(): void {}
来源：http://hz.yonumen.top/gtbmhjgfgh.html

Java: static void f() {}
来源：http://hz.yuxming.cn/gtstywnavo.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yj20258888.top/gtxtdyhitu.html

Ruby: def self.f; end
来源：http://hz.mhx1999.top/gtaanutcem.html

C#:   public static void F() {}
来源：http://hz.cheryme.top/gtlirfbafq.html

[G09] 接口 / 抽象类
来源：http://hz.zhijiandao.cn/gtkqdlfteg.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.sxryk.cn/gttjbqveqf.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yvedp.cn/gtnnzawfvv.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zhoulong.xyz/gtzpuadtyu.html

TS:   interface Shape { area(): number; }
来源：http://hz.yuxming.cn/gthysxlbgw.html

Java: interface Shape { double area(); }
来源：http://hz.tanke756.top/gtrwkiwuun.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.smart0.xyz/gtbcoryyrb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.nwbrower.top/gtmcangiqd.html

C#:   interface IShape { double Area(); }
来源：http://hz.hfpthk.cn/gtefzvhuvv.html

[G10] 访问控制
来源：http://hz.zhaomingkeji.xyz/gtdjoctauq.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.chenlongwang.top/gtaasddifs.html

PHP:  public / protected / private
来源：http://hz.ivvv.top/gtslwznrqd.html

JS:   #private 字段；其余公开
来源：http://hz.sweek.top/gtyjwpdwoi.html

TS:   public / protected / private
来源：http://hz.ivvv.top/gttvlbesvu.html

Java: public / protected / private / 默认包级
来源：http://hz.xylfe.cn/gtuirjlyly.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhijiandao.cn/gtrseepdet.html

Ruby: public / protected / private
来源：http://hz.yj20258888.top/gttvyaffjf.html

C#:   public / protected / private / internal
来源：http://hz.yvedp.cn/gtyfsziyvx.html

[G11] getter / setter
来源：http://hz.havefunace.top/gtpyzknlgj.html

Py:   @property 与 @x.setter
来源：http://hz.mhx1999.top/gttoohdgmb.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.iojbl.cn/gtaidqgzay.html


<!-- 参考信息 -->