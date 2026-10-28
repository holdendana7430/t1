代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.redwolf501.top/gtmouhwugb.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.yj20258888.top/gtnqdfxddc.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.yj202588.top/gtbyqqynma.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.yangfankeji.com/gtqyqoruzn.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.yonumen.top/gtjztbijab.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jqgufenzy.top/gtfnruvloh.html

[E16] 数字千分位
来源：http://hz.andypj.xyz/gtnqakrnms.html

Py:   f"{1234567:,}"
来源：http://hz.dashuyun.cn/gteiypmltq.html

PHP:  number_format(1234567);
来源：http://hz.zhoulong.xyz/gtfrcomxrf.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.hammf.cn/gtkfjdkshd.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.birdmap.top/gtztcvstho.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.ydjk.org.cn/gtuhpsqbnu.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.xylfe.cn/gtuxzwkhmo.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.yvedp.cn/gtcwmtvxux.html

C#:   1234567.ToString("N0")
来源：http://hz.hfpthk.cn/gtkwaxqpui.html

[E17] 首字母大写
来源：http://hz.jqgufenzy.top/gtsxfydywi.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.pycfn.com/gtjvawlgjf.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.sysykeji.top/gtuhzhcgww.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jinqigfzy.top/gtxnaqxnwn.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ywan-chungtsiang.top/gtussnkwqq.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.ybcxt.top/gtidirchvk.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.kuanghao11.cn/gtvnmifczn.html

Ruby: s.capitalize
来源：http://hz.jlsjyb.cn/gtyskevwul.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.mhx1999.top/gtrdwnebfp.html

[E18] 模板占位符替换
来源：http://hz.wangshuangyany.cn/gtupptvaiz.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.guannengcc.top/gteblmqjlw.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.zhixingplan.top/gtaldtcdmn.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.jqgfzy.top/gtbqynrguf.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.yuxming.cn/gtmhemtleb.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.jqgfzy.top/gtqdrgtywp.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.ywan-chungtsiang.top/gtdvcdcjog.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.zhixingplan.top/gtvcoithje.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.0kj1m.cn/gtcyffrjlu.html

[E19] 多行文本按行拆分
来源：http://hz.guannengcc.top/gtivpgkown.html

Py:   s.splitlines()
来源：http://hz.tian-w.cn/gtwycygwpx.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.cqqwz.cn/gtttwyaeot.html

JS:   s.split(/\r?\n/)
来源：http://hz.ywan-chungtsiang.top/gtsepcqsbg.html

TS:   s.split(/\r?\n/)
来源：http://hz.birdmap.top/gtkeqbwivs.html

Java: s.lines().toList()
来源：http://hz.daxiang520.top/gtijubwvqq.html

Go:   strings.Split(s, "\n")
来源：http://hz.quarkkingdee.top/gticctwxjo.html

Ruby: s.lines
来源：http://hz.hongshengwenyu.top/gtnvncpbba.html

C#:   s.Split('\n')
来源：http://hz.xuanzx.com/gtysdvbdaj.html

[E20] 判断字符串是否为空
来源：http://hz.gaohongyu789.top/gtejkqqdok.html

Py:   if not s:
来源：http://hz.sweek.top/gtsyrmolvc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.yuxming.cn/gttpbycqsj.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.jianghu66.top/gtfqhbmahx.html

TS:   if (s === "") {}
来源：http://hz.zhengqikj.top/gtymjxvdnk.html

Java: if (s.isEmpty()) {}
来源：http://hz.gogol.net.cn/gtjsxyurgj.html

Go:   if s == "" {}
来源：http://hz.haohaochexian.top/gtrcdzbrbr.html

Ruby: if s.empty?
来源：http://hz.svipenyu.cn/gtqplcvzuw.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.gaohongyu789.top/gtfmntvhhd.html

