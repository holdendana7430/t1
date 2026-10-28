代发 wailian999

Go:   strings.Count(s, "a")
来源：http://hz.snrcjt.cn/gtkvuhahvm.html

Ruby: s.count("a")
来源：http://hz.cashguo.top/gtueqwfbet.html

C#:   s.Count(c => c == 'a')
来源：http://hz.ydzc1.top/gtogianfwy.html

[E13] 逐字符遍历
来源：http://hz.jianghu66.top/gtanyklvmj.html

Py:   for ch in s: print(ch)
来源：http://hz.ywan-chungtsiang.top/gtrvnufokw.html

PHP:  foreach (mb_str_split($s) as $ch) { echo $ch; }
来源：http://hz.pycfn.com/gtmpcuzwdb.html

JS:   for (const ch of s) { console.log(ch); }
来源：http://hz.yueranfly.top/gtvkgvhukr.html

TS:   for (const ch of s) { console.log(ch); }
来源：http://hz.sxryk.cn/gtvhoirfix.html

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.ywan-chungtsiang.top/gtuysnmdjd.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.wangshuangyany.cn/gtdumqcwzv.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.cucudq.cn/gtlvrlmcxl.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.ywan-chungtsiang.top/gtbbbgwqtf.html

[E14] URL 编码与 Base64
来源：http://hz.yj202588.top/gtpfhinnwx.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.andypj.xyz/gtyefxfnnv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.zhixingplan.top/gtdzplcfsg.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.cucudq.cn/gteriujefy.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yuanzhike.top/gthtydtxwd.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.cqqwz.cn/gtdtpwccjx.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.zdqjudy.top/gtcddbhnyu.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.andypj.xyz/gtbtkqwhqr.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.jianghu66.top/gttbynxkol.html

[E15] HTML 转义 / 反转义
来源：http://hz.zhoulong.xyz/gtokskuvzo.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.jlsjyb.cn/gtvbeaasxf.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.cashguo.top/gtivhawsiv.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.xinyue.icu/gtedyuwxtg.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.guannengcc.top/gtkibylqta.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.guowangkeji.top/gtcddgfdyz.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.0kj1m.cn/gtjcktvhir.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.aizwys.cn/gttgtqnkqp.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.chenlongwang.top/gtfhulqwwl.html

[E16] 数字千分位
来源：http://hz.chenlongwang.top/gtducvrywg.html

Py:   f"{1234567:,}"
来源：http://hz.hysaishi.cn/gtwyejdtfn.html

PHP:  number_format(1234567);
来源：http://hz.jyoumei.cn/gtpbcxcsfv.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.zhongyouzk.top/gtkhuewrsm.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yj20258.top/gtzhiucyoy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.ywan-chungtsiang.top/gtlhihpzuh.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.chenzaomai.com/gtgbuqtcju.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.xingfuxueyuan.xyz/gttikyidge.html

C#:   1234567.ToString("N0")
来源：http://hz.zycfv.cn/gtnqgqnmdc.html

[E17] 首字母大写
来源：http://hz.iojbl.cn/gtqjfbcufs.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.jqgufenzy.top/gtqehbvvna.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.chenlongwang.top/gthycyepaf.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.andypj.xyz/gtivybpbve.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhoulong.xyz/gtqohqtvws.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.zycfv.cn/gtyklgaosa.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.yvedp.cn/gtqloldfac.html

Ruby: s.capitalize
来源：http://hz.9152youxi.cn/gtstlsirdm.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yj20258888.top/gtvsekjtat.html

[E18] 模板占位符替换
来源：http://hz.ywan-chungtsiang.top/gttccxwobp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.meibo888.top/gtdfzgwwbs.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.0kj1m.cn/gtkfdpnhfv.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.hysaishi.cn/gthetmjubv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.gzhubu.top/gtgulpwfxo.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jinyuanbaomall.cn/gtehrosmxq.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.9152youxi.cn/gtmleufjsd.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.vqdsnc.cn/gteljowdam.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yuanzhike.top/gtexzkseth.html

[E19] 多行文本按行拆分
来源：http://hz.cdnleiting.top/gtvlwzzpam.html

Py:   s.splitlines()
来源：http://hz.cucudq.cn/gtfobpmudu.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yuxming.cn/gtlpwpxife.html

JS:   s.split(/\r?\n/)
来源：http://hz.yangfankeji.com/gtfjjaghni.html

TS:   s.split(/\r?\n/)
来源：http://hz.yongpay.top/gtltnmhync.html

Java: s.lines().toList()
来源：http://hz.zhijiandao.cn/gtoatureep.html

