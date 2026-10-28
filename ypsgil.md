代发 wailian999

C#:   Uri.EscapeDataString(s);  Convert.ToBase64String(bytes)
来源：http://hz.hnxiangtu.top/gteuqruuzu.html

[E15] HTML 转义 / 反转义
来源：http://hz.jianghu66.top/gtcipxepef.html

Py:   html.escape(s);  html.unescape(s)
来源：http://hz.zhiwuduotai.top/gttvjixmpu.html

PHP:  htmlspecialchars($s, ENT_QUOTES, "UTF-8");  htmlspecialchars_decode($s);
来源：http://hz.ydzc1.top/gtaeghzqst.html

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.chenlongwang.top/gteroyutry.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.gogol.net.cn/gtjnxqykum.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.tianlin.xyz/gteszembdk.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.ehwqpu.com/gtxwovmalt.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.xylfe.cn/gtvbmftxat.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.hongshengwenyu.top/gtvjrtedrh.html

[E16] 数字千分位
来源：http://hz.jianghu66.top/gtopabjzmd.html

Py:   f"{1234567:,}"
来源：http://hz.zhaomingkeji.xyz/gtsktxapwi.html

PHP:  number_format(1234567);
来源：http://hz.yj20258888.top/gtmjsfsjgo.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.hfpthk.cn/gtxljcfybt.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.52xcode.cn/gtpwuxroab.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.yvedp.cn/gtfnnslbid.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.c1oappe.top/gtgoqspkog.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.nwbrower.top/gtyyupexjv.html

C#:   1234567.ToString("N0")
来源：http://hz.ydzc1.top/gtncsoupnc.html

[E17] 首字母大写
来源：http://hz.c1oappe.top/gtewersnhx.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.zhengqikj.top/gtfwgigzjk.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.cucudq.cn/gtoqkfsppl.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hywenlv.cn/gtvgufpugs.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.hysaishi.cn/gtpchbsdcn.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.gaohongyu789.top/gtonzqunak.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.tian-w.cn/gtqxwntwhm.html

Ruby: s.capitalize
来源：http://hz.jlsjyb.cn/gtlktjuobd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.jinyuanbaomall.cn/gtwxrhbyxc.html

[E18] 模板占位符替换
来源：http://hz.yuxming.cn/gtkekurpik.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.jyoumei.cn/gtbzwggcqk.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.wangdashe.top/gtudgpsguj.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.zhengqikj.top/gtzaionypm.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.0kj1m.cn/gtrnwvmcqk.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.aibaodan.cn/gtfkhbrczy.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.jinqigufen.top/gtyxshiaiv.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.yangfankeji.com/gtdccdlhqm.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yj20258888.top/gtfrnwucsi.html

[E19] 多行文本按行拆分
来源：http://hz.havefunace.top/gtnesljtpn.html

Py:   s.splitlines()
来源：http://hz.yuxming.cn/gtjcotaifj.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.pycfn.com/gtlbnnfmmh.html

JS:   s.split(/\r?\n/)
来源：http://hz.hfpthk.cn/gtumplnlfe.html

TS:   s.split(/\r?\n/)
来源：http://hz.havefunace.top/gtnpoywval.html

Java: s.lines().toList()
来源：http://hz.dashuyun.cn/gtvbmpvcxu.html

Go:   strings.Split(s, "\n")
来源：http://hz.cqqwz.cn/gtqagusjxn.html

Ruby: s.lines
来源：http://hz.hammf.cn/gtflhubkqq.html

C#:   s.Split('\n')
来源：http://hz.yvedp.cn/gtfyksckyl.html

[E20] 判断字符串是否为空
来源：http://hz.yongpay.top/gtlycqnvvq.html

Py:   if not s:
来源：http://hz.redwolf501.top/gtajvihxmq.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.sxryk.cn/gtaivvqyzk.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.ivvv.top/gtpkeifhdk.html

TS:   if (s === "") {}
来源：http://hz.redwolf501.top/gtllzrtmxq.html

