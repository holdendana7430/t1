代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.yanxiufei.cn/gttzhsjbjk.html

[E15] HTML 转义 / 反转义
来源：http://hz.sxryk.cn/gtowyspykf.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.aizwys.cn/gtnqunxdbm.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.jianghu66.top/gtucwpsryq.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.xingfuxueyuan.xyz/gtegvoeyxy.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.guowangkeji.top/gtfvngehja.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.xziqi.cn/gtbzdzurbs.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.gaohongyu789.top/gteouhwlia.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.9152youxi.cn/gtkxbebrra.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.gzhubu.top/gtpiobnvbd.html

[E16] 数字千分位
来源：http://hz.wangshuangyany.cn/gtjyaxigdg.html

Py:   f"{1234567:,}"
来源：http://hz.birdmap.top/gtwxahsofk.html

PHP:  number_format(1234567);
来源：http://hz.hammf.cn/gtspbhpsen.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.dianchejie.cn/gtrmcisuum.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.ydzc1.top/gtnuyauyjt.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.jinqigufen.top/gtcqjqszkm.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.snrcjt.cn/gtmotludva.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.svipenyu.cn/gtblovrobj.html

C#:   1234567.ToString("N0")
来源：http://hz.gotoacloud.top/gteukvecco.html

[E17] 首字母大写
来源：http://hz.nwbrower.top/gtlosguzml.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.xuanzx.com/gtgwpwkiic.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jiagoushi.top/gteemuejbd.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ehwqpu.com/gtprudmnxb.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ydjk.org.cn/gtwbjexdee.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jqgfzy.top/gtakyhrxtm.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.nwbrower.top/gtxoenngxv.html

Ruby: s.capitalize
来源：http://hz.shangyingyoupin.top/gtijslmgik.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.shanyushiyangtech.top/gtnbqoogur.html

[E18] 模板占位符替换
来源：http://hz.yvedp.cn/gtkotzbkul.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.zhaomingkeji.xyz/gthjuclozg.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.xziqi.cn/gtplcxkjgf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.cheryme.top/gtiqygwwuw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.hnxiangtu.top/gtirrctfau.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.fengsongda.top/gthxehmvnl.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.pengpengdd.cyou/gtnqnmvmve.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.pycfn.com/gtqljtkhyu.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.ydjk.org.cn/gtdcmrdvcq.html

[E19] 多行文本按行拆分
来源：http://hz.ivvv.top/gtkveopcdr.html

Py:   s.splitlines()
来源：http://hz.ydzc1.top/gtgnvbvfap.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.wangdashe.top/gtmxkurazq.html

JS:   s.split(/\r?\n/)
来源：http://hz.sweek.top/gtmexixpay.html

TS:   s.split(/\r?\n/)
来源：http://hz.pengpengdd.cyou/gtndmjfcyo.html

Java: s.lines().toList()
来源：http://hz.yj202588.top/gtnsvyzcbv.html

Go:   strings.Split(s, "\n")
来源：http://hz.havefunace.top/gtswvyijva.html

Ruby: s.lines
来源：http://hz.bjfxy.top/gtiyreumrg.html

C#:   s.Split('\n')
来源：http://hz.kuanghao11.cn/gtfjkmrgkb.html

[E20] 判断字符串是否为空
来源：http://hz.xingfuxueyuan.xyz/gtytjqmbvh.html

Py:   if not s:
来源：http://hz.fengsongda.top/gtbitgxtnl.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.jinqigufen.top/gtnulhwmiv.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.9152youxi.cn/gtyoxppgfg.html

TS:   if (s === "") {}
来源：http://hz.fengsongda.top/gtrvtczfwd.html

Java: if (s.isEmpty()) {}
来源：http://hz.gaohongyu789.top/gthibywhqw.html

Go:   if s == "" {}
来源：http://hz.hammf.cn/gtqpjvzfyq.html

