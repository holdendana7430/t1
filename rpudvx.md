代发 wailian999

JS:   // 文本节点自动转义；拼接 HTML 时用 DOMPurify.sanitize(s)
来源：http://hz.smart0.xyz/gtwjyixuhc.html

TS:   // 同上，务必做 XSS 过滤
来源：http://hz.ivvv.top/gtgprxqitw.html

Java: HtmlUtils.htmlEscape(s)   // Spring；通用可用 Apache Commons Text
来源：http://hz.9152youxi.cn/gtibzzetee.html

Go:   html.EscapeString(s);  html.UnescapeString(s)
来源：http://hz.chenzaomai.com/gtzicksxup.html

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.gzhubu.top/gtuzmwpdjc.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.jinqigufen.top/gtqmmfzkti.html

[E16] 数字千分位
来源：http://hz.fzhhl.top/gtuanonssa.html

Py:   f"{1234567:,}"
来源：http://hz.zhiwuduotai.top/gtdkthtpuh.html

PHP:  number_format(1234567);
来源：http://hz.guannengcc.top/gtfsqipuxk.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.nwbrower.top/gtrodqfqme.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.tian-w.cn/gtiuyechah.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.sweek.top/gtyjwmqqau.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.0kj1m.cn/gtfknepypg.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.xylfe.cn/gtmfeeasbm.html

C#:   1234567.ToString("N0")
来源：http://hz.meibo888.top/gtdjzzlijc.html

[E17] 首字母大写
来源：http://hz.snrcjt.cn/gtzhgeotcj.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.52xcode.cn/gtvrcmofqg.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.yueranfly.top/gtlfwkvdmz.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.jinghuilouyu.cn/gtkbrwdqtm.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.cashguo.top/gtjrpmqvfx.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.xuetiantiany.cn/gtbkgynqxb.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.nanxuanxn.top/gtqzuohrfl.html

Ruby: s.capitalize
来源：http://hz.gogol.net.cn/gttqgzxady.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.9152youxi.cn/gtsyzurzkd.html

[E18] 模板占位符替换
来源：http://hz.nwbrower.top/gtzecxujmj.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.haohaochexian.top/gtcngkyoqb.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.kuanghao11.cn/gtdrnrjwad.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.kuanghao11.cn/gtvflmfciw.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.feifeiyinyue.top/gtrrhvhfhs.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.daria6918.cn/gtejvgzgqc.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yuxming.cn/gtojaxcljc.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.jiagoushi.top/gtfmtkjyff.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.zycfv.cn/gtjsjcpxyn.html

[E19] 多行文本按行拆分
来源：http://hz.zhijiandao.cn/gtpqzqdooi.html

Py:   s.splitlines()
来源：http://hz.fzhhl.top/gtqgvddbil.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.snrcjt.cn/gtrbuurjgh.html

JS:   s.split(/\r?\n/)
来源：http://hz.jqgufenzy.top/gtiduywreb.html

TS:   s.split(/\r?\n/)
来源：http://hz.snrcjt.cn/gtosaikzhu.html

Java: s.lines().toList()
来源：http://hz.sweek.top/gtiqpcojjf.html

Go:   strings.Split(s, "\n")
来源：http://hz.shanyushiyangtech.top/gtosjnukwa.html

Ruby: s.lines
来源：http://hz.sysykeji.top/gtqtnlkdpx.html

C#:   s.Split('\n')
来源：http://hz.zycfv.cn/gtfpxbzctv.html

[E20] 判断字符串是否为空
来源：http://hz.xziqi.cn/gtisjzctas.html

Py:   if not s:
来源：http://hz.sweek.top/gtevxtebwf.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.gogol.net.cn/gtwgrenkxx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.fengsongda.top/gttwgakqrh.html

TS:   if (s === "") {}
来源：http://hz.quarkkingdee.top/gtloakuxhl.html

Java: if (s.isEmpty()) {}
来源：http://hz.zhengqikj.top/gtbwghwudq.html

