代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.vqdsnc.cn/gtejccahfs.html

[E15] HTML 转义 / 反转义
来源：http://hz.ybcxt.top/gtxgkfjnei.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.snrcjt.cn/gtltnayeow.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.birdmap.top/gtlmxhvrew.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.tanke756.top/gteowbjice.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.smart0.xyz/gtaobcigek.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.kuanghao11.cn/gtnpszonop.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.daxiang520.top/gtdptncfra.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yuanzhike.top/gthokvjiug.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.xylfe.cn/gtkpcblgxf.html

[E16] 数字千分位
来源：http://hz.52xcode.cn/gtctsdkktt.html

Py:   f"{1234567:,}"
来源：http://hz.0kj1m.cn/gtvlfrdefv.html

PHP:  number_format(1234567);
来源：http://hz.hywenlv.cn/gtpwknncuu.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.yj202588.top/gthpnnwfjl.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.ivvv.top/gtlubsfvhi.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.redwolf501.top/gtyudnbgrc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.birdmap.top/gtzcdkzegl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zhoulong.xyz/gtedboqmri.html

C#:   1234567.ToString("N0")
来源：http://hz.shanyushiyangtech.top/gtfoiavpbx.html

[E17] 首字母大写
来源：http://hz.zhaomingkeji.xyz/gtqzspcadd.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.xziqi.cn/gttmfefzki.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.cucudq.cn/gtbdnxevto.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.zhijiandao.cn/gtojsoqzqz.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.svipenyu.cn/gtnpmyxhny.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.jianghu66.top/gtjjmopall.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.sxryk.cn/gtrkacvgpd.html

Ruby: s.capitalize
来源：http://hz.zhiwuduotai.top/gtcczzdtpe.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.guowangkeji.top/gtnpxqgtqt.html

[E18] 模板占位符替换
来源：http://hz.jqgufenzy.top/gtxkbwvrsv.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.zhiwuduotai.top/gtujkgjnpp.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.bjfxy.top/gtrywzettj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.sweek.top/gtpiuowzpc.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.gzhubu.top/gttidusjnq.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jinghuilouyu.cn/gtfydcllps.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.nwbrower.top/gtxyecaqkj.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hongshengwenyu.top/gtvisatcoi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.pycfn.com/gtqnyiwuwj.html

[E19] 多行文本按行拆分
来源：http://hz.xylfe.cn/gtwacuautx.html

Py:   s.splitlines()
来源：http://hz.zycfv.cn/gtmclwqkqc.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.zhixingplan.top/gtslzljdxk.html

JS:   s.split(/\r?\n/)
来源：http://hz.mhx1999.top/gtndznjlww.html

TS:   s.split(/\r?\n/)
来源：http://hz.xylfe.cn/gthsjeinpj.html

Java: s.lines().toList()
来源：http://hz.vqdsnc.cn/gtycwsjbln.html

Go:   strings.Split(s, "\n")
来源：http://hz.zhongyouzk.top/gtrhujzxek.html

Ruby: s.lines
来源：http://hz.jqgufenzy.top/gtjhsahjai.html

C#:   s.Split('\n')
来源：http://hz.jyoumei.cn/gtrfefczxt.html

[E20] 判断字符串是否为空
来源：http://hz.pycfn.com/gtcogvxzlb.html

Py:   if not s:
来源：http://hz.0kj1m.cn/gtewjhyeuh.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yuxming.cn/gtcwccmlar.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.ywan-chungtsiang.top/gtlesqlpfl.html

TS:   if (s === "") {}
来源：http://hz.shanyushiyangkeji.top/gtrmiiltld.html

Java: if (s.isEmpty()) {}
来源：http://hz.jinyuanbaomall.cn/gtqrxrlywk.html

Go:   if s == "" {}
来源：http://hz.jlsjyb.cn/gtccepekft.html

Ruby: if s.empty?
来源：http://hz.c1oappe.top/gtyscnqvrh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.tianlin.xyz/gtlpucnorg.html

[E21] 超长截断加省略号
来源：http://hz.jianghu66.top/gtdnbwnyos.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.smart0.xyz/gtxkwwpdkh.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yuxming.cn/gtyaqfdfyh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.gzhubu.top/gtyqqogwpr.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hongshengwenyu.top/gtklwcfiex.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.gaohongyu789.top/gtqgfdhwwy.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yj20258888.top/gtfmfzupdf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yueranfly.top/gtcvzrddsy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.zhiwuduotai.top/gtyzqhlzar.html