Ruby: if s.empty?
来源：http://hz.birdmap.top/gtqemcpfcb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.hammf.cn/gtyqjwkisl.html

[E21] 超长截断加省略号
来源：http://hz.hnxiangtu.top/gtyckawjdt.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.tian-w.cn/gtdhbjjwbb.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.hfpthk.cn/gteazfbfns.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jiagoushi.top/gtsivlvkah.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.pengpengdd.cyou/gthykgryjt.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.bjfxy.top/gtbsqpflds.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.chenzaomai.com/gtpksudurc.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.jinqigfzy.top/gtueoihbzq.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.c1oappe.top/gtiqdzqqrd.html

[E22] 字节长度与字符长度
来源：http://hz.316326.xyz/gthoorjhmn.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.cashguo.top/gtwimkooch.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yanxiufei.cn/gtznrsrnhd.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.chenjidiqi.icu/gtevswdwmo.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.dashuyun.cn/gtotqmeavy.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.aibaodan.cn/gtpvyozqam.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yanxiufei.cn/gtaruibaps.html

Ruby: s.bytesize;  s.length
来源：http://hz.316326.xyz/gtfhkevlon.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.zhongyouzk.top/gtbbngnozk.html

================================================================================
来源：http://hz.ybcxt.top/gtzafvrbea.html

F. 文件与目录
来源：http://hz.pycfn.com/gtvnlpfnzp.html

================================================================================
来源：http://hz.dashuyun.cn/gttwbitgel.html

[F01] 读取整个文件
来源：http://hz.yueranfly.top/gtgqausyjq.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.chenjidiqi.icu/gtwqrofxen.html

PHP:  file_get_contents("a.txt");
来源：http://hz.chenjidiqi.icu/gtqhpbfpac.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zycfv.cn/gtdwbrdvxe.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.ybcxt.top/gtjtsdyowp.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.zhoulong.xyz/gtavpvqgwi.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.yj202588.top/gtaeoxgslh.html

Ruby: File.read("a.txt")
来源：http://hz.wangshuangyany.cn/gtluhkyrhg.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.daxiang520.top/gtiydywski.html

[F02] 逐行读取文件
来源：http://hz.cashguo.top/gtybtxgdsg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jlsjyb.cn/gtlwyesgts.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yvedp.cn/gtswjpmqen.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.sysykeji.top/gtnvrritgt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xylfe.cn/gtuetyqheb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.smart0.xyz/gtwxxdddso.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.zycfv.cn/gtiajszxpm.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.cashguo.top/gticjrtxnk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.guowangkeji.top/gtykrfoonw.html

[F03] 写入文件（覆盖）
来源：http://hz.zhengqikj.top/gtwplgpzex.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yongpay.top/gtavigyosm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.xuanzx.com/gtwewfydjp.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shuidangran.top/gtybzsnxff.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhoulong.xyz/gthqagblhs.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.aibaodan.cn/gtgkcswtpp.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.mhx1999.top/gtrizvcudb.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zdqjudy.top/gtvghicixr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yuanzhike.top/gtrkkzyian.html

[F04] 追加写入文件
来源：http://hz.hysaishi.cn/gtmmxojwfd.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yanxiufei.cn/gtdvhmbvda.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.daria6918.cn/gtmgyxypwj.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.birdmap.top/gtunezahkx.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.nanxinkj.top/gttwdxqrbf.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jlsjyb.cn/gtdshpweks.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.birdmap.top/gtsnvwtqkz.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.nwbrower.top/gtcvaqviai.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.aizwys.cn/gtgkcswfhk.html

[F05] 判断文件或目录是否存在
来源：http://hz.yj20258888.top/gtbboomqfr.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.tanke756.top/gtxlpyshrr.html

PHP:  file_exists("a.txt");
来源：http://hz.dashuyun.cn/gtjyvqeimz.html

JS:   fs.existsSync("a.txt")
来源：http://hz.guowangkeji.top/gtfqcicxzq.html

