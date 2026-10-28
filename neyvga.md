代发 wailian999

TS:   encodeURIComponent(s);  btoa(s)
来源：http://hz.xuanzx.com/gtenrjrccb.html

Java: URLEncoder.encode(s, StandardCharsets.UTF_8);  Base64.getEncoder().encodeToString(bytes)
来源：http://hz.shuidangran.top/gttzdarfwm.html

Go:   url.QueryEscape(s);  base64.StdEncoding.EncodeToString([]byte(s))
来源：http://hz.andypj.xyz/gtioloijrz.html

Ruby: URI.encode_www_form_component(s);  [s].pack("m0")
来源：http://hz.shanyushiyangkeji.top/gtrwpljdwu.html

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.ppjwa.cn/gturyreuzj.html

[E15] HTML 转义 / 反转义
来源：http://hz.yonumen.top/gtfkaflzkn.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.quarkkingdee.top/gtwjirvfiv.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.hywenlv.cn/gtpawsewct.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.jlsjyb.cn/gtpagwetve.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.shanyushiyangkeji.top/gtvenzijvo.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.ppjwa.cn/gthslsiypb.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.gaohongyu789.top/gtyxbvdiig.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.jinqigfzy.top/gtvkbpocrc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.sysykeji.top/gttbaquloa.html

[E16] 数字千分位
来源：http://hz.jinyuanbaomall.cn/gtzhtltpmk.html

Py:   f"{1234567:,}"
来源：http://hz.yongpay.top/gtnihulvqi.html

PHP:  number_format(1234567);
来源：http://hz.gogol.net.cn/gtythiobor.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.hnxiangtu.top/gtspobyomj.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.fzhhl.top/gtjjiwproy.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.zdqjudy.top/gthvmqslne.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.tanke756.top/gtnmliqhec.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.chenzaomai.com/gtwmlmaaev.html

C#:   1234567.ToString("N0")
来源：http://hz.jiagoushi.top/gtwkfkrmfa.html

[E17] 首字母大写
来源：http://hz.xuetiantiany.cn/gtlrrqopha.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.zhongyouzk.top/gtmafmqcnp.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yanxiufei.cn/gtmmxnlolb.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.pycfn.com/gtdiybuura.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.tian-w.cn/gtnrdzwojo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.gotoacloud.top/gtpzyrkqou.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.cheryme.top/gtrrafmnkg.html

Ruby: s.capitalize
来源：http://hz.vqdsnc.cn/gtwqthufyw.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.guannengcc.top/gtlfbiikcb.html

[E18] 模板占位符替换
来源：http://hz.0kj1m.cn/gtguhopxyl.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.zhongyouzk.top/gtduabesen.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.ybcxt.top/gtehvcnntu.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.nanxuanxn.top/gtpvdvatdw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.jinqigufen.top/gtzqflxpym.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jqgufenzy.top/gtwmitphnc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.ydzc1.top/gtrhobaufw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.xylfe.cn/gthsbtibrd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.52xcode.cn/gtuuxhslqr.html

[E19] 多行文本按行拆分
来源：http://hz.guowangkeji.top/gtxyhsdqdf.html

Py:   s.splitlines()
来源：http://hz.xuetiantiany.cn/gtohphgass.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.yvedp.cn/gtcukuwmsl.html

JS:   s.split(/\r?\n/)
来源：http://hz.birdmap.top/gtskkechda.html

TS:   s.split(/\r?\n/)
来源：http://hz.jqgufenzy.top/gtqisfdgog.html

Java: s.lines().toList()
来源：http://hz.nanxuanxn.top/gtrjpucnjy.html

Go:   strings.Split(s, "\n")
来源：http://hz.jlsjyb.cn/gtummfadli.html

Ruby: s.lines
来源：http://hz.hysaishi.cn/gtrcgftdng.html

C#:   s.Split('\n')
来源：http://hz.yueranfly.top/gtirnsixxg.html

