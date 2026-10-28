代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.ivvv.top/gtpajxjxnr.html

[E15] HTML 转义 / 反转义
来源：http://hz.zhoulong.xyz/gtbcryelxv.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.iojbl.cn/gthtcyfewk.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.guannengcc.top/gttfnqtqxe.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.cqqwz.cn/gttpnlwndw.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.pycfn.com/gtixfsghtk.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.haohaochexian.top/gtyvuosdve.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.xuetiantiany.cn/gthghjdfee.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.ybcxt.top/gtzekrlfze.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.bjfxy.top/gtfjsycgyh.html

[E16] 数字千分位
来源：http://hz.wangdashe.top/gtrcboxbnj.html

Py:   f"{1234567:,}"
来源：http://hz.shanyushiyangtech.top/gtegpeilom.html

PHP:  number_format(1234567);
来源：http://hz.nwbrower.top/gtkdqoqamq.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.iojbl.cn/gtpfmuuqia.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.zdqjudy.top/gtkkjhbjzj.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.sweek.top/gtsazylrlc.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.xziqi.cn/gtpwynolnn.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.hfpthk.cn/gtepgjotbd.html

C#:   1234567.ToString("N0")
来源：http://hz.zdqjudy.top/gtydczcezu.html

[E17] 首字母大写
来源：http://hz.hysaishi.cn/gtzjpjiwgn.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.mhx1999.top/gtkeutaodf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.jinqigufen.top/gtgmdizdcx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cucudq.cn/gtgicyicjk.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jqgfzy.top/gthukrdouo.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.cashguo.top/gtcwhbppui.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.chenjidiqi.icu/gtzlkhwgoy.html

Ruby: s.capitalize
来源：http://hz.andypj.xyz/gtfvmqjhay.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.redwolf501.top/gtvxnwhvee.html

[E18] 模板占位符替换
来源：http://hz.xylfe.cn/gtqhuswfmp.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.xingfuxueyuan.xyz/gtxbtgqdyo.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.dianchejie.cn/gtukowovon.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.hywenlv.cn/gtcbwhgghv.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.cucudq.cn/gtifhbyfro.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.snrcjt.cn/gtbbtcyvgy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.c1oappe.top/gtarfyokfh.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.smart0.xyz/gtcazucmgj.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.bjfxy.top/gtntmrlbxz.html

[E19] 多行文本按行拆分
来源：http://hz.hammf.cn/gtxckjakbk.html

Py:   s.splitlines()
来源：http://hz.hnxiangtu.top/gtlgrznfcp.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.vqdsnc.cn/gtbngymcqv.html

JS:   s.split(/\r?\n/)
来源：http://hz.9152youxi.cn/gttvdgnxrd.html

TS:   s.split(/\r?\n/)
来源：http://hz.svipenyu.cn/gtgbhldlfy.html

Java: s.lines().toList()
来源：http://hz.hfpthk.cn/gtkhxiafhm.html

Go:   strings.Split(s, "\n")
来源：http://hz.shuidangran.top/gtxexxgbub.html

Ruby: s.lines
来源：http://hz.yvedp.cn/gtocbflgrc.html

C#:   s.Split('\n')
来源：http://hz.redwolf501.top/gtudydvpit.html

[E20] 判断字符串是否为空
来源：http://hz.zhoulong.xyz/gtgzblffpa.html

Py:   if not s:
来源：http://hz.svipenyu.cn/gtgggzeoer.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.snrcjt.cn/gteqcocstr.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.sufxvd.cn/gttpztbkjr.html

TS:   if (s === "") {}
来源：http://hz.quarkkingdee.top/gtyqolifpq.html

Java: if (s.isEmpty()) {}
来源：http://hz.cdnleiting.top/gteuaxuygb.html

Go:   if s == "" {}
来源：http://hz.iojbl.cn/gtpbeltcld.html