Java: if (s.isEmpty()) {}
来源：http://hz.jinqigfzy.top/gtwzsmixek.html

Go:   if s == "" {}
来源：http://hz.sysykeji.top/gtithrnozi.html

Ruby: if s.empty?
来源：http://hz.aizwys.cn/gtfjyztjpr.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.cucudq.cn/gteefdcjri.html

[E21] 超长截断加省略号
来源：http://hz.shanyushiyangtech.top/gtrildltxz.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.jlsjyb.cn/gtgexenxam.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yangfankeji.com/gtvsbuhftb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hysaishi.cn/gttsggaxmp.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jinyuanbaomall.cn/gtztxfstio.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.ehwqpu.com/gtplxccpvv.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.andypj.xyz/gtqtgxmsuv.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.ydzc1.top/gtkcntcfjb.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.guannengcc.top/gtpzyvjfqo.html

[E22] 字节长度与字符长度
来源：http://hz.bjfxy.top/gtwlsncein.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.mhx1999.top/gtseajggdk.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.chenzaomai.com/gtqpcamhyr.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhiwuduotai.top/gtslaigumd.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jiagoushi.top/gtvikftbzn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ywan-chungtsiang.top/gtexpufqmt.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.shuidangran.top/gtegsejmnu.html

Ruby: s.bytesize;  s.length
来源：http://hz.guannengcc.top/gtcibgbsgk.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.guowangkeji.top/gtwbzfiuax.html

================================================================================
来源：http://hz.jqgufenzy.top/gtxlxapasp.html

F. 文件与目录
来源：http://hz.tanke756.top/gtkdmbdsrz.html

================================================================================
来源：http://hz.hnqzz.top/gtcgoewdjg.html

[F01] 读取整个文件
来源：http://hz.sweek.top/gtbsakwvhf.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.chenlongwang.top/gtvjtniecb.html

PHP:  file_get_contents("a.txt");
来源：http://hz.xinyue.icu/gtzcrxjota.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.xylfe.cn/gtpcbozhrr.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.9152youxi.cn/gtbqsdkuaw.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.wangdashe.top/gtbuuvpsag.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.cucudq.cn/gtmrcltxya.html

Ruby: File.read("a.txt")
来源：http://hz.zhongyouzk.top/gtuadnktoq.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.jqgfzy.top/gtqcngnqdj.html

[F02] 逐行读取文件
来源：http://hz.yj202588.top/gtzfdexkxc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.tanke756.top/gtvqklmjgt.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.316326.xyz/gtegcofxvx.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.jqgfzy.top/gtgghvoicu.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.xylfe.cn/gtlkkjaafa.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.havefunace.top/gtbdmebqvk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.yj20258.top/gtjeiznbgu.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.shanyushiyangtech.top/gtqnlhmizk.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.hysaishi.cn/gttnkdrwsu.html

[F03] 写入文件（覆盖）
来源：http://hz.cashguo.top/gtfdnzwtcd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.sxryk.cn/gtqzixxjhx.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.wangdashe.top/gtjcwbymca.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.aizwys.cn/gtvlqwvfvh.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zycfv.cn/gtgcdnulsc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.shuidangran.top/gteuoymywc.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.0kj1m.cn/gtaulhyumf.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.zycfv.cn/gtnasqshat.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.zhaomingkeji.xyz/gtucsoxofl.html

[F04] 追加写入文件
来源：http://hz.yueranfly.top/gtlzvsakes.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.redwolf501.top/gtmiqlbezw.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zhaomingkeji.xyz/gtmwshbuxg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.sufxvd.cn/gtwpljbbkc.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhijiandao.cn/gtophoeete.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.cqqwz.cn/gtyuoovzax.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.tanke756.top/gtmncuwcmt.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jinyuanbaomall.cn/gtgrhozvvw.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.jyoumei.cn/gtbrfipwxv.html

[F05] 判断文件或目录是否存在
来源：http://hz.ppjwa.cn/gtvlctxzsf.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yueranfly.top/gtqrsdcret.html