[E20] 判断字符串是否为空
来源：http://hz.cqqwz.cn/gtovcolojx.html

Py:   if not s:
来源：http://hz.yvedp.cn/gtsmpkwmqn.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.zhengqikj.top/gtjbvmymkc.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.gaohongyu789.top/gtkxvkjtqb.html

TS:   if (s === "") {}
来源：http://hz.birdmap.top/gtbvzpnswo.html

Java: if (s.isEmpty()) {}
来源：http://hz.c1oappe.top/gtfzzbgtml.html

Go:   if s == "" {}
来源：http://hz.ivvv.top/gtithayqrb.html

Ruby: if s.empty?
来源：http://hz.aibaodan.cn/gtedodgxdq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.jqgufenzy.top/gteafmpyyc.html

[E21] 超长截断加省略号
来源：http://hz.ydjk.org.cn/gtzwyggjqf.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.ydjk.org.cn/gtpzgrgvpc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yj20258.top/gtaiqontjj.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.zhongyouzk.top/gtpsgnemks.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.snrcjt.cn/gtqspnbytv.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.gzhubu.top/gtypcbotzx.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.316326.xyz/gtzkimflmz.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.dianchejie.cn/gtdqnwjglo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.snrcjt.cn/gtlkutkesd.html

[E22] 字节长度与字符长度
来源：http://hz.redwolf501.top/gtsiqrtcfx.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.sysykeji.top/gtdqobglhm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yvedp.cn/gtzktbkugq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.smart0.xyz/gtcejaufjb.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.meibo888.top/gtxbffhdmn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.wangdashe.top/gtdfvniotp.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.wangshuangyany.cn/gtajhbbptv.html

Ruby: s.bytesize;  s.length
来源：http://hz.9152youxi.cn/gtazwaopjd.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.shangyingyoupin.top/gtyqnuzczi.html

================================================================================
来源：http://hz.jqgufenzy.top/gtvmbibakb.html

F. 文件与目录
来源：http://hz.0kj1m.cn/gttcljuyhk.html

================================================================================
来源：http://hz.zhiwuduotai.top/gtrqczxaxj.html

[F01] 读取整个文件
来源：http://hz.cdnleiting.top/gtnuarxhui.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.zycfv.cn/gtedawlrqo.html

PHP:  file_get_contents("a.txt");
来源：http://hz.gzhubu.top/gtlzihwbej.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.gotoacloud.top/gtzsxkvnby.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.jinqigfzy.top/gtwntrchde.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.yanxiufei.cn/gtiogwoxhk.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.redwolf501.top/gtpgtndula.html

Ruby: File.read("a.txt")
来源：http://hz.yvedp.cn/gtqyvjjgim.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.ybcxt.top/gtpgpiiiie.html

[F02] 逐行读取文件
来源：http://hz.c1oappe.top/gtdpsblomn.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.jqgfzy.top/gtzabbmbbw.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.snrcjt.cn/gtqbizwfgh.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.sxryk.cn/gtlfttvyxw.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.c1oappe.top/gtpmszituo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.52xcode.cn/gtogkxfasz.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.tian-w.cn/gtqdrqiyba.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.shanyushiyangkeji.top/gtuqjehfvd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.cashguo.top/gtcdrntnqj.html

[F03] 写入文件（覆盖）
来源：http://hz.dianchejie.cn/gthbeajlhm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.xingfuxueyuan.xyz/gtdqcpcqpt.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jyoumei.cn/gtzbghqnss.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.hysaishi.cn/gtggaklghj.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xuanzx.com/gtpmzflomd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.nanxinkj.top/gtzccpzprj.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.bjfxy.top/gtoinxphqy.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.chenzaomai.com/gtwrfvsqlq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.zycfv.cn/gtkpnxtjwg.html