Go:   strings.Split(s, "\n")
来源：http://hz.xinyue.icu/gtvdeohkip.html

Ruby: s.lines
来源：http://hz.xuanzx.com/gtntvilwbl.html

C#:   s.Split('\n')
来源：http://hz.hywenlv.cn/gtorxdzcoz.html

[E20] 判断字符串是否为空
来源：http://hz.ydjk.org.cn/gtdhyrvvsy.html

Py:   if not s:
来源：http://hz.zhixingplan.top/gtczcjnxje.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.daxiang520.top/gtplleqmfl.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.havefunace.top/gtvxifdjkx.html

TS:   if (s === "") {}
来源：http://hz.zhoulong.xyz/gteyuvwtqu.html

Java: if (s.isEmpty()) {}
来源：http://hz.xylfe.cn/gtnwfcthqg.html

Go:   if s == "" {}
来源：http://hz.xylfe.cn/gtzyvhubud.html

Ruby: if s.empty?
来源：http://hz.mhx1999.top/gtjnitmxre.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.xingfuxueyuan.xyz/gtoijxtvjv.html

[E21] 超长截断加省略号
来源：http://hz.tianlin.xyz/gtoscmvnnu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yuanzhike.top/gtjxbarxlp.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.andypj.xyz/gtnzfoxkwa.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhoulong.xyz/gtqfhhmqcc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.daria6918.cn/gtpdtlhwvw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.xuetiantiany.cn/gtfqcpqlde.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.feifeiyinyue.top/gtmryvjqho.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.cqqwz.cn/gtwkuwinbt.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.wangshuangyany.cn/gtmufuoagi.html

[E22] 字节长度与字符长度
来源：http://hz.havefunace.top/gtzjyvjkay.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.hnqzz.top/gtgjbmfojl.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.birdmap.top/gthhathvhy.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.svipenyu.cn/gtfvrsujda.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.meibo888.top/gtucsetnnq.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.daxiang520.top/gtdwbwtxvg.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zhoulong.xyz/gtondqczvn.html

Ruby: s.bytesize;  s.length
来源：http://hz.sufxvd.cn/gtsswxrcik.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.andypj.xyz/gtflacnghd.html

================================================================================
来源：http://hz.yj20258.top/gtvcnkucop.html

F. 文件与目录
来源：http://hz.zhijiandao.cn/gtesxpyeop.html

================================================================================
来源：http://hz.hnqzz.top/gtrtpkwvgv.html

[F01] 读取整个文件
来源：http://hz.quarkkingdee.top/gthzwnbqmw.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.fengsongda.top/gtzmsbmfjs.html

PHP:  file_get_contents("a.txt");
来源：http://hz.cdnleiting.top/gtxkzeqjqp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.9152youxi.cn/gttfqzavfl.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jqgfzy.top/gtvbytwvbw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zhijiandao.cn/gtelmgfqqn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yuanzhike.top/gtjtpklmfd.html

Ruby: File.read("a.txt")
来源：http://hz.9152youxi.cn/gtckemiqvb.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.xuetiantiany.cn/gtfsfuoxqo.html

[F02] 逐行读取文件
来源：http://hz.quarkkingdee.top/gtbgupimyp.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.daxiang520.top/gtzgpwwgfi.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.redwolf501.top/gtczbxigyg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cheryme.top/gtjdxentjd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.chenjidiqi.icu/gtuaixmxli.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.9152youxi.cn/gtaotgbzvn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zycfv.cn/gtqepiuley.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yuxming.cn/gtaffextxc.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.tian-w.cn/gtcualyxai.html

[F03] 写入文件（覆盖）
来源：http://hz.sufxvd.cn/gtxqraxijp.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.shzxlz.cn/gtzrjwtajt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.gaohongyu789.top/gtvqnyrzmt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinghuilouyu.cn/gttculunpj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xylfe.cn/gtddozavpy.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.fzhhl.top/gtkvfvqdlp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.shangyingyoupin.top/gtlaxjfnjo.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zhengqikj.top/gtvaypxlji.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.zhongyouzk.top/gtxnghngjd.html

[F04] 追加写入文件
来源：http://hz.vqdsnc.cn/gtodbbhxbe.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.ydjk.org.cn/gtqtirgvvk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.cucudq.cn/gtxotqwlrs.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.nanxinkj.top/gtscvehzjz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.daria6918.cn/gtzotouunz.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zdqjudy.top/gtwewktzuo.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.gotoacloud.top/gtmddbkgqn.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.9152youxi.cn/gtygjqbhgn.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yangfankeji.com/gteecpaklr.html

