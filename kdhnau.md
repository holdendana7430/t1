代发 wailian999

[E14] URL 编码与 Base64
来源：http://hz.hnxiangtu.top/gtaxtwubhk.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.yj202588.top/gtumdkpghq.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.shangyingyoupin.top/gtertomccr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.shzxlz.cn/gtcrttoajz.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.sxryk.cn/gtpspkxsky.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.haohaochexian.top/gtfligvieg.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.xziqi.cn/gtwgkruyiv.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.yj202588.top/gtutgtstku.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.hysaishi.cn/gtcuhtzwau.html

[E15] HTML 转义 / 反转义
来源：http://hz.meibo888.top/gtyjwfccgt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.redwolf501.top/gtktrdhkdl.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jinyuanbaomall.cn/gtrcthwywh.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.daria6918.cn/gttbjdccrf.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yvedp.cn/gtqsqgypeu.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.hysaishi.cn/gtfibznrxk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.nanxuanxn.top/gtaevminwj.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.daria6918.cn/gtaliekzhz.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jiagoushi.top/gtxrcaoxsg.html

[E16] 数字千分位
来源：http://hz.yuxming.cn/gtmodkiaxl.html

Py:   f"{1234567:,}"
来源：http://hz.jlsjyb.cn/gtpuzdotyn.html

PHP:  number_format(1234567);
来源：http://hz.jlsjyb.cn/gtgkbyzirc.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.fzhhl.top/gtnvvosgkl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.hongshengwenyu.top/gtndcuhpmu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.hysaishi.cn/gtwljyqvtc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.sweek.top/gtjbgbnbcu.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.chenzaomai.com/gtjfkqjqrs.html

C#:   1234567.ToString("N0")
来源：http://hz.ppjwa.cn/gtoxcfrzyx.html

[E17] 首字母大写
来源：http://hz.zdqjudy.top/gtfeuufmtk.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.jyoumei.cn/gtpzyalmrl.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.snrcjt.cn/gtcowoenjt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.dashuyun.cn/gtnxeorfum.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yuanzhike.top/gtpxhgnnko.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.xylfe.cn/gtdhvcqbtp.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.ydzc1.top/gtfwcgjejd.html

Ruby: s.capitalize
来源：http://hz.zhongyouzk.top/gtqpnrfzlx.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.tian-w.cn/gtbklohfhm.html

[E18] 模板占位符替换
来源：http://hz.52xcode.cn/gtrifgnymx.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.dianchejie.cn/gtycuqkbhl.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.fengsongda.top/gtnbaxetlg.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.dianchejie.cn/gtpsglczkg.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.zycfv.cn/gtcbsxgkwe.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.andypj.xyz/gtwcwpsmfp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.zhoulong.xyz/gtwaxxbieg.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.haohaochexian.top/gtunnhhcvf.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zdqjudy.top/gtosxxwssi.html

[E19] 多行文本按行拆分
来源：http://hz.kuanghao11.cn/gtpriyewev.html

Py:   s.splitlines()
来源：http://hz.9152youxi.cn/gtndtuitie.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.kuanghao11.cn/gtohotyyov.html

JS:   s.split(/\r?\n/)
来源：http://hz.yvedp.cn/gtskxcjjwf.html

TS:   s.split(/\r?\n/)
来源：http://hz.redwolf501.top/gtuoyknbrm.html

Java: s.lines().toList()
来源：http://hz.hongshengwenyu.top/gtjoympmjz.html

Go:   strings.Split(s, "\n")
来源：http://hz.feifeiyinyue.top/gtekzrmbyu.html

Ruby: s.lines
来源：http://hz.yvedp.cn/gtboxxmdam.html

C#:   s.Split('\n')
来源：http://hz.bjfxy.top/gtarjdhcrt.html

[E20] 判断字符串是否为空
来源：http://hz.zdqjudy.top/gtjxqhdpiu.html

Py:   if not s:
来源：http://hz.zhixingplan.top/gtxgbywbfh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.hongshengwenyu.top/gtzeijxqdi.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yj20258888.top/gtynrdejqg.html

TS:   if (s === "") {}
来源：http://hz.wangshuangyany.cn/gtdcjknyec.html

Java: if (s.isEmpty()) {}
来源：http://hz.zycfv.cn/gtqvixhntk.html

Go:   if s == "" {}
来源：http://hz.shanyushiyangtech.top/gtgrifizww.html

Ruby: if s.empty?
来源：http://hz.cheryme.top/gtvdynfkvj.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.yanxiufei.cn/gteuchzcyb.html