[F04] 追加写入文件
来源：http://hz.cucudq.cn/gtsibwtvnk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.cucudq.cn/gtomshdcwe.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.hammf.cn/gtvebfzanc.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhiwuduotai.top/gtzyjohndz.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.ybcxt.top/gthhaortoc.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.cqqwz.cn/gtndtmkmiw.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zhengqikj.top/gtnuuuqxhw.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.daxiang520.top/gthkxsoyhj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.zhaomingkeji.xyz/gtpksseooi.html

[F05] 判断文件或目录是否存在
来源：http://hz.yonumen.top/gtsisgblzm.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jlsjyb.cn/gtargozqpl.html

PHP:  file_exists("a.txt");
来源：http://hz.hysaishi.cn/gtrprrsfva.html

JS:   fs.existsSync("a.txt")
来源：http://hz.yj202588.top/gtjdjeoxrj.html

TS:   fs.existsSync("a.txt")
来源：http://hz.jqgfzy.top/gtjniiizcr.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.ppjwa.cn/gtstmzddbu.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.yueranfly.top/gtfsncxqtf.html

Ruby: File.exist?("a.txt")
来源：http://hz.aizwys.cn/gtclrerrvk.html

C#:   File.Exists("a.txt")
来源：http://hz.hongshengwenyu.top/gtrxwbxcmx.html

[F06] 删除文件
来源：http://hz.chenlongwang.top/gtybujsopt.html

Py:   os.remove("a.txt")
来源：http://hz.hywenlv.cn/gtxneztoxe.html

PHP:  unlink("a.txt");
来源：http://hz.zhoulong.xyz/gtethrsuue.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.xziqi.cn/gtjzqgqepa.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.zhengqikj.top/gtqfaqobex.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.zhiwuduotai.top/gtmosxybjx.html

Go:   os.Remove("a.txt")
来源：http://hz.snrcjt.cn/gtzxvwuqeq.html

Ruby: File.delete("a.txt")
来源：http://hz.pycfn.com/gteyriemrb.html

C#:   File.Delete("a.txt");
来源：http://hz.cashguo.top/gtphithiyt.html

[F07] 创建目录（含多级）
来源：http://hz.andypj.xyz/gtslkbghxe.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zhijiandao.cn/gtbvhdebop.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.ydzc1.top/gtxtzqlgdo.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hysaishi.cn/gtvalwibbr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.tanke756.top/gtuyqrwspk.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.jlsjyb.cn/gtelbnmirc.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.xylfe.cn/gtgulhjfhi.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.shzxlz.cn/gtqwgngsvg.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.havefunace.top/gtjllbmspq.html

[F08] 遍历目录
来源：http://hz.316326.xyz/gtxirnzfto.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.smart0.xyz/gtfgefcbnd.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.birdmap.top/gttwocsuyx.html

JS:   fs.readdirSync("dir")
来源：http://hz.sweek.top/gtjpkrvehr.html

TS:   fs.readdirSync("dir")
来源：http://hz.yanxiufei.cn/gtgjrbqqij.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.gaohongyu789.top/gtnpxyykrf.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.pycfn.com/gtfliqkiml.html

Ruby: Dir.children("dir")
来源：http://hz.shzxlz.cn/gttcbfyxvw.html

C#:   Directory.GetFiles("dir")
来源：http://hz.zhoulong.xyz/gturcawnkh.html

[F09] 获取文件大小
来源：http://hz.yj202588.top/gteugflffb.html

Py:   os.path.getsize("a.txt")
来源：http://hz.52xcode.cn/gtjimqawrh.html

PHP:  filesize("a.txt");
来源：http://hz.shanyushiyangkeji.top/gtbuxaeblj.html

JS:   fs.statSync("a.txt").size
来源：http://hz.sxryk.cn/gtyegrxczx.html

TS:   fs.statSync("a.txt").size
来源：http://hz.guannengcc.top/gtuxjafzfz.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.tianlin.xyz/gtsiepwemu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.sufxvd.cn/gtozcgzmpj.html