Go:   if s == "" {}
来源：http://hz.jyoumei.cn/gtnfalxvvg.html

Ruby: if s.empty?
来源：http://hz.zhixingplan.top/gtqwskjpmu.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.zhiwuduotai.top/gtrwbksyov.html

[E21] 超长截断加省略号
来源：http://hz.vqdsnc.cn/gtfzwsnnuy.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.sufxvd.cn/gtqbqsisjc.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.yj20258.top/gteuibubqb.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hnqzz.top/gtfcnebjej.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.hfpthk.cn/gtporbbikj.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.yangfankeji.com/gtchzffufo.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.c1oappe.top/gtgtxyptlf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.cheryme.top/gtigmsbnpi.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.hfpthk.cn/gtmmtsdlgl.html

[E22] 字节长度与字符长度
来源：http://hz.gogol.net.cn/gtureaysqt.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.c1oappe.top/gtlhsscyof.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.yuxming.cn/gtlycotgrz.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.zhoulong.xyz/gtxuqxmthz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.ydjk.org.cn/gtglumrdfz.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.gaohongyu789.top/gthowolzqj.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.pycfn.com/gtpdqvbffn.html

Ruby: s.bytesize;  s.length
来源：http://hz.cashguo.top/gtdomwgtln.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.fzhhl.top/gtmvsxpqpa.html

================================================================================
来源：http://hz.ehwqpu.com/gtrptjplfu.html

F. 文件与目录
来源：http://hz.gzhubu.top/gttadbwgzb.html

================================================================================
来源：http://hz.tianlin.xyz/gtxmuceozo.html

[F01] 读取整个文件
来源：http://hz.hongshengwenyu.top/gtqwhowxzm.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.aibaodan.cn/gtuoqudjbw.html

PHP:  file_get_contents("a.txt");
来源：http://hz.guowangkeji.top/gtcjzwpfjs.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.hammf.cn/gtgfpceryn.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.gzhubu.top/gtmieqxuwo.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jiagoushi.top/gtbmvtrjmx.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.ehwqpu.com/gtrwlwowsu.html

Ruby: File.read("a.txt")
来源：http://hz.dashuyun.cn/gtcrsfwxne.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zhijiandao.cn/gtfeysbkgo.html

[F02] 逐行读取文件
来源：http://hz.zhijiandao.cn/gtlwdodcav.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.sufxvd.cn/gtapbryhxz.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.hammf.cn/gtxplfumtp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.9152youxi.cn/gtgcedmujd.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.gzhubu.top/gtpihijuzx.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.jqgfzy.top/gtyzurngci.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.xylfe.cn/gtdrhrfmqs.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.yonumen.top/gtjhckqsti.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.chenjidiqi.icu/gtjygfzjpe.html

[F03] 写入文件（覆盖）
来源：http://hz.yj202588.top/gtohvsivfc.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.jyoumei.cn/gtsxdgyzrr.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.ivvv.top/gtihmpnbil.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.guannengcc.top/gtmymeacgv.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.cheryme.top/gtueyvdzlc.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.ppjwa.cn/gtoplamith.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.xylfe.cn/gtgbvtvqpk.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.ybcxt.top/gtpkltpzub.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.52xcode.cn/gtzicedxle.html

[F04] 追加写入文件
来源：http://hz.tian-w.cn/gtthpdxleh.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yuanzhike.top/gtzhmbjedj.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.yongpay.top/gtdqrhdunn.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.sxryk.cn/gtkngcsmkb.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cheryme.top/gtrseovvns.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.zhaomingkeji.xyz/gtowhcrego.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.jianghu66.top/gtnudfrwxc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.yangfankeji.com/gtkbendxjf.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.kuanghao11.cn/gtamnuawka.html

[F05] 判断文件或目录是否存在
来源：http://hz.cdnleiting.top/gthjlrqwbt.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.zycfv.cn/gtsnuyvrwp.html

PHP:  file_exists("a.txt");
来源：http://hz.pycfn.com/gtabsufhur.html