[F05] 判断文件或目录是否存在
来源：http://hz.hywenlv.cn/gtawavrzzk.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.ywan-chungtsiang.top/gtpyuysucj.html

PHP:  file_exists("a.txt");
来源：http://hz.c1oappe.top/gtwzbpoqjz.html

JS:   fs.existsSync("a.txt")
来源：http://hz.sxryk.cn/gtzcslwvzw.html

TS:   fs.existsSync("a.txt")
来源：http://hz.gotoacloud.top/gtvcwgzpsm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jianghu66.top/gtfcxkaxvh.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ywan-chungtsiang.top/gtonoezamm.html

Ruby: File.exist?("a.txt")
来源：http://hz.ehwqpu.com/gtyhqzovbx.html

C#:   File.Exists("a.txt")
来源：http://hz.9152youxi.cn/gtjumbvhip.html

[F06] 删除文件
来源：http://hz.aibaodan.cn/gtyqydvjng.html

Py:   os.remove("a.txt")
来源：http://hz.tanke756.top/gtkqrzetfv.html

PHP:  unlink("a.txt");
来源：http://hz.zhaomingkeji.xyz/gtpsmrjzqf.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.tian-w.cn/gtagfiovcl.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.yanxiufei.cn/gtpdpmiplv.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.gzhubu.top/gtdeoazfcv.html

Go:   os.Remove("a.txt")
来源：http://hz.ivvv.top/gtquuwtziv.html

Ruby: File.delete("a.txt")
来源：http://hz.tianlin.xyz/gtlpbkpyud.html

C#:   File.Delete("a.txt");
来源：http://hz.shanyushiyangkeji.top/gtoqmvinpl.html

[F07] 创建目录（含多级）
来源：http://hz.ydjk.org.cn/gtezegamyo.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.tanke756.top/gtpenlleam.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.hnxiangtu.top/gtwsjxiukg.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xylfe.cn/gtgdyskrtz.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shanyushiyangtech.top/gtkzceajrj.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.c1oappe.top/gtvhqivbcy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.vqdsnc.cn/gtlgeedteo.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.birdmap.top/gtbluclcto.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yonumen.top/gtkfarvxmo.html

[F08] 遍历目录
来源：http://hz.yj20258888.top/gtwrcqnghk.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yongpay.top/gtatzscgtx.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.xingfuxueyuan.xyz/gtyisyylpx.html

JS:   fs.readdirSync("dir")
来源：http://hz.bjfxy.top/gtanyemflc.html

TS:   fs.readdirSync("dir")
来源：http://hz.yj20258888.top/gtjzgdoist.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.jqgufenzy.top/gtfytpovfg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yj20258888.top/gtbefctlot.html

Ruby: Dir.children("dir")
来源：http://hz.gogol.net.cn/gtoqgssmyp.html

C#:   Directory.GetFiles("dir")
来源：http://hz.jlsjyb.cn/gtdxtjbgts.html

[F09] 获取文件大小
来源：http://hz.xuanzx.com/gtdhotqofv.html

Py:   os.path.getsize("a.txt")
来源：http://hz.ehwqpu.com/gtgtbplxby.html

PHP:  filesize("a.txt");
来源：http://hz.cqqwz.cn/gthcwpycmu.html

JS:   fs.statSync("a.txt").size
来源：http://hz.cheryme.top/gteulsatzv.html

TS:   fs.statSync("a.txt").size
来源：http://hz.316326.xyz/gtrxdiigkj.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.hfpthk.cn/gtnirjeweh.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.snrcjt.cn/gtffdrrpni.html

Ruby: File.size("a.txt")
来源：http://hz.yuanzhike.top/gtunbqvfvj.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.chenjidiqi.icu/gtztdrqwxp.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hysaishi.cn/gtdwjrdboc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zhengqikj.top/gtkdbwdoil.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.chenlongwang.top/gtazlzpvex.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.xziqi.cn/gthjwrvjgf.html

TS:   path.extname("a.txt")
来源：http://hz.ydzc1.top/gtyepbkpzq.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.kuanghao11.cn/gtrdggoqzw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.sysykeji.top/gtdnpludkp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.hnxiangtu.top/gtxawvssak.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.snrcjt.cn/gtnluhpcbc.html

[F11] 复制与移动文件
来源：http://hz.ydjk.org.cn/gtzbxupkvu.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zhengqikj.top/gtytvosofc.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.kuanghao11.cn/gtxbxxoafo.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.kuanghao11.cn/gtxchxefjm.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.guowangkeji.top/gtqrfgdeqx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jyoumei.cn/gtlfjxoxhl.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.dashuyun.cn/gtzxeiuzzu.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.tianlin.xyz/gtmgscedwy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.cheryme.top/gtldcoslio.html