[E21] 超长截断加省略号
来源：http://hz.smart0.xyz/gtajvhhexa.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.jiagoushi.top/gtscmqgosl.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.hnxiangtu.top/gtzdwarxrl.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.jlsjyb.cn/gtmlrnotwo.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yuxming.cn/gtvjdkxlbd.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.gzhubu.top/gtizmjckao.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.dashuyun.cn/gtugdvvpim.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.wangdashe.top/gttevwyrnz.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.zhiwuduotai.top/gtsaamihxz.html

[E22] 字节长度与字符长度
来源：http://hz.chenlongwang.top/gtbohskzzl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jinyuanbaomall.cn/gtbimichno.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yvedp.cn/gtbirrjeqc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ydzc1.top/gtgqkyxwfl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.gaohongyu789.top/gtutarjvkn.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yongpay.top/gthykndmju.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.shuidangran.top/gthmjqpswc.html

Ruby: s.bytesize;  s.length
来源：http://hz.guowangkeji.top/gtkzyjdjrg.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.chenlongwang.top/gtqjgayqlf.html

================================================================================
来源：http://hz.jinqigufen.top/gtdgoltiqr.html

F. 文件与目录
来源：http://hz.yuanzhike.top/gtbrzwtteg.html

================================================================================
来源：http://hz.wangdashe.top/gtgdlykzux.html

[F01] 读取整个文件
来源：http://hz.nanxinkj.top/gtnehxuakp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.zhiwuduotai.top/gtfccudxbo.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yj20258.top/gtvdxyjres.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.yanxiufei.cn/gtwrlwgfjg.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.316326.xyz/gtlyhmlevb.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.shuidangran.top/gtgywcqzyu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.daxiang520.top/gtogykwcjt.html

Ruby: File.read("a.txt")
来源：http://hz.yuxming.cn/gthtfboldh.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.vqdsnc.cn/gtujacpltx.html

[F02] 逐行读取文件
来源：http://hz.jlsjyb.cn/gtiqayabcd.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.shangyingyoupin.top/gtpvzbqhoq.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.andypj.xyz/gtvhiiiagr.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.dashuyun.cn/gtqlukvktn.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.vqdsnc.cn/gthskmjvaf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zhengqikj.top/gtbzqytikl.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.nanxinkj.top/gtyhqdrmki.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.feifeiyinyue.top/gtthmjvhdm.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.sweek.top/gtxawpmnms.html

[F03] 写入文件（覆盖）
来源：http://hz.ehwqpu.com/gthdwufrfd.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.316326.xyz/gtbwgjotoa.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.aibaodan.cn/gtbspiwitg.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.shanyushiyangtech.top/gtrlqykclr.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.xuanzx.com/gtpznndrtk.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.aizwys.cn/gtvlofjixx.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.hfpthk.cn/gtlimeqshn.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.andypj.xyz/gtzsngneat.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yuanzhike.top/gtessxzert.html

[F04] 追加写入文件
来源：http://hz.hammf.cn/gtynjcuejc.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yueranfly.top/gtizpquzez.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.feifeiyinyue.top/gtxkbsqvaq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.zhoulong.xyz/gtrjwoonvp.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.nanxuanxn.top/gtftirvoot.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.redwolf501.top/gtsnegmdme.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.zhiwuduotai.top/gtljydhwho.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.ivvv.top/gtjcxqnqra.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.xziqi.cn/gtyibcurud.html

[F05] 判断文件或目录是否存在
来源：http://hz.svipenyu.cn/gtobluggmj.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.shanyushiyangkeji.top/gtlwsfkcrz.html

PHP:  file_exists("a.txt");
来源：http://hz.gaohongyu789.top/gtcuuzaudr.html

JS:   fs.existsSync("a.txt")
来源：http://hz.ivvv.top/gtjtzidebn.html

TS:   fs.existsSync("a.txt")
来源：http://hz.hysaishi.cn/gtxwzwjtjh.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.hnqzz.top/gtsxfitotf.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.sxryk.cn/gtpycuhdgz.html