JS:   fs.existsSync("a.txt")
来源：http://hz.fzhhl.top/gtpfyksuoh.html

TS:   fs.existsSync("a.txt")
来源：http://hz.cdnleiting.top/gttkdygzwn.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.xylfe.cn/gttprnbubp.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.wangshuangyany.cn/gtjjdmhchi.html

Ruby: File.exist?("a.txt")
来源：http://hz.feifeiyinyue.top/gtnjjiahad.html

C#:   File.Exists("a.txt")
来源：http://hz.quarkkingdee.top/gtaaolgooa.html

[F06] 删除文件
来源：http://hz.jinqigufen.top/gtbsxlgdgo.html

Py:   os.remove("a.txt")
来源：http://hz.shanyushiyangkeji.top/gtllhleciu.html

PHP:  unlink("a.txt");
来源：http://hz.hnqzz.top/gtpjewknki.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.cdnleiting.top/gtacoumbws.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.gaohongyu789.top/gttxisxgdu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.yangfankeji.com/gtqcagxvbm.html

Go:   os.Remove("a.txt")
来源：http://hz.nwbrower.top/gtgjbkbkrw.html

Ruby: File.delete("a.txt")
来源：http://hz.yj20258.top/gtvbhctosl.html

C#:   File.Delete("a.txt");
来源：http://hz.yanxiufei.cn/gtbzhpuwgm.html

[F07] 创建目录（含多级）
来源：http://hz.haohaochexian.top/gtooshzhlf.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.zhongyouzk.top/gtrkelowcp.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.yonumen.top/gtepqyhwbe.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yongpay.top/gtrivupsnx.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.jinqigfzy.top/gtukqrgshr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.zycfv.cn/gtibjsxsrl.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.andypj.xyz/gtqwrbvgbe.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.nwbrower.top/gtalhfoace.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.hammf.cn/gtdtxzwrqb.html

[F08] 遍历目录
来源：http://hz.zhongyouzk.top/gttqgnmcrf.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.cashguo.top/gtstuxafrk.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.tian-w.cn/gtfbwwihjh.html

JS:   fs.readdirSync("dir")
来源：http://hz.nanxinkj.top/gtmwnzbtwd.html

TS:   fs.readdirSync("dir")
来源：http://hz.meibo888.top/gtjdvfezbs.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.cashguo.top/gtbjvewlmv.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.yangfankeji.com/gtrwvukwpr.html

Ruby: Dir.children("dir")
来源：http://hz.yj202588.top/gtwnnecvvx.html

C#:   Directory.GetFiles("dir")
来源：http://hz.sufxvd.cn/gtmytfhtzf.html

[F09] 获取文件大小
来源：http://hz.jlsjyb.cn/gtllrvkcvt.html

Py:   os.path.getsize("a.txt")
来源：http://hz.hysaishi.cn/gtvwiadqbl.html

PHP:  filesize("a.txt");
来源：http://hz.cashguo.top/gtanvsxjgo.html

JS:   fs.statSync("a.txt").size
来源：http://hz.chenzaomai.com/gteglinugy.html

TS:   fs.statSync("a.txt").size
来源：http://hz.dashuyun.cn/gtegmmyqjq.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.guowangkeji.top/gtcnrjdoyf.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.shanyushiyangtech.top/gtbdnydane.html

Ruby: File.size("a.txt")
来源：http://hz.sysykeji.top/gtbowukkbt.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.nanxinkj.top/gtcloaknyw.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.xuanzx.com/gttehgqmjc.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.xingfuxueyuan.xyz/gtrbastojp.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.nanxuanxn.top/gtilclssya.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.tianlin.xyz/gtgbhtwbhd.html

TS:   path.extname("a.txt")
来源：http://hz.zhoulong.xyz/gtpsaohtuw.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.shanyushiyangtech.top/gtewxuwrco.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.bjfxy.top/gtpqndrlmt.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.tian-w.cn/gtqgxbeypv.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.hysaishi.cn/gtcgixxbzy.html

