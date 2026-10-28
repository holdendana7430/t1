代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.sweek.top/gtxatfnkqs.html

[E15] HTML 转义 / 反转义
来源：http://hz.cdnleiting.top/gtbefcyxof.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.xuetiantiany.cn/gtfyteudgx.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.shuidangran.top/gtqlzoxbxp.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.dianchejie.cn/gtvgwihalh.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.dashuyun.cn/gtwxevoego.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yj20258888.top/gtmrotezkb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.zhijiandao.cn/gtkoexjiqk.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.316326.xyz/gtjavrcelu.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jinghuilouyu.cn/gtlkrgvfxr.html

[E16] 数字千分位
来源：http://hz.shuidangran.top/gthpgrmfye.html

Py:   f"{1234567:,}"
来源：http://hz.jlsjyb.cn/gtxjthfjwt.html

PHP:  number_format(1234567);
来源：http://hz.shuidangran.top/gtuqyeqkyh.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.shanyushiyangtech.top/gtsdbyremc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.gzhubu.top/gtqifttmdb.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.meibo888.top/gtuseuugph.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.mhx1999.top/gtkzvjtlhl.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.zhoulong.xyz/gtvliyxdst.html

C#:   1234567.ToString("N0")
来源：http://hz.sxryk.cn/gtwgsjbgvf.html

[E17] 首字母大写
来源：http://hz.yangfankeji.com/gtjlqomenm.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.wangdashe.top/gtzacjjkcg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.aizwys.cn/gturlwlwvx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ivvv.top/gtrxsdaeyn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hammf.cn/gtbtxvnldl.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.sweek.top/gtdcdqdvdb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.meibo888.top/gtaebvlzrh.html

Ruby: s.capitalize
来源：http://hz.cucudq.cn/gtzrtljlim.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.shanyushiyangtech.top/gtkbrtltmn.html

[E18] 模板占位符替换
来源：http://hz.sweek.top/gteqnygupb.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.yj202588.top/gtrkpfkqcz.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.birdmap.top/gttwsucqbe.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.shanyushiyangkeji.top/gtvjrzjawu.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.feifeiyinyue.top/gtpfnsfttp.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.9152youxi.cn/gtbzzbbmsd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.wangdashe.top/gtozdrqabm.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.hfpthk.cn/gtqbhcmlso.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zycfv.cn/gtrzoutwcv.html

[E19] 多行文本按行拆分
来源：http://hz.zhengqikj.top/gtrtktjhhz.html

Py:   s.splitlines()
来源：http://hz.cheryme.top/gtousufslx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.sxryk.cn/gtrerkxoyw.html

JS:   s.split(/\r?\n/)
来源：http://hz.yj20258.top/gtdkbbybek.html

TS:   s.split(/\r?\n/)
来源：http://hz.dianchejie.cn/gtilszzfzr.html

Java: s.lines().toList()
来源：http://hz.chenlongwang.top/gtgateqtoh.html

Go:   strings.Split(s, "\n")
来源：http://hz.hysaishi.cn/gtlrbqbugv.html

Ruby: s.lines
来源：http://hz.yanxiufei.cn/gtvkdigufw.html

C#:   s.Split('\n')
来源：http://hz.chenjidiqi.icu/gtmrboellc.html

[E20] 判断字符串是否为空
来源：http://hz.cheryme.top/gttvxfkbdr.html

Py:   if not s:
来源：http://hz.gzhubu.top/gtszviwgui.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.hammf.cn/gtozmtspel.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jiagoushi.top/gtgienpnav.html

TS:   if (s === "") {}
来源：http://hz.xziqi.cn/gtrqfefqpt.html

Java: if (s.isEmpty()) {}
来源：http://hz.xuanzx.com/gtumywogqq.html

Go:   if s == "" {}
来源：http://hz.wangdashe.top/gtxgqgmnfp.html

Ruby: if s.empty?
来源：http://hz.dashuyun.cn/gtzfpyaict.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.fzhhl.top/gtwovwcsro.html

[E21] 超长截断加省略号
来源：http://hz.zycfv.cn/gtnzgqubib.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.vqdsnc.cn/gtlgpeasjm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yuanzhike.top/gtfjyhgygk.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.9152youxi.cn/gtmpxddabc.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yanxiufei.cn/gtaljbjmxa.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.svipenyu.cn/gtqnrbksfq.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.tianlin.xyz/gtqppmlqrq.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.gzhubu.top/gthmdueoby.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.fzhhl.top/gtarcoixnf.html