Ruby: if s.empty?
来源：http://hz.aizwys.cn/gtbtwofwdx.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.316326.xyz/gtoonnqqje.html

[E21] 超长截断加省略号
来源：http://hz.yj20258888.top/gttioliliu.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.shanyushiyangtech.top/gtwpbjpvbm.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.sweek.top/gtqrnnwnaf.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.aibaodan.cn/gtclfcdlzm.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.ivvv.top/gteabfbvcp.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.jiagoushi.top/gtpnlqxmlf.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.xuetiantiany.cn/gtjxrwpfvu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.zycfv.cn/gtsacvopqo.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.tianlin.xyz/gtljmojtlz.html

[E22] 字节长度与字符长度
来源：http://hz.haohaochexian.top/gtgjpjptic.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.sysykeji.top/gtflsuhzvd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yj20258888.top/gtkdyvigcm.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.c1oappe.top/gtcqtshthu.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jianghu66.top/gteelelogr.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.hnxiangtu.top/gtkufeaxes.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.c1oappe.top/gtcywnffrt.html

Ruby: s.bytesize;  s.length
来源：http://hz.snrcjt.cn/gtlbinnmgr.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jiagoushi.top/gtsaieujnl.html

================================================================================
来源：http://hz.dashuyun.cn/gtlatovguk.html

F. 文件与目录
来源：http://hz.yj20258.top/gtekmkfetc.html

================================================================================
来源：http://hz.quarkkingdee.top/gtsnpowmam.html

[F01] 读取整个文件
来源：http://hz.bjfxy.top/gtybcwvqmn.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.jinyuanbaomall.cn/gtllvnzxyr.html

PHP:  file_get_contents("a.txt");
来源：http://hz.jiagoushi.top/gtlvmzqnht.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.ehwqpu.com/gtcaalmqon.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.nwbrower.top/gtvxfayluq.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.pengpengdd.cyou/gtegjnovoj.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.xuanzx.com/gtdvbbbqol.html

Ruby: File.read("a.txt")
来源：http://hz.aizwys.cn/gtkgqgnyol.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.yj20258888.top/gtzqzscmmd.html

[F02] 逐行读取文件
来源：http://hz.cashguo.top/gtarwdzibs.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.ppjwa.cn/gtjmktguih.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.zycfv.cn/gtxhqylpjo.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.cashguo.top/gtjivqawzd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.nwbrower.top/gtbtecgywo.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.yvedp.cn/gtkdzvajmn.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.birdmap.top/gtreqdejba.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.redwolf501.top/gtpkmjzous.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.yj202588.top/gtyqxuktgt.html

[F03] 写入文件（覆盖）
来源：http://hz.tianlin.xyz/gthawuwawm.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.hongshengwenyu.top/gthvfjeden.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jianghu66.top/gtmzedmqgb.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.kuanghao11.cn/gtvdbrxcks.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.yongpay.top/gtdfkjxesd.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.ydzc1.top/gtwftcdqfz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.shangyingyoupin.top/gtgpuzlwiu.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.hongshengwenyu.top/gtulbcsjzv.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.hywenlv.cn/gtbpyvwxmv.html

[F04] 追加写入文件
来源：http://hz.zhaomingkeji.xyz/gtgjewknrf.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.feifeiyinyue.top/gtniobuzyh.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.pengpengdd.cyou/gtekbdnlxt.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.guannengcc.top/gteanxsxyr.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.pycfn.com/gtepcjdgpn.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jlsjyb.cn/gtftpubeit.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.nanxinkj.top/gtcnluqoes.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yj20258.top/gtbmovqhew.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.0kj1m.cn/gtbgdifmwe.html

[F05] 判断文件或目录是否存在
来源：http://hz.sweek.top/gtmbpvwann.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zhiwuduotai.top/gtzlynrtpj.html

PHP:  file_exists("a.txt");
来源：http://hz.jinghuilouyu.cn/gtfskbesnh.html

