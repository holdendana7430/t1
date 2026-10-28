代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.jqgfzy.top/gtbyhglnwe.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.hammf.cn/gtzfdvpklt.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yongpay.top/gtiuoxdpej.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.ivvv.top/gthlvlffba.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.wangshuangyany.cn/gtkhvemklx.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.gotoacloud.top/gtuarcyygo.html

[E16] 数字千分位
来源：http://hz.gotoacloud.top/gtccjbmtnt.html

Py:   f"{1234567:,}"
来源：http://hz.feifeiyinyue.top/gtjajzioha.html

PHP:  number_format(1234567);
来源：http://hz.zhongyouzk.top/gttayrqfab.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.sufxvd.cn/gtdrliwdlk.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.bjfxy.top/gtdvwesabw.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.dianchejie.cn/gttmervfuq.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.mhx1999.top/gtpymiuuqh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.cqqwz.cn/gtyjgojvxo.html

C#:   1234567.ToString("N0")
来源：http://hz.aibaodan.cn/gtyhqzdmcl.html

[E17] 首字母大写
来源：http://hz.yvedp.cn/gtkufqanie.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.yvedp.cn/gtmetmxkni.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.aizwys.cn/gttvxzzirt.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.tanke756.top/gtrxkhrwws.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yueranfly.top/gtcorfutfr.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.ivvv.top/gtxovnyofb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.fzhhl.top/gtepxfytgb.html

Ruby: s.capitalize
来源：http://hz.zhixingplan.top/gtdamuiaqd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.tianlin.xyz/gtawtqktus.html

[E18] 模板占位符替换
来源：http://hz.hnqzz.top/gthobbdcaa.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.dianchejie.cn/gtosgxkzba.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.ppjwa.cn/gtlzlmslsp.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.feifeiyinyue.top/gtwjboyend.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.cdnleiting.top/gtktyqjcts.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.shanyushiyangkeji.top/gtmdszivsw.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.hywenlv.cn/gtfqskoklx.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.birdmap.top/gtdspymlhi.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.aizwys.cn/gtbslkqdgb.html

[E19] 多行文本按行拆分
来源：http://hz.jyoumei.cn/gtqwuxfwyf.html

Py:   s.splitlines()
来源：http://hz.redwolf501.top/gthrtuucsu.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.iojbl.cn/gtqtsbembi.html

JS:   s.split(/\r?\n/)
来源：http://hz.jianghu66.top/gtimbrwrpj.html

TS:   s.split(/\r?\n/)
来源：http://hz.jyoumei.cn/gtkafknoex.html

Java: s.lines().toList()
来源：http://hz.kuanghao11.cn/gteesrezhw.html

Go:   strings.Split(s, "\n")
来源：http://hz.havefunace.top/gtogcoyaon.html

Ruby: s.lines
来源：http://hz.nanxinkj.top/gtzgffgjem.html

C#:   s.Split('\n')
来源：http://hz.andypj.xyz/gtkmozbeuf.html

[E20] 判断字符串是否为空
来源：http://hz.tanke756.top/gtnspsuqbp.html

Py:   if not s:
来源：http://hz.shuidangran.top/gtxecylqkk.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.aizwys.cn/gtwigmixru.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.yongpay.top/gtslutmipq.html

TS:   if (s === "") {}
来源：http://hz.nanxuanxn.top/gtkmqarfcd.html

Java: if (s.isEmpty()) {}
来源：http://hz.sweek.top/gtlbtzxwui.html

Go:   if s == "" {}
来源：http://hz.ivvv.top/gtqefhsdpt.html

Ruby: if s.empty?
来源：http://hz.bjfxy.top/gtzmnffzlm.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.ydjk.org.cn/gtbsepssse.html

[E21] 超长截断加省略号
来源：http://hz.quarkkingdee.top/gtvzywtgxg.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.zhongyouzk.top/gtokrkgxmi.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.zhongyouzk.top/gtxnckocav.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yvedp.cn/gtasnivhfe.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.sufxvd.cn/gtrwsndsna.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.zhaomingkeji.xyz/gtekmakkjj.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.wangdashe.top/gtwnhcsewu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.zhijiandao.cn/gtosatrqhj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.zycfv.cn/gtidncoglj.html

[E22] 字节长度与字符长度
来源：http://hz.wangshuangyany.cn/gtvxkzyloq.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.gzhubu.top/gtgalkwsgg.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.jlsjyb.cn/gtmmyaldwu.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.xuanzx.com/gtvlrcvdzw.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhaomingkeji.xyz/gthaboaqmb.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.jyoumei.cn/gtarvwjukr.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.shanyushiyangkeji.top/gtzlkldtos.html

