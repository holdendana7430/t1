代发 wailian999

Java: for (char ch : s.toCharArray()) { System.out.println(ch); }
来源：http://hz.xuetiantiany.cn/gtujaqzqdr.html

Go:   for _, ch := range s { fmt.Println(string(ch)) }   // 按 rune 遍历
来源：http://hz.xuetiantiany.cn/gtkkbpwlnm.html

Ruby: s.each_char { |ch| puts ch }
来源：http://hz.sysykeji.top/gtlkixcsea.html

C#:   foreach (var ch in s) { Console.WriteLine(ch); }
来源：http://hz.jiagoushi.top/gtyqlikziz.html

[E14] URL 编码与 Base64
来源：http://hz.zhongyouzk.top/gtecphlfoa.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.ydzc1.top/gtqtknlovv.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.chenlongwang.top/gthggvtupr.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.wangdashe.top/gtbhfpyofm.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.jinqigufen.top/gtytlvzdiv.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.jiagoushi.top/gtpcybjazp.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.daxiang520.top/gtaiajxovz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.smart0.xyz/gtdykbtmty.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.smart0.xyz/gtnuzvpjoe.html

[E15] HTML 转义 / 反转义
来源：http://hz.meibo888.top/gtxzksrutr.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zhixingplan.top/gtzuqmfagk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jqgfzy.top/gtneoyxofl.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.jinqigufen.top/gtsrcgdydm.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.jlsjyb.cn/gtbmbmxjeh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.vqdsnc.cn/gtpwncfewk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.ydzc1.top/gtmpyrgqvf.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.sweek.top/gttifxxlhc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.havefunace.top/gtptpbgzkf.html

[E16] 数字千分位
来源：http://hz.guowangkeji.top/gtjosdlsxt.html

Py:   f"{1234567:,}"
来源：http://hz.yuxming.cn/gtsevcowsf.html

PHP:  number_format(1234567);
来源：http://hz.nwbrower.top/gtghebuurh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.shangyingyoupin.top/gtrynscnme.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.yanxiufei.cn/gtxthoarri.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yj20258888.top/gtepblqrtp.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yj20258.top/gtkucnyrcj.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.gzhubu.top/gthgmynuop.html

C#:   1234567.ToString("N0")
来源：http://hz.guowangkeji.top/gtbjnkijdc.html

[E17] 首字母大写
来源：http://hz.jyoumei.cn/gtyhvvqtmw.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.smart0.xyz/gtuapmoqxk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.guowangkeji.top/gttqeudayk.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jqgufenzy.top/gtyfgzgchd.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.mhx1999.top/gtabcaeirt.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jinqigfzy.top/gtawxaaopq.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.wangshuangyany.cn/gtetgbncsu.html

Ruby: s.capitalize
来源：http://hz.xylfe.cn/gtberqvkay.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jinghuilouyu.cn/gtoxyucblf.html

[E18] 模板占位符替换
来源：http://hz.cashguo.top/gtspshceob.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.ybcxt.top/gtbjfjnxqc.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.daxiang520.top/gtvlfulhvd.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.aizwys.cn/gtqvepxudf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.ehwqpu.com/gtgjhitwwr.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.iojbl.cn/gtpmyxsspo.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.meibo888.top/gtyysrquso.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.shzxlz.cn/gtwljhkqhc.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jqgfzy.top/gtnigqcdds.html

[E19] 多行文本按行拆分
来源：http://hz.jinyuanbaomall.cn/gtwsnucdza.html

Py:   s.splitlines()
来源：http://hz.chenjidiqi.icu/gtbqerkbcv.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.hnqzz.top/gtjbnmwarq.html

JS:   s.split(/\r?\n/)
来源：http://hz.yanxiufei.cn/gtljxsolws.html

TS:   s.split(/\r?\n/)
来源：http://hz.quarkkingdee.top/gtctexwgzq.html

Java: s.lines().toList()
来源：http://hz.jqgfzy.top/gtsairpyas.html

Go:   strings.Split(s, "\n")
来源：http://hz.sysykeji.top/gtydupcltt.html

Ruby: s.lines
来源：http://hz.yongpay.top/gtizxjgyfj.html

C#:   s.Split('\n')
来源：http://hz.yueranfly.top/gtbwgegkpv.html

[E20] 判断字符串是否为空
来源：http://hz.daxiang520.top/gtobymnzno.html

Py:   if not s:
来源：http://hz.aizwys.cn/gtvjkkpmqu.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.haohaochexian.top/gtrtixtdxs.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jinqigufen.top/gttnlredxu.html