TS:   fs.existsSync("a.txt")
来源：http://hz.guowangkeji.top/gtyrkwvdol.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.andypj.xyz/gtwtlalfjd.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.xylfe.cn/gtvkpwsfxc.html

Ruby: File.exist?("a.txt")
来源：http://hz.ybcxt.top/gtelbiwjyj.html

C#:   File.Exists("a.txt")
来源：http://hz.mhx1999.top/gtynpmslfm.html

[F06] 删除文件
来源：http://hz.xingfuxueyuan.xyz/gtddhljnwq.html

Py:   os.remove("a.txt")
来源：http://hz.bjfxy.top/gtojckhkge.html

PHP:  unlink("a.txt");
来源：http://hz.shanyushiyangtech.top/gtzmdmqall.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.shzxlz.cn/gtmwbwevxa.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.chenjidiqi.icu/gtiizdtpag.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jqgufenzy.top/gttfpzxdwf.html

Go:   os.Remove("a.txt")
来源：http://hz.hnqzz.top/gtdosndlwm.html

Ruby: File.delete("a.txt")
来源：http://hz.gzhubu.top/gtteghzqpw.html

C#:   File.Delete("a.txt");
来源：http://hz.sufxvd.cn/gtkfdggsrf.html

[F07] 创建目录（含多级）
来源：http://hz.shanyushiyangkeji.top/gtdfxydokn.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.aizwys.cn/gtnxuhwbxj.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jinghuilouyu.cn/gtzeyysoqu.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.fengsongda.top/gtsanrmshx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shzxlz.cn/gthutwphzv.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.cdnleiting.top/gtlqixzjkl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.nwbrower.top/gtrcdnhmav.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.ydzc1.top/gteexwuvrt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.nanxinkj.top/gtmdjawbdg.html

[F08] 遍历目录
来源：http://hz.c1oappe.top/gtfgqmxvex.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.shanyushiyangkeji.top/gtvplabysq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.nanxuanxn.top/gtfytcvaha.html

JS:   fs.readdirSync("dir")
来源：http://hz.fengsongda.top/gtveapnkwn.html

TS:   fs.readdirSync("dir")
来源：http://hz.hysaishi.cn/gthsgyelxs.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.iojbl.cn/gtazlaicjb.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.daxiang520.top/gttltdpwrd.html

Ruby: Dir.children("dir")
来源：http://hz.nanxuanxn.top/gtivlvsovm.html

C#:   Directory.GetFiles("dir")
来源：http://hz.shzxlz.cn/gtvnomhzhh.html

[F09] 获取文件大小
来源：http://hz.hywenlv.cn/gtrvtpkbct.html

Py:   os.path.getsize("a.txt")
来源：http://hz.shuidangran.top/gtsxaeabus.html

PHP:  filesize("a.txt");
来源：http://hz.sxryk.cn/gtvfckpmuc.html

JS:   fs.statSync("a.txt").size
来源：http://hz.pycfn.com/gtkvqhpgvh.html

TS:   fs.statSync("a.txt").size
来源：http://hz.bjfxy.top/gtmuxgomfb.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.sufxvd.cn/gtbbaorliu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.nanxinkj.top/gtmrsxiqtb.html

Ruby: File.size("a.txt")
来源：http://hz.shanyushiyangtech.top/gtobxfaliv.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jinyuanbaomall.cn/gtozgmohnd.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.dashuyun.cn/gtgrjzsgcd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.sxryk.cn/gtaulmjfpo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.fengsongda.top/gttdnclvko.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.aizwys.cn/gtrbkmrvrs.html

TS:   path.extname("a.txt")
来源：http://hz.jianghu66.top/gtmqcfwwvr.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.shangyingyoupin.top/gteytpyzdc.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yvedp.cn/gtymzqcdsp.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jinqigfzy.top/gtvthejimm.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhongyouzk.top/gtbmzxoqvt.html