Ruby: s.bytesize;  s.length
来源：http://hz.yongpay.top/gtgipurwea.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.yj202588.top/gtgdeknxjf.html

================================================================================
来源：http://hz.cdnleiting.top/gtinlmoddm.html

F. 文件与目录
来源：http://hz.jinqigufen.top/gtdedotwis.html

================================================================================
来源：http://hz.cheryme.top/gtzbcwunes.html

[F01] 读取整个文件
来源：http://hz.andypj.xyz/gtnhfccysm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jinyuanbaomall.cn/gtdjfcehgj.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hywenlv.cn/gtosacpqrg.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.fengsongda.top/gttezzfydi.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.cashguo.top/gtebldyqdo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.xylfe.cn/gtihjlyccy.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.zhoulong.xyz/gthqwaeymv.html

Ruby: File.read("a.txt")
来源：http://hz.hysaishi.cn/gtkaocjipb.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.gotoacloud.top/gtntjbusfr.html

[F02] 逐行读取文件
来源：http://hz.ybcxt.top/gtwczuidmy.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.hnxiangtu.top/gtzxkqhawv.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.chenjidiqi.icu/gtnifkxbve.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.guowangkeji.top/gttbasuvyy.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ydzc1.top/gtvkusowxs.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.cashguo.top/gtchrngnpt.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.ivvv.top/gtluefdofy.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jinqigufen.top/gtwlrwntzb.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.xinyue.icu/gtorjniqct.html

[F03] 写入文件（覆盖）
来源：http://hz.yongpay.top/gthozgsykn.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.havefunace.top/gtoseldnhh.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.shuidangran.top/gtyshnzyod.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.fzhhl.top/gtckuclkls.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.316326.xyz/gtvclwxsta.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.c1oappe.top/gtcqtrjfov.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.316326.xyz/gtwsmgtjja.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.jinqigfzy.top/gtuezxinap.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.cashguo.top/gtdwrexamp.html

[F04] 追加写入文件
来源：http://hz.gogol.net.cn/gtfogepyik.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.jqgfzy.top/gtvuqjrpms.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.gogol.net.cn/gtjgeabfsb.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ywan-chungtsiang.top/gttweluhdf.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.shzxlz.cn/gtzpntwczh.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jqgfzy.top/gtidzzulfk.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.svipenyu.cn/gtwmeacewe.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yvedp.cn/gttabptjzi.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.zhengqikj.top/gtbkrfpijc.html

[F05] 判断文件或目录是否存在
来源：http://hz.yj20258888.top/gtscwkpfzc.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.nanxuanxn.top/gtniokmutf.html

PHP:  file_exists("a.txt");
来源：http://hz.andypj.xyz/gtssgyrdoi.html

JS:   fs.existsSync("a.txt")
来源：http://hz.wangdashe.top/gtjmzckusu.html

TS:   fs.existsSync("a.txt")
来源：http://hz.cheryme.top/gtuhqawjok.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.sxryk.cn/gtddjdevuo.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yvedp.cn/gtktffwjis.html

Ruby: File.exist?("a.txt")
来源：http://hz.shuidangran.top/gtijddfjuj.html

C#:   File.Exists("a.txt")
来源：http://hz.0kj1m.cn/gtoreqbufv.html

[F06] 删除文件
来源：http://hz.iojbl.cn/gtzzuandxl.html

Py:   os.remove("a.txt")
来源：http://hz.yj20258.top/gtrcvkuapd.html

PHP:  unlink("a.txt");
来源：http://hz.jyoumei.cn/gtlftnzyxh.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.sweek.top/gtqxiyiqcr.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.fengsongda.top/gtlphvzhud.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.meibo888.top/gtpobjjmki.html

Go:   os.Remove("a.txt")
来源：http://hz.yangfankeji.com/gtnzgfuygu.html

Ruby: File.delete("a.txt")
来源：http://hz.yvedp.cn/gtrapjuwfz.html

C#:   File.Delete("a.txt");
来源：http://hz.sxryk.cn/gtlezixomx.html

[F07] 创建目录（含多级）
来源：http://hz.jinqigfzy.top/gtqejtntmb.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.shangyingyoupin.top/gtaawcctmw.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zdqjudy.top/gtaynlzfxj.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.xziqi.cn/gtkrsgedur.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.sxryk.cn/gtltpomcwg.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.ywan-chungtsiang.top/gtzknavbns.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.jqgfzy.top/gtizldnjry.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.ywan-chungtsiang.top/gttvtliwat.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yj20258.top/gtnavwkvuf.html