Ruby: File.size("a.txt")
来源：http://hz.jinghuilouyu.cn/gtkffhkoen.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.cqqwz.cn/gtnlhxydzq.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.ivvv.top/gtlnprfmpd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.zhongyouzk.top/gtbgwevwhx.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zycfv.cn/gtltpzdcgf.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.xuetiantiany.cn/gtbbprnkns.html

TS:   path.extname("a.txt")
来源：http://hz.nanxuanxn.top/gtgraxwaae.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.vqdsnc.cn/gtttlozpkn.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.cucudq.cn/gtmgnijsoc.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.birdmap.top/gtdjbgasit.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.zhijiandao.cn/gtvjshfeqj.html

[F11] 复制与移动文件
来源：http://hz.sysykeji.top/gtkrkohkfy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.vqdsnc.cn/gtvsgdwwtz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.mhx1999.top/gtaeicwqzs.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.haohaochexian.top/gtcyyxhwbh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.fengsongda.top/gtnxwksyax.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.yj20258888.top/gtzgmybhod.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hammf.cn/gttjdcmjli.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.chenlongwang.top/gtbcsslsxu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.tian-w.cn/gtiztpbvjp.html

[F12] CSV 读写
来源：http://hz.cucudq.cn/gtjishfhhz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.xuanzx.com/gtmttvqptl.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.yuanzhike.top/gtwoqqkyjy.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yuxming.cn/gtpsopxnmt.html

TS:   // 同上
来源：http://hz.iojbl.cn/gtkeccbabn.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.gaohongyu789.top/gtbikiarsj.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.gzhubu.top/gttipxvuhz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yanxiufei.cn/gtlbptztzn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.zhixingplan.top/gtmuuvkmfh.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtrmhxjuqa.html

G. 面向对象
来源：http://hz.yangfankeji.com/gtqwqgtpxc.html

================================================================================
来源：http://hz.gzhubu.top/gtixlheowu.html

[G01] 定义类
来源：http://hz.dashuyun.cn/gtdwvqfnki.html

Py:   class User: pass
来源：http://hz.shuidangran.top/gtggxvxgdc.html

PHP:  class User {}
来源：http://hz.ydzc1.top/gtusulrubi.html

JS:   class User {}
来源：http://hz.xylfe.cn/gtfdnhpshe.html

TS:   class User { name: string = ""; }
来源：http://hz.zhaomingkeji.xyz/gtavkifank.html

Java: class User {}
来源：http://hz.0kj1m.cn/gtgvxqrogo.html

Go:   type User struct { Name string }
来源：http://hz.jiagoushi.top/gtnmvngqqu.html

Ruby: class User; end
来源：http://hz.hnxiangtu.top/gtejbnghcc.html

C#:   class User {}
来源：http://hz.shanyushiyangtech.top/gtniptmsco.html

[G02] 构造函数
来源：http://hz.yuxming.cn/gttadrthkt.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.nanxinkj.top/gtaavfpdis.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.hysaishi.cn/gteshmfpbb.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.nanxuanxn.top/gthhyetaoq.html

TS:   constructor(public name: string) {}
来源：http://hz.yj20258888.top/gtuxvlxnjx.html

Java: User(String name) { this.name = name; }
来源：http://hz.9152youxi.cn/gtvvzmsfmg.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.shuidangran.top/gttvqenhmc.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jinyuanbaomall.cn/gtntkuihdz.html

C#:   public User(string name) { Name = name; }
来源：http://hz.xuetiantiany.cn/gthdrbmpxm.html

[G03] 实例属性
来源：http://hz.bjfxy.top/gtkkxxgahw.html

Py:   self.name = "x"
来源：http://hz.zhiwuduotai.top/gtohxzbxqg.html

PHP:  public string $name = "x";
来源：http://hz.mhx1999.top/gtfmzlhcrp.html

JS:   this.name = "x";
来源：http://hz.andypj.xyz/gtcjivklzm.html

TS:   name: string = "x";
来源：http://hz.zycfv.cn/gtrjnkkqzg.html