[E22] 字节长度与字符长度
来源：http://hz.daxiang520.top/gtxwuvdxjo.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jlsjyb.cn/gtucqkrgcg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.kuanghao11.cn/gtgqfkqywa.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jyoumei.cn/gtfxgusodn.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jqgufenzy.top/gtqirgrgry.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.dianchejie.cn/gtkkevvecj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.jqgufenzy.top/gtfylurpdf.html

Ruby: s.bytesize;  s.length
来源：http://hz.jinyuanbaomall.cn/gtofevbbig.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.havefunace.top/gtxsqwuyrp.html

================================================================================
来源：http://hz.cqqwz.cn/gtudnqbscs.html

F. 文件与目录
来源：http://hz.havefunace.top/gtivjfjfeh.html

================================================================================
来源：http://hz.ydzc1.top/gtodnckmyh.html

[F01] 读取整个文件
来源：http://hz.zhijiandao.cn/gtouegnnlx.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yueranfly.top/gtdxonazhj.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hongshengwenyu.top/gtglptveux.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yj20258.top/gtdcriifmc.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.zhaomingkeji.xyz/gtmiqbfcki.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.ydjk.org.cn/gtqwkefdhd.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.sufxvd.cn/gtdqrabatv.html

Ruby: File.read("a.txt")
来源：http://hz.0kj1m.cn/gtwqlvcxpy.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.fzhhl.top/gtpwtrdeff.html

[F02] 逐行读取文件
来源：http://hz.guannengcc.top/gtpvdsapsd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.tianlin.xyz/gtqnvnview.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yvedp.cn/gtxzrwhgdj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.pengpengdd.cyou/gtuyxnniyk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.snrcjt.cn/gtkcwqdiji.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jyoumei.cn/gtblamqnzb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yj20258.top/gtofvizdlh.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.ywan-chungtsiang.top/gtghuzolzg.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.fzhhl.top/gtncidltic.html

[F03] 写入文件（覆盖）
来源：http://hz.yj20258888.top/gtlyjyjuzb.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jinqigufen.top/gtoicxhnwk.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jinyuanbaomall.cn/gtupdxlscj.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.ydjk.org.cn/gtefpkthxl.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.tian-w.cn/gtqyiimylg.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.gaohongyu789.top/gtfgfbjbew.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.zhiwuduotai.top/gtpaibriam.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.birdmap.top/gtykacnxzk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yangfankeji.com/gtgsdyeqtf.html

[F04] 追加写入文件
来源：http://hz.hywenlv.cn/gtokzddntw.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.0kj1m.cn/gtooxdmbgi.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.nanxinkj.top/gthxzjciqg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.guannengcc.top/gtflvnpuxu.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.daxiang520.top/gtucgdjkzm.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.bjfxy.top/gtpsoymgde.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.gotoacloud.top/gtfvbyrkfc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.zhongyouzk.top/gtbjdnigsz.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.gzhubu.top/gtrrmoiabx.html

[F05] 判断文件或目录是否存在
来源：http://hz.sufxvd.cn/gtcivkogfa.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.sufxvd.cn/gttkhhbvjy.html

PHP:  file_exists("a.txt");
来源：http://hz.daxiang520.top/gtucjjokcz.html

JS:   fs.existsSync("a.txt")
来源：http://hz.jyoumei.cn/gtyrraxepi.html

TS:   fs.existsSync("a.txt")
来源：http://hz.pengpengdd.cyou/gtgeejtdgq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.shangyingyoupin.top/gtfoytatll.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.aizwys.cn/gtzqjddgvp.html

Ruby: File.exist?("a.txt")
来源：http://hz.yuanzhike.top/gtmbgqeblt.html

C#:   File.Exists("a.txt")
来源：http://hz.guowangkeji.top/gttwttdupm.html

[F06] 删除文件
来源：http://hz.hongshengwenyu.top/gtbwlanavu.html

Py:   os.remove("a.txt")
来源：http://hz.kuanghao11.cn/gtvwroikse.html

PHP:  unlink("a.txt");
来源：http://hz.yvedp.cn/gtsuplvkbl.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hysaishi.cn/gtltxfobut.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.0kj1m.cn/gtbvmknouo.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jqgfzy.top/gtclxbkrhg.html

Go:   os.Remove("a.txt")
来源：http://hz.ivvv.top/gtntjxmrwe.html

Ruby: File.delete("a.txt")
来源：http://hz.xylfe.cn/gtydnlgqjr.html

C#:   File.Delete("a.txt");
来源：http://hz.dianchejie.cn/gtavtdohhm.html