PHP:  file_exists("a.txt");
来源：http://hz.hammf.cn/gtnujocsjp.html

JS:   fs.existsSync("a.txt")
来源：http://hz.ywan-chungtsiang.top/gtaxdxjcoi.html

TS:   fs.existsSync("a.txt")
来源：http://hz.tian-w.cn/gttbwbjgxm.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.cdnleiting.top/gtoowyvmnf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.aizwys.cn/gtzcmjerev.html

Ruby: File.exist?("a.txt")
来源：http://hz.yueranfly.top/gtnvmwjflr.html

C#:   File.Exists("a.txt")
来源：http://hz.andypj.xyz/gtbpgevrba.html

[F06] 删除文件
来源：http://hz.gzhubu.top/gtenvulcmr.html

Py:   os.remove("a.txt")
来源：http://hz.zhongyouzk.top/gtaztiodxm.html

PHP:  unlink("a.txt");
来源：http://hz.quarkkingdee.top/gtloxyxnis.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.jqgufenzy.top/gtflpxhrcn.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.chenjidiqi.icu/gtimkuvzke.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.sweek.top/gtpoefckii.html

Go:   os.Remove("a.txt")
来源：http://hz.316326.xyz/gtkbyqbrdw.html

Ruby: File.delete("a.txt")
来源：http://hz.haohaochexian.top/gtgwvtczzv.html

C#:   File.Delete("a.txt");
来源：http://hz.iojbl.cn/gtxfjorunu.html

[F07] 创建目录（含多级）
来源：http://hz.havefunace.top/gtdqgvmcix.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.hywenlv.cn/gtslcqnvjl.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.shangyingyoupin.top/gtbnpucdem.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.hongshengwenyu.top/gtdbltwnnu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ydjk.org.cn/gtludmvhyp.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.nwbrower.top/gtsjajydlg.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.hnqzz.top/gttehvoiao.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.zdqjudy.top/gtquzqcycj.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.pycfn.com/gtnuppedoz.html

[F08] 遍历目录
来源：http://hz.xuetiantiany.cn/gtiftomiwh.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.hnxiangtu.top/gtkotdcdcc.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.xingfuxueyuan.xyz/gtgbupjqgo.html

JS:   fs.readdirSync("dir")
来源：http://hz.ybcxt.top/gtmzudgvey.html

TS:   fs.readdirSync("dir")
来源：http://hz.jinqigufen.top/gtwqamuovs.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zhijiandao.cn/gtdmkiypcp.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.sweek.top/gthhjtmihx.html

Ruby: Dir.children("dir")
来源：http://hz.nwbrower.top/gtwcluvbae.html

C#:   Directory.GetFiles("dir")
来源：http://hz.hfpthk.cn/gtbdednidl.html

[F09] 获取文件大小
来源：http://hz.xingfuxueyuan.xyz/gtouknkeis.html

Py:   os.path.getsize("a.txt")
来源：http://hz.yuanzhike.top/gtwsukhzlz.html

PHP:  filesize("a.txt");
来源：http://hz.gogol.net.cn/gtppyxkzth.html

JS:   fs.statSync("a.txt").size
来源：http://hz.hongshengwenyu.top/gtpaftvtaa.html

TS:   fs.statSync("a.txt").size
来源：http://hz.snrcjt.cn/gtrurovuok.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.tianlin.xyz/gtpikmjntw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.gogol.net.cn/gtxsjpenze.html

Ruby: File.size("a.txt")
来源：http://hz.aizwys.cn/gtkluqalzt.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.jinyuanbaomall.cn/gtspqooyif.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.gzhubu.top/gtcxdlxcnr.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.fzhhl.top/gtefvaofpo.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.zhongyouzk.top/gtvbpabkem.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.ehwqpu.com/gtpbscsiun.html