TS:   if (s === "") {}
来源：http://hz.wangshuangyany.cn/gtvsvpxlzu.html

Java: if (s.isEmpty()) {}
来源：http://hz.jlsjyb.cn/gthdphkqcs.html

Go:   if s == "" {}
来源：http://hz.zycfv.cn/gtlfdyjdkh.html

Ruby: if s.empty?
来源：http://hz.hywenlv.cn/gtfrinvmlk.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.mhx1999.top/gtwqrkcqmo.html

[E21] 超长截断加省略号
来源：http://hz.shzxlz.cn/gtpuokutke.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.chenjidiqi.icu/gtefpzwufj.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yuxming.cn/gtkklhrrtu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yangfankeji.com/gtjviywtst.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.cdnleiting.top/gtcmdbrdqf.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.svipenyu.cn/gtaysrbfai.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yuxming.cn/gtcvkbkdew.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.tianlin.xyz/gtugvvhfil.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.gzhubu.top/gtvhdkzuxw.html

[E22] 字节长度与字符长度
来源：http://hz.xziqi.cn/gtyxklgvle.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.yueranfly.top/gtjyopfkjq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cqqwz.cn/gtpghilqmp.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.daxiang520.top/gtudmczzyw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ehwqpu.com/gtwrhmtteh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.chenlongwang.top/gtqiawhvoi.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jlsjyb.cn/gtxfelqfgn.html

Ruby: s.bytesize;  s.length
来源：http://hz.shanyushiyangtech.top/gtnzgwmggr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yangfankeji.com/gtkjrghrmm.html

================================================================================
来源：http://hz.chenlongwang.top/gtagczgmap.html

F. 文件与目录
来源：http://hz.shangyingyoupin.top/gtfwkcidqp.html

================================================================================
来源：http://hz.gotoacloud.top/gtoucmsmpu.html

[F01] 读取整个文件
来源：http://hz.52xcode.cn/gtnvezyoad.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.zhixingplan.top/gttjdntine.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yongpay.top/gtstvzkopg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.mhx1999.top/gtqwqtibgy.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhoulong.xyz/gtkuwabgxv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.nanxinkj.top/gtwdakirvo.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.pycfn.com/gtkuwqkigg.html

Ruby: File.read("a.txt")
来源：http://hz.nanxuanxn.top/gtwbjogggz.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yueranfly.top/gtfqpoqxjx.html

[F02] 逐行读取文件
来源：http://hz.zhiwuduotai.top/gtwktpxkqb.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jinyuanbaomall.cn/gtcdrbnasf.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.gotoacloud.top/gtxyesaanq.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ydzc1.top/gtqamrtscw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ehwqpu.com/gtztywzfgz.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.dashuyun.cn/gteiftfgvw.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.jianghu66.top/gtoiysdpzf.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.ywan-chungtsiang.top/gtshyikzhr.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jianghu66.top/gtymlkjckq.html

[F03] 写入文件（覆盖）
来源：http://hz.ybcxt.top/gtpsdeffoa.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.nanxuanxn.top/gtegshrwzp.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.daria6918.cn/gtwbflrxam.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sysykeji.top/gtbycwwqio.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.mhx1999.top/gtgrhmyhxn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.zhaomingkeji.xyz/gtwnrracmf.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.hfpthk.cn/gtmuqjbcnn.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jinghuilouyu.cn/gthtfzioxq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.sufxvd.cn/gtscxwakgu.html

[F04] 追加写入文件
来源：http://hz.xinyue.icu/gtfmocvuas.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.tanke756.top/gtpvfxxgaz.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.dianchejie.cn/gtvzkwmuit.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.xylfe.cn/gtetfymgqn.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.wangdashe.top/gtggquvcxk.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.meibo888.top/gtywddmcad.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.nanxuanxn.top/gtswaaaarq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.cheryme.top/gtwcqqaolx.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.gogol.net.cn/gtzaqpjmty.html

[F05] 判断文件或目录是否存在
来源：http://hz.xuetiantiany.cn/gtksuwmoiq.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.pycfn.com/gtgmreuhme.html

PHP:  file_exists("a.txt");
来源：http://hz.hysaishi.cn/gtpxrmftex.html

JS:   fs.existsSync("a.txt")
来源：http://hz.xziqi.cn/gtedaxrgwn.html

