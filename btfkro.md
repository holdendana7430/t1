代发 wailian999

[E14] URL 编码与 Base64
来源：http://hz.chenzaomai.com/gtuekugyhv.html

Py:   urllib.parse.quote(s);  base64.b64encode(b).decode()
来源：http://hz.zhongyouzk.top/gtityqgoey.html

PHP:  urlencode($s);  base64_encode($s);
来源：http://hz.zhaomingkeji.xyz/gtvxdpcins.html

JS:   encodeURIComponent(s);  btoa(s);  atob(b64)
来源：http://hz.yj202588.top/gttzfqhkak.html

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.yj202588.top/gtwyfrhxaf.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.daria6918.cn/gtgasovzts.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.cheryme.top/gtgbxmzgxh.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.hfpthk.cn/gtehfisyns.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.smart0.xyz/gtydrmwspy.html

[E15] HTML 转义 / 反转义
来源：http://hz.jqgufenzy.top/gtzetqzsmt.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.xuetiantiany.cn/gtpzfkaqfb.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jyoumei.cn/gtlrtkljce.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.yonumen.top/gtcovjsntj.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.havefunace.top/gtqpimhalh.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.aibaodan.cn/gtrovwkzvh.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yongpay.top/gtuyaczfjv.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jqgfzy.top/gtdflmhqka.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.yueranfly.top/gteczworgn.html

[E16] 数字千分位
来源：http://hz.smart0.xyz/gtjfksyfew.html

Py:   f"{1234567:,}"
来源：http://hz.ppjwa.cn/gtvfinioge.html

PHP:  number_format(1234567);
来源：http://hz.pycfn.com/gtafrqpjqe.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.aibaodan.cn/gtwinlmkwv.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.jinghuilouyu.cn/gtykfowtwb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.gzhubu.top/gtosemzvju.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.tianlin.xyz/gttagkdjup.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.sysykeji.top/gtfohiywxa.html

C#:   1234567.ToString("N0")
来源：http://hz.zhijiandao.cn/gtjfotsdnn.html

[E17] 首字母大写
来源：http://hz.redwolf501.top/gtbngkysup.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.zhaomingkeji.xyz/gtxtdvecjj.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.hnqzz.top/gtdgwkucjj.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zdqjudy.top/gtqbdxlnqa.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.c1oappe.top/gtdbbsdzhd.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.zhijiandao.cn/gtetenigji.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.ivvv.top/gtfnbsbpik.html

Ruby: s.capitalize
来源：http://hz.hammf.cn/gtsskhusqw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.sufxvd.cn/gtwxoyrfre.html

[E18] 模板占位符替换
来源：http://hz.nanxinkj.top/gtxfulxsps.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yuanzhike.top/gtkuzbydqb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.bjfxy.top/gtgvbelhsq.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.dashuyun.cn/gtqvewtzkk.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.quarkkingdee.top/gtjesffecm.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.zhaomingkeji.xyz/gtgbabguri.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yongpay.top/gtsfbkznui.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.ivvv.top/gtjkbsdwzd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.smart0.xyz/gtrkufvmyc.html

[E19] 多行文本按行拆分
来源：http://hz.gaohongyu789.top/gtfebvjnhp.html

Py:   s.splitlines()
来源：http://hz.cucudq.cn/gtiehhexrw.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.cqqwz.cn/gtirnmewxa.html

JS:   s.split(/\r?\n/)
来源：http://hz.xuanzx.com/gtqugailap.html

TS:   s.split(/\r?\n/)
来源：http://hz.havefunace.top/gtrqazjyhf.html

Java: s.lines().toList()
来源：http://hz.hnqzz.top/gtnvpssbzp.html

Go:   strings.Split(s, "\n")
来源：http://hz.jqgufenzy.top/gtmxzhnxmo.html

Ruby: s.lines
来源：http://hz.cdnleiting.top/gtkllfwdjg.html