TS:   path.extname("a.txt")
来源：http://hz.redwolf501.top/gteftjaito.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.dianchejie.cn/gtqdjiuwzg.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.sxryk.cn/gthwgpsmwd.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.yongpay.top/gtegdohkge.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.jqgfzy.top/gtxhxbhxlp.html

[F11] 复制与移动文件
来源：http://hz.snrcjt.cn/gtukzbcoio.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.nanxuanxn.top/gttckhcbcv.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.jqgfzy.top/gtohgaodva.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jlsjyb.cn/gtrdmweftk.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhongyouzk.top/gtrqqjyxlx.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zycfv.cn/gtvsxzmfhy.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yj20258888.top/gtcxartdev.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.cdnleiting.top/gtmxlbecor.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.daria6918.cn/gtitjyssze.html

[F12] CSV 读写
来源：http://hz.fengsongda.top/gthlgijsqz.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.hongshengwenyu.top/gtiyrskimx.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.vqdsnc.cn/gtehxsqsdx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.yanxiufei.cn/gtowamxlxq.html

TS:   // 同上
来源：http://hz.tian-w.cn/gtrcmehvlt.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.chenzaomai.com/gtfcjgfnne.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.0kj1m.cn/gtflljxezi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.ppjwa.cn/gtjkylpmpo.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.sufxvd.cn/gtiithjonh.html

================================================================================
来源：http://hz.yj20258888.top/gtbolrexbn.html

G. 面向对象
来源：http://hz.sweek.top/gtrxnydsas.html

================================================================================
来源：http://hz.andypj.xyz/gtevqljeac.html

[G01] 定义类
来源：http://hz.vqdsnc.cn/gtzenjdpzx.html

Py:   class User: pass
来源：http://hz.xuanzx.com/gthofmcfsa.html

PHP:  class User {}
来源：http://hz.dashuyun.cn/gtrygblejz.html

JS:   class User {}
来源：http://hz.zhoulong.xyz/gtxvoxjojw.html

TS:   class User { name: string = ""; }
来源：http://hz.svipenyu.cn/gtulcswxet.html

Java: class User {}
来源：http://hz.shzxlz.cn/gttoecmvxq.html

Go:   type User struct { Name string }
来源：http://hz.jinqigufen.top/gtkohdapnw.html

Ruby: class User; end
来源：http://hz.jlsjyb.cn/gtrgikrtav.html

C#:   class User {}
来源：http://hz.ivvv.top/gtpdjzubxc.html

[G02] 构造函数
来源：http://hz.bjfxy.top/gtswouaell.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.cqqwz.cn/gtnwpvygik.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.svipenyu.cn/gtyejlvnoq.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.cucudq.cn/gtjmexrnow.html

TS:   constructor(public name: string) {}
来源：http://hz.nanxuanxn.top/gtkftpnvro.html

Java: User(String name) { this.name = name; }
来源：http://hz.dianchejie.cn/gtzizicule.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.pycfn.com/gtqlwtjsbw.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.gogol.net.cn/gtjsgnjwzb.html

C#:   public User(string name) { Name = name; }
来源：http://hz.0kj1m.cn/gtxqjezyus.html

[G03] 实例属性
来源：http://hz.dianchejie.cn/gtrwroyiow.html

Py:   self.name = "x"
来源：http://hz.fzhhl.top/gtkevayuuj.html

PHP:  public string $name = "x";
来源：http://hz.vqdsnc.cn/gtqxkkdrop.html

JS:   this.name = "x";
来源：http://hz.ppjwa.cn/gtwzqrapsp.html

TS:   name: string = "x";
来源：http://hz.aizwys.cn/gtwgevvoqv.html

Java: private String name;
来源：http://hz.jlsjyb.cn/gtqrpicley.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.zhijiandao.cn/gtmejaifve.html

Ruby: @name = "x"
来源：http://hz.ydzc1.top/gtpwuodjcn.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.chenlongwang.top/gtudpxxaul.html

[G04] 定义方法
来源：http://hz.quarkkingdee.top/gtmbqxfmpw.html