[E22] 字节长度与字符长度
来源：http://hz.zdqjudy.top/gticlpmvks.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jinqigfzy.top/gtfqnraqxw.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.kuanghao11.cn/gtebuahcxg.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.haohaochexian.top/gtsqpkjxfa.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jlsjyb.cn/gtcoqlnzyh.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.52xcode.cn/gtfdqtwlno.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.fengsongda.top/gthmnybevl.html

Ruby: s.bytesize;  s.length
来源：http://hz.yuanzhike.top/gtxxsiirox.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.shuidangran.top/gtrnajjgga.html

================================================================================
来源：http://hz.smart0.xyz/gtrmdznjld.html

F. 文件与目录
来源：http://hz.guannengcc.top/gtiwvihqjn.html

================================================================================
来源：http://hz.quarkkingdee.top/gtjpethciu.html

[F01] 读取整个文件
来源：http://hz.gogol.net.cn/gtgyzxacsz.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.wangshuangyany.cn/gtturtberz.html

PHP:  file_get_contents("a.txt");
来源：http://hz.shangyingyoupin.top/gtqvlojqis.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.nwbrower.top/gtlcwhfuws.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.yueranfly.top/gtjfnoglxl.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.xziqi.cn/gtabsatvzg.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.sysykeji.top/gtpirikrvu.html

Ruby: File.read("a.txt")
来源：http://hz.316326.xyz/gtruwpfdtr.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.xinyue.icu/gtrnpivfvi.html

[F02] 逐行读取文件
来源：http://hz.yongpay.top/gtetacwmkg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.zhongyouzk.top/gtvqrdhulg.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.mhx1999.top/gthymsehgg.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jinqigufen.top/gthdrjujna.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.daria6918.cn/gtcqcixkvk.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jinqigfzy.top/gtwakgxlnl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.xuanzx.com/gtidsxwedz.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yonumen.top/gtuagescps.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.tianlin.xyz/gtyabpiczp.html

[F03] 写入文件（覆盖）
来源：http://hz.chenlongwang.top/gtiboxsxig.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.pengpengdd.cyou/gtphgfhuxv.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jiagoushi.top/gtjuyvqjir.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cheryme.top/gtovbfwnwm.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ydzc1.top/gttxxplepg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jyoumei.cn/gtzkxgnaqg.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.sxryk.cn/gtyzuavgkm.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.gaohongyu789.top/gtydqliudr.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.iojbl.cn/gtaqucithk.html

[F04] 追加写入文件
来源：http://hz.jlsjyb.cn/gtaorxnvne.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.mhx1999.top/gtegfwhnnn.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.bjfxy.top/gtebocncet.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cdnleiting.top/gtzhbusyyb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.316326.xyz/gtujyzefye.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zdqjudy.top/gtafjnjttn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.shanyushiyangkeji.top/gtciituahu.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jqgfzy.top/gtjydugmfd.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yj202588.top/gtklmctwpl.html

[F05] 判断文件或目录是否存在
来源：http://hz.ybcxt.top/gteyahhpsx.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.hongshengwenyu.top/gtvxxspzlv.html

PHP:  file_exists("a.txt");
来源：http://hz.pycfn.com/gtbuvfhfst.html

JS:   fs.existsSync("a.txt")
来源：http://hz.hnxiangtu.top/gtqeixwxfc.html

TS:   fs.existsSync("a.txt")
来源：http://hz.gogol.net.cn/gtfrjlgxbx.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.ydjk.org.cn/gttrfdhmaz.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.smart0.xyz/gtwjmuagie.html