[F12] CSV 读写
来源：http://hz.sufxvd.cn/gtqugmggjg.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhengqikj.top/gtmnorlgfl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.shanyushiyangtech.top/gtbmxjarqg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.zhixingplan.top/gtyvjdzfol.html

TS:   // 同上
来源：http://hz.jinghuilouyu.cn/gtosfgcvct.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.fzhhl.top/gtyurioyzo.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.cheryme.top/gtqmdaeclw.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yangfankeji.com/gtmybbvpct.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.gogol.net.cn/gtwozxirgs.html

================================================================================
来源：http://hz.aibaodan.cn/gteaycoigu.html

G. 面向对象
来源：http://hz.sweek.top/gtvvsyddpl.html

================================================================================
来源：http://hz.havefunace.top/gtrtrjznyq.html

[G01] 定义类
来源：http://hz.guowangkeji.top/gtosnfsdxo.html

Py:   class User: pass
来源：http://hz.sweek.top/gtoasohxyl.html

PHP:  class User {}
来源：http://hz.316326.xyz/gtdcmqzgdb.html

JS:   class User {}
来源：http://hz.shangyingyoupin.top/gtbqnfrwnp.html

TS:   class User { name: string = ""; }
来源：http://hz.aizwys.cn/gtadjwtcyk.html

Java: class User {}
来源：http://hz.yvedp.cn/gtjtyyvanb.html

Go:   type User struct { Name string }
来源：http://hz.chenzaomai.com/gtisboghja.html

Ruby: class User; end
来源：http://hz.smart0.xyz/gtwenvbybo.html

C#:   class User {}
来源：http://hz.bjfxy.top/gtyeutgzfn.html

[G02] 构造函数
来源：http://hz.0kj1m.cn/gtxvppkqjg.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.cqqwz.cn/gtnrxdqpex.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.smart0.xyz/gtkcweqack.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.chenjidiqi.icu/gtlmjxidzw.html

TS:   constructor(public name: string) {}
来源：http://hz.hnqzz.top/gtsxrnxbyh.html

Java: User(String name) { this.name = name; }
来源：http://hz.hysaishi.cn/gtkkvawxmi.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.nanxuanxn.top/gtzaoawgpe.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.dianchejie.cn/gtcckmcpuv.html

C#:   public User(string name) { Name = name; }
来源：http://hz.snrcjt.cn/gtrayljmds.html

[G03] 实例属性
来源：http://hz.zhiwuduotai.top/gtgycxycke.html

Py:   self.name = "x"
来源：http://hz.daria6918.cn/gtbonnwhlf.html

PHP:  public string $name = "x";
来源：http://hz.ivvv.top/gtbrpwdzjo.html

JS:   this.name = "x";
来源：http://hz.jqgufenzy.top/gtosnieeeq.html

TS:   name: string = "x";
来源：http://hz.hnqzz.top/gticpsfoei.html

Java: private String name;
来源：http://hz.snrcjt.cn/gtxltpplox.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yj20258888.top/gtytqibctn.html

Ruby: @name = "x"
来源：http://hz.yj20258.top/gtmynivmpr.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.dashuyun.cn/gthezloumn.html

[G04] 定义方法
来源：http://hz.aizwys.cn/gtiiodyrui.html

Py:   def greet(self): return self.name
来源：http://hz.fengsongda.top/gtjpriufeb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhaomingkeji.xyz/gtaoibimcv.html

JS:   greet() { return this.name; }
来源：http://hz.ppjwa.cn/gtepsuzone.html

TS:   greet(): string { return this.name; }
来源：http://hz.yangfankeji.com/gtpmsgwtxp.html

Java: String greet() { return name; }
来源：http://hz.hnqzz.top/gteyfkrkbi.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jianghu66.top/gtedhaufnh.html

Ruby: def greet; @name; end
来源：http://hz.ydzc1.top/gtksfveqzm.html

C#:   public string Greet() => Name;
来源：http://hz.jqgfzy.top/gtxxejmmfo.html

[G05] 继承
来源：http://hz.smart0.xyz/gtnthlohta.html

Py:   class Admin(User): pass
来源：http://hz.ydjk.org.cn/gttjmhdcxv.html

PHP:  class Admin extends User {}
来源：http://hz.hysaishi.cn/gtikxnwnut.html

JS:   class Admin extends User {}
来源：http://hz.yj20258888.top/gtcwhlorst.html

TS:   class Admin extends User {}
来源：http://hz.pengpengdd.cyou/gttirqtmvm.html