Java: private String name;
来源：http://hz.nanxuanxn.top/gtcsensjia.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zhengqikj.top/gtoiadscge.html

Ruby: @name = "x"
来源：http://hz.jlsjyb.cn/gtzmfyhxbf.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.9152youxi.cn/gtjgaaxszn.html

[G04] 定义方法
来源：http://hz.zhoulong.xyz/gtuxnlszyo.html

Py:   def greet(self): return self.name
来源：http://hz.haohaochexian.top/gtwbxyrjqr.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.gzhubu.top/gtvbdbmxqd.html

JS:   greet() { return this.name; }
来源：http://hz.yonumen.top/gtwdaeqpci.html

TS:   greet(): string { return this.name; }
来源：http://hz.cqqwz.cn/gtiranxpkm.html

Java: String greet() { return name; }
来源：http://hz.shangyingyoupin.top/gtgshrdcqv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.cdnleiting.top/gthbsxqeqy.html

Ruby: def greet; @name; end
来源：http://hz.quarkkingdee.top/gthqgtjuex.html

C#:   public string Greet() => Name;
来源：http://hz.daxiang520.top/gtidkbwcss.html

[G05] 继承
来源：http://hz.jinyuanbaomall.cn/gtywhaydpd.html

Py:   class Admin(User): pass
来源：http://hz.havefunace.top/gtnftlizzn.html

PHP:  class Admin extends User {}
来源：http://hz.fzhhl.top/gtqwzeblah.html

JS:   class Admin extends User {}
来源：http://hz.0kj1m.cn/gtkdgsbgzw.html

TS:   class Admin extends User {}
来源：http://hz.tian-w.cn/gtngaybyaj.html

Java: class Admin extends User {}
来源：http://hz.9152youxi.cn/gtedbtcvro.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.ehwqpu.com/gtvnzileer.html

Ruby: class Admin < User; end
来源：http://hz.yanxiufei.cn/gtzgeoszhj.html

C#:   class Admin : User {}
来源：http://hz.ydzc1.top/gttywatihh.html

[G06] 重写方法
来源：http://hz.hysaishi.cn/gtxzthoifh.html

Py:   def greet(self): return "admin"
来源：http://hz.yonumen.top/gtzpahzvwr.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.ppjwa.cn/gtipebvymk.html

JS:   greet() { return "admin"; }
来源：http://hz.havefunace.top/gthkmorshj.html

TS:   greet(): string { return "admin"; }
来源：http://hz.tanke756.top/gtlsrtlayt.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.sufxvd.cn/gtahwayqlb.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.hysaishi.cn/gtijokreoy.html

Ruby: def greet; "admin"; end
来源：http://hz.cqqwz.cn/gtirsdvlrj.html

C#:   public override string Greet() => "admin";
来源：http://hz.pengpengdd.cyou/gtialtvvoa.html

[G07] 调用父类方法
来源：http://hz.guannengcc.top/gtgzuoopbe.html

Py:   super().greet()
来源：http://hz.aizwys.cn/gtqdgfucjq.html

PHP:  parent::greet();
来源：http://hz.jlsjyb.cn/gtmnnutxsm.html

JS:   super.greet();
来源：http://hz.shanyushiyangtech.top/gtckbiggbz.html

TS:   super.greet();
来源：http://hz.hongshengwenyu.top/gtpafqmauf.html

Java: super.greet();
来源：http://hz.pycfn.com/gtppxbzpiu.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.sxryk.cn/gtpdeaoext.html

Ruby: super
来源：http://hz.ppjwa.cn/gtstvomwpc.html

C#:   base.Greet();
来源：http://hz.hongshengwenyu.top/gtbpphrevk.html

[G08] 静态方法与属性
来源：http://hz.sxryk.cn/gtpjkbuxeq.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.jinqigfzy.top/gtlqrnfgqc.html

PHP:  public static function f() {}
来源：http://hz.chenlongwang.top/gthwdklkce.html