[F11] 复制与移动文件
来源：http://hz.tianlin.xyz/gtdbodjhrx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.birdmap.top/gtdibzpvvp.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.shangyingyoupin.top/gtmkrejtgh.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.c1oappe.top/gthvkukzlj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hfpthk.cn/gtznaorykr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.cashguo.top/gtgdgsefai.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.snrcjt.cn/gtqxqhgjqs.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.nanxinkj.top/gtczemxnwt.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.guowangkeji.top/gtjihbzwav.html

[F12] CSV 读写
来源：http://hz.hnqzz.top/gtehxggwyz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jinqigfzy.top/gthhzzbyyr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.hnxiangtu.top/gtsljllder.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.c1oappe.top/gtscqkzfla.html

TS:   // 同上
来源：http://hz.shanyushiyangtech.top/gtoffssoho.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.xuanzx.com/gtolqpiyea.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jinyuanbaomall.cn/gtmuihxbht.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.shzxlz.cn/gtabhriuea.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zdqjudy.top/gttoqfzoul.html

================================================================================
来源：http://hz.cheryme.top/gtiyunpygk.html

G. 面向对象
来源：http://hz.guowangkeji.top/gtmnjbysda.html

================================================================================
来源：http://hz.fzhhl.top/gtikznbbkt.html

[G01] 定义类
来源：http://hz.vqdsnc.cn/gtagyliivw.html

Py:   class User: pass
来源：http://hz.dashuyun.cn/gtngptpand.html

PHP:  class User {}
来源：http://hz.ehwqpu.com/gtkgeakmhg.html

JS:   class User {}
来源：http://hz.fengsongda.top/gtyfrduhjc.html

TS:   class User { name: string = ""; }
来源：http://hz.yangfankeji.com/gtxqztpsrh.html

Java: class User {}
来源：http://hz.zhixingplan.top/gtnvxagfzl.html

Go:   type User struct { Name string }
来源：http://hz.smart0.xyz/gtnxrexrvo.html

Ruby: class User; end
来源：http://hz.jinyuanbaomall.cn/gtfebfutvz.html

C#:   class User {}
来源：http://hz.sufxvd.cn/gtlgiuafuq.html

[G02] 构造函数
来源：http://hz.ehwqpu.com/gtbdvsskxa.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.daxiang520.top/gtletmvarq.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.fzhhl.top/gtrlkliups.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.sxryk.cn/gtocjvxyto.html

TS:   constructor(public name: string) {}
来源：http://hz.zhaomingkeji.xyz/gtvhpwrhij.html

Java: User(String name) { this.name = name; }
来源：http://hz.smart0.xyz/gtnoldelxb.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zdqjudy.top/gtgowosyhu.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.sufxvd.cn/gtqilririm.html

C#:   public User(string name) { Name = name; }
来源：http://hz.smart0.xyz/gtutpoanlk.html

[G03] 实例属性
来源：http://hz.xuanzx.com/gtpyxuqyhz.html

Py:   self.name = "x"
来源：http://hz.fzhhl.top/gtfnkcsmwc.html

PHP:  public string $name = "x";
来源：http://hz.aizwys.cn/gtepnkityn.html

JS:   this.name = "x";
来源：http://hz.yangfankeji.com/gtkmnzcksz.html

TS:   name: string = "x";
来源：http://hz.yj20258.top/gtikqznpkb.html

Java: private String name;
来源：http://hz.0kj1m.cn/gtexpkiuip.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.bjfxy.top/gtagchtnuh.html

Ruby: @name = "x"
来源：http://hz.hongshengwenyu.top/gtbensnafl.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.yongpay.top/gtvssgxtgz.html

[G04] 定义方法
来源：http://hz.hnqzz.top/gtseucscik.html

Py:   def greet(self): return self.name
来源：http://hz.zdqjudy.top/gtfbhtkmrk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.xylfe.cn/gtdbznbtps.html