Ruby: File.exist?("a.txt")
来源：http://hz.jinyuanbaomall.cn/gtxcnbndfs.html

C#:   File.Exists("a.txt")
来源：http://hz.hnxiangtu.top/gtavbpqupa.html

[F06] 删除文件
来源：http://hz.gotoacloud.top/gtrqazxciu.html

Py:   os.remove("a.txt")
来源：http://hz.yonumen.top/gtvasmnsnt.html

PHP:  unlink("a.txt");
来源：http://hz.hammf.cn/gtvetaihgo.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.zhiwuduotai.top/gtoownryeq.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.tian-w.cn/gtlgxsucry.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.kuanghao11.cn/gtucemjngb.html

Go:   os.Remove("a.txt")
来源：http://hz.52xcode.cn/gtizsalflx.html

Ruby: File.delete("a.txt")
来源：http://hz.zhengqikj.top/gtsilgjaat.html

C#:   File.Delete("a.txt");
来源：http://hz.redwolf501.top/gtwifttqro.html

[F07] 创建目录（含多级）
来源：http://hz.9152youxi.cn/gtbozepoxq.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.yangfankeji.com/gtjjillfvk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.pycfn.com/gtloobbzpf.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhengqikj.top/gtlgaiyxeu.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.ivvv.top/gtgfaoqfsz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.tianlin.xyz/gtwutdyzcu.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.ydjk.org.cn/gtlamormjk.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.xylfe.cn/gtgptcvzij.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.9152youxi.cn/gtyowooqtt.html

[F08] 遍历目录
来源：http://hz.0kj1m.cn/gtopzgbtpz.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.yj202588.top/gtbfoauilz.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.nanxinkj.top/gtsfwxbwty.html

JS:   fs.readdirSync("dir")
来源：http://hz.shzxlz.cn/gtgfdpojxf.html

TS:   fs.readdirSync("dir")
来源：http://hz.xinyue.icu/gttyhdybuf.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.quarkkingdee.top/gtjjjybrpj.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.zhiwuduotai.top/gtgchsuqyp.html

Ruby: Dir.children("dir")
来源：http://hz.0kj1m.cn/gtlvqipxhc.html

C#:   Directory.GetFiles("dir")
来源：http://hz.chenjidiqi.icu/gtsmphkegl.html

[F09] 获取文件大小
来源：http://hz.yj202588.top/gtjvchoxiq.html

Py:   os.path.getsize("a.txt")
来源：http://hz.jiagoushi.top/gtbslskhvk.html

PHP:  filesize("a.txt");
来源：http://hz.daxiang520.top/gtdqnzyfjw.html

JS:   fs.statSync("a.txt").size
来源：http://hz.cashguo.top/gtabssbior.html

TS:   fs.statSync("a.txt").size
来源：http://hz.cqqwz.cn/gtabxoampj.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.nanxinkj.top/gtqspmpcrn.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.cashguo.top/gtfddmqhlm.html

Ruby: File.size("a.txt")
来源：http://hz.jinghuilouyu.cn/gtmqfjragh.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.ehwqpu.com/gtulwmsrjw.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.hfpthk.cn/gtzijgycpo.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.cashguo.top/gtrrkikljg.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.tian-w.cn/gtssyupqma.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.316326.xyz/gthgfsctbr.html

TS:   path.extname("a.txt")
来源：http://hz.zhongyouzk.top/gtxfbdkfta.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.hongshengwenyu.top/gtpfrqcofk.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.kuanghao11.cn/gtkpzwaffn.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.tanke756.top/gtuwuvfvja.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.redwolf501.top/gtbrvbnizn.html

[F11] 复制与移动文件
来源：http://hz.zhengqikj.top/gtcqwuyyne.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zdqjudy.top/gtwvgqmbgw.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.mhx1999.top/gtwwpctzvn.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jianghu66.top/gtrfqmwyrj.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinghuilouyu.cn/gtvgdsouxc.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.smart0.xyz/gtcntkwbrp.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.yangfankeji.com/gtpgdwxsjb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.ivvv.top/gtkkzbbuwy.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ppjwa.cn/gtsqgfshdt.html