C#:   s.Split('\n')
来源：http://hz.yvedp.cn/gtzmmjtlag.html

[E20] 判断字符串是否为空
来源：http://hz.zhijiandao.cn/gttprrsouw.html

Py:   if not s:
来源：http://hz.tian-w.cn/gtwiyoaljl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.shanyushiyangtech.top/gtgwiupfpb.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.kuanghao11.cn/gttyvjvtoh.html

TS:   if (s === "") {}
来源：http://hz.daxiang520.top/gtenkeptdb.html

Java: if (s.isEmpty()) {}
来源：http://hz.jyoumei.cn/gttgrnzbvi.html

Go:   if s == "" {}
来源：http://hz.sufxvd.cn/gtgetozwop.html

Ruby: if s.empty?
来源：http://hz.zhijiandao.cn/gtuogxivjf.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.cdnleiting.top/gtxxdujhbs.html

[E21] 超长截断加省略号
来源：http://hz.yj202588.top/gtodhbbvis.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.jlsjyb.cn/gtewzgdgdu.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zhoulong.xyz/gtuwybejof.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.quarkkingdee.top/gtprwjdzje.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.tianlin.xyz/gttgpqjltt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.aizwys.cn/gtcllswijl.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.xingfuxueyuan.xyz/gtxgbzvnsi.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yvedp.cn/gtzzkmeqit.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.jyoumei.cn/gtbaixewhg.html

[E22] 字节长度与字符长度
来源：http://hz.zdqjudy.top/gtticjctvt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.nwbrower.top/gtwlvljfqo.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.shanyushiyangkeji.top/gtsphcafab.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hnxiangtu.top/gtjinkpxir.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.nanxuanxn.top/gttdwvjcrf.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.nanxuanxn.top/gtudlnwkua.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yj202588.top/gtfjditjya.html

Ruby: s.bytesize;  s.length
来源：http://hz.jyoumei.cn/gtgrakilmw.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.meibo888.top/gtlfpndhfh.html

================================================================================
来源：http://hz.zycfv.cn/gtsirutxpc.html

F. 文件与目录
来源：http://hz.fengsongda.top/gtyousvkbx.html

================================================================================
来源：http://hz.dashuyun.cn/gtnmgidnsy.html

[F01] 读取整个文件
来源：http://hz.shangyingyoupin.top/gtgeuautky.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.smart0.xyz/gtumugaxht.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jinqigfzy.top/gtafsuejnp.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.gaohongyu789.top/gthkbnqxzb.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.9152youxi.cn/gtfpcglbid.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.xingfuxueyuan.xyz/gtztzlyzaz.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.xylfe.cn/gtfnsgaqpv.html

Ruby: File.read("a.txt")
来源：http://hz.jiagoushi.top/gtritbfbeg.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.feifeiyinyue.top/gtzqkpykyo.html

[F02] 逐行读取文件
来源：http://hz.yvedp.cn/gtzorcwjvy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zhixingplan.top/gtwqwavewi.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.gogol.net.cn/gthylcbsdx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.sxryk.cn/gthtrioatx.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.hongshengwenyu.top/gtrpzauspi.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zhijiandao.cn/gtxcttysyk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.xuetiantiany.cn/gtwryitena.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.zhijiandao.cn/gtihuxdxgb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.jianghu66.top/gtswpldjdp.html

[F03] 写入文件（覆盖）
来源：http://hz.tanke756.top/gtzbnfoemj.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.kuanghao11.cn/gtlkuwnkpn.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.gogol.net.cn/gtgyuvphzm.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jqgufenzy.top/gtvjnrdpll.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ehwqpu.com/gtrwfrofta.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.316326.xyz/gteawcxwrr.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.daxiang520.top/gtrpygedex.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jinghuilouyu.cn/gtsnrbtktc.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.quarkkingdee.top/gtvtcszvaa.html