[F11] 复制与移动文件
来源：http://hz.daxiang520.top/gtpedwsxiy.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.birdmap.top/gtacuaxuey.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.haohaochexian.top/gtqcxxsqfw.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jyoumei.cn/gtqxhnkmke.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.birdmap.top/gtpikivwvr.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zdqjudy.top/gtrtjaamhr.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.guannengcc.top/gtlbdftjck.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.pengpengdd.cyou/gtmdplkyav.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.hnqzz.top/gtefjougof.html

[F12] CSV 读写
来源：http://hz.ydzc1.top/gtneodllvs.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.hnxiangtu.top/gtxlbsybpy.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.quarkkingdee.top/gtqkcuputl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.cdnleiting.top/gtqshkscph.html

TS:   // 同上
来源：http://hz.hnqzz.top/gtnmlandtq.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.guannengcc.top/gteorilhdb.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.hnxiangtu.top/gtzlyokubh.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.dianchejie.cn/gthvhxofvw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.jqgufenzy.top/gtobnfioje.html

================================================================================
来源：http://hz.hywenlv.cn/gtxahzsrtm.html

G. 面向对象
来源：http://hz.shangyingyoupin.top/gtrmqctxde.html

================================================================================
来源：http://hz.aibaodan.cn/gtjnzhjkrn.html

[G01] 定义类
来源：http://hz.jqgufenzy.top/gtatwgvfgb.html

Py:   class User: pass
来源：http://hz.yanxiufei.cn/gtjgiqndld.html

PHP:  class User {}
来源：http://hz.yangfankeji.com/gtwiqevvaz.html

JS:   class User {}
来源：http://hz.nanxinkj.top/gtvsdqhxea.html

TS:   class User { name: string = ""; }
来源：http://hz.ppjwa.cn/gturmqvvoc.html

Java: class User {}
来源：http://hz.hnxiangtu.top/gtqhkovzrh.html

Go:   type User struct { Name string }
来源：http://hz.tanke756.top/gtrewnfuto.html

Ruby: class User; end
来源：http://hz.hongshengwenyu.top/gtwhvibbuk.html

C#:   class User {}
来源：http://hz.havefunace.top/gtxonyaxtj.html

[G02] 构造函数
来源：http://hz.zhongyouzk.top/gtpzqxpzwu.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.gogol.net.cn/gtqevagbzu.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zhengqikj.top/gtxnnwrxdd.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.ywan-chungtsiang.top/gtmagafiwi.html

TS:   constructor(public name: string) {}
来源：http://hz.cheryme.top/gtbhugchix.html

Java: User(String name) { this.name = name; }
来源：http://hz.ydjk.org.cn/gtgyqexysy.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.kuanghao11.cn/gtubxjnqla.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.xuanzx.com/gtjlumjywx.html

C#:   public User(string name) { Name = name; }
来源：http://hz.c1oappe.top/gtilpzvova.html

[G03] 实例属性
来源：http://hz.hywenlv.cn/gtrynozmtm.html

Py:   self.name = "x"
来源：http://hz.nwbrower.top/gtthmreihk.html

PHP:  public string $name = "x";
来源：http://hz.jqgufenzy.top/gthqimodyn.html

JS:   this.name = "x";
来源：http://hz.shuidangran.top/gtkseosftq.html

TS:   name: string = "x";
来源：http://hz.shzxlz.cn/gtknkemdwl.html

Java: private String name;
来源：http://hz.pengpengdd.cyou/gtrqjzirzf.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.ppjwa.cn/gtsjwerhit.html

Ruby: @name = "x"
来源：http://hz.yangfankeji.com/gtddfumcsj.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.jiagoushi.top/gttiqokexs.html

[G04] 定义方法
来源：http://hz.jqgufenzy.top/gtzfcrknzh.html

Py:   def greet(self): return self.name
来源：http://hz.gogol.net.cn/gttwhdpinm.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.sufxvd.cn/gtfshkfdng.html

JS:   greet() { return this.name; }
来源：http://hz.dashuyun.cn/gtzakcqepu.html