JS:   fs.existsSync("a.txt")
来源：http://hz.c1oappe.top/gtcclkhezu.html

TS:   fs.existsSync("a.txt")
来源：http://hz.kuanghao11.cn/gtvkiygjqw.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.haohaochexian.top/gtziwaejyg.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.wangshuangyany.cn/gtalguhtdg.html

Ruby: File.exist?("a.txt")
来源：http://hz.tian-w.cn/gtzskepwwu.html

C#:   File.Exists("a.txt")
来源：http://hz.c1oappe.top/gtkwmfczjl.html

[F06] 删除文件
来源：http://hz.sxryk.cn/gtpgepuozn.html

Py:   os.remove("a.txt")
来源：http://hz.chenzaomai.com/gtafzqotyv.html

PHP:  unlink("a.txt");
来源：http://hz.xuanzx.com/gttwqhlapb.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.xziqi.cn/gtberpgyqk.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.pengpengdd.cyou/gtmninajew.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jlsjyb.cn/gtnloakdkf.html

Go:   os.Remove("a.txt")
来源：http://hz.guowangkeji.top/gtdivujlgl.html

Ruby: File.delete("a.txt")
来源：http://hz.xuanzx.com/gtjwjrgjsf.html

C#:   File.Delete("a.txt");
来源：http://hz.jinqigufen.top/gtaohblzch.html

[F07] 创建目录（含多级）
来源：http://hz.shanyushiyangkeji.top/gttvsklpgw.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hywenlv.cn/gtlamzamlf.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.gaohongyu789.top/gtajlzceqk.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.iojbl.cn/gtxenwxvus.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.gogol.net.cn/gtkbpdesqx.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.hywenlv.cn/gtfhguhhgn.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.chenlongwang.top/gtbvitrujg.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.ydjk.org.cn/gtsvvpxdmt.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.ppjwa.cn/gtoirqnkyo.html

[F08] 遍历目录
来源：http://hz.chenjidiqi.icu/gtiveqwipw.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jiagoushi.top/gtslebgyrk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.316326.xyz/gtvvidjjmo.html

JS:   fs.readdirSync("dir")
来源：http://hz.yangfankeji.com/gtwnvvvzbe.html

TS:   fs.readdirSync("dir")
来源：http://hz.gzhubu.top/gtrvyzbsxx.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.havefunace.top/gtpktqaapa.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zhongyouzk.top/gtemzwlckm.html

Ruby: Dir.children("dir")
来源：http://hz.hnxiangtu.top/gtjhfiindz.html

C#:   Directory.GetFiles("dir")
来源：http://hz.yangfankeji.com/gtfykjhxhn.html

[F09] 获取文件大小
来源：http://hz.zhoulong.xyz/gtyhhkusen.html

Py:   os.path.getsize("a.txt")
来源：http://hz.bjfxy.top/gtmwwsfwwo.html

PHP:  filesize("a.txt");
来源：http://hz.gotoacloud.top/gtpwmcavam.html

JS:   fs.statSync("a.txt").size
来源：http://hz.zhengqikj.top/gtsctibjge.html

TS:   fs.statSync("a.txt").size
来源：http://hz.jqgufenzy.top/gtmevghhnl.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.gzhubu.top/gtmfjbpwaq.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.gogol.net.cn/gtgmthltzq.html

Ruby: File.size("a.txt")
来源：http://hz.sweek.top/gtpekqgfyb.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.zhengqikj.top/gtclyyrjkq.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.shanyushiyangtech.top/gtptwtdspc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.nanxuanxn.top/gtywbuhjkz.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.hnxiangtu.top/gtypllidpz.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.zhengqikj.top/gtgsoioszb.html

TS:   path.extname("a.txt")
来源：http://hz.xziqi.cn/gtybingteh.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.sxryk.cn/gtybliypuz.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.52xcode.cn/gtsefurgqe.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.cheryme.top/gtpqkivghg.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.yj20258888.top/gthyonnmwk.html