[E21] 超长截断加省略号
来源：http://hz.chenlongwang.top/gtidmqofrq.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.yuxming.cn/gtciborrca.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.316326.xyz/gtqrpnqtdd.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhoulong.xyz/gtqmpwhadl.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yangfankeji.com/gtmqksuthc.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.bjfxy.top/gthtfdhmlf.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.hnxiangtu.top/gtdhqkypte.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.bjfxy.top/gtbpyhwvnk.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.hysaishi.cn/gtonmlvnuv.html

[E22] 字节长度与字符长度
来源：http://hz.jlsjyb.cn/gtdcugorjm.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.nwbrower.top/gtisegztrp.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.9152youxi.cn/gtoyijhluk.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.c1oappe.top/gtolcdkvyz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.gogol.net.cn/gtzivcrijr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ivvv.top/gtsrlbccrc.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.zhiwuduotai.top/gtdnxewszw.html

Ruby: s.bytesize;  s.length
来源：http://hz.hywenlv.cn/gtppqlszva.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.zhixingplan.top/gtjnfiyxoq.html

================================================================================
来源：http://hz.xuetiantiany.cn/gtbtpcosmq.html

F. 文件与目录
来源：http://hz.cucudq.cn/gtvqmoulbd.html

================================================================================
来源：http://hz.9152youxi.cn/gtuabggrce.html

[F01] 读取整个文件
来源：http://hz.zhaomingkeji.xyz/gtgqewtkui.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.xylfe.cn/gtujmdxpdd.html

PHP:  file_get_contents("a.txt");
来源：http://hz.tian-w.cn/gtpssreqee.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.pycfn.com/gtyjmuaoxm.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.ydjk.org.cn/gtivrtnnhy.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.cqqwz.cn/gtxgnkqkkb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yj202588.top/gtunanschu.html

Ruby: File.read("a.txt")
来源：http://hz.cashguo.top/gtchbopwct.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.haohaochexian.top/gtejrabdto.html

[F02] 逐行读取文件
来源：http://hz.hnqzz.top/gtcxasatrz.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.snrcjt.cn/gtbyxtaekt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.xinyue.icu/gtzzfgjcnd.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ydzc1.top/gthxqcovjx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ppjwa.cn/gtssyfdkmw.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.kuanghao11.cn/gtlgowlxum.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jyoumei.cn/gtanribdgt.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.meibo888.top/gtvagnsbfj.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.cdnleiting.top/gtwyswlctw.html

[F03] 写入文件（覆盖）
来源：http://hz.jqgufenzy.top/gtjghjcrcx.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hywenlv.cn/gtdaztazci.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.ywan-chungtsiang.top/gtlbjdorqd.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhiwuduotai.top/gtzpkxtmgx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinqigfzy.top/gtywyydowx.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.yanxiufei.cn/gtctzxavgs.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yvedp.cn/gtkysjxbde.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.guannengcc.top/gtnibounji.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.jinyuanbaomall.cn/gtwetrcyhn.html

[F04] 追加写入文件
来源：http://hz.birdmap.top/gtlwhshxgl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.ehwqpu.com/gtsnvzlntk.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yj20258.top/gtjmalzdno.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.quarkkingdee.top/gtdydswsgg.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.smart0.xyz/gthyigqsgg.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.guowangkeji.top/gtrcxyjmux.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zdqjudy.top/gtfqqqpyet.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jqgufenzy.top/gtwbberfdu.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.dashuyun.cn/gtlqjpgaoa.html

[F05] 判断文件或目录是否存在
来源：http://hz.dashuyun.cn/gtxydweltp.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.hongshengwenyu.top/gtiabraunb.html

PHP:  file_exists("a.txt");
来源：http://hz.hongshengwenyu.top/gtvqfsghhu.html

JS:   fs.existsSync("a.txt")
来源：http://hz.shzxlz.cn/gthfjwuthe.html

TS:   fs.existsSync("a.txt")
来源：http://hz.guannengcc.top/gtdsunfszl.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.zhiwuduotai.top/gtumzzoqah.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jiagoushi.top/gteqibekfw.html

Ruby: File.exist?("a.txt")
来源：http://hz.nanxuanxn.top/gtyqccmire.html

C#:   File.Exists("a.txt")
来源：http://hz.yj202588.top/gthokneitc.html

[F06] 删除文件
来源：http://hz.shuidangran.top/gtgjsthdxy.html

Py:   os.remove("a.txt")
来源：http://hz.shuidangran.top/gtvlzvpcps.html

PHP:  unlink("a.txt");
来源：http://hz.yuanzhike.top/gtkrnbzcis.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hammf.cn/gtypemcybm.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hfpthk.cn/gtglrtiran.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.ydzc1.top/gtszynqdet.html