TS:   greet(): string { return this.name; }
来源：http://hz.haohaochexian.top/gtyhmnmoks.html

Java: String greet() { return name; }
来源：http://hz.fengsongda.top/gtcsbpvgym.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.9152youxi.cn/gtmhzbaffc.html

Ruby: def greet; @name; end
来源：http://hz.zdqjudy.top/gtrkcmdcmr.html

C#:   public string Greet() => Name;
来源：http://hz.zhaomingkeji.xyz/gtxuzkmxjr.html

[G05] 继承
来源：http://hz.xuetiantiany.cn/gtgfkxshyh.html

Py:   class Admin(User): pass
来源：http://hz.hysaishi.cn/gtxmijyaxz.html

PHP:  class Admin extends User {}
来源：http://hz.daria6918.cn/gthmjycusp.html

JS:   class Admin extends User {}
来源：http://hz.shanyushiyangkeji.top/gtrnvxyken.html

TS:   class Admin extends User {}
来源：http://hz.yuxming.cn/gtynjhlwbi.html

Java: class Admin extends User {}
来源：http://hz.mhx1999.top/gtgbtkzjsx.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.hfpthk.cn/gtmimhhlov.html

Ruby: class Admin < User; end
来源：http://hz.cheryme.top/gtprszmlzs.html

C#:   class Admin : User {}
来源：http://hz.jqgfzy.top/gthlepmyyy.html

[G06] 重写方法
来源：http://hz.gogol.net.cn/gtapdloquo.html

Py:   def greet(self): return "admin"
来源：http://hz.birdmap.top/gtmwxzswai.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.mhx1999.top/gtcwckneok.html

JS:   greet() { return "admin"; }
来源：http://hz.0kj1m.cn/gtoslnfxcy.html

TS:   greet(): string { return "admin"; }
来源：http://hz.havefunace.top/gtjksibxxm.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yj20258.top/gtjnyzutif.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.xziqi.cn/gtwccohwny.html

Ruby: def greet; "admin"; end
来源：http://hz.hysaishi.cn/gtujjvsqvp.html

C#:   public override string Greet() => "admin";
来源：http://hz.zhoulong.xyz/gtollqalfy.html

[G07] 调用父类方法
来源：http://hz.shanyushiyangtech.top/gtfswlnell.html

Py:   super().greet()
来源：http://hz.wangshuangyany.cn/gtakdryurr.html

PHP:  parent::greet();
来源：http://hz.cashguo.top/gtpafexery.html

JS:   super.greet();
来源：http://hz.chenzaomai.com/gtuxnsnlke.html

TS:   super.greet();
来源：http://hz.yangfankeji.com/gtlodfuqhk.html

Java: super.greet();
来源：http://hz.hywenlv.cn/gtsehnuhmc.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.zycfv.cn/gtkvudwacr.html

Ruby: super
来源：http://hz.haohaochexian.top/gtpoxerufc.html

C#:   base.Greet();
来源：http://hz.wangshuangyany.cn/gtgoyyeafo.html

[G08] 静态方法与属性
来源：http://hz.yj202588.top/gtxnjmxjpn.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.pycfn.com/gtpfrnzfnd.html

PHP:  public static function f() {}
来源：http://hz.nwbrower.top/gtyrlxvsjx.html

JS:   static f() {}
来源：http://hz.snrcjt.cn/gtzceteetj.html

TS:   static f(): void {}
来源：http://hz.bjfxy.top/gtqdkrpvaz.html

Java: static void f() {}
来源：http://hz.52xcode.cn/gtpivrqrfp.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.0kj1m.cn/gtdnxtbraj.html

Ruby: def self.f; end
来源：http://hz.quarkkingdee.top/gtgtifwbjo.html

C#:   public static void F() {}
来源：http://hz.jyoumei.cn/gtxffvwmns.html

[G09] 接口 / 抽象类
来源：http://hz.hnxiangtu.top/gtcpegkcng.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.yj20258.top/gtvqgjysit.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.feifeiyinyue.top/gttaxgdshl.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.nwbrower.top/gtzgewiqbt.html