[F04] 追加写入文件
来源：http://hz.yonumen.top/gtyofgtiwy.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.hysaishi.cn/gtpgrrxals.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.gaohongyu789.top/gtwgbvmecs.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.tanke756.top/gtvwgvahod.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zycfv.cn/gtnajqixcx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.sysykeji.top/gterbphyap.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.quarkkingdee.top/gtgbkrmsfs.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.ywan-chungtsiang.top/gteiinefcj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.hysaishi.cn/gtewbhekuj.html

[F05] 判断文件或目录是否存在
来源：http://hz.nanxinkj.top/gtuqhemelh.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.hammf.cn/gtilevxhuc.html

PHP:  file_exists("a.txt");
来源：http://hz.zhoulong.xyz/gtfwuzahcg.html

JS:   fs.existsSync("a.txt")
来源：http://hz.hysaishi.cn/gtyfokwlqd.html

TS:   fs.existsSync("a.txt")
来源：http://hz.hongshengwenyu.top/gtvdbcgbrg.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.dianchejie.cn/gtjulbcowe.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.zhaomingkeji.xyz/gtnobkypib.html

Ruby: File.exist?("a.txt")
来源：http://hz.tian-w.cn/gtijlywwyo.html

C#:   File.Exists("a.txt")
来源：http://hz.hysaishi.cn/gtgadxvecz.html

[F06] 删除文件
来源：http://hz.xingfuxueyuan.xyz/gtkuoktfgr.html

Py:   os.remove("a.txt")
来源：http://hz.jianghu66.top/gtjqvzkvvd.html

PHP:  unlink("a.txt");
来源：http://hz.pengpengdd.cyou/gtenanqsoq.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hnqzz.top/gtfjqwnfnc.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.dashuyun.cn/gtcefyvkhs.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.iojbl.cn/gtceqontyx.html

Go:   os.Remove("a.txt")
来源：http://hz.ydjk.org.cn/gtelwdobbu.html

Ruby: File.delete("a.txt")
来源：http://hz.gogol.net.cn/gtwuksfhbj.html

C#:   File.Delete("a.txt");
来源：http://hz.jinqigfzy.top/gtzmneazhx.html

[F07] 创建目录（含多级）
来源：http://hz.kuanghao11.cn/gthwtknqqb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.quarkkingdee.top/gtxvtffflh.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yj202588.top/gtqnvxjwbe.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.snrcjt.cn/gtufjxgnsc.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.feifeiyinyue.top/gthmdmptvf.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.xuanzx.com/gtpwpbvfxy.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hysaishi.cn/gtowlczgru.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.jyoumei.cn/gtmzvhodgk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.xinyue.icu/gttxjhvsfw.html

[F08] 遍历目录
来源：http://hz.jinqigfzy.top/gtefkjcbji.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.zhijiandao.cn/gtwilmawvl.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.sufxvd.cn/gtxkjsywyq.html

JS:   fs.readdirSync("dir")
来源：http://hz.c1oappe.top/gtxqosloak.html

TS:   fs.readdirSync("dir")
来源：http://hz.ivvv.top/gtbewuflal.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.xylfe.cn/gtxjzgbykr.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.gzhubu.top/gthmdjkcnn.html

Ruby: Dir.children("dir")
来源：http://hz.tian-w.cn/gtwbfinpgz.html

C#:   Directory.GetFiles("dir")
来源：http://hz.chenzaomai.com/gtxroippbu.html

[F09] 获取文件大小
来源：http://hz.xylfe.cn/gtkbjsplew.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jiagoushi.top/gtxucyizzb.html

PHP:  filesize("a.txt");
来源：http://hz.nwbrower.top/gttslidlbv.html

JS:   fs.statSync("a.txt").size
来源：http://hz.snrcjt.cn/gtrqacmqao.html