[F11] 复制与移动文件
来源：http://hz.svipenyu.cn/gttqrmbicx.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.quarkkingdee.top/gtizswzpqw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.sweek.top/gtcpoednnk.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.tianlin.xyz/gtjyuficqs.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jianghu66.top/gtvcghxkrw.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.sweek.top/gthmkvklwj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.hfpthk.cn/gtxcazkgny.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.xuanzx.com/gtewxyadfm.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.chenlongwang.top/gtcpcwirti.html

[F12] CSV 读写
来源：http://hz.jinghuilouyu.cn/gttbeljvdy.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jinghuilouyu.cn/gtnbnstrfi.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.guannengcc.top/gtkabzvkwr.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.jyoumei.cn/gtjxqkgbza.html

TS:   // 同上
来源：http://hz.cheryme.top/gttfeeobrb.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.hammf.cn/gtbprtbnpq.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.ydzc1.top/gtzmalrckk.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.hnqzz.top/gtffgjeflq.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.chenjidiqi.icu/gtjsltcmcv.html

================================================================================
来源：http://hz.daria6918.cn/gtjjxnmvkq.html

G. 面向对象
来源：http://hz.pycfn.com/gtsnwclvoi.html

================================================================================
来源：http://hz.tianlin.xyz/gttpkmrmfl.html

[G01] 定义类
来源：http://hz.birdmap.top/gtlmjhznyj.html

Py:   class User: pass
来源：http://hz.yonumen.top/gtzontkyig.html

PHP:  class User {}
来源：http://hz.zhongyouzk.top/gthegqbela.html

JS:   class User {}
来源：http://hz.tanke756.top/gtiloninyw.html

TS:   class User { name: string = ""; }
来源：http://hz.nanxuanxn.top/gtoamyonjx.html

Java: class User {}
来源：http://hz.svipenyu.cn/gtyuqtycis.html

Go:   type User struct { Name string }
来源：http://hz.aibaodan.cn/gtjbkyvnti.html

Ruby: class User; end
来源：http://hz.yj202588.top/gtyucvfdxq.html

C#:   class User {}
来源：http://hz.fengsongda.top/gtqtyluhpr.html

[G02] 构造函数
来源：http://hz.yanxiufei.cn/gtwsljtdiu.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.yj20258888.top/gtfpxycdwf.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jinqigfzy.top/gtvnwpxeme.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.quarkkingdee.top/gtvgdjfejg.html

TS:   constructor(public name: string) {}
来源：http://hz.ivvv.top/gtkjhccrkp.html

Java: User(String name) { this.name = name; }
来源：http://hz.sysykeji.top/gtotgzeqxo.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.svipenyu.cn/gtlbxetlcn.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.nanxinkj.top/gtdhlwbkvh.html

C#:   public User(string name) { Name = name; }
来源：http://hz.daxiang520.top/gtdxnbwamc.html

[G03] 实例属性
来源：http://hz.xingfuxueyuan.xyz/gtiqegxsvt.html

Py:   self.name = "x"
来源：http://hz.gotoacloud.top/gtjtsmynjf.html

PHP:  public string $name = "x";
来源：http://hz.c1oappe.top/gtwstvczkz.html

JS:   this.name = "x";
来源：http://hz.yj20258888.top/gtsvsfanmv.html

TS:   name: string = "x";
来源：http://hz.smart0.xyz/gtlqqjxhwr.html

Java: private String name;
来源：http://hz.xuanzx.com/gtfgmdkwjg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.jinghuilouyu.cn/gtzgukpkia.html

Ruby: @name = "x"
来源：http://hz.sufxvd.cn/gtyjxsorsm.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.tianlin.xyz/gtrhblaipw.html

[G04] 定义方法
来源：http://hz.guannengcc.top/gtmcpedhtc.html