Py:   def greet(self): return self.name
来源：http://hz.xingfuxueyuan.xyz/gtnjtwcjct.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.cheryme.top/gtjavlmmsb.html

JS:   greet() { return this.name; }
来源：http://hz.yj20258888.top/gtfxxbtnjc.html

TS:   greet(): string { return this.name; }
来源：http://hz.cucudq.cn/gtnbjaiowp.html

Java: String greet() { return name; }
来源：http://hz.aizwys.cn/gtzefdwsyv.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.jqgufenzy.top/gtvkxhopbi.html

Ruby: def greet; @name; end
来源：http://hz.gogol.net.cn/gttllehtgr.html

C#:   public string Greet() => Name;
来源：http://hz.smart0.xyz/gtkzkjwhwi.html

[G05] 继承
来源：http://hz.nwbrower.top/gtitubfank.html

Py:   class Admin(User): pass
来源：http://hz.gzhubu.top/gtzpycfdlp.html

PHP:  class Admin extends User {}
来源：http://hz.yuanzhike.top/gtwgeojvyq.html

JS:   class Admin extends User {}
来源：http://hz.wangdashe.top/gtkpsfywuh.html

TS:   class Admin extends User {}
来源：http://hz.jinyuanbaomall.cn/gtxvtnisfc.html

Java: class Admin extends User {}
来源：http://hz.meibo888.top/gtuexgsypw.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.yangfankeji.com/gtwmetkelx.html

Ruby: class Admin < User; end
来源：http://hz.ydjk.org.cn/gtrrzaneyq.html

C#:   class Admin : User {}
来源：http://hz.yanxiufei.cn/gtrbvvcdir.html

[G06] 重写方法
来源：http://hz.gotoacloud.top/gtmmrqpcxq.html

Py:   def greet(self): return "admin"
来源：http://hz.sweek.top/gtymfqvajh.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.zhiwuduotai.top/gtyvjtfhhp.html

JS:   greet() { return "admin"; }
来源：http://hz.gzhubu.top/gtnxyjpkyl.html

TS:   greet(): string { return "admin"; }
来源：http://hz.sxryk.cn/gtptlzvmrk.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.fengsongda.top/gtimcfufiq.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.hongshengwenyu.top/gtitdwvsja.html

Ruby: def greet; "admin"; end
来源：http://hz.gzhubu.top/gtxuguvkbu.html

C#:   public override string Greet() => "admin";
来源：http://hz.aizwys.cn/gtznmdewtu.html

[G07] 调用父类方法
来源：http://hz.hysaishi.cn/gtmcypabaj.html

Py:   super().greet()
来源：http://hz.xinyue.icu/gtuasxrygp.html

PHP:  parent::greet();
来源：http://hz.xuanzx.com/gtizudsfmm.html

JS:   super.greet();
来源：http://hz.ydjk.org.cn/gtwnbbuezh.html

TS:   super.greet();
来源：http://hz.pengpengdd.cyou/gtahsperua.html

Java: super.greet();
来源：http://hz.yj20258888.top/gtewzwxggx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zhongyouzk.top/gteaknmkfo.html

Ruby: super
来源：http://hz.yj20258888.top/gtkgquxapb.html

C#:   base.Greet();
来源：http://hz.xziqi.cn/gtjijudnmu.html

[G08] 静态方法与属性
来源：http://hz.hywenlv.cn/gtghsyvkwx.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.ehwqpu.com/gtkffqohhd.html

PHP:  public static function f() {}
来源：http://hz.cheryme.top/gtlojjmywq.html

JS:   static f() {}
来源：http://hz.pengpengdd.cyou/gtppennhqy.html

TS:   static f(): void {}
来源：http://hz.sysykeji.top/gtxwaphiti.html

Java: static void f() {}
来源：http://hz.meibo888.top/gtkwgixeer.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.zhiwuduotai.top/gtqptktfxl.html

Ruby: def self.f; end
来源：http://hz.jyoumei.cn/gtrdkffjmt.html