TS:   fs.statSync("a.txt").size
来源：http://hz.birdmap.top/gtxvyryltb.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.zhijiandao.cn/gtcgbidwvq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.ywan-chungtsiang.top/gtdehjnvyo.html

Ruby: File.size("a.txt")
来源：http://hz.sweek.top/gtxxnzewuo.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.yangfankeji.com/gtbziqamhn.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.dashuyun.cn/gtvfhobymv.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.yueranfly.top/gtbzauacwr.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.c1oappe.top/gtzsiawesh.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.gotoacloud.top/gtxtadqnro.html

TS:   path.extname("a.txt")
来源：http://hz.cheryme.top/gtettweimf.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.zhengqikj.top/gtqqjwfnhk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhiwuduotai.top/gtuaokuhxr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.cqqwz.cn/gttgxeuxqc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jyoumei.cn/gtkeiiwbty.html

[F11] 复制与移动文件
来源：http://hz.shuidangran.top/gtderclirj.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.sweek.top/gtuaojglrh.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.cqqwz.cn/gtdiqtifiv.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ivvv.top/gtizppzrxi.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.ybcxt.top/gtphxfggdx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.gaohongyu789.top/gtrlpbmtiy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.shzxlz.cn/gtoaashoxb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.feifeiyinyue.top/gtmficubtn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.wangshuangyany.cn/gtwldxgtgc.html

[F12] CSV 读写
来源：http://hz.hammf.cn/gtkgsejyym.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.hnxiangtu.top/gtedmetrln.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.ydzc1.top/gtyzsvdesq.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jinqigfzy.top/gtpofebvqr.html

TS:   // 同上
来源：http://hz.snrcjt.cn/gtpkkfecnr.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.feifeiyinyue.top/gtdmtwrykq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.ehwqpu.com/gtidwwrgfx.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yuanzhike.top/gterbulwfa.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.hnxiangtu.top/gtsxrnames.html

================================================================================
来源：http://hz.sxryk.cn/gtnbgulebg.html

G. 面向对象
来源：http://hz.yangfankeji.com/gtpukfjvqj.html

================================================================================
来源：http://hz.zhengqikj.top/gtxievjvgu.html

[G01] 定义类
来源：http://hz.shuidangran.top/gtggpbqyxo.html

Py:   class User: pass
来源：http://hz.yonumen.top/gtgfhrbvwd.html

PHP:  class User {}
来源：http://hz.vqdsnc.cn/gtqfxqiatm.html

JS:   class User {}
来源：http://hz.yongpay.top/gtwpyeeyqk.html

TS:   class User { name: string = ""; }
来源：http://hz.hnqzz.top/gtbuhhzqwt.html

Java: class User {}
来源：http://hz.jinqigfzy.top/gtvcovqfnx.html

Go:   type User struct { Name string }
来源：http://hz.shanyushiyangtech.top/gtbjinvelk.html

Ruby: class User; end
来源：http://hz.tianlin.xyz/gtvgzmmquo.html

C#:   class User {}
来源：http://hz.guannengcc.top/gtkexybfqk.html

[G02] 构造函数
来源：http://hz.yj202588.top/gtqkszswkg.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yanxiufei.cn/gthmtkuqnr.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.nanxuanxn.top/gtpybuavhr.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.mhx1999.top/gtmxjninnj.html

TS:   constructor(public name: string) {}
来源：http://hz.kuanghao11.cn/gtjvmyueqm.html

Java: User(String name) { this.name = name; }
来源：http://hz.zhoulong.xyz/gtcvwkfspy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.nwbrower.top/gtnehyqdlj.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.cashguo.top/gtuvomzgcz.html

C#:   public User(string name) { Name = name; }
来源：http://hz.shzxlz.cn/gtfxalskuh.html

[G03] 实例属性
来源：http://hz.ybcxt.top/gtheanqhyx.html

Py:   self.name = "x"
来源：http://hz.yongpay.top/gtgpczabwk.html