Go:   os.Remove("a.txt")
来源：http://hz.chenlongwang.top/gtgzagoaho.html

Ruby: File.delete("a.txt")
来源：http://hz.9152youxi.cn/gtceiimhes.html

C#:   File.Delete("a.txt");
来源：http://hz.jqgufenzy.top/gtgpsfajcl.html

[F07] 创建目录（含多级）
来源：http://hz.shangyingyoupin.top/gtjpfsqtvj.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.gzhubu.top/gthvzuuinh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.daria6918.cn/gtdbbljhen.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hywenlv.cn/gtjnoqkxvl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yanxiufei.cn/gtrhvnqtvn.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hfpthk.cn/gtfdmsygml.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.smart0.xyz/gtpoiczivf.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.svipenyu.cn/gtlltwpzjz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jianghu66.top/gtkkqyggzw.html

[F08] 遍历目录
来源：http://hz.hnxiangtu.top/gtkicvsoxe.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.ywan-chungtsiang.top/gtbbvrfdny.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.tian-w.cn/gtnrcpawgd.html

JS:   fs.readdirSync("dir")
来源：http://hz.tianlin.xyz/gtjbeocnhc.html

TS:   fs.readdirSync("dir")
来源：http://hz.svipenyu.cn/gtzcpqynqx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.ehwqpu.com/gtuewvgnex.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zhoulong.xyz/gtownhedhl.html

Ruby: Dir.children("dir")
来源：http://hz.gotoacloud.top/gtciikzdcx.html

C#:   Directory.GetFiles("dir")
来源：http://hz.ybcxt.top/gtqdcozsmn.html

[F09] 获取文件大小
来源：http://hz.xuetiantiany.cn/gtdyjrujgj.html

Py:   os.path.getsize("a.txt")
来源：http://hz.guowangkeji.top/gtcmylbrfm.html

PHP:  filesize("a.txt");
来源：http://hz.birdmap.top/gtiztjvxsc.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jyoumei.cn/gtcebcucix.html

TS:   fs.statSync("a.txt").size
来源：http://hz.ivvv.top/gtqlcyuvge.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.aizwys.cn/gtqisdevhl.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.0kj1m.cn/gtjsejxsrf.html

Ruby: File.size("a.txt")
来源：http://hz.ivvv.top/gtklxusqgf.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.ywan-chungtsiang.top/gtswjzvjqt.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hfpthk.cn/gtbolfbmnb.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.hongshengwenyu.top/gtgwtyggfv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.gogol.net.cn/gteyqaksbp.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.birdmap.top/gtuoydqvoy.html

TS:   path.extname("a.txt")
来源：http://hz.xuanzx.com/gtjubzltym.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.hysaishi.cn/gtokywntjx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.smart0.xyz/gthruxttdu.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.guowangkeji.top/gtemxgpuxz.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.nanxuanxn.top/gtntpntnjl.html

[F11] 复制与移动文件
来源：http://hz.zycfv.cn/gtclvxihbs.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.yanxiufei.cn/gtihgxgxjp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.0kj1m.cn/gtaegfaqpp.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.kuanghao11.cn/gtkjltjbuv.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.snrcjt.cn/gtawlajges.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.gotoacloud.top/gtkyfwoalg.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.jqgfzy.top/gtetwbthrs.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.dashuyun.cn/gtyfqkkmyi.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.gogol.net.cn/gtwndjmpwp.html

[F12] CSV 读写
来源：http://hz.fzhhl.top/gtkcebxedu.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jqgfzy.top/gtimmbdfma.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.dashuyun.cn/gtzoetgxjc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.ywan-chungtsiang.top/gttxoamntf.html

TS:   // 同上
来源：http://hz.jianghu66.top/gtkralssai.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.xingfuxueyuan.xyz/gtxquulpky.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.9152youxi.cn/gtmrccyuzo.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.guannengcc.top/gtygultiti.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.sysykeji.top/gtiusurbge.html

================================================================================
来源：http://hz.yvedp.cn/gtvbsepvjr.html

G. 面向对象
来源：http://hz.dianchejie.cn/gtshsmawgl.html

================================================================================
来源：http://hz.hongshengwenyu.top/gtupzqsvmk.html

[G01] 定义类
来源：http://hz.daria6918.cn/gttcvolnxa.html

Py:   class User: pass
来源：http://hz.bjfxy.top/gtzcdyrndv.html

PHP:  class User {}
来源：http://hz.pengpengdd.cyou/gtqkpuqdgf.html

JS:   class User {}
来源：http://hz.cqqwz.cn/gtyhnlxzud.html

