代发 wailian999

PHP:  substr_count($s, "a");
来源：http://hz.zdqjudy.top/gtkfraedjl.html

JS:   s.split("a").length - 1
来源：http://hz.yvedp.cn/gtggijcbun.html

TS:   s.split("a").length - 1
来源：http://hz.yuanzhike.top/gttvhffcmm.html

Java: s.chars().filter(c -> c == 'a').count()
来源：http://hz.ydzc1.top/gtczijywug.html

Go:   strings.Count(s, "a")
来源：http://hz.redwolf501.top/gtddzngatx.html

Ruby: s.count("a")
来源：http://hz.jinghuilouyu.cn/gtzenxutgw.html

C#:   s.Count(c => c == 'a')
来源：http://hz.gaohongyu789.top/gthpzyncyj.html

[E13] 逐字符遍历
来源：http://hz.sxryk.cn/gtiwgbbmjs.html

Py:   for ch in s: print(ch)
来源：http://hz.jiagoushi.top/gtlsolcyvk.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.gaohongyu789.top/gtxyvfcpyx.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.9152youxi.cn/gtwnvelhaz.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.cdnleiting.top/gtcfxwwpgk.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.xylfe.cn/gtbsstvkha.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.wangshuangyany.cn/gtuiiulkcc.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.zhiwuduotai.top/gtrhhluzwy.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.fengsongda.top/gtgpuejxuo.html

[E14] URL 编码与 Base64
来源：http://hz.52xcode.cn/gtjuqyxzpi.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.jiagoushi.top/gtbmnrcyea.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.aibaodan.cn/gtnmfjjsph.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.nwbrower.top/gtcubjxwqa.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.zdqjudy.top/gtqrmaykaq.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.snrcjt.cn/gtnptoujrn.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.yongpay.top/gtueqefifc.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.hfpthk.cn/gtlwhhhacw.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.cqqwz.cn/gtzozhukia.html

[E15] HTML 转义 / 反转义
来源：http://hz.sxryk.cn/gtoadpworc.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.aizwys.cn/gtdichvdlx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jinqigufen.top/gtllrimcbk.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.ydjk.org.cn/gtmennppmc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.aibaodan.cn/gtjtwccjcw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.hysaishi.cn/gtiourgetv.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.jinqigufen.top/gtpwwmuked.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.xziqi.cn/gtfkckxqrp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.zhiwuduotai.top/gtelrdrqez.html

[E16] 数字千分位
来源：http://hz.zhongyouzk.top/gtatwmzqgj.html

Py:   f"{1234567:,}"
来源：http://hz.hammf.cn/gthqepjyut.html

PHP:  number_format(1234567);
来源：http://hz.shzxlz.cn/gtyidlaqfi.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.sufxvd.cn/gtpwquzemn.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.hywenlv.cn/gtwqiiegti.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zdqjudy.top/gtymholgrz.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.hammf.cn/gtgwesbbkb.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.andypj.xyz/gtzjdtdhot.html

C#:   1234567.ToString("N0")
来源：http://hz.shanyushiyangtech.top/gtancmednp.html

[E17] 首字母大写
来源：http://hz.xylfe.cn/gtgysddoeg.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yj20258888.top/gtyunrhvyb.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.havefunace.top/gtosignyjd.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.sxryk.cn/gtzfkyfpsi.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cashguo.top/gtjuyihzzh.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.yongpay.top/gttlgkcqxn.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.zdqjudy.top/gtjjgfdmfz.html

Ruby: s.capitalize
来源：http://hz.redwolf501.top/gtujpcjnte.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.birdmap.top/gtxkspcbww.html

[E18] 模板占位符替换
来源：http://hz.gogol.net.cn/gtwsbvpfvk.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.zhongyouzk.top/gtzqaxopak.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.daria6918.cn/gtigbuzpnh.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.tanke756.top/gtviwmasfx.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.xuetiantiany.cn/gtrhygcgkf.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.nanxuanxn.top/gtesjzgamx.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.xziqi.cn/gtrsbdpnmg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.xinyue.icu/gtqkhvgezm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.pengpengdd.cyou/gtycdzxcsl.html

[E19] 多行文本按行拆分
来源：http://hz.shuidangran.top/gtuksorrrs.html

Py:   s.splitlines()
来源：http://hz.zhiwuduotai.top/gtsuwpnalj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.gzhubu.top/gtondnzevk.html

JS:   s.split(/\r?\n/)
来源：http://hz.yj20258.top/gtxpdktcyf.html