PHP:  public string $name = "x";
来源：http://hz.jiagoushi.top/gtsputziam.html

JS:   this.name = "x";
来源：http://hz.nwbrower.top/gttswbjpsg.html

TS:   name: string = "x";
来源：http://hz.ppjwa.cn/gtclsglbka.html

Java: private String name;
来源：http://hz.guowangkeji.top/gttjupgltn.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.ydzc1.top/gtycqbvitc.html

Ruby: @name = "x"
来源：http://hz.xuetiantiany.cn/gtflymunsn.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.aibaodan.cn/gtkwcmuxal.html

[G04] 定义方法
来源：http://hz.cucudq.cn/gtlemkzmxn.html

Py:   def greet(self): return self.name
来源：http://hz.wangdashe.top/gtiqxxrxhj.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.xziqi.cn/gtjqopdejd.html

JS:   greet() { return this.name; }
来源：http://hz.andypj.xyz/gtalfxfapd.html

TS:   greet(): string { return this.name; }
来源：http://hz.nwbrower.top/gtaubuwbix.html

Java: String greet() { return name; }
来源：http://hz.shanyushiyangtech.top/gtxmtgznnv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.bjfxy.top/gtzfrgbbwt.html

Ruby: def greet; @name; end
来源：http://hz.ppjwa.cn/gtzcsxaikj.html

C#:   public string Greet() => Name;
来源：http://hz.jinghuilouyu.cn/gtutwhrnlh.html

[G05] 继承
来源：http://hz.zhengqikj.top/gtrhxyeusg.html

Py:   class Admin(User): pass
来源：http://hz.xziqi.cn/gtooixuzct.html

PHP:  class Admin extends User {}
来源：http://hz.mhx1999.top/gtsnhfllme.html

JS:   class Admin extends User {}
来源：http://hz.gotoacloud.top/gtbptstlpz.html

TS:   class Admin extends User {}
来源：http://hz.yj202588.top/gtcounvdie.html

Java: class Admin extends User {}
来源：http://hz.yueranfly.top/gthjptxkcz.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.316326.xyz/gtjlhfnfzd.html

Ruby: class Admin < User; end
来源：http://hz.hnqzz.top/gtazwldnzo.html

C#:   class Admin : User {}
来源：http://hz.hywenlv.cn/gtlrhxdwyo.html

[G06] 重写方法
来源：http://hz.zhiwuduotai.top/gtdrcxevta.html

Py:   def greet(self): return "admin"
来源：http://hz.tian-w.cn/gtfnkihvlb.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.mhx1999.top/gtyrthppru.html

JS:   greet() { return "admin"; }
来源：http://hz.sufxvd.cn/gtyfumsphm.html

TS:   greet(): string { return "admin"; }
来源：http://hz.guannengcc.top/gtegjtlnbs.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.316326.xyz/gtexagcblg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.aibaodan.cn/gtojhkffok.html

Ruby: def greet; "admin"; end
来源：http://hz.yuanzhike.top/gtxlrkmjdi.html

C#:   public override string Greet() => "admin";
来源：http://hz.tian-w.cn/gtgljkubgb.html

[G07] 调用父类方法
来源：http://hz.pycfn.com/gtnrsqfqic.html

Py:   super().greet()
来源：http://hz.jinghuilouyu.cn/gtgiqiqrlc.html

PHP:  parent::greet();
来源：http://hz.tanke756.top/gtjtsdlygc.html

JS:   super.greet();
来源：http://hz.hywenlv.cn/gtyieqgyyq.html

TS:   super.greet();
来源：http://hz.ydzc1.top/gtfhvbgvak.html

Java: super.greet();
来源：http://hz.hysaishi.cn/gtyqrtpqbi.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.meibo888.top/gtlgyeicno.html

Ruby: super
来源：http://hz.ydjk.org.cn/gtxlmawwvy.html