TS:   class User { name: string = ""; }
来源：http://hz.zhixingplan.top/gtkbervjpr.html

Java: class User {}
来源：http://hz.sxryk.cn/gtvlhbxpuc.html

Go:   type User struct { Name string }
来源：http://hz.hammf.cn/gtpwjolgrw.html

Ruby: class User; end
来源：http://hz.daxiang520.top/gtnzxsydfk.html

C#:   class User {}
来源：http://hz.zhaomingkeji.xyz/gtukmahhgo.html

[G02] 构造函数
来源：http://hz.ehwqpu.com/gtpohbotbo.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.zhengqikj.top/gtuyvjwbtw.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zhiwuduotai.top/gthpzxaaou.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xingfuxueyuan.xyz/gtajtlzrxp.html

TS:   constructor(public name: string) {}
来源：http://hz.smart0.xyz/gtcixhxhme.html

Java: User(String name) { this.name = name; }
来源：http://hz.xuetiantiany.cn/gtygzzbjmp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.shzxlz.cn/gtspabysoi.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.mhx1999.top/gtcwoimxwt.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhengqikj.top/gtkxuvquxs.html

[G03] 实例属性
来源：http://hz.vqdsnc.cn/gttmxcvlkb.html

Py:   self.name = "x"
来源：http://hz.cashguo.top/gtqmzwyadp.html

PHP:  public string $name = "x";
来源：http://hz.jqgfzy.top/gtgrcwxlyx.html

JS:   this.name = "x";
来源：http://hz.kuanghao11.cn/gtsddxsmul.html

TS:   name: string = "x";
来源：http://hz.gaohongyu789.top/gtfxhgxkvw.html

Java: private String name;
来源：http://hz.birdmap.top/gttlrmcuch.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jinyuanbaomall.cn/gthpckqipi.html

Ruby: @name = "x"
来源：http://hz.tianlin.xyz/gtraeokzsd.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.sufxvd.cn/gtzndcosly.html

[G04] 定义方法
来源：http://hz.nwbrower.top/gtssolooih.html

Py:   def greet(self): return self.name
来源：http://hz.52xcode.cn/gtqbbrwcgz.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.svipenyu.cn/gtqbqivwxv.html

JS:   greet() { return this.name; }
来源：http://hz.tianlin.xyz/gtdwiawvau.html

TS:   greet(): string { return this.name; }
来源：http://hz.chenzaomai.com/gtkiczjcch.html

Java: String greet() { return name; }
来源：http://hz.zhongyouzk.top/gtqoslfxrm.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.chenzaomai.com/gtoofyndrb.html

Ruby: def greet; @name; end
来源：http://hz.pycfn.com/gtthrkyyvc.html

C#:   public string Greet() => Name;
来源：http://hz.52xcode.cn/gtezdtdhjq.html

[G05] 继承
来源：http://hz.ehwqpu.com/gtqwlkxyqw.html

Py:   class Admin(User): pass
来源：http://hz.nanxuanxn.top/gttwjidhlw.html

PHP:  class Admin extends User {}
来源：http://hz.wangshuangyany.cn/gtqgtonfjc.html

JS:   class Admin extends User {}
来源：http://hz.zhaomingkeji.xyz/gtsaddibex.html

TS:   class Admin extends User {}
来源：http://hz.guannengcc.top/gtfzmzmilh.html

Java: class Admin extends User {}
来源：http://hz.cdnleiting.top/gtbxejqpgq.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.daxiang520.top/gtskabcxht.html

Ruby: class Admin < User; end
来源：http://hz.guannengcc.top/gtnvludepa.html

C#:   class Admin : User {}
来源：http://hz.zhongyouzk.top/gtbsmunevt.html

[G06] 重写方法
来源：http://hz.zhoulong.xyz/gtkqdojdho.html

Py:   def greet(self): return "admin"
来源：http://hz.smart0.xyz/gtnprixdxa.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.jinghuilouyu.cn/gtgvpxoenv.html

JS:   greet() { return "admin"; }
来源：http://hz.jinyuanbaomall.cn/gtbkfgythl.html

TS:   greet(): string { return "admin"; }
来源：http://hz.nanxuanxn.top/gtilnfjiri.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.nwbrower.top/gtvuzrfiri.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.shuidangran.top/gtkrchqduh.html

Ruby: def greet; "admin"; end
来源：http://hz.sweek.top/gtgwvleimt.html

C#:   public override string Greet() => "admin";
来源：http://hz.fengsongda.top/gtkopuwpmm.html

[G07] 调用父类方法
来源：http://hz.wangshuangyany.cn/gtjfwecotj.html