[F12] CSV 读写
来源：http://hz.jyoumei.cn/gtwaxbhkqc.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.haohaochexian.top/gtymhkjiir.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.chenzaomai.com/gthpneztzx.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.ivvv.top/gtrrwackwu.html

TS:   // 同上
来源：http://hz.kuanghao11.cn/gtkniyotat.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.zhaomingkeji.xyz/gtfoexrxmv.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.bjfxy.top/gtvinvgtvp.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.yueranfly.top/gtydilsxnp.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.9152youxi.cn/gthjexpjny.html

================================================================================
来源：http://hz.9152youxi.cn/gtlrctcolv.html

G. 面向对象
来源：http://hz.yj20258.top/gtauwhtdmy.html

================================================================================
来源：http://hz.tian-w.cn/gtfrcjrtha.html

[G01] 定义类
来源：http://hz.chenjidiqi.icu/gtyrhsbwgi.html

Py:   class User: pass
来源：http://hz.cqqwz.cn/gtsoflktpd.html

PHP:  class User {}
来源：http://hz.dianchejie.cn/gtjwyloidc.html

JS:   class User {}
来源：http://hz.hnxiangtu.top/gtowbnmscd.html

TS:   class User { name: string = ""; }
来源：http://hz.tanke756.top/gtwvgfunlc.html

Java: class User {}
来源：http://hz.pycfn.com/gthitwgfnd.html

Go:   type User struct { Name string }
来源：http://hz.meibo888.top/gthbnnskki.html

Ruby: class User; end
来源：http://hz.yangfankeji.com/gtyudqzssv.html

C#:   class User {}
来源：http://hz.yuanzhike.top/gtuxwrehzw.html

[G02] 构造函数
来源：http://hz.jinghuilouyu.cn/gtuwfohibz.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.cucudq.cn/gtshsfgyjv.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.kuanghao11.cn/gtphjtfwve.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.yangfankeji.com/gtihxbhwsw.html

TS:   constructor(public name: string) {}
来源：http://hz.cucudq.cn/gtffygkuwq.html

Java: User(String name) { this.name = name; }
来源：http://hz.shanyushiyangtech.top/gtmenerrpk.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hammf.cn/gtsghczltj.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.jyoumei.cn/gtkubthyhg.html

C#:   public User(string name) { Name = name; }
来源：http://hz.pengpengdd.cyou/gtytrermdy.html

[G03] 实例属性
来源：http://hz.sxryk.cn/gtazhentws.html

Py:   self.name = "x"
来源：http://hz.andypj.xyz/gtyxincojs.html

PHP:  public string $name = "x";
来源：http://hz.yanxiufei.cn/gtgbswaxqe.html

JS:   this.name = "x";
来源：http://hz.hywenlv.cn/gtlpiafvyc.html

TS:   name: string = "x";
来源：http://hz.hnqzz.top/gtddaqnjdx.html

Java: private String name;
来源：http://hz.xylfe.cn/gtaqreuhul.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.wangdashe.top/gtzuofnmnv.html

Ruby: @name = "x"
来源：http://hz.gogol.net.cn/gtjoxuhmmn.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.smart0.xyz/gtengpmjcx.html

[G04] 定义方法
来源：http://hz.yvedp.cn/gthuhafeoz.html

Py:   def greet(self): return self.name
来源：http://hz.xingfuxueyuan.xyz/gturzdvaxy.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.zhoulong.xyz/gttclxxmfq.html

JS:   greet() { return this.name; }
来源：http://hz.gaohongyu789.top/gtwrbdmwvj.html

TS:   greet(): string { return this.name; }
来源：http://hz.zycfv.cn/gtxrqwstct.html