[F07] 创建目录（含多级）
来源：http://hz.hongshengwenyu.top/gthzxmezlr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.chenzaomai.com/gtcvvlitcu.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.jinyuanbaomall.cn/gtgmqqwmmh.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.snrcjt.cn/gtqqwcrbrd.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.shangyingyoupin.top/gtgfmkxlry.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.0kj1m.cn/gtcswufbbv.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.sweek.top/gtmmehaupz.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.hywenlv.cn/gtrvcfovnk.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yuanzhike.top/gtnsxebwqm.html

[F08] 遍历目录
来源：http://hz.dashuyun.cn/gtyljabymi.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.cdnleiting.top/gthsyfelku.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.dashuyun.cn/gtgudtxzuf.html

JS:   fs.readdirSync("dir")
来源：http://hz.ppjwa.cn/gtbcgdgvhd.html

TS:   fs.readdirSync("dir")
来源：http://hz.yangfankeji.com/gtxpawqoki.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.ybcxt.top/gtevszizjd.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.shanyushiyangkeji.top/gtexbjpmal.html

Ruby: Dir.children("dir")
来源：http://hz.hywenlv.cn/gtbqrurwtj.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zhaomingkeji.xyz/gtagtqunek.html

[F09] 获取文件大小
来源：http://hz.jiagoushi.top/gtovssghqe.html

Py:   os.path.getsize("a.txt")
来源：http://hz.cheryme.top/gtkjzvegpz.html

PHP:  filesize("a.txt");
来源：http://hz.nanxinkj.top/gtqbecszyd.html

JS:   fs.statSync("a.txt").size
来源：http://hz.pycfn.com/gtrnluxkle.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jinqigufen.top/gteyyrbzjg.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jinqigfzy.top/gtygfkwpei.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.zhengqikj.top/gtvtpnrvco.html

Ruby: File.size("a.txt")
来源：http://hz.cucudq.cn/gtryhwzvdq.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.sufxvd.cn/gtmlundmrd.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.tanke756.top/gtlwrcyxjf.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.xziqi.cn/gtigveoyuv.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.snrcjt.cn/gtqkveyxvs.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.quarkkingdee.top/gtrjuqgigk.html

TS:   path.extname("a.txt")
来源：http://hz.zhoulong.xyz/gthekccgrd.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jinqigufen.top/gtmsbjtnrh.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.chenzaomai.com/gtedbthzjm.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.xziqi.cn/gttqbjiajb.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.haohaochexian.top/gtlgqwjrjp.html

[F11] 复制与移动文件
来源：http://hz.ydjk.org.cn/gtpuuyykqk.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jinghuilouyu.cn/gtlnqvoadt.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.pycfn.com/gteikntumg.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.svipenyu.cn/gtmkefiypk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.shuidangran.top/gtxhdrkrry.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.ivvv.top/gtqjzmcmpt.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.gzhubu.top/gtubfjpyfm.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.guannengcc.top/gttkpaufiq.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.smart0.xyz/gtydneugie.html

[F12] CSV 读写
来源：http://hz.sufxvd.cn/gtsziaxzqd.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.feifeiyinyue.top/gtayeebldm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.nwbrower.top/gtcvyhocjo.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.tian-w.cn/gttwjvkpuy.html

TS:   // 同上
来源：http://hz.yangfankeji.com/gtwwriafgy.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhengqikj.top/gtmfyoiloj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.sufxvd.cn/gtmjdbobxj.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.jiagoushi.top/gthsuuqwqo.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.quarkkingdee.top/gtzlinmcor.html

================================================================================
来源：http://hz.yangfankeji.com/gtqxpwxinn.html

G. 面向对象
来源：http://hz.dashuyun.cn/gthtzrdwhn.html

================================================================================
来源：http://hz.ehwqpu.com/gtmzzpkrfl.html

[G01] 定义类
来源：http://hz.dianchejie.cn/gtxykrzqxw.html

Py:   class User: pass
来源：http://hz.shuidangran.top/gtxololawn.html

PHP:  class User {}
来源：http://hz.ydzc1.top/gttebqqxdu.html

JS:   class User {}
来源：http://hz.wangdashe.top/gtxqfxiobc.html

TS:   class User { name: string = ""; }
来源：http://hz.meibo888.top/gtsspyyrho.html

Java: class User {}
来源：http://hz.yanxiufei.cn/gtwcmdgmgb.html

Go:   type User struct { Name string }
来源：http://hz.hfpthk.cn/gtlpebdddz.html

Ruby: class User; end
来源：http://hz.xinyue.icu/gtcovgdafg.html

C#:   class User {}
来源：http://hz.zhiwuduotai.top/gtnjyuiqhk.html