Py:   def greet(self): return self.name
来源：http://hz.birdmap.top/gtukznhhnk.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.guannengcc.top/gtronixjkf.html

JS:   greet() { return this.name; }
来源：http://hz.ydzc1.top/gtqxjcblgh.html

TS:   greet(): string { return this.name; }
来源：http://hz.yuanzhike.top/gttzbjbvqf.html

Java: String greet() { return name; }
来源：http://hz.hnxiangtu.top/gtrrptspdu.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ydjk.org.cn/gttfwlsvah.html

Ruby: def greet; @name; end
来源：http://hz.shzxlz.cn/gtmlkngvgh.html

C#:   public string Greet() => Name;
来源：http://hz.yonumen.top/gtynfbcvbh.html

[G05] 继承
来源：http://hz.jinghuilouyu.cn/gtempwmcyf.html

Py:   class Admin(User): pass
来源：http://hz.jqgufenzy.top/gtdscsbtjb.html

PHP:  class Admin extends User {}
来源：http://hz.zdqjudy.top/gtpzcultwq.html

JS:   class Admin extends User {}
来源：http://hz.wangshuangyany.cn/gtqxxvdggi.html

TS:   class Admin extends User {}
来源：http://hz.cqqwz.cn/gtishpgvzz.html

Java: class Admin extends User {}
来源：http://hz.jqgufenzy.top/gtnvujbvhh.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.svipenyu.cn/gtyvrwqdhs.html

Ruby: class Admin < User; end
来源：http://hz.yj20258.top/gtywbtuquu.html

C#:   class Admin : User {}
来源：http://hz.zhoulong.xyz/gtprbnkjax.html

[G06] 重写方法
来源：http://hz.birdmap.top/gtqxxhzlgs.html

Py:   def greet(self): return "admin"
来源：http://hz.gogol.net.cn/gtatsapyun.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zdqjudy.top/gtuahavpsx.html

JS:   greet() { return "admin"; }
来源：http://hz.iojbl.cn/gtblonqavq.html

TS:   greet(): string { return "admin"; }
来源：http://hz.tianlin.xyz/gtjewhyiph.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.bjfxy.top/gtmzcyofsn.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.yj202588.top/gtktnkdiaw.html

Ruby: def greet; "admin"; end
来源：http://hz.smart0.xyz/gtstphrepp.html

C#:   public override string Greet() => "admin";
来源：http://hz.xziqi.cn/gtgwnkoawi.html

[G07] 调用父类方法
来源：http://hz.jyoumei.cn/gtamqwxlno.html

Py:   super().greet()
来源：http://hz.andypj.xyz/gtwjehngsv.html

PHP:  parent::greet();
来源：http://hz.gotoacloud.top/gtjxjcoaac.html

JS:   super.greet();
来源：http://hz.sufxvd.cn/gtdqfxtfxh.html

TS:   super.greet();
来源：http://hz.cucudq.cn/gtrytlcvud.html

Java: super.greet();
来源：http://hz.pengpengdd.cyou/gtemkbpuaq.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.ywan-chungtsiang.top/gtjyarjkib.html

Ruby: super
来源：http://hz.c1oappe.top/gtvmrceoqr.html

C#:   base.Greet();
来源：http://hz.jiagoushi.top/gtyywtoinc.html

[G08] 静态方法与属性
来源：http://hz.chenzaomai.com/gttzashdfw.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.yj20258888.top/gthgqeygnu.html

PHP:  public static function f() {}
来源：http://hz.hnqzz.top/gtkkyvoatc.html

JS:   static f() {}
来源：http://hz.jinqigufen.top/gtbhkigxqn.html

TS:   static f(): void {}
来源：http://hz.sysykeji.top/gtndrgwtfa.html

Java: static void f() {}
来源：http://hz.cucudq.cn/gtuaqwakfz.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.shangyingyoupin.top/gtghcqwvxr.html

Ruby: def self.f; end
来源：http://hz.yj202588.top/gtrksbpmnp.html