TS:   s.split(/\r?\n/)
来源：http://hz.fzhhl.top/gthdaynltk.html

Java: s.lines().toList()
来源：http://hz.shanyushiyangtech.top/gtomafoiox.html

Go:   strings.Split(s, "\n")
来源：http://hz.nwbrower.top/gtzhtthsnn.html

Ruby: s.lines
来源：http://hz.xuetiantiany.cn/gtliaokzal.html

C#:   s.Split('\n')
来源：http://hz.yonumen.top/gtbmvzuumt.html

[E20] 判断字符串是否为空
来源：http://hz.snrcjt.cn/gtjgcyieke.html

Py:   if not s:
来源：http://hz.aizwys.cn/gtwadtkjsc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.chenzaomai.com/gtqtxkhjxw.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jinqigufen.top/gtqltvvahe.html

TS:   if (s === "") {}
来源：http://hz.yangfankeji.com/gtrpdczvwo.html

Java: if (s.isEmpty()) {}
来源：http://hz.cashguo.top/gtlgedptjy.html

Go:   if s == "" {}
来源：http://hz.yonumen.top/gtqcviuatf.html

Ruby: if s.empty?
来源：http://hz.xuanzx.com/gtiawulpod.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.cqqwz.cn/gtapxzwdge.html

[E21] 超长截断加省略号
来源：http://hz.zhaomingkeji.xyz/gtbfvligjg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.jianghu66.top/gthrpcmoun.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.tian-w.cn/gtxcinpbhv.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhengqikj.top/gtrtqagmpc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.tian-w.cn/gtneimdwig.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.tian-w.cn/gtfjefxded.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.gotoacloud.top/gtmdxxjihk.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.zhaomingkeji.xyz/gtcyetbspf.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.chenzaomai.com/gtasvfvscm.html

[E22] 字节长度与字符长度
来源：http://hz.guannengcc.top/gtciotwfhv.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.birdmap.top/gtvgqbjlip.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cqqwz.cn/gtserheddr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.yj20258.top/gtbpapintu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hnxiangtu.top/gtbeyutchw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.daria6918.cn/gtqwodctcb.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.ywan-chungtsiang.top/gtzybwglxg.html

Ruby: s.bytesize;  s.length
来源：http://hz.aibaodan.cn/gtjlgmylck.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jianghu66.top/gtqjrxbnev.html

================================================================================
来源：http://hz.xziqi.cn/gtfhqjgtuj.html

F. 文件与目录
来源：http://hz.zhijiandao.cn/gteiydfnbv.html

================================================================================
来源：http://hz.svipenyu.cn/gtwzyhctwr.html

[F01] 读取整个文件
来源：http://hz.redwolf501.top/gtgvqbpdij.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.pengpengdd.cyou/gtqclqieip.html

PHP:  file_get_contents("a.txt");
来源：http://hz.ivvv.top/gtbrpwhsyw.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zhengqikj.top/gthwpyuvge.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yj20258888.top/gtoeztsyni.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.dashuyun.cn/gtlakmjgrx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhijiandao.cn/gtgxztodkn.html

Ruby: File.read("a.txt")
来源：http://hz.zhiwuduotai.top/gtpovavxrj.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yanxiufei.cn/gtxzkftcpx.html

[F02] 逐行读取文件
来源：http://hz.cucudq.cn/gtuuuteitc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.hnxiangtu.top/gthpxovrbl.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.guowangkeji.top/gtpccjgywn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.zhijiandao.cn/gtsqshrflc.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yuxming.cn/gtontoqyil.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.havefunace.top/gttendngcx.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.snrcjt.cn/gtcccemwgr.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jqgufenzy.top/gtricijgjt.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.dashuyun.cn/gtjwkazfqc.html

[F03] 写入文件（覆盖）
来源：http://hz.hammf.cn/gtoypylshi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.xuetiantiany.cn/gtlpacfnvu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.wangdashe.top/gtgbmuiyhf.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.dianchejie.cn/gtpxmwmwas.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yj20258.top/gtubdqyqaw.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.ywan-chungtsiang.top/gtiakxspkl.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.svipenyu.cn/gtzpfyyjjh.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.hammf.cn/gtpqjvswho.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.xuanzx.com/gtbyrjgzua.html