JS:   static f() {}
来源：http://hz.nwbrower.top/gtadodkdse.html

TS:   static f(): void {}
来源：http://hz.cqqwz.cn/gtathfztgl.html

Java: static void f() {}
来源：http://hz.yj202588.top/gtvzcmrwsr.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.bjfxy.top/gtllwurgrx.html

Ruby: def self.f; end
来源：http://hz.vqdsnc.cn/gtujkudzoa.html

C#:   public static void F() {}
来源：http://hz.yuxming.cn/gtobtmsayi.html

[G09] 接口 / 抽象类
来源：http://hz.daria6918.cn/gtjymbmrmh.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.zycfv.cn/gtkoznzxlf.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ybcxt.top/gtnfeunvym.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.jinyuanbaomall.cn/gtferhblhp.html

TS:   interface Shape { area(): number; }
来源：http://hz.kuanghao11.cn/gteelrmpjs.html

Java: interface Shape { double area(); }
来源：http://hz.quarkkingdee.top/gtetiqmult.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.0kj1m.cn/gtdnvyciul.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.jinyuanbaomall.cn/gtclkciitp.html

C#:   interface IShape { double Area(); }
来源：http://hz.shanyushiyangtech.top/gtvxnboqdr.html

[G10] 访问控制
来源：http://hz.vqdsnc.cn/gtojwbmvzj.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.gogol.net.cn/gtvfllgjuc.html

PHP:  public / protected / private
来源：http://hz.gogol.net.cn/gtzqgrzqvz.html

JS:   #private 字段；其余公开
来源：http://hz.shanyushiyangtech.top/gtqmpuffdg.html

TS:   public / protected / private
来源：http://hz.daria6918.cn/gtfbkwvkou.html

Java: public / protected / private / 默认包级
来源：http://hz.aizwys.cn/gtyttcikph.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.xuetiantiany.cn/gtybhvratr.html

Ruby: public / protected / private
来源：http://hz.0kj1m.cn/gtostsncfk.html

C#:   public / protected / private / internal
来源：http://hz.feifeiyinyue.top/gtkoiqyvfa.html

[G11] getter / setter
来源：http://hz.zycfv.cn/gtaxtsaqgl.html

Py:   @property 与 @x.setter
来源：http://hz.cucudq.cn/gtbydmfbrt.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.chenlongwang.top/gtwjnqggsn.html

JS:   get name() { return this._name; }
来源：http://hz.jyoumei.cn/gtzqacxtoy.html

TS:   get name(): string { return this._name; }
来源：http://hz.birdmap.top/gtrgrlkdzg.html

Java: public String getName() { return name; }
来源：http://hz.dianchejie.cn/gtcdquzzhe.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.havefunace.top/gtdhrfcoid.html

Ruby: attr_accessor :name
来源：http://hz.ppjwa.cn/gtlfdntrsd.html

C#:   public string Name { get; set; }
来源：http://hz.bjfxy.top/gtbxroxxxw.html

[G12] 对象转字符串
来源：http://hz.yongpay.top/gtesrnakmp.html

Py:   def __str__(self): return self.name
来源：http://hz.tanke756.top/gtnabvysus.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.hfpthk.cn/gtlmeogkxs.html

JS:   toString() { return this.name; }
来源：http://hz.dashuyun.cn/gtmujafegu.html

TS:   toString(): string { return this.name; }
来源：http://hz.birdmap.top/gtikoewqik.html

Java: @Override public String toString() { return name; }
来源：http://hz.jinyuanbaomall.cn/gtdgrhwtkh.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.hongshengwenyu.top/gtyashuxcr.html

Ruby: def to_s; @name; end
来源：http://hz.jinyuanbaomall.cn/gtjklyncbo.html

C#:   public override string ToString() => Name;
来源：http://hz.wangshuangyany.cn/gtizywwfcn.html

[G13] 判断对象类型
来源：http://hz.hongshengwenyu.top/gtvmcmptlb.html


<!-- 参考信息 -->