[F08] 遍历目录
来源：http://hz.hammf.cn/gtzdbenypv.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xuanzx.com/gtvlncpxvb.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.tian-w.cn/gtovwejbmz.html

JS:   fs.readdirSync("dir")
来源：http://hz.shuidangran.top/gtxlzkvaep.html

TS:   fs.readdirSync("dir")
来源：http://hz.yvedp.cn/gtvbymscvt.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.meibo888.top/gtdidkkuik.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.shanyushiyangkeji.top/gtmceaujyh.html

Ruby: Dir.children("dir")
来源：http://hz.chenlongwang.top/gtbwgnbbfw.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yueranfly.top/gtwckxzqgg.html

[F09] 获取文件大小
来源：http://hz.chenzaomai.com/gtmhlmzyat.html

Py:   os.path.getsize("a.txt")
来源：http://hz.nanxuanxn.top/gtbclhmkfo.html

PHP:  filesize("a.txt");
来源：http://hz.zycfv.cn/gttumlhgic.html

JS:   fs.statSync("a.txt").size
来源：http://hz.sysykeji.top/gttgidmtfs.html

TS:   fs.statSync("a.txt").size
来源：http://hz.birdmap.top/gteobsypmz.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.shangyingyoupin.top/gtlywdsjxj.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jlsjyb.cn/gtxwofnbjf.html

Ruby: File.size("a.txt")
来源：http://hz.redwolf501.top/gtsykkersc.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.c1oappe.top/gtpwzvfqqe.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.shzxlz.cn/gtvbdmkift.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.xinyue.icu/gtvizniyus.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.chenlongwang.top/gtzgmstxgx.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.daria6918.cn/gtxrvsyblq.html

TS:   path.extname("a.txt")
来源：http://hz.shanyushiyangtech.top/gtmqifgixa.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jianghu66.top/gtnnslwdgb.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.zhengqikj.top/gtdukvcysr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.hammf.cn/gtjnwohfgg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.birdmap.top/gtomonhnjy.html

[F11] 复制与移动文件
来源：http://hz.zhiwuduotai.top/gtbnctiktb.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.hfpthk.cn/gtccdugmjg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.nanxuanxn.top/gtbnqlwhqi.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.feifeiyinyue.top/gtpshemmpz.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.bjfxy.top/gtmbhetwex.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.redwolf501.top/gtriwajntk.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.shangyingyoupin.top/gtapttvxia.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.chenzaomai.com/gtasiewnlv.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hysaishi.cn/gtgcpsmmbk.html

[F12] CSV 读写
来源：http://hz.kuanghao11.cn/gtmoymxfft.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jqgfzy.top/gtolngsukh.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.jiagoushi.top/gtbhcobbcg.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.aibaodan.cn/gtuxmpyqoe.html

TS:   // 同上
来源：http://hz.bjfxy.top/gtkrwxqckk.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.iojbl.cn/gtwqlxdxen.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.gogol.net.cn/gturtftbbc.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.shuidangran.top/gtzdefvehg.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.havefunace.top/gtscdljsak.html

================================================================================
来源：http://hz.sweek.top/gtwunopwzs.html

G. 面向对象
来源：http://hz.0kj1m.cn/gthmneklzs.html

================================================================================
来源：http://hz.smart0.xyz/gtcfwuvjgk.html

[G01] 定义类
来源：http://hz.cashguo.top/gtcpnpnybi.html

Py:   class User: pass
来源：http://hz.shanyushiyangkeji.top/gtzwcgqapp.html

PHP:  class User {}
来源：http://hz.mhx1999.top/gtelatalir.html

JS:   class User {}
来源：http://hz.zhijiandao.cn/gtahtuhifb.html

TS:   class User { name: string = ""; }
来源：http://hz.xinyue.icu/gtmlacemua.html

Java: class User {}
来源：http://hz.jqgfzy.top/gtssuzrefs.html

Go:   type User struct { Name string }
来源：http://hz.chenlongwang.top/gtufazpvbi.html

Ruby: class User; end
来源：http://hz.9152youxi.cn/gtypxuarnr.html

C#:   class User {}
来源：http://hz.gogol.net.cn/gtluvdxfge.html

[G02] 构造函数
来源：http://hz.zhijiandao.cn/gterrszkmb.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.iojbl.cn/gtrkcyegyv.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.andypj.xyz/gtzypravxg.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.tianlin.xyz/gtmjlrasez.html

TS:   constructor(public name: string) {}
来源：http://hz.iojbl.cn/gtcgqkqqrf.html

Java: User(String name) { this.name = name; }
来源：http://hz.ivvv.top/gtauqalwkn.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.shuidangran.top/gtmqqrnrig.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.bjfxy.top/gttlohtpup.html