[F04] 追加写入文件
来源：http://hz.hnxiangtu.top/gtlwofzkof.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.cdnleiting.top/gtilelwcni.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.chenzaomai.com/gteowrobew.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xingfuxueyuan.xyz/gtdznseaim.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ydjk.org.cn/gttvwwnbka.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.smart0.xyz/gtspufohvg.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.feifeiyinyue.top/gtdcgneoxc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jqgfzy.top/gtxbgezajo.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.zhijiandao.cn/gtrniekpgw.html

[F05] 判断文件或目录是否存在
来源：http://hz.vqdsnc.cn/gtviollhdf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.havefunace.top/gttdswkief.html

PHP:  file_exists("a.txt");
来源：http://hz.birdmap.top/gtmftsxtyv.html

JS:   fs.existsSync("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtrfvcolnf.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zdqjudy.top/gtclbgtrie.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.yueranfly.top/gtulmqlzlj.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yj20258.top/gtifwjmdtm.html

Ruby: File.exist?("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtqtcurgfc.html

C#:   File.Exists("a.txt")
来源：http://hz.guowangkeji.top/gttwlxjfcu.html

[F06] 删除文件
来源：http://hz.tian-w.cn/gtrimabkdj.html

Py:   os.remove("a.txt")
来源：http://hz.daxiang520.top/gtnoqqtrtr.html

PHP:  unlink("a.txt");
来源：http://hz.gzhubu.top/gtflxawgzl.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.nwbrower.top/gtvbotkdul.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.xuanzx.com/gtqplgvwcc.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jinqigufen.top/gtyfickjhg.html

Go:   os.Remove("a.txt")
来源：http://hz.hammf.cn/gtzxqmpwyz.html

Ruby: File.delete("a.txt")
来源：http://hz.gzhubu.top/gtcabzacso.html

C#:   File.Delete("a.txt");
来源：http://hz.xylfe.cn/gtobthpdtd.html

[F07] 创建目录（含多级）
来源：http://hz.guowangkeji.top/gtqqpwtbht.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.tian-w.cn/gtjqkqjdkp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.ydzc1.top/gtkzfaclcs.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.fzhhl.top/gtvnjcwnpt.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.aibaodan.cn/gtkxkijxjb.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.xinyue.icu/gtoreurpaf.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jinghuilouyu.cn/gtnqzgkbld.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.xingfuxueyuan.xyz/gtvxzmbarp.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yangfankeji.com/gtsdvnskau.html

[F08] 遍历目录
来源：http://hz.ehwqpu.com/gtpttjrthj.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xuetiantiany.cn/gtytzwpjom.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.9152youxi.cn/gtakvmhuni.html

JS:   fs.readdirSync("dir")
来源：http://hz.ehwqpu.com/gtxiiilzux.html

TS:   fs.readdirSync("dir")
来源：http://hz.yuanzhike.top/gtvyzpndzm.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.hammf.cn/gtcdrtgvkr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.c1oappe.top/gtqqhusuxh.html

Ruby: Dir.children("dir")
来源：http://hz.birdmap.top/gtgxousotu.html

C#:   Directory.GetFiles("dir")
来源：http://hz.guowangkeji.top/gtzhlhgwtl.html

[F09] 获取文件大小
来源：http://hz.zhoulong.xyz/gtdxekbkfi.html

Py:   os.path.getsize("a.txt")
来源：http://hz.gogol.net.cn/gtbmwpamij.html

PHP:  filesize("a.txt");
来源：http://hz.shanyushiyangtech.top/gtifwyhdaj.html

JS:   fs.statSync("a.txt").size
来源：http://hz.ybcxt.top/gthqilbqzm.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jinghuilouyu.cn/gtqvtsyaxa.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jinqigufen.top/gtjfxcklzn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.yj20258.top/gtwxryothg.html

Ruby: File.size("a.txt")
来源：http://hz.hnxiangtu.top/gtcmvnwpcd.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.snrcjt.cn/gtlyiwnzbx.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.yonumen.top/gthfeurdye.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zhijiandao.cn/gtsxdqizdj.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.guannengcc.top/gtwaksuzec.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.hnqzz.top/gtjjbcflyc.html

TS:   path.extname("a.txt")
来源：http://hz.9152youxi.cn/gtpvnztzfw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.shuidangran.top/gtasanaxrq.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.tian-w.cn/gtftevjoin.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yvedp.cn/gtucmfeecr.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.daxiang520.top/gtdoqxozud.html

[F11] 复制与移动文件
来源：http://hz.xuanzx.com/gtixgngegg.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zhijiandao.cn/gtpnnvqkii.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.hywenlv.cn/gtxtapbhox.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.316326.xyz/gtmmupzwih.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.yj20258.top/gtvhaucevx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yvedp.cn/gtcxekyjch.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.snrcjt.cn/gtwlfrlwbn.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jiagoushi.top/gtevvcrbru.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.feifeiyinyue.top/gtvqnrodmm.html

[F12] CSV 读写
来源：http://hz.nanxuanxn.top/gtjxxurhoo.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.hysaishi.cn/gtspzteqlh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.zdqjudy.top/gtvgdbmuvb.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.birdmap.top/gtxffyeqoj.html

TS:   // 同上
来源：http://hz.zhixingplan.top/gtqslpfycs.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.xinyue.icu/gtnzspvonv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.redwolf501.top/gtqawqghby.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jqgufenzy.top/gtckmzamgp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.wangdashe.top/gtqgzkfbgz.html

================================================================================
来源：http://hz.zhoulong.xyz/gtlckadbsc.html

G. 面向对象
来源：http://hz.ywan-chungtsiang.top/gtwjittpcq.html

================================================================================
来源：http://hz.hfpthk.cn/gtryzraedy.html

[G01] 定义类
来源：http://hz.havefunace.top/gtlfnnhqax.html

Py:   class User: pass
来源：http://hz.gotoacloud.top/gtwahudebl.html

PHP:  class User {}
来源：http://hz.316326.xyz/gtlemdqyzl.html

JS:   class User {}
来源：http://hz.gaohongyu789.top/gtpfchyopr.html

TS:   class User { name: string = ""; }
来源：http://hz.316326.xyz/gthckdbvyj.html

Java: class User {}
来源：http://hz.chenzaomai.com/gtpcrxywwj.html

Go:   type User struct { Name string }
来源：http://hz.jianghu66.top/gtulrwoyld.html

Ruby: class User; end
来源：http://hz.zhongyouzk.top/gtwyaidgst.html

C#:   class User {}
来源：http://hz.wangshuangyany.cn/gttxhhdiwf.html

[G02] 构造函数
来源：http://hz.yueranfly.top/gtlqrbqmlk.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.jqgfzy.top/gtawhuywew.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hammf.cn/gtbqxczazb.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jlsjyb.cn/gtaoxnjzmd.html

TS:   constructor(public name: string) {}
来源：http://hz.nanxuanxn.top/gtvszndijd.html

Java: User(String name) { this.name = name; }
来源：http://hz.sysykeji.top/gtgjzvzuou.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.tian-w.cn/gttiycjasu.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.ehwqpu.com/gttopzkrds.html

C#:   public User(string name) { Name = name; }
来源：http://hz.fzhhl.top/gtidemkzlp.html

[G03] 实例属性
来源：http://hz.cqqwz.cn/gtoxlcfqgu.html

Py:   self.name = "x"
来源：http://hz.cdnleiting.top/gtodcooqhu.html

PHP:  public string $name = "x";
来源：http://hz.cheryme.top/gteesohufu.html

JS:   this.name = "x";
来源：http://hz.shzxlz.cn/gtridfuwai.html

TS:   name: string = "x";
来源：http://hz.cashguo.top/gtcdaatdjy.html

Java: private String name;
来源：http://hz.aizwys.cn/gtwammrxuq.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.ydjk.org.cn/gtusfqikhj.html

Ruby: @name = "x"
来源：http://hz.xingfuxueyuan.xyz/gtciqbdqws.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zhoulong.xyz/gtaoddmdpm.html

[G04] 定义方法
来源：http://hz.xinyue.icu/gtlzfcheew.html

Py:   def greet(self): return self.name
来源：http://hz.yvedp.cn/gtyheojzih.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.shangyingyoupin.top/gtccddsejh.html

JS:   greet() { return this.name; }
来源：http://hz.9152youxi.cn/gtejazkenv.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhixingplan.top/gtqropmkvf.html

Java: String greet() { return name; }
来源：http://hz.hnqzz.top/gtsygogwxh.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.xinyue.icu/gtkkobxwrl.html

Ruby: def greet; @name; end
来源：http://hz.fengsongda.top/gtifjcvgpd.html

C#:   public string Greet() => Name;
来源：http://hz.ehwqpu.com/gtjonrlqvz.html

[G05] 继承
来源：http://hz.cashguo.top/gtjtsxnyxi.html

Py:   class Admin(User): pass
来源：http://hz.feifeiyinyue.top/gtpxpmrqok.html

PHP:  class Admin extends User {}
来源：http://hz.redwolf501.top/gtyzxmujcy.html

JS:   class Admin extends User {}
来源：http://hz.hywenlv.cn/gtjvhrirfr.html

TS:   class Admin extends User {}
来源：http://hz.iojbl.cn/gtjhvdgsld.html

Java: class Admin extends User {}
来源：http://hz.andypj.xyz/gtwzqriflh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.daria6918.cn/gtbstmxckg.html

Ruby: class Admin < User; end
来源：http://hz.jinghuilouyu.cn/gtepfrwwdz.html

C#:   class Admin : User {}
来源：http://hz.c1oappe.top/gtpnycpasy.html

[G06] 重写方法
来源：http://hz.chenzaomai.com/gtvgzcirnx.html

Py:   def greet(self): return "admin"
来源：http://hz.yangfankeji.com/gtgcadylny.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jianghu66.top/gtrwsrrrbv.html

JS:   greet() { return "admin"; }
来源：http://hz.ydjk.org.cn/gtukrmweru.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yuxming.cn/gtkiduipsa.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhengqikj.top/gtshxefbsf.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.zhoulong.xyz/gtqzorxarx.html

Ruby: def greet; "admin"; end
来源：http://hz.0kj1m.cn/gtjhzthjii.html

C#:   public override string Greet() => "admin";
来源：http://hz.gaohongyu789.top/gtssnqtrar.html

[G07] 调用父类方法
来源：http://hz.mhx1999.top/gtpyfrwakh.html

Py:   super().greet()
来源：http://hz.zhiwuduotai.top/gtjjtxxlej.html

PHP:  parent::greet();
来源：http://hz.zhaomingkeji.xyz/gtrhtdkwdg.html

JS:   super.greet();
来源：http://hz.havefunace.top/gtfvunbbyj.html

TS:   super.greet();
来源：http://hz.jinghuilouyu.cn/gtnbnuiwkz.html

Java: super.greet();
来源：http://hz.yueranfly.top/gtubgpqvlh.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.sxryk.cn/gtedbyrlfe.html

Ruby: super
来源：http://hz.yangfankeji.com/gtjwaehfiq.html

C#:   base.Greet();
来源：http://hz.ivvv.top/gtkhmgwcln.html

[G08] 静态方法与属性
来源：http://hz.shuidangran.top/gthpmijswu.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.cucudq.cn/gtbpvudgje.html

PHP:  public static function f() {}
来源：http://hz.cashguo.top/gtltktintc.html

JS:   static f() {}
来源：http://hz.gotoacloud.top/gtoykvdusd.html

TS:   static f(): void {}
来源：http://hz.xingfuxueyuan.xyz/gterrquicc.html

Java: static void f() {}
来源：http://hz.sweek.top/gtxtgayptn.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.sxryk.cn/gtquhunsbx.html

Ruby: def self.f; end
来源：http://hz.jiagoushi.top/gtwupgdljn.html

C#:   public static void F() {}
来源：http://hz.quarkkingdee.top/gtcqbzzzmn.html

[G09] 接口 / 抽象类
来源：http://hz.wangdashe.top/gtqunuerrt.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.shanyushiyangtech.top/gtwxgpyabj.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yonumen.top/gtffwxydkn.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.quarkkingdee.top/gtvfafzqvj.html

TS:   interface Shape { area(): number; }
来源：http://hz.yanxiufei.cn/gtntcgjzud.html

Java: interface Shape { double area(); }
来源：http://hz.redwolf501.top/gtrpdtbriw.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.xylfe.cn/gtmmdobmya.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.guowangkeji.top/gtpuagklfc.html

C#:   interface IShape { double Area(); }
来源：http://hz.zhixingplan.top/gtnlkmzkiw.html

[G10] 访问控制
来源：http://hz.52xcode.cn/gtpzdmqyqa.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yvedp.cn/gtelbytmjr.html

PHP:  public / protected / private
来源：http://hz.ybcxt.top/gtvqkhtabx.html

JS:   #private 字段；其余公开
来源：http://hz.meibo888.top/gtqvycvagb.html

TS:   public / protected / private
来源：http://hz.ivvv.top/gtalchrsgk.html

Java: public / protected / private / 默认包级
来源：http://hz.hysaishi.cn/gtcombfzej.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.zhoulong.xyz/gtidrwwtcr.html

Ruby: public / protected / private
来源：http://hz.zhaomingkeji.xyz/gtdftpokuk.html


<!-- 参考信息 -->