Py:   super().greet()
来源：http://hz.yongpay.top/gtavgvgjwl.html

PHP:  parent::greet();
来源：http://hz.redwolf501.top/gtttphkwcr.html

JS:   super.greet();
来源：http://hz.chenzaomai.com/gtheixciag.html

TS:   super.greet();
来源：http://hz.yuanzhike.top/gtdywdoqrj.html

Java: super.greet();
来源：http://hz.yongpay.top/gtygbuuvml.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zhoulong.xyz/gtahajbbem.html

Ruby: super
来源：http://hz.redwolf501.top/gtsxkfenvg.html

C#:   base.Greet();
来源：http://hz.sysykeji.top/gttkdfvmpz.html

[G08] 静态方法与属性
来源：http://hz.zhoulong.xyz/gtrvkeypmx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.chenjidiqi.icu/gtplucpswv.html

PHP:  public static function f() {}
来源：http://hz.yonumen.top/gttbpamjdx.html

JS:   static f() {}
来源：http://hz.shanyushiyangkeji.top/gtvqfuxyjy.html

TS:   static f(): void {}
来源：http://hz.andypj.xyz/gtaqdhxzvs.html

Java: static void f() {}
来源：http://hz.nwbrower.top/gtxkzypjlt.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.gaohongyu789.top/gtuvatnfvp.html

Ruby: def self.f; end
来源：http://hz.ppjwa.cn/gtgtlddzqn.html

C#:   public static void F() {}
来源：http://hz.tanke756.top/gtbhqquqal.html

[G09] 接口 / 抽象类
来源：http://hz.cdnleiting.top/gtjvgaweok.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.jyoumei.cn/gtwvfopstv.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.cdnleiting.top/gthclryxda.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.fengsongda.top/gtnqicqvgw.html

TS:   interface Shape { area(): number; }
来源：http://hz.tanke756.top/gtzoyybgxt.html

Java: interface Shape { double area(); }
来源：http://hz.xuetiantiany.cn/gtaphvijtv.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yangfankeji.com/gtvtsjewii.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.ydjk.org.cn/gtwnjtoang.html

C#:   interface IShape { double Area(); }
来源：http://hz.shanyushiyangtech.top/gtkjptfjuq.html

[G10] 访问控制
来源：http://hz.guannengcc.top/gtdttvqari.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jqgfzy.top/gttzpjozmc.html

PHP:  public / protected / private
来源：http://hz.gotoacloud.top/gttlehgdcb.html

JS:   #private 字段；其余公开
来源：http://hz.wangdashe.top/gtsectcbfm.html

TS:   public / protected / private
来源：http://hz.jianghu66.top/gtpsxvrdcz.html

Java: public / protected / private / 默认包级
来源：http://hz.aibaodan.cn/gtnpymrvyb.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ydzc1.top/gtrxvslxlh.html

Ruby: public / protected / private
来源：http://hz.haohaochexian.top/gtlhspvmcg.html

C#:   public / protected / private / internal
来源：http://hz.jiagoushi.top/gtpcdpxdtq.html

[G11] getter / setter
来源：http://hz.xingfuxueyuan.xyz/gtcdguqwxv.html

Py:   @property 与 @x.setter
来源：http://hz.hnqzz.top/gtnqxojrgg.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.hywenlv.cn/gttsxpwzwt.html

JS:   get name() { return this._name; }
来源：http://hz.jinyuanbaomall.cn/gtpvilxasx.html

TS:   get name(): string { return this._name; }
来源：http://hz.snrcjt.cn/gtmtqeyfhe.html

Java: public String getName() { return name; }
来源：http://hz.pycfn.com/gtdfcgonbh.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jinqigufen.top/gtorpjbtwp.html

Ruby: attr_accessor :name
来源：http://hz.c1oappe.top/gtdmsbpmlt.html

C#:   public string Name { get; set; }
来源：http://hz.cucudq.cn/gtpibpplkj.html

[G12] 对象转字符串
来源：http://hz.yueranfly.top/gthkkiyxfr.html

Py:   def __str__(self): return self.name
来源：http://hz.ppjwa.cn/gtgzkexsva.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.xingfuxueyuan.xyz/gtzedoqxzt.html

JS:   toString() { return this.name; }
来源：http://hz.fengsongda.top/gtnszawpjj.html

TS:   toString(): string { return this.name; }
来源：http://hz.cdnleiting.top/gtxeyjlypt.html

Java: @Override public String toString() { return name; }
来源：http://hz.gogol.net.cn/gtmrdpibyl.html


<!-- 参考信息 -->