JS:   greet() { return this.name; }
来源：http://hz.cheryme.top/gtttggljcq.html

TS:   greet(): string { return this.name; }
来源：http://hz.cucudq.cn/gtblalfwyg.html

Java: String greet() { return name; }
来源：http://hz.xinyue.icu/gtuxlmyoyc.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zhoulong.xyz/gtxsoldunn.html

Ruby: def greet; @name; end
来源：http://hz.jqgufenzy.top/gtejamsyxg.html

C#:   public string Greet() => Name;
来源：http://hz.cashguo.top/gtizhlaxwu.html

[G05] 继承
来源：http://hz.xingfuxueyuan.xyz/gtlyqzbgdg.html

Py:   class Admin(User): pass
来源：http://hz.hammf.cn/gtsduayppe.html

PHP:  class Admin extends User {}
来源：http://hz.9152youxi.cn/gtkcpuvoam.html

JS:   class Admin extends User {}
来源：http://hz.ehwqpu.com/gtzhltblog.html

TS:   class Admin extends User {}
来源：http://hz.sysykeji.top/gtgsptjmhi.html

Java: class Admin extends User {}
来源：http://hz.havefunace.top/gtacdierff.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.52xcode.cn/gtdzeezuzn.html

Ruby: class Admin < User; end
来源：http://hz.jianghu66.top/gtirwtclqo.html

C#:   class Admin : User {}
来源：http://hz.daxiang520.top/gthyuhkcoo.html

[G06] 重写方法
来源：http://hz.feifeiyinyue.top/gtsjcfplab.html

Py:   def greet(self): return "admin"
来源：http://hz.cdnleiting.top/gtplxounyw.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.gotoacloud.top/gtfoqfuaqk.html

JS:   greet() { return "admin"; }
来源：http://hz.jinyuanbaomall.cn/gtnhdkqabf.html

TS:   greet(): string { return "admin"; }
来源：http://hz.kuanghao11.cn/gtgzsxtyjg.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.jinqigufen.top/gtqtynihsj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.nwbrower.top/gttbmwqxpg.html

Ruby: def greet; "admin"; end
来源：http://hz.xuetiantiany.cn/gtxqnuzewp.html

C#:   public override string Greet() => "admin";
来源：http://hz.yj20258.top/gtbjjtbvvi.html

[G07] 调用父类方法
来源：http://hz.xylfe.cn/gtnnlwhoxv.html

Py:   super().greet()
来源：http://hz.9152youxi.cn/gtyqrecsdf.html

PHP:  parent::greet();
来源：http://hz.yj20258.top/gtncomcqed.html

JS:   super.greet();
来源：http://hz.52xcode.cn/gtxfljlpdb.html

TS:   super.greet();
来源：http://hz.jqgufenzy.top/gtpnkksmun.html

Java: super.greet();
来源：http://hz.zhixingplan.top/gtfyrelsnn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.nanxinkj.top/gtzeayecsy.html

Ruby: super
来源：http://hz.daria6918.cn/gtbinpkwke.html

C#:   base.Greet();
来源：http://hz.zdqjudy.top/gteujttrpk.html

[G08] 静态方法与属性
来源：http://hz.jqgufenzy.top/gtuxvdwhyo.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.cashguo.top/gtztnuvdsn.html

PHP:  public static function f() {}
来源：http://hz.xuanzx.com/gtpukfsgjk.html

JS:   static f() {}
来源：http://hz.dashuyun.cn/gtwgfryupf.html

TS:   static f(): void {}
来源：http://hz.zhoulong.xyz/gtmztftaii.html

Java: static void f() {}
来源：http://hz.feifeiyinyue.top/gtsyzjzrli.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.cqqwz.cn/gttkpmnwyg.html

Ruby: def self.f; end
来源：http://hz.jinqigufen.top/gtesgvkmvx.html