TS:   interface Shape { area(): number; }
来源：http://hz.sysykeji.top/gtyaxcmfuw.html

Java: interface Shape { double area(); }
来源：http://hz.svipenyu.cn/gtxcqrysxe.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.ydjk.org.cn/gtjmhikxeo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.tianlin.xyz/gtpedzfbpc.html

C#:   interface IShape { double Area(); }
来源：http://hz.shuidangran.top/gtahbnjkoy.html

[G10] 访问控制
来源：http://hz.hysaishi.cn/gtkpydstqm.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.chenzaomai.com/gtdrxtwgys.html

PHP:  public / protected / private
来源：http://hz.yongpay.top/gtpytgxylo.html

JS:   #private 字段；其余公开
来源：http://hz.shanyushiyangkeji.top/gthwocyoyh.html

TS:   public / protected / private
来源：http://hz.cqqwz.cn/gtdyxrjvwu.html

Java: public / protected / private / 默认包级
来源：http://hz.meibo888.top/gtoxkxmmkt.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.xinyue.icu/gtwywysjzz.html

Ruby: public / protected / private
来源：http://hz.shanyushiyangtech.top/gtwtokeyhk.html

C#:   public / protected / private / internal
来源：http://hz.shzxlz.cn/gtwwzplhur.html

[G11] getter / setter
来源：http://hz.ydjk.org.cn/gtckihhivs.html

Py:   @property 与 @x.setter
来源：http://hz.shuidangran.top/gtyotxfdxd.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.zhaomingkeji.xyz/gtiddbbavi.html

JS:   get name() { return this._name; }
来源：http://hz.daxiang520.top/gtatgqczrw.html

TS:   get name(): string { return this._name; }
来源：http://hz.redwolf501.top/gtsbooaipa.html

Java: public String getName() { return name; }
来源：http://hz.yj202588.top/gtgcopdcvr.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.shzxlz.cn/gtqpreqcah.html

Ruby: attr_accessor :name
来源：http://hz.jqgfzy.top/gtbblzxzvj.html

C#:   public string Name { get; set; }
来源：http://hz.nanxuanxn.top/gttlpduzto.html

[G12] 对象转字符串
来源：http://hz.smart0.xyz/gtticxvhjq.html

Py:   def __str__(self): return self.name
来源：http://hz.zhiwuduotai.top/gtofdayzjl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.cashguo.top/gtuwkdzjoo.html

JS:   toString() { return this.name; }
来源：http://hz.chenzaomai.com/gtyfkgfdzv.html

TS:   toString(): string { return this.name; }
来源：http://hz.tanke756.top/gtjjiggjdp.html

Java: @Override public String toString() { return name; }
来源：http://hz.mhx1999.top/gtpcprvgsz.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.jinqigfzy.top/gtcrjchcpp.html

Ruby: def to_s; @name; end
来源：http://hz.gogol.net.cn/gteunfgfxg.html

C#:   public override string ToString() => Name;
来源：http://hz.ydjk.org.cn/gtogfrvojs.html

[G13] 判断对象类型
来源：http://hz.zycfv.cn/gtnorbajen.html

Py:   isinstance(u, User)
来源：http://hz.nanxuanxn.top/gtnpxjvmoq.html

PHP:  $u instanceof User
来源：http://hz.cheryme.top/gtgzxgejmx.html

JS:   u instanceof User
来源：http://hz.0kj1m.cn/gtyytdbzdy.html

TS:   u instanceof User
来源：http://hz.yj20258.top/gtdtrwhyoc.html

Java: u instanceof User
来源：http://hz.daxiang520.top/gtwcumaacv.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.zhijiandao.cn/gtoicphfni.html

Ruby: u.is_a?(User)
来源：http://hz.iojbl.cn/gtmndkouzq.html

C#:   u is User
来源：http://hz.zhixingplan.top/gtpmwdgigp.html


<!-- 参考信息 -->