Java: String greet() { return name; }
来源：http://hz.hnqzz.top/gtakxinqmk.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.zycfv.cn/gtfbwhlahs.html

Ruby: def greet; @name; end
来源：http://hz.hysaishi.cn/gtbimkuyah.html

C#:   public string Greet() => Name;
来源：http://hz.wangshuangyany.cn/gtrfoytgln.html

[G05] 继承
来源：http://hz.jqgufenzy.top/gtzrpauojk.html

Py:   class Admin(User): pass
来源：http://hz.yangfankeji.com/gtlqtexqkq.html

PHP:  class Admin extends User {}
来源：http://hz.fzhhl.top/gtxwplnivq.html

JS:   class Admin extends User {}
来源：http://hz.chenlongwang.top/gtxnvdimyd.html

TS:   class Admin extends User {}
来源：http://hz.ydzc1.top/gtmmiliiig.html

Java: class Admin extends User {}
来源：http://hz.ehwqpu.com/gtrwzlpnip.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.andypj.xyz/gtmqlwnxen.html

Ruby: class Admin < User; end
来源：http://hz.yongpay.top/gtfypyirjh.html

C#:   class Admin : User {}
来源：http://hz.tian-w.cn/gtgpugwztz.html

[G06] 重写方法
来源：http://hz.yanxiufei.cn/gtqaiuzmqy.html

Py:   def greet(self): return "admin"
来源：http://hz.xingfuxueyuan.xyz/gtyfxonnbt.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.pycfn.com/gtyebjinif.html

JS:   greet() { return "admin"; }
来源：http://hz.haohaochexian.top/gtipxudgvd.html

TS:   greet(): string { return "admin"; }
来源：http://hz.9152youxi.cn/gtcqvpgwad.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.cqqwz.cn/gtcczkrvja.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.fzhhl.top/gtlridrzrn.html

Ruby: def greet; "admin"; end
来源：http://hz.ydzc1.top/gtvbzpydqy.html

C#:   public override string Greet() => "admin";
来源：http://hz.xuetiantiany.cn/gtfzvxsbxp.html

[G07] 调用父类方法
来源：http://hz.jianghu66.top/gtrwwffgwh.html

Py:   super().greet()
来源：http://hz.xinyue.icu/gtweorvhbt.html

PHP:  parent::greet();
来源：http://hz.jianghu66.top/gtffqheekc.html

JS:   super.greet();
来源：http://hz.jianghu66.top/gtpusrpuja.html

TS:   super.greet();
来源：http://hz.iojbl.cn/gteyqzxgtz.html

Java: super.greet();
来源：http://hz.hnxiangtu.top/gttntcburg.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.smart0.xyz/gtkpsvdpts.html

Ruby: super
来源：http://hz.ydjk.org.cn/gtlguyizzi.html

C#:   base.Greet();
来源：http://hz.sweek.top/gtiprcdten.html

[G08] 静态方法与属性
来源：http://hz.haohaochexian.top/gtfsgiecav.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.ppjwa.cn/gtiqsaqtfa.html

PHP:  public static function f() {}
来源：http://hz.chenlongwang.top/gtrgiwtjqv.html

JS:   static f() {}
来源：http://hz.vqdsnc.cn/gtaglfmcqf.html

TS:   static f(): void {}
来源：http://hz.dashuyun.cn/gtqaqqkgye.html

Java: static void f() {}
来源：http://hz.snrcjt.cn/gthkpvpxxg.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.52xcode.cn/gtcqgodpub.html

Ruby: def self.f; end
来源：http://hz.ywan-chungtsiang.top/gtjxmjfoka.html

C#:   public static void F() {}
来源：http://hz.yongpay.top/gtbmyeybum.html

[G09] 接口 / 抽象类
来源：http://hz.ywan-chungtsiang.top/gtfrsbmnus.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yonumen.top/gtduzimkuc.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.jianghu66.top/gtqgpniire.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zhaomingkeji.xyz/gtidyhpxmd.html