C#:   public User(string name) { Name = name; }
来源：http://hz.tianlin.xyz/gtycpejlrz.html

[G03] 实例属性
来源：http://hz.cucudq.cn/gtapjulobj.html

Py:   self.name = "x"
来源：http://hz.meibo888.top/gtvjtvyvka.html

PHP:  public string $name = "x";
来源：http://hz.chenlongwang.top/gtxfvvcqhn.html

JS:   this.name = "x";
来源：http://hz.hywenlv.cn/gtigxdvqjj.html

TS:   name: string = "x";
来源：http://hz.ehwqpu.com/gtqtqzhvnc.html

Java: private String name;
来源：http://hz.yuxming.cn/gtdrkxcjgk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jyoumei.cn/gtsyxumima.html

Ruby: @name = "x"
来源：http://hz.yj20258.top/gtmjwfepuz.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.svipenyu.cn/gtghwzlqvd.html

[G04] 定义方法
来源：http://hz.zhongyouzk.top/gtqbamyozb.html

Py:   def greet(self): return self.name
来源：http://hz.tianlin.xyz/gtquibslqb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.ehwqpu.com/gttforukjv.html

JS:   greet() { return this.name; }
来源：http://hz.shzxlz.cn/gtnkuchlkz.html

TS:   greet(): string { return this.name; }
来源：http://hz.xylfe.cn/gtyyuiogwx.html

Java: String greet() { return name; }
来源：http://hz.nanxinkj.top/gtfpiwjjox.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.pengpengdd.cyou/gtfkcctlmb.html

Ruby: def greet; @name; end
来源：http://hz.gogol.net.cn/gthokrnwyk.html

C#:   public string Greet() => Name;
来源：http://hz.zhengqikj.top/gtttpjnoiw.html

[G05] 继承
来源：http://hz.xinyue.icu/gtianzefjf.html

Py:   class Admin(User): pass
来源：http://hz.ydzc1.top/gtelyflazr.html

PHP:  class Admin extends User {}
来源：http://hz.0kj1m.cn/gtqkslueqt.html

JS:   class Admin extends User {}
来源：http://hz.vqdsnc.cn/gtcckitilw.html

TS:   class Admin extends User {}
来源：http://hz.bjfxy.top/gtyykwdwxg.html

Java: class Admin extends User {}
来源：http://hz.ybcxt.top/gtnwykwdug.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.xuetiantiany.cn/gtesygbpps.html

Ruby: class Admin < User; end
来源：http://hz.pengpengdd.cyou/gtrglpavrl.html

C#:   class Admin : User {}
来源：http://hz.zhijiandao.cn/gtzhqlgusf.html

[G06] 重写方法
来源：http://hz.wangdashe.top/gtbanjcfpe.html

Py:   def greet(self): return "admin"
来源：http://hz.shangyingyoupin.top/gtcggydjxc.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.svipenyu.cn/gtkmreddmx.html

JS:   greet() { return "admin"; }
来源：http://hz.xuanzx.com/gtdjropwzp.html

TS:   greet(): string { return "admin"; }
来源：http://hz.9152youxi.cn/gtdvvbnmkz.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.xziqi.cn/gtvkuolnqk.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.hongshengwenyu.top/gtrbkqheax.html

Ruby: def greet; "admin"; end
来源：http://hz.pengpengdd.cyou/gtjerbzgyr.html

C#:   public override string Greet() => "admin";
来源：http://hz.jiagoushi.top/gtnmziewlc.html

[G07] 调用父类方法
来源：http://hz.cqqwz.cn/gtudyxcuce.html

Py:   super().greet()
来源：http://hz.c1oappe.top/gtytgrdvsr.html

PHP:  parent::greet();
来源：http://hz.smart0.xyz/gtdernenhj.html

JS:   super.greet();
来源：http://hz.hywenlv.cn/gtpdjxlbpk.html

TS:   super.greet();
来源：http://hz.zhijiandao.cn/gtfqsyfllh.html

Java: super.greet();
来源：http://hz.nwbrower.top/gthplrneuc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.hfpthk.cn/gtjgcjtzlo.html

Ruby: super
来源：http://hz.yvedp.cn/gtvpsypxbj.html

C#:   base.Greet();
来源：http://hz.snrcjt.cn/gtumqqgeec.html

[G08] 静态方法与属性
来源：http://hz.hnxiangtu.top/gtvmiuoypr.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.nanxuanxn.top/gtwezqdoss.html

PHP:  public static function f() {}
来源：http://hz.wangdashe.top/gtyrzqtfrx.html