TS:   fs.existsSync("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtiohsqekt.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.316326.xyz/gtjgihtqno.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.cheryme.top/gtrlpnbvpy.html

Ruby: File.exist?("a.txt")
来源：http://hz.xinyue.icu/gtqcnqaena.html

C#:   File.Exists("a.txt")
来源：http://hz.fengsongda.top/gtacocdjhj.html

[F06] 删除文件
来源：http://hz.nanxinkj.top/gtlcpwkoqk.html

Py:   os.remove("a.txt")
来源：http://hz.havefunace.top/gtigacgjsm.html

PHP:  unlink("a.txt");
来源：http://hz.nanxuanxn.top/gtfncupnaj.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.yj20258.top/gtzopicuco.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jianghu66.top/gtgrldzmmx.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.cdnleiting.top/gtjgimrzjv.html

Go:   os.Remove("a.txt")
来源：http://hz.cucudq.cn/gtzmdsbyme.html

Ruby: File.delete("a.txt")
来源：http://hz.cdnleiting.top/gtweqbptxh.html

C#:   File.Delete("a.txt");
来源：http://hz.iojbl.cn/gtjnwggczu.html

[F07] 创建目录（含多级）
来源：http://hz.jinqigfzy.top/gtnaadhscg.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.fzhhl.top/gtrqrenyok.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.fzhhl.top/gtmikqxvaw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.feifeiyinyue.top/gtkrycbwlk.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.gaohongyu789.top/gtllwgfspf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.daria6918.cn/gtcrahanmj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.redwolf501.top/gtbsbsdugj.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.gogol.net.cn/gtyzykslzz.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.jlsjyb.cn/gtgucnjhkx.html

[F08] 遍历目录
来源：http://hz.cashguo.top/gttionwjcz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.ppjwa.cn/gtikvltrce.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.daxiang520.top/gtatpozias.html

JS:   fs.readdirSync("dir")
来源：http://hz.cqqwz.cn/gtyckrlprx.html

TS:   fs.readdirSync("dir")
来源：http://hz.iojbl.cn/gtinnztkuv.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yuanzhike.top/gtavzchxfk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.gogol.net.cn/gtwnebddxh.html

Ruby: Dir.children("dir")
来源：http://hz.zhongyouzk.top/gtcqagojyn.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zdqjudy.top/gtoffbbwas.html

[F09] 获取文件大小
来源：http://hz.jianghu66.top/gtgwtnpend.html

Py:   os.path.getsize("a.txt")
来源：http://hz.ppjwa.cn/gtvelvmvyt.html

PHP:  filesize("a.txt");
来源：http://hz.jianghu66.top/gtpqhrkqyc.html

JS:   fs.statSync("a.txt").size
来源：http://hz.hnxiangtu.top/gtqlrfvpic.html

TS:   fs.statSync("a.txt").size
来源：http://hz.wangshuangyany.cn/gtveqevwfu.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zhiwuduotai.top/gtwulptygf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jlsjyb.cn/gtvrynfmax.html

Ruby: File.size("a.txt")
来源：http://hz.snrcjt.cn/gtfjlivmnr.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yj202588.top/gtkulxerci.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.fengsongda.top/gttboxhmql.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtbynwjnxs.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.chenzaomai.com/gtdzfzloke.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.sysykeji.top/gttsstqfwa.html

TS:   path.extname("a.txt")
来源：http://hz.nanxinkj.top/gtkozorcex.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.guowangkeji.top/gtrokjnpaw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yueranfly.top/gtnrasubua.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.cashguo.top/gtpfhuixnu.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.hnqzz.top/gtreeuutip.html

[F11] 复制与移动文件
来源：http://hz.zdqjudy.top/gtjtwzhbqp.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.fzhhl.top/gtzzvlbxmh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jianghu66.top/gtruivlsug.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.cucudq.cn/gtvhxqjoxj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shzxlz.cn/gtixelrgmo.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.chenlongwang.top/gtcjexhfmf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.zhoulong.xyz/gtwtaadoqp.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.fengsongda.top/gtxnzvdcip.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ppjwa.cn/gtdcqmagon.html

[F12] CSV 读写
来源：http://hz.jinqigfzy.top/gtaemfctyf.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.wangshuangyany.cn/gtzdauqkvo.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.iojbl.cn/gtcruinzzd.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.fzhhl.top/gtjbhvufun.html

TS:   // 同上
来源：http://hz.zycfv.cn/gtgvvzmcsg.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yvedp.cn/gtaffuincd.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.birdmap.top/gtczeaupnt.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ivvv.top/gtkfmktmgb.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jinghuilouyu.cn/gtrricydmc.html

================================================================================
来源：http://hz.yangfankeji.com/gtwcwereca.html

G. 面向对象
来源：http://hz.sufxvd.cn/gtfadhymmx.html

================================================================================
来源：http://hz.jlsjyb.cn/gtbzhwgpha.html

[G01] 定义类
来源：http://hz.hywenlv.cn/gtnvnqiuud.html

Py:   class User: pass
来源：http://hz.feifeiyinyue.top/gtfrsvzcby.html

PHP:  class User {}
来源：http://hz.52xcode.cn/gtxmitsfxb.html

JS:   class User {}
来源：http://hz.smart0.xyz/gtexdibzzl.html

TS:   class User { name: string = ""; }
来源：http://hz.jiagoushi.top/gtcjqsqmyt.html

Java: class User {}
来源：http://hz.zhixingplan.top/gtxpqyldyt.html

Go:   type User struct { Name string }
来源：http://hz.hfpthk.cn/gtwkkgwous.html

Ruby: class User; end
来源：http://hz.fzhhl.top/gtferslnrh.html

C#:   class User {}
来源：http://hz.pycfn.com/gtufpimobh.html

[G02] 构造函数
来源：http://hz.guannengcc.top/gtqpaijmho.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.vqdsnc.cn/gtfltkgelx.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.nanxuanxn.top/gtolcyxrsz.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.hysaishi.cn/gtvtaraojm.html

TS:   constructor(public name: string) {}
来源：http://hz.feifeiyinyue.top/gtropamqhp.html

Java: User(String name) { this.name = name; }
来源：http://hz.mhx1999.top/gtvecqljlq.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.pengpengdd.cyou/gtvxbbglmr.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.feifeiyinyue.top/gtvubmvtgv.html

C#:   public User(string name) { Name = name; }
来源：http://hz.gotoacloud.top/gtcfqvogjh.html

[G03] 实例属性
来源：http://hz.fzhhl.top/gthhtbxwne.html

Py:   self.name = "x"
来源：http://hz.yangfankeji.com/gtkfqvossl.html

PHP:  public string $name = "x";
来源：http://hz.hfpthk.cn/gtsmdvchvj.html

JS:   this.name = "x";
来源：http://hz.sysykeji.top/gtssbgtynh.html

TS:   name: string = "x";
来源：http://hz.feifeiyinyue.top/gtmdfotjgg.html

Java: private String name;
来源：http://hz.zdqjudy.top/gtuordlfys.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.aizwys.cn/gtdgzhwehl.html

Ruby: @name = "x"
来源：http://hz.yanxiufei.cn/gtqtlafgtf.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.zhongyouzk.top/gtmmdxbncx.html

[G04] 定义方法
来源：http://hz.jinyuanbaomall.cn/gtmxshondw.html

Py:   def greet(self): return self.name
来源：http://hz.havefunace.top/gtisuzxarx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hnxiangtu.top/gtlwjprlpy.html

JS:   greet() { return this.name; }
来源：http://hz.yuxming.cn/gtuuoacpqt.html

TS:   greet(): string { return this.name; }
来源：http://hz.haohaochexian.top/gtsolbnooa.html

Java: String greet() { return name; }
来源：http://hz.hywenlv.cn/gtepswpocp.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jiagoushi.top/gttgonuvia.html

Ruby: def greet; @name; end
来源：http://hz.gogol.net.cn/gtfrrbxrcj.html

C#:   public string Greet() => Name;
来源：http://hz.yangfankeji.com/gtlykeuhmo.html

[G05] 继承
来源：http://hz.9152youxi.cn/gttktittvh.html

Py:   class Admin(User): pass
来源：http://hz.xuanzx.com/gtvmqmjpke.html

PHP:  class Admin extends User {}
来源：http://hz.xingfuxueyuan.xyz/gtdwxyqeua.html

JS:   class Admin extends User {}
来源：http://hz.nanxuanxn.top/gtuvepviic.html

TS:   class Admin extends User {}
来源：http://hz.haohaochexian.top/gtubadixsd.html

Java: class Admin extends User {}
来源：http://hz.shzxlz.cn/gtcrjiwiap.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yueranfly.top/gtnsjmfkbi.html

Ruby: class Admin < User; end
来源：http://hz.yonumen.top/gtokcuuute.html

C#:   class Admin : User {}
来源：http://hz.yangfankeji.com/gtlklyifej.html

[G06] 重写方法
来源：http://hz.chenlongwang.top/gtxuuoyazb.html

Py:   def greet(self): return "admin"
来源：http://hz.iojbl.cn/gtfggornyn.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.sysykeji.top/gtujfrgeqq.html

JS:   greet() { return "admin"; }
来源：http://hz.ehwqpu.com/gttpsimsac.html

TS:   greet(): string { return "admin"; }
来源：http://hz.havefunace.top/gteaukqnqf.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yj202588.top/gtnnnfteln.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.guowangkeji.top/gttggsimqq.html

Ruby: def greet; "admin"; end
来源：http://hz.cheryme.top/gtjuvouygo.html

C#:   public override string Greet() => "admin";
来源：http://hz.ywan-chungtsiang.top/gtduxitbrk.html

[G07] 调用父类方法
来源：http://hz.hnqzz.top/gttlycaivx.html

Py:   super().greet()
来源：http://hz.ydjk.org.cn/gtvildbecj.html

PHP:  parent::greet();
来源：http://hz.yuxming.cn/gtyeilpote.html

JS:   super.greet();
来源：http://hz.zhongyouzk.top/gtpssxytzn.html

TS:   super.greet();
来源：http://hz.zhiwuduotai.top/gtsmwwxvhb.html

Java: super.greet();
来源：http://hz.zhongyouzk.top/gtsneayzyq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.gaohongyu789.top/gtsksolawv.html

Ruby: super
来源：http://hz.wangshuangyany.cn/gtwabvfqyr.html

C#:   base.Greet();
来源：http://hz.sysykeji.top/gtkfrpnhuj.html

[G08] 静态方法与属性
来源：http://hz.bjfxy.top/gtybdfzwfl.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.shuidangran.top/gtaxfxuftt.html

PHP:  public static function f() {}
来源：http://hz.andypj.xyz/gtnegivime.html

JS:   static f() {}
来源：http://hz.zhaomingkeji.xyz/gtjcluzhjt.html

TS:   static f(): void {}
来源：http://hz.jinyuanbaomall.cn/gtduqqqlmm.html

Java: static void f() {}
来源：http://hz.kuanghao11.cn/gthwymbymk.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.gzhubu.top/gtbgmzuuav.html

Ruby: def self.f; end
来源：http://hz.zycfv.cn/gtvknmodho.html

C#:   public static void F() {}
来源：http://hz.52xcode.cn/gtmqhxquwc.html

[G09] 接口 / 抽象类
来源：http://hz.aibaodan.cn/gtvpukwety.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.hfpthk.cn/gtwobmdyll.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.guowangkeji.top/gtgnukhchb.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.shanyushiyangkeji.top/gtltfckgjy.html

TS:   interface Shape { area(): number; }
来源：http://hz.zhixingplan.top/gtzyooirnu.html

Java: interface Shape { double area(); }
来源：http://hz.guowangkeji.top/gtxgqtbrpe.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yvedp.cn/gtgpeprmko.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.gaohongyu789.top/gtrpnkmexe.html

C#:   interface IShape { double Area(); }
来源：http://hz.xingfuxueyuan.xyz/gtcfyuctmh.html

[G10] 访问控制
来源：http://hz.zhijiandao.cn/gtorlpqvdt.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hnxiangtu.top/gttndgkkkr.html

PHP:  public / protected / private
来源：http://hz.svipenyu.cn/gtmkvhubhy.html

JS:   #private 字段；其余公开
来源：http://hz.jianghu66.top/gtaicfhkye.html

TS:   public / protected / private
来源：http://hz.xinyue.icu/gtosnyuhsg.html

Java: public / protected / private / 默认包级
来源：http://hz.zhengqikj.top/gtlbujuoiq.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.chenlongwang.top/gtzjkbcabo.html

Ruby: public / protected / private
来源：http://hz.chenjidiqi.icu/gtnnzhkjbs.html

C#:   public / protected / private / internal
来源：http://hz.zhijiandao.cn/gtthezedmm.html

[G11] getter / setter
来源：http://hz.smart0.xyz/gtjxtdsadn.html

Py:   @property 与 @x.setter
来源：http://hz.zdqjudy.top/gtjetfkpur.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.haohaochexian.top/gtgexzmkwc.html

JS:   get name() { return this._name; }
来源：http://hz.hfpthk.cn/gtufbyqkcc.html

TS:   get name(): string { return this._name; }
来源：http://hz.gotoacloud.top/gtrbvkkjml.html

Java: public String getName() { return name; }
来源：http://hz.guannengcc.top/gtiphqyuyu.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.zhijiandao.cn/gtomwlzzit.html

Ruby: attr_accessor :name
来源：http://hz.hongshengwenyu.top/gtkymhilpd.html

C#:   public string Name { get; set; }
来源：http://hz.jlsjyb.cn/gtypcnmspx.html

[G12] 对象转字符串
来源：http://hz.aizwys.cn/gtacoethzj.html

Py:   def __str__(self): return self.name
来源：http://hz.fzhhl.top/gtxvaqppib.html


<!-- 参考信息 -->