C#:   base.Greet();
来源：http://hz.ybcxt.top/gtxvfiytyr.html

[G08] 静态方法与属性
来源：http://hz.jqgufenzy.top/gtoywaxrfz.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yueranfly.top/gtwnqwjuqa.html

PHP:  public static function f() {}
来源：http://hz.jqgufenzy.top/gtibueaauq.html

JS:   static f() {}
来源：http://hz.chenzaomai.com/gtgyokufsf.html

TS:   static f(): void {}
来源：http://hz.zhixingplan.top/gtyiksfijj.html

Java: static void f() {}
来源：http://hz.9152youxi.cn/gtcwdvjrpz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.chenzaomai.com/gtmsjjkoas.html

Ruby: def self.f; end
来源：http://hz.zhengqikj.top/gtdkcwucbh.html

C#:   public static void F() {}
来源：http://hz.yvedp.cn/gtekqnuhnr.html

[G09] 接口 / 抽象类
来源：http://hz.hysaishi.cn/gtivzddcdb.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.c1oappe.top/gtrwmcvazc.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.cdnleiting.top/gtnpsfetdi.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.chenzaomai.com/gtynooqglh.html

TS:   interface Shape { area(): number; }
来源：http://hz.havefunace.top/gtqnnhgqkn.html

Java: interface Shape { double area(); }
来源：http://hz.xziqi.cn/gtrgargtdo.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.ivvv.top/gtehrkstdd.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jiagoushi.top/gthdzbbaah.html

C#:   interface IShape { double Area(); }
来源：http://hz.cqqwz.cn/gtovudhfbt.html

[G10] 访问控制
来源：http://hz.jianghu66.top/gtazwsujnu.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.ivvv.top/gtqpihhmcm.html

PHP:  public / protected / private
来源：http://hz.hfpthk.cn/gtycayqqdk.html

JS:   #private 字段；其余公开
来源：http://hz.jqgufenzy.top/gtollnlklf.html

TS:   public / protected / private
来源：http://hz.hnqzz.top/gtprgemqkz.html

Java: public / protected / private / 默认包级
来源：http://hz.havefunace.top/gtzxqgwnvj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.feifeiyinyue.top/gtuwhstxol.html

Ruby: public / protected / private
来源：http://hz.kuanghao11.cn/gtkzbpfaom.html

C#:   public / protected / private / internal
来源：http://hz.xuanzx.com/gtnexeposx.html

[G11] getter / setter
来源：http://hz.jianghu66.top/gtoednwbwk.html

Py:   @property 与 @x.setter
来源：http://hz.dashuyun.cn/gtnvuowxal.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.andypj.xyz/gtabvwdzmx.html

JS:   get name() { return this._name; }
来源：http://hz.ywan-chungtsiang.top/gtavgqkyhx.html

TS:   get name(): string { return this._name; }
来源：http://hz.chenjidiqi.icu/gtggruixpv.html

Java: public String getName() { return name; }
来源：http://hz.sxryk.cn/gtpgqsqwpw.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yuxming.cn/gtmchwiyep.html

Ruby: attr_accessor :name
来源：http://hz.sweek.top/gtfffqovde.html

C#:   public string Name { get; set; }
来源：http://hz.sweek.top/gteyjsqfmh.html

[G12] 对象转字符串
来源：http://hz.hysaishi.cn/gtohplurdz.html

Py:   def __str__(self): return self.name
来源：http://hz.jqgufenzy.top/gtqaththaj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.chenjidiqi.icu/gtwfugrstb.html

JS:   toString() { return this.name; }
来源：http://hz.jyoumei.cn/gtwmorckxi.html

TS:   toString(): string { return this.name; }
来源：http://hz.birdmap.top/gtxrrbvzhu.html

Java: @Override public String toString() { return name; }
来源：http://hz.ybcxt.top/gtkjmmxrvt.html


<!-- 参考信息 -->