JS:   static f() {}
来源：http://hz.hysaishi.cn/gtrhkeprfd.html

TS:   static f(): void {}
来源：http://hz.aibaodan.cn/gtjlhscfdb.html

Java: static void f() {}
来源：http://hz.zhiwuduotai.top/gtnixcnzgv.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.sxryk.cn/gteqrkuyzw.html

Ruby: def self.f; end
来源：http://hz.316326.xyz/gtoewifsaq.html

C#:   public static void F() {}
来源：http://hz.tanke756.top/gtkuidzhyn.html

[G09] 接口 / 抽象类
来源：http://hz.nanxuanxn.top/gtxclafpgy.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yangfankeji.com/gtbxtceyzl.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ydjk.org.cn/gtgsezzbig.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.9152youxi.cn/gtarcpybvi.html

TS:   interface Shape { area(): number; }
来源：http://hz.316326.xyz/gtyaitjaep.html

Java: interface Shape { double area(); }
来源：http://hz.hnxiangtu.top/gtasozpprd.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.andypj.xyz/gtrpwccact.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.feifeiyinyue.top/gttrpnnxyj.html

C#:   interface IShape { double Area(); }
来源：http://hz.yonumen.top/gtqkmzyqwo.html

[G10] 访问控制
来源：http://hz.yj20258888.top/gtedzzpqqz.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.smart0.xyz/gtbrtndruv.html

PHP:  public / protected / private
来源：http://hz.gaohongyu789.top/gtlksrajtl.html

JS:   #private 字段；其余公开
来源：http://hz.zdqjudy.top/gtorrnkkty.html

TS:   public / protected / private
来源：http://hz.yj20258.top/gtdjlbkads.html

Java: public / protected / private / 默认包级
来源：http://hz.ehwqpu.com/gtxhxhnyzi.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.aibaodan.cn/gturaqvthj.html

Ruby: public / protected / private
来源：http://hz.chenzaomai.com/gtqhkswfkf.html

C#:   public / protected / private / internal
来源：http://hz.yueranfly.top/gtajhblibw.html

[G11] getter / setter
来源：http://hz.nwbrower.top/gtdkfzlqsk.html

Py:   @property 与 @x.setter
来源：http://hz.zdqjudy.top/gtmimxnrws.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.yj20258.top/gtrvqytuqi.html

JS:   get name() { return this._name; }
来源：http://hz.hysaishi.cn/gtjbmcsjfv.html

TS:   get name(): string { return this._name; }
来源：http://hz.yuxming.cn/gtpvkqpfgz.html

Java: public String getName() { return name; }
来源：http://hz.ivvv.top/gtsfwoqocf.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.bjfxy.top/gtdjqdtcwl.html

Ruby: attr_accessor :name
来源：http://hz.tanke756.top/gtovbchzwq.html

C#:   public string Name { get; set; }
来源：http://hz.zycfv.cn/gtysxqjehh.html

[G12] 对象转字符串
来源：http://hz.shuidangran.top/gtfcljavzu.html

Py:   def __str__(self): return self.name
来源：http://hz.xuanzx.com/gtqsfvuygt.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zdqjudy.top/gtwsyeesxa.html

JS:   toString() { return this.name; }
来源：http://hz.shuidangran.top/gtxqyyiipj.html

TS:   toString(): string { return this.name; }
来源：http://hz.jqgfzy.top/gtemdezswf.html

Java: @Override public String toString() { return name; }
来源：http://hz.ybcxt.top/gtayxdbhei.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.kuanghao11.cn/gtlurroywo.html

Ruby: def to_s; @name; end
来源：http://hz.mhx1999.top/gtrqjrpeoh.html

C#:   public override string ToString() => Name;
来源：http://hz.xinyue.icu/gtnvwhojns.html

[G13] 判断对象类型
来源：http://hz.xinyue.icu/gtkkfqnjkv.html

Py:   isinstance(u, User)
来源：http://hz.jlsjyb.cn/gtmvglacwk.html

PHP:  $u instanceof User
来源：http://hz.smart0.xyz/gtbgdquicw.html

JS:   u instanceof User
来源：http://hz.cucudq.cn/gtezcziubx.html

TS:   u instanceof User
来源：http://hz.ywan-chungtsiang.top/gtxmhmpmwm.html

Java: u instanceof User
来源：http://hz.hnqzz.top/gtxtrrrbaq.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.iojbl.cn/gtojfhzyom.html

Ruby: u.is_a?(User)
来源：http://hz.gaohongyu789.top/gtgrwotrje.html

C#:   u is User
来源：http://hz.yj20258888.top/gtijvbxkxv.html


<!-- 参考信息 -->