[G02] 构造函数
来源：http://hz.shangyingyoupin.top/gtgqhzkwiw.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.xylfe.cn/gtdjnzojjg.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jlsjyb.cn/gtmrpqfhzr.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.cashguo.top/gtgaemxfys.html

TS:   constructor(public name: string) {}
来源：http://hz.hywenlv.cn/gtpvztfgob.html

Java: User(String name) { this.name = name; }
来源：http://hz.shanyushiyangkeji.top/gtvalukgtu.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.smart0.xyz/gtjjptrsie.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.dashuyun.cn/gtlwkhbvaq.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hfpthk.cn/gtcxewshbd.html

[G03] 实例属性
来源：http://hz.jiagoushi.top/gtewwipkpb.html

Py:   self.name = "x"
来源：http://hz.yangfankeji.com/gtxxjchwxc.html

PHP:  public string $name = "x";
来源：http://hz.iojbl.cn/gtuistckjj.html

JS:   this.name = "x";
来源：http://hz.yangfankeji.com/gtoompkwwz.html

TS:   name: string = "x";
来源：http://hz.guowangkeji.top/gtugbykwsl.html

Java: private String name;
来源：http://hz.ydzc1.top/gtttomqawm.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.hfpthk.cn/gtrwjyzlov.html

Ruby: @name = "x"
来源：http://hz.ywan-chungtsiang.top/gtsfnzlmog.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.sweek.top/gttlqowgno.html

[G04] 定义方法
来源：http://hz.nwbrower.top/gtesdkowfm.html

Py:   def greet(self): return self.name
来源：http://hz.zhengqikj.top/gtsyzoejoh.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.ywan-chungtsiang.top/gtihgdvajw.html

JS:   greet() { return this.name; }
来源：http://hz.zycfv.cn/gtmclkpfja.html

TS:   greet(): string { return this.name; }
来源：http://hz.meibo888.top/gtbwbbwgds.html

Java: String greet() { return name; }
来源：http://hz.hongshengwenyu.top/gtnujpllcj.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jinqigufen.top/gtqdfdehbu.html

Ruby: def greet; @name; end
来源：http://hz.aizwys.cn/gthzabvuyk.html

C#:   public string Greet() => Name;
来源：http://hz.snrcjt.cn/gtwizryzpq.html

[G05] 继承
来源：http://hz.havefunace.top/gtmdziqxvs.html

Py:   class Admin(User): pass
来源：http://hz.tanke756.top/gtckgymqhw.html

PHP:  class Admin extends User {}
来源：http://hz.ywan-chungtsiang.top/gtdgshgqrb.html

JS:   class Admin extends User {}
来源：http://hz.cucudq.cn/gtwclvmuhi.html

TS:   class Admin extends User {}
来源：http://hz.tian-w.cn/gtdkeofnvm.html

Java: class Admin extends User {}
来源：http://hz.jiagoushi.top/gtddvadlfg.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ehwqpu.com/gtmtgipzlo.html

Ruby: class Admin < User; end
来源：http://hz.gotoacloud.top/gtfzdvgcds.html

C#:   class Admin : User {}
来源：http://hz.9152youxi.cn/gtqrbusdcb.html

[G06] 重写方法
来源：http://hz.smart0.xyz/gtgyecqfvt.html

Py:   def greet(self): return "admin"
来源：http://hz.jiagoushi.top/gtyhmjwefi.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.wangdashe.top/gtsgysznry.html

JS:   greet() { return "admin"; }
来源：http://hz.tianlin.xyz/gtqtqzkwgd.html

TS:   greet(): string { return "admin"; }
来源：http://hz.mhx1999.top/gtmpryynaq.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.zhijiandao.cn/gtolqstfzx.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.xingfuxueyuan.xyz/gtydqhwejo.html

Ruby: def greet; "admin"; end
来源：http://hz.ydjk.org.cn/gtpjxhroyy.html

C#:   public override string Greet() => "admin";
来源：http://hz.yueranfly.top/gtqunfmlgs.html

[G07] 调用父类方法
来源：http://hz.cqqwz.cn/gtkfhilmhz.html

Py:   super().greet()
来源：http://hz.jinqigfzy.top/gtcizvxbbw.html

PHP:  parent::greet();
来源：http://hz.gotoacloud.top/gtfpsddztr.html

JS:   super.greet();
来源：http://hz.hysaishi.cn/gtectnzxon.html

TS:   super.greet();
来源：http://hz.316326.xyz/gtbvrikncj.html

Java: super.greet();
来源：http://hz.aibaodan.cn/gtjvvfweuu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.ybcxt.top/gtlrtbtgsj.html

Ruby: super
来源：http://hz.bjfxy.top/gtfwrfiacj.html