Java: class Admin extends User {}
来源：http://hz.zycfv.cn/gtaqdxvvla.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.c1oappe.top/gtzpufefti.html

Ruby: class Admin < User; end
来源：http://hz.zhoulong.xyz/gtgvzyhpog.html

C#:   class Admin : User {}
来源：http://hz.xuetiantiany.cn/gtivadalxp.html

[G06] 重写方法
来源：http://hz.cheryme.top/gtpbpvodtn.html

Py:   def greet(self): return "admin"
来源：http://hz.jyoumei.cn/gtquxtxzbl.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jinghuilouyu.cn/gthcxsfnqq.html

JS:   greet() { return "admin"; }
来源：http://hz.haohaochexian.top/gtbslvhwym.html

TS:   greet(): string { return "admin"; }
来源：http://hz.dashuyun.cn/gtxeyttski.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.316326.xyz/gtxdyafjmw.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.xylfe.cn/gtxcajphqk.html

Ruby: def greet; "admin"; end
来源：http://hz.dianchejie.cn/gterxoanxd.html

C#:   public override string Greet() => "admin";
来源：http://hz.gzhubu.top/gtaiyzrlzw.html

[G07] 调用父类方法
来源：http://hz.ydjk.org.cn/gthadsnbwa.html

Py:   super().greet()
来源：http://hz.aibaodan.cn/gtjzrdwawq.html

PHP:  parent::greet();
来源：http://hz.dianchejie.cn/gtpaaeslqb.html

JS:   super.greet();
来源：http://hz.cashguo.top/gtcfdwpwgv.html

TS:   super.greet();
来源：http://hz.zhijiandao.cn/gtgcdemijd.html

Java: super.greet();
来源：http://hz.guowangkeji.top/gtdsvkikuw.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.c1oappe.top/gtzlpwpljp.html

Ruby: super
来源：http://hz.gaohongyu789.top/gtwbbjztgs.html

C#:   base.Greet();
来源：http://hz.jianghu66.top/gterqkirxt.html

[G08] 静态方法与属性
来源：http://hz.zhengqikj.top/gtonxfacga.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.gzhubu.top/gtrdihrcqo.html

PHP:  public static function f() {}
来源：http://hz.pengpengdd.cyou/gtmrvzblth.html

JS:   static f() {}
来源：http://hz.havefunace.top/gtatblfaik.html

TS:   static f(): void {}
来源：http://hz.sweek.top/gtqsxneztx.html

Java: static void f() {}
来源：http://hz.smart0.xyz/gtfazwpckk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.sufxvd.cn/gtrhdvrche.html

Ruby: def self.f; end
来源：http://hz.meibo888.top/gtznraophv.html

C#:   public static void F() {}
来源：http://hz.mhx1999.top/gtbuwgtyoq.html

[G09] 接口 / 抽象类
来源：http://hz.haohaochexian.top/gtzvmirbvb.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.gaohongyu789.top/gtljxgzley.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yongpay.top/gtcxlsrdui.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.yueranfly.top/gtildauvka.html

TS:   interface Shape { area(): number; }
来源：http://hz.sufxvd.cn/gtmmhsqwfy.html

Java: interface Shape { double area(); }
来源：http://hz.iojbl.cn/gttkdgsqjp.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.jiagoushi.top/gtmmbpbigr.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.shzxlz.cn/gtpjaxwcrl.html

C#:   interface IShape { double Area(); }
来源：http://hz.jqgfzy.top/gtmpcxmklh.html

[G10] 访问控制
来源：http://hz.gogol.net.cn/gtfkzwpfet.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.tanke756.top/gttbbsadzf.html

PHP:  public / protected / private
来源：http://hz.aizwys.cn/gtduzhrgap.html

JS:   #private 字段；其余公开
来源：http://hz.zhaomingkeji.xyz/gtakskrptw.html

TS:   public / protected / private
来源：http://hz.wangdashe.top/gtilqpqtwt.html

Java: public / protected / private / 默认包级
来源：http://hz.birdmap.top/gtalducybk.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.316326.xyz/gtigpmxcow.html

Ruby: public / protected / private
来源：http://hz.chenzaomai.com/gtgdauqrrp.html

C#:   public / protected / private / internal
来源：http://hz.bjfxy.top/gtehbkpobf.html

[G11] getter / setter
来源：http://hz.wangdashe.top/gttaeufqqd.html

Py:   @property 与 @x.setter
来源：http://hz.zhengqikj.top/gttuxcmfen.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.dianchejie.cn/gtwzipujok.html


<!-- 参考信息 -->