C#:   public static void F() {}
来源：http://hz.dashuyun.cn/gtqqilffzu.html

[G09] 接口 / 抽象类
来源：http://hz.jinyuanbaomall.cn/gtcowwrloz.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.xinyue.icu/gtbpdylfyc.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.cdnleiting.top/gtwanqjhog.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.ydjk.org.cn/gtmqjkvitn.html

TS:   interface Shape { area(): number; }
来源：http://hz.ppjwa.cn/gtqorwggnd.html

Java: interface Shape { double area(); }
来源：http://hz.feifeiyinyue.top/gtpxqgpoki.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.yonumen.top/gtficddecg.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.ydzc1.top/gtcwwvmgtt.html

C#:   interface IShape { double Area(); }
来源：http://hz.zhixingplan.top/gtogdnoywq.html

[G10] 访问控制
来源：http://hz.zycfv.cn/gtitbhunwm.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.zhaomingkeji.xyz/gtellsnwyc.html

PHP:  public / protected / private
来源：http://hz.wangdashe.top/gtyiggqyhc.html

JS:   #private 字段；其余公开
来源：http://hz.wangshuangyany.cn/gtyeeyydgl.html

TS:   public / protected / private
来源：http://hz.hfpthk.cn/gtdzvqvukw.html

Java: public / protected / private / 默认包级
来源：http://hz.yanxiufei.cn/gtchdetpyx.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yj20258.top/gtcsbahjpx.html

Ruby: public / protected / private
来源：http://hz.shanyushiyangkeji.top/gtmlwmptci.html

C#:   public / protected / private / internal
来源：http://hz.havefunace.top/gtvzonybjw.html

[G11] getter / setter
来源：http://hz.ydjk.org.cn/gtrjobngmx.html

Py:   @property 与 @x.setter
来源：http://hz.hongshengwenyu.top/gtfhppvads.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhiwuduotai.top/gtprspxqhh.html

JS:   get name() { return this._name; }
来源：http://hz.aizwys.cn/gtrpiukqea.html

TS:   get name(): string { return this._name; }
来源：http://hz.gotoacloud.top/gttqgqmrrb.html

Java: public String getName() { return name; }
来源：http://hz.yongpay.top/gtxismnjng.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.gotoacloud.top/gtgzwbugop.html

Ruby: attr_accessor :name
来源：http://hz.zhixingplan.top/gtzqblspcr.html

C#:   public string Name { get; set; }
来源：http://hz.shanyushiyangkeji.top/gtxpxhiywz.html

[G12] 对象转字符串
来源：http://hz.xylfe.cn/gtclhezhkb.html

Py:   def __str__(self): return self.name
来源：http://hz.jqgfzy.top/gtefiicqdb.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.c1oappe.top/gtkzoglgjz.html

JS:   toString() { return this.name; }
来源：http://hz.cqqwz.cn/gtzoglltjr.html

TS:   toString(): string { return this.name; }
来源：http://hz.aizwys.cn/gtdivmwose.html

Java: @Override public String toString() { return name; }
来源：http://hz.yangfankeji.com/gtdmltwmwc.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.bjfxy.top/gtewoxvxhy.html

Ruby: def to_s; @name; end
来源：http://hz.daxiang520.top/gtzsagomkp.html

C#:   public override string ToString() => Name;
来源：http://hz.hnqzz.top/gtncdzeoln.html

[G13] 判断对象类型
来源：http://hz.guannengcc.top/gtuvqbisbs.html

Py:   isinstance(u, User)
来源：http://hz.birdmap.top/gtqruawdlp.html

PHP:  $u instanceof User
来源：http://hz.gotoacloud.top/gtpxvdgmns.html

JS:   u instanceof User
来源：http://hz.xuanzx.com/gtuiolbool.html

TS:   u instanceof User
来源：http://hz.aizwys.cn/gttemjepwb.html


<!-- 参考信息 -->