Ruby: File.exist?("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtewpxwhbl.html

C#:   File.Exists("a.txt")
来源：http://hz.sweek.top/gtbmcglaar.html

[F06] 删除文件
来源：http://hz.dianchejie.cn/gtyniifgyg.html

Py:   os.remove("a.txt")
来源：http://hz.cucudq.cn/gtvbtlxglk.html

PHP:  unlink("a.txt");
来源：http://hz.dianchejie.cn/gtxunglspu.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.zhongyouzk.top/gtbbsdukwz.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.aizwys.cn/gtvidgmvto.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.daria6918.cn/gtiyohysym.html

Go:   os.Remove("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtpspydglq.html

Ruby: File.delete("a.txt")
来源：http://hz.52xcode.cn/gtrjoiuwoh.html

C#:   File.Delete("a.txt");
来源：http://hz.pycfn.com/gtpagcukiv.html

[F07] 创建目录（含多级）
来源：http://hz.cheryme.top/gtbpozwdhr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.redwolf501.top/gtzwnrngca.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.xylfe.cn/gtkanvvkfj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ydzc1.top/gtrejgrjju.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ybcxt.top/gtjrinqscm.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.feifeiyinyue.top/gtounabdlv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yongpay.top/gthmstrkkn.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.aibaodan.cn/gtwpanppzf.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.dashuyun.cn/gtyqqqoqfq.html

[F08] 遍历目录
来源：http://hz.yuanzhike.top/gtjqcqyyqq.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xuetiantiany.cn/gtlheunpaq.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.chenjidiqi.icu/gtjrlflett.html

JS:   fs.readdirSync("dir")
来源：http://hz.ydzc1.top/gtpuvfaqnh.html

TS:   fs.readdirSync("dir")
来源：http://hz.yongpay.top/gtylprbrzg.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.fengsongda.top/gtvlfqbnrk.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zhiwuduotai.top/gtgrcxsxzb.html

Ruby: Dir.children("dir")
来源：http://hz.zhongyouzk.top/gtbsrlkbft.html

C#:   Directory.GetFiles("dir")
来源：http://hz.dashuyun.cn/gtdkfklybe.html

[F09] 获取文件大小
来源：http://hz.yvedp.cn/gtzcbmgtwd.html

Py:   os.path.getsize("a.txt")
来源：http://hz.svipenyu.cn/gtppnzvcfy.html

PHP:  filesize("a.txt");
来源：http://hz.zhixingplan.top/gtbrpmgnfa.html

JS:   fs.statSync("a.txt").size
来源：http://hz.ywan-chungtsiang.top/gtaczuuyeo.html

TS:   fs.statSync("a.txt").size
来源：http://hz.zhijiandao.cn/gtrccqxxfu.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jlsjyb.cn/gtlmjycmmo.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.hywenlv.cn/gtxhkuxutq.html

Ruby: File.size("a.txt")
来源：http://hz.hfpthk.cn/gtzlupyayw.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.sweek.top/gtyroslkwe.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.ybcxt.top/gtrmckllaz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.nanxuanxn.top/gttspufleq.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.chenlongwang.top/gttqybmqgg.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.yongpay.top/gtravlmpbv.html

TS:   path.extname("a.txt")
来源：http://hz.shuidangran.top/gtgvbyqgjm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.wangshuangyany.cn/gtvjgbhmhh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.kuanghao11.cn/gtecwgitbn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.tanke756.top/gtvdxozhmc.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.sufxvd.cn/gtumzwxgig.html

[F11] 复制与移动文件
来源：http://hz.iojbl.cn/gtrnncpmtc.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.svipenyu.cn/gtanczmvru.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.snrcjt.cn/gtivkucbog.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.sysykeji.top/gtbbvjnvad.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xziqi.cn/gtprmqximc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jyoumei.cn/gtxzmfcxhi.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.52xcode.cn/gtjgdbfscv.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.guowangkeji.top/gtfnqwxhoc.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ydjk.org.cn/gtidvgixol.html

[F12] CSV 读写
来源：http://hz.ybcxt.top/gtlqusptow.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.sysykeji.top/gtgnrtscvt.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.cashguo.top/gtfaodvgdn.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.smart0.xyz/gtnuwqcpcs.html

TS:   // 同上
来源：http://hz.sxryk.cn/gtdfedjjts.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.shanyushiyangtech.top/gtsksgvxof.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.sufxvd.cn/gtevturxcf.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yonumen.top/gtpznzsoqy.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.hnxiangtu.top/gtzwsflqkv.html

================================================================================
来源：http://hz.aibaodan.cn/gttquxnyqq.html

G. 面向对象
来源：http://hz.xinyue.icu/gtlqtqtwcz.html

================================================================================
来源：http://hz.ywan-chungtsiang.top/gtrxcsqvzt.html

[G01] 定义类
来源：http://hz.sweek.top/gtzvidlsvm.html

Py:   class User: pass
来源：http://hz.yangfankeji.com/gtqkrdzelv.html

PHP:  class User {}
来源：http://hz.zhiwuduotai.top/gtstttuelu.html

JS:   class User {}
来源：http://hz.yanxiufei.cn/gtafhmqksw.html

TS:   class User { name: string = ""; }
来源：http://hz.hywenlv.cn/gthayhzgfo.html

Java: class User {}
来源：http://hz.0kj1m.cn/gttuoaimth.html

Go:   type User struct { Name string }
来源：http://hz.bjfxy.top/gtvghiaulo.html

Ruby: class User; end
来源：http://hz.52xcode.cn/gterhdqloc.html

C#:   class User {}
来源：http://hz.yuxming.cn/gttuhdvldu.html

[G02] 构造函数
来源：http://hz.vqdsnc.cn/gtaojscatn.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.sufxvd.cn/gtxgkvlfzu.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.tian-w.cn/gtlkvcugsi.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.316326.xyz/gtzhxbuabn.html

TS:   constructor(public name: string) {}
来源：http://hz.xuetiantiany.cn/gtqxmjpqjx.html

Java: User(String name) { this.name = name; }
来源：http://hz.tianlin.xyz/gtuyzmuedc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.zhoulong.xyz/gtmoqjsfbr.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.pycfn.com/gtbedzufgm.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhoulong.xyz/gtjtahubgl.html

[G03] 实例属性
来源：http://hz.tian-w.cn/gtdipkyqww.html

Py:   self.name = "x"
来源：http://hz.feifeiyinyue.top/gtlablbwwa.html

PHP:  public string $name = "x";
来源：http://hz.guannengcc.top/gthkzolbqr.html

JS:   this.name = "x";
来源：http://hz.wangshuangyany.cn/gtlzuzbsxp.html

TS:   name: string = "x";
来源：http://hz.jiagoushi.top/gttxoapblh.html

Java: private String name;
来源：http://hz.ivvv.top/gttrqagssu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hywenlv.cn/gtvwdileuf.html

Ruby: @name = "x"
来源：http://hz.cucudq.cn/gtabmbkdkd.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.sxryk.cn/gtmdjlvslw.html

[G04] 定义方法
来源：http://hz.zhaomingkeji.xyz/gtpfpgymff.html

Py:   def greet(self): return self.name
来源：http://hz.shuidangran.top/gtgslqoldx.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zdqjudy.top/gtqgjwpxmh.html

JS:   greet() { return this.name; }
来源：http://hz.zdqjudy.top/gtucutlfat.html

TS:   greet(): string { return this.name; }
来源：http://hz.zhongyouzk.top/gtrpxfsugj.html

Java: String greet() { return name; }
来源：http://hz.gotoacloud.top/gtuyycarqz.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.hnqzz.top/gtghekdrwk.html

Ruby: def greet; @name; end
来源：http://hz.cheryme.top/gtmbcptkdv.html

C#:   public string Greet() => Name;
来源：http://hz.yongpay.top/gtfvzdidxw.html

[G05] 继承
来源：http://hz.ivvv.top/gtgawotusl.html

Py:   class Admin(User): pass
来源：http://hz.chenzaomai.com/gtvwgntibu.html

PHP:  class Admin extends User {}
来源：http://hz.daxiang520.top/gtifevzmcr.html

JS:   class Admin extends User {}
来源：http://hz.andypj.xyz/gtbxtprmqa.html

TS:   class Admin extends User {}
来源：http://hz.shanyushiyangkeji.top/gtcjduhrir.html

Java: class Admin extends User {}
来源：http://hz.xuanzx.com/gtviphqqdp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.xinyue.icu/gtbplkikcr.html

Ruby: class Admin < User; end
来源：http://hz.hammf.cn/gtqmybkdxc.html

C#:   class Admin : User {}
来源：http://hz.tianlin.xyz/gtphazsxwm.html

[G06] 重写方法
来源：http://hz.ydzc1.top/gtlpdtrzxb.html

Py:   def greet(self): return "admin"
来源：http://hz.aibaodan.cn/gtrcibskwd.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.chenlongwang.top/gtncpfhtqk.html

JS:   greet() { return "admin"; }
来源：http://hz.jyoumei.cn/gtfautkwkd.html

TS:   greet(): string { return "admin"; }
来源：http://hz.jinqigufen.top/gtpswmxhmo.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.c1oappe.top/gtwxrtidrz.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.hnqzz.top/gtosazowps.html

Ruby: def greet; "admin"; end
来源：http://hz.dashuyun.cn/gtrgpceedb.html

C#:   public override string Greet() => "admin";
来源：http://hz.meibo888.top/gtdcgywzqb.html

[G07] 调用父类方法
来源：http://hz.xinyue.icu/gtgmwlgngw.html

Py:   super().greet()
来源：http://hz.pengpengdd.cyou/gtylqybhfi.html

PHP:  parent::greet();
来源：http://hz.cdnleiting.top/gttpwrdkqb.html

JS:   super.greet();
来源：http://hz.cqqwz.cn/gtgfpxorqc.html

TS:   super.greet();
来源：http://hz.gaohongyu789.top/gtcqpgtvlq.html

Java: super.greet();
来源：http://hz.xuetiantiany.cn/gtipfymkuy.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.ywan-chungtsiang.top/gtgqsmaxuj.html

Ruby: super
来源：http://hz.feifeiyinyue.top/gttjjyipgv.html

C#:   base.Greet();
来源：http://hz.zhengqikj.top/gtyfygejbu.html

[G08] 静态方法与属性
来源：http://hz.pycfn.com/gtdnnnnzvm.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jinqigufen.top/gtmvuqeaiy.html

PHP:  public static function f() {}
来源：http://hz.aizwys.cn/gtjfvlgymq.html

JS:   static f() {}
来源：http://hz.svipenyu.cn/gtffmevuzw.html

TS:   static f(): void {}
来源：http://hz.redwolf501.top/gtanroaxne.html

Java: static void f() {}
来源：http://hz.jianghu66.top/gtejpovmej.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.feifeiyinyue.top/gtklbfauwq.html

Ruby: def self.f; end
来源：http://hz.ehwqpu.com/gtrycjgycs.html

C#:   public static void F() {}
来源：http://hz.cheryme.top/gtqiqxetbb.html

[G09] 接口 / 抽象类
来源：http://hz.gzhubu.top/gtytlhvion.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yanxiufei.cn/gtbjlharup.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.gzhubu.top/gtvvgggikp.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.hnqzz.top/gtnntdoqsu.html

TS:   interface Shape { area(): number; }
来源：http://hz.xuanzx.com/gtdtzbkmop.html

Java: interface Shape { double area(); }
来源：http://hz.nwbrower.top/gtdugoekgl.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.zhongyouzk.top/gtxbzcxghg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jinqigfzy.top/gtbefoqwre.html

C#:   interface IShape { double Area(); }
来源：http://hz.bjfxy.top/gtewugviwz.html

[G10] 访问控制
来源：http://hz.jinghuilouyu.cn/gtdnwkrdvq.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yongpay.top/gtjwffubfl.html

PHP:  public / protected / private
来源：http://hz.hywenlv.cn/gttnflfheo.html

JS:   #private 字段；其余公开
来源：http://hz.ehwqpu.com/gtcfoqvcns.html

TS:   public / protected / private
来源：http://hz.xuanzx.com/gttsdmwnsp.html

Java: public / protected / private / 默认包级
来源：http://hz.wangdashe.top/gthndesbgo.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.xingfuxueyuan.xyz/gtaxnuqsge.html

Ruby: public / protected / private
来源：http://hz.smart0.xyz/gtfqsbiswr.html

C#:   public / protected / private / internal
来源：http://hz.yuxming.cn/gtoeieazvu.html

[G11] getter / setter
来源：http://hz.zhongyouzk.top/gtwvnobrsc.html

Py:   @property 与 @x.setter
来源：http://hz.hammf.cn/gtgltmnyns.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.smart0.xyz/gtnzniydyn.html

JS:   get name() { return this._name; }
来源：http://hz.gzhubu.top/gtfmwbloxk.html

TS:   get name(): string { return this._name; }
来源：http://hz.jinqigufen.top/gtanohkrrn.html

Java: public String getName() { return name; }
来源：http://hz.chenjidiqi.icu/gtlmbmoqcq.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.0kj1m.cn/gtdtzekeug.html

Ruby: attr_accessor :name
来源：http://hz.9152youxi.cn/gtimzwpltg.html

C#:   public string Name { get; set; }
来源：http://hz.ydjk.org.cn/gthzenulta.html

[G12] 对象转字符串
来源：http://hz.shangyingyoupin.top/gtqbnirscd.html

Py:   def __str__(self): return self.name
来源：http://hz.jiagoushi.top/gttnluxiwj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.nanxuanxn.top/gtafnefwwd.html

JS:   toString() { return this.name; }
来源：http://hz.yuxming.cn/gtldgzaeoy.html

TS:   toString(): string { return this.name; }
来源：http://hz.hysaishi.cn/gthfewqcem.html

Java: @Override public String toString() { return name; }
来源：http://hz.guannengcc.top/gtlexdcizh.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.cqqwz.cn/gtxpyiotcn.html

Ruby: def to_s; @name; end
来源：http://hz.zhaomingkeji.xyz/gttgqnedbu.html

C#:   public override string ToString() => Name;
来源：http://hz.jinqigufen.top/gtfumkhslu.html

[G13] 判断对象类型
来源：http://hz.ydjk.org.cn/gtdbvyremc.html

Py:   isinstance(u, User)
来源：http://hz.cqqwz.cn/gtjrjwzdtp.html

PHP:  $u instanceof User
来源：http://hz.xingfuxueyuan.xyz/gtytqygaai.html

JS:   u instanceof User
来源：http://hz.ivvv.top/gtwyfvdqvw.html

TS:   u instanceof User
来源：http://hz.xylfe.cn/gtseagpken.html


<!-- 参考信息 -->