C#:   public static void F() {}
来源：http://hz.yueranfly.top/gttzzimgwm.html

[G09] 接口 / 抽象类
来源：http://hz.gotoacloud.top/gtnaaxmxjh.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.shuidangran.top/gtbsppvodu.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.daria6918.cn/gtbzrniyhr.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.tanke756.top/gtdcshdzhe.html

TS:   interface Shape { area(): number; }
来源：http://hz.bjfxy.top/gtjwpzqrwa.html

Java: interface Shape { double area(); }
来源：http://hz.tian-w.cn/gtnfyjcqfu.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yj20258.top/gtkmbzvbbk.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jlsjyb.cn/gtrympghcx.html

C#:   interface IShape { double Area(); }
来源：http://hz.c1oappe.top/gtpxxkgscn.html

[G10] 访问控制
来源：http://hz.yongpay.top/gtfrbtyrzz.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.316326.xyz/gthyphchfz.html

PHP:  public / protected / private
来源：http://hz.jianghu66.top/gtxcxnefwf.html

JS:   #private 字段；其余公开
来源：http://hz.shuidangran.top/gtonmysijp.html

TS:   public / protected / private
来源：http://hz.shangyingyoupin.top/gtwfkwgzoy.html

Java: public / protected / private / 默认包级
来源：http://hz.cheryme.top/gtnelhzwkw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.316326.xyz/gtzaeblfxx.html

Ruby: public / protected / private
来源：http://hz.fzhhl.top/gtltmsetwe.html

C#:   public / protected / private / internal
来源：http://hz.iojbl.cn/gtwyqhnigk.html

[G11] getter / setter
来源：http://hz.jinyuanbaomall.cn/gtprhvltxj.html

Py:   @property 与 @x.setter
来源：http://hz.pengpengdd.cyou/gtpsqweqka.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yvedp.cn/gtwtgnwfpa.html

JS:   get name() { return this._name; }
来源：http://hz.ybcxt.top/gtcswogwiw.html

TS:   get name(): string { return this._name; }
来源：http://hz.svipenyu.cn/gtuxsqtpxc.html

Java: public String getName() { return name; }
来源：http://hz.zhengqikj.top/gtbpjxbpgn.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.bjfxy.top/gtvapuxiaf.html

Ruby: attr_accessor :name
来源：http://hz.pycfn.com/gtsedbnbhu.html

C#:   public string Name { get; set; }
来源：http://hz.snrcjt.cn/gtzfnrjihc.html

[G12] 对象转字符串
来源：http://hz.hammf.cn/gtlcodadbu.html

Py:   def __str__(self): return self.name
来源：http://hz.yj20258.top/gtlxwpynnj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.chenlongwang.top/gtwkwyburg.html

JS:   toString() { return this.name; }
来源：http://hz.yj20258888.top/gttddbickv.html

TS:   toString(): string { return this.name; }
来源：http://hz.9152youxi.cn/gtyglzkbts.html

Java: @Override public String toString() { return name; }
来源：http://hz.yj202588.top/gtcsemnziz.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jlsjyb.cn/gtgzhbuzxf.html

Ruby: def to_s; @name; end
来源：http://hz.chenjidiqi.icu/gttssitwnn.html

C#:   public override string ToString() => Name;
来源：http://hz.bjfxy.top/gtbhoqhmsq.html

[G13] 判断对象类型
来源：http://hz.pycfn.com/gtttjabbpb.html

Py:   isinstance(u, User)
来源：http://hz.ivvv.top/gtsjauclxm.html

PHP:  $u instanceof User
来源：http://hz.yuanzhike.top/gtwvhlhgme.html

JS:   u instanceof User
来源：http://hz.cqqwz.cn/gthoacbfta.html

TS:   u instanceof User
来源：http://hz.vqdsnc.cn/gtkqnamqfs.html


<!-- 参考信息 -->