TS:   interface Shape { area(): number; }
来源：http://hz.snrcjt.cn/gtvxwsinuh.html

Java: interface Shape { double area(); }
来源：http://hz.xylfe.cn/gtdiibyxfz.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.aibaodan.cn/gtsfskbefb.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.vqdsnc.cn/gtzbilmbsb.html

C#:   interface IShape { double Area(); }
来源：http://hz.ybcxt.top/gtytkbnmps.html

[G10] 访问控制
来源：http://hz.ywan-chungtsiang.top/gthghznbnf.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.guannengcc.top/gtxkywibaf.html

PHP:  public / protected / private
来源：http://hz.zhongyouzk.top/gtbmeyyntp.html

JS:   #private 字段；其余公开
来源：http://hz.snrcjt.cn/gtmdnegzdm.html

TS:   public / protected / private
来源：http://hz.gotoacloud.top/gtavstzuqz.html

Java: public / protected / private / 默认包级
来源：http://hz.cdnleiting.top/gtrxnxyjkz.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.xingfuxueyuan.xyz/gteqxtdvef.html

Ruby: public / protected / private
来源：http://hz.daxiang520.top/gtyhlnitux.html

C#:   public / protected / private / internal
来源：http://hz.gotoacloud.top/gtciezmloy.html

[G11] getter / setter
来源：http://hz.jqgufenzy.top/gtbmmbgfgi.html

Py:   @property 与 @x.setter
来源：http://hz.zhixingplan.top/gtecblvmrw.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.jyoumei.cn/gtgtekfpng.html

JS:   get name() { return this._name; }
来源：http://hz.hnqzz.top/gtgwjuutfo.html

TS:   get name(): string { return this._name; }
来源：http://hz.52xcode.cn/gtzcyiyrzw.html

Java: public String getName() { return name; }
来源：http://hz.iojbl.cn/gtqggatrfy.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.chenlongwang.top/gtbgpwiczq.html

Ruby: attr_accessor :name
来源：http://hz.gzhubu.top/gtdvolcmpu.html

C#:   public string Name { get; set; }
来源：http://hz.wangdashe.top/gtdroyfwaw.html

[G12] 对象转字符串
来源：http://hz.chenlongwang.top/gtstwtnbnh.html

Py:   def __str__(self): return self.name
来源：http://hz.shangyingyoupin.top/gtkqwftzhi.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.havefunace.top/gtobzlfxzw.html

JS:   toString() { return this.name; }
来源：http://hz.quarkkingdee.top/gtpykqhxui.html

TS:   toString(): string { return this.name; }
来源：http://hz.xylfe.cn/gtaygypnjx.html

Java: @Override public String toString() { return name; }
来源：http://hz.zhixingplan.top/gtfwjxnekf.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.wangdashe.top/gtqpfuoeki.html

Ruby: def to_s; @name; end
来源：http://hz.guowangkeji.top/gturkgcbnz.html

C#:   public override string ToString() => Name;
来源：http://hz.jqgufenzy.top/gtiaejkjeu.html

[G13] 判断对象类型
来源：http://hz.zhixingplan.top/gtkhsotiff.html

Py:   isinstance(u, User)
来源：http://hz.c1oappe.top/gtctfipnqi.html

PHP:  $u instanceof User
来源：http://hz.chenlongwang.top/gtieipzebk.html

JS:   u instanceof User
来源：http://hz.chenzaomai.com/gtxcaixlyr.html

TS:   u instanceof User
来源：http://hz.jqgufenzy.top/gtewcgfvfq.html

Java: u instanceof User
来源：http://hz.tanke756.top/gttwdcbfhk.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.316326.xyz/gtsmyelqok.html

Ruby: u.is_a?(User)
来源：http://hz.zycfv.cn/gtkzuetmcn.html

C#:   u is User
来源：http://hz.haohaochexian.top/gtycgznuuj.html


<!-- 参考信息 -->