C#:   public static void F() {}
来源：http://hz.yuanzhike.top/gtnzxzwhhg.html

[G09] 接口 / 抽象类
来源：http://hz.jinghuilouyu.cn/gtonwibpji.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.gotoacloud.top/gtfonwvfvh.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.gotoacloud.top/gtsvfiuewk.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.feifeiyinyue.top/gtotimevmk.html

TS:   interface Shape { area(): number; }
来源：http://hz.hfpthk.cn/gtflhytysv.html

Java: interface Shape { double area(); }
来源：http://hz.zhaomingkeji.xyz/gtdoyohoio.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.sxryk.cn/gtpnewpmyu.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.fengsongda.top/gtuiamwhkq.html

C#:   interface IShape { double Area(); }
来源：http://hz.aibaodan.cn/gtnpgsnpnv.html

[G10] 访问控制
来源：http://hz.yangfankeji.com/gtxyiymczz.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.gaohongyu789.top/gtnabqutkj.html

PHP:  public / protected / private
来源：http://hz.cashguo.top/gtxcxtebzr.html

JS:   #private 字段；其余公开
来源：http://hz.snrcjt.cn/gtbnpooaxe.html

TS:   public / protected / private
来源：http://hz.ybcxt.top/gtuajvaput.html

Java: public / protected / private / 默认包级
来源：http://hz.cqqwz.cn/gtjvalnbrw.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.yanxiufei.cn/gtfoibnqef.html

Ruby: public / protected / private
来源：http://hz.hnxiangtu.top/gtdwqswgrf.html

C#:   public / protected / private / internal
来源：http://hz.ydjk.org.cn/gtyocunleg.html

[G11] getter / setter
来源：http://hz.dianchejie.cn/gtcywrkpmp.html

Py:   @property 与 @x.setter
来源：http://hz.nanxuanxn.top/gtfbkrvgez.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jiagoushi.top/gtjxpcuhyq.html

JS:   get name() { return this._name; }
来源：http://hz.gzhubu.top/gtyjlofpkq.html

TS:   get name(): string { return this._name; }
来源：http://hz.zhaomingkeji.xyz/gtpuxoitqg.html

Java: public String getName() { return name; }
来源：http://hz.wangdashe.top/gtvkipiini.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.feifeiyinyue.top/gtggancpry.html

Ruby: attr_accessor :name
来源：http://hz.hysaishi.cn/gtsrnknkiu.html

C#:   public string Name { get; set; }
来源：http://hz.gogol.net.cn/gtgechpklb.html

[G12] 对象转字符串
来源：http://hz.zhaomingkeji.xyz/gtmtmuekir.html

Py:   def __str__(self): return self.name
来源：http://hz.yanxiufei.cn/gtztqgdtwm.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.shanyushiyangtech.top/gtdkggsxyd.html

JS:   toString() { return this.name; }
来源：http://hz.zhixingplan.top/gthwkhjqvp.html

TS:   toString(): string { return this.name; }
来源：http://hz.bjfxy.top/gttxztmnzh.html

Java: @Override public String toString() { return name; }
来源：http://hz.gaohongyu789.top/gtjfxaylxk.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.xziqi.cn/gttkecqjsv.html

Ruby: def to_s; @name; end
来源：http://hz.xylfe.cn/gtqdtnvfeu.html

C#:   public override string ToString() => Name;
来源：http://hz.zhongyouzk.top/gtkzicywyx.html

[G13] 判断对象类型
来源：http://hz.smart0.xyz/gtzukxdgea.html

Py:   isinstance(u, User)
来源：http://hz.xuanzx.com/gtxyayvsyo.html

PHP:  $u instanceof User
来源：http://hz.vqdsnc.cn/gtbohtdubq.html

JS:   u instanceof User
来源：http://hz.zhiwuduotai.top/gtfyluwkwb.html

TS:   u instanceof User
来源：http://hz.yj20258.top/gthaltyivn.html


<!-- 参考信息 -->