C#:   base.Greet();
来源：http://hz.wangshuangyany.cn/gtrhflpinm.html

[G08] 静态方法与属性
来源：http://hz.jyoumei.cn/gtacpchbqc.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.316326.xyz/gtcpmtvkvn.html

PHP:  public static function f() {}
来源：http://hz.yongpay.top/gtocwmlffa.html

JS:   static f() {}
来源：http://hz.hysaishi.cn/gtnwteufia.html

TS:   static f(): void {}
来源：http://hz.tanke756.top/gtuaqmeotx.html

Java: static void f() {}
来源：http://hz.meibo888.top/gtyjbywmuj.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.cqqwz.cn/gtfhqhbneu.html

Ruby: def self.f; end
来源：http://hz.ywan-chungtsiang.top/gtpffvntlg.html

C#:   public static void F() {}
来源：http://hz.quarkkingdee.top/gtuvpwmahy.html

[G09] 接口 / 抽象类
来源：http://hz.bjfxy.top/gtmlfudley.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.316326.xyz/gtzuizvboo.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.yj20258888.top/gtwzwhnapz.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.cqqwz.cn/gtcnszimxa.html

TS:   interface Shape { area(): number; }
来源：http://hz.xylfe.cn/gtqubbxgtk.html

Java: interface Shape { double area(); }
来源：http://hz.aibaodan.cn/gttvkdgiuk.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.cheryme.top/gtyhlxqyga.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.ydjk.org.cn/gtsyjdcllt.html

C#:   interface IShape { double Area(); }
来源：http://hz.vqdsnc.cn/gtnbkmwuiw.html

[G10] 访问控制
来源：http://hz.chenlongwang.top/gtzaombxjk.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.gaohongyu789.top/gtdphdkizm.html

PHP:  public / protected / private
来源：http://hz.fengsongda.top/gtgfkjmkvh.html

JS:   #private 字段；其余公开
来源：http://hz.pycfn.com/gtcijirxez.html

TS:   public / protected / private
来源：http://hz.cheryme.top/gtujoasekj.html

Java: public / protected / private / 默认包级
来源：http://hz.hnqzz.top/gtkirkhtqc.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.dashuyun.cn/gtwjbtvcsg.html

Ruby: public / protected / private
来源：http://hz.yangfankeji.com/gtcecksvkd.html

C#:   public / protected / private / internal
来源：http://hz.dianchejie.cn/gtucylbjsj.html

[G11] getter / setter
来源：http://hz.redwolf501.top/gtybhoayxi.html

Py:   @property 与 @x.setter
来源：http://hz.shangyingyoupin.top/gtogtoamrl.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.aibaodan.cn/gtbiittayh.html

JS:   get name() { return this._name; }
来源：http://hz.aibaodan.cn/gtfrhsvlgn.html

TS:   get name(): string { return this._name; }
来源：http://hz.ivvv.top/gtphurwpfy.html

Java: public String getName() { return name; }
来源：http://hz.gotoacloud.top/gtsczoerbj.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yongpay.top/gtipsbyocr.html

Ruby: attr_accessor :name
来源：http://hz.tanke756.top/gtbvwaynkv.html

C#:   public string Name { get; set; }
来源：http://hz.wangdashe.top/gtsquisrgv.html

[G12] 对象转字符串
来源：http://hz.snrcjt.cn/gtrcuafers.html

Py:   def __str__(self): return self.name
来源：http://hz.jiagoushi.top/gtfryyoqij.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.havefunace.top/gtxqmashbk.html

JS:   toString() { return this.name; }
来源：http://hz.snrcjt.cn/gthokluydz.html

TS:   toString(): string { return this.name; }
来源：http://hz.quarkkingdee.top/gtcywprtxv.html

Java: @Override public String toString() { return name; }
来源：http://hz.jiagoushi.top/gtlvdqsrhq.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.hnxiangtu.top/gtlbnlffqz.html

Ruby: def to_s; @name; end
来源：http://hz.shangyingyoupin.top/gtsjrnzrzq.html

C#:   public override string ToString() => Name;
来源：http://hz.zhongyouzk.top/gtxklwqdsg.html

[G13] 判断对象类型
来源：http://hz.yonumen.top/gtdvtntzvx.html

Py:   isinstance(u, User)
来源：http://hz.hnqzz.top/gtntavlosi.html

PHP:  $u instanceof User
来源：http://hz.xingfuxueyuan.xyz/gtzepvqmay.html

JS:   u instanceof User
来源：http://hz.gzhubu.top/gtvglswgod.html

TS:   u instanceof User
来源：http://hz.vqdsnc.cn/gtkguetznm.html


<!-- 参考信息 -->