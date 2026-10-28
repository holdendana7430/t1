代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.chenlongwang.top/gtmzgnormf.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.shanyushiyangtech.top/gtaadvaedg.html

[E16] 数字千分位
来源：http://hz.fzhhl.top/gtkukuazok.html

Py:   f"{1234567:,}"
来源：http://hz.chenzaomai.com/gtorunpsjv.html

PHP:  number_format(1234567);
来源：http://hz.wangshuangyany.cn/gtfxqsggvz.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.sysykeji.top/gtcsryahci.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.iojbl.cn/gtebhdidkl.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.nanxuanxn.top/gtyiolvhpo.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.yonumen.top/gtgifsjhwh.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.dianchejie.cn/gtqsagaqcz.html

C#:   1234567.ToString("N0")
来源：http://hz.sweek.top/gtisuynlng.html

[E17] 首字母大写
来源：http://hz.tian-w.cn/gttiflecek.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.iojbl.cn/gtjaiwecds.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.guowangkeji.top/gtjuonpejd.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.yj20258888.top/gteqkmsagi.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.ydzc1.top/gtlitrycvu.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.redwolf501.top/gtxjfxytju.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.fzhhl.top/gtllzrgrer.html

Ruby: s.capitalize
来源：http://hz.zhixingplan.top/gtcpmiykhv.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.shanyushiyangtech.top/gtpywcxzdo.html

[E18] 模板占位符替换
来源：http://hz.ivvv.top/gtnoglrzux.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.hnqzz.top/gtpaquyzao.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.hongshengwenyu.top/gtiachdefz.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.yvedp.cn/gteempspdq.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.316326.xyz/gtsjcdbpay.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.cdnleiting.top/gtkwoabttf.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.dashuyun.cn/gtjjqarwhp.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.haohaochexian.top/gtnykwthmd.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yonumen.top/gthunoaohb.html

[E19] 多行文本按行拆分
来源：http://hz.xuanzx.com/gtjpixdfbe.html

Py:   s.splitlines()
来源：http://hz.tian-w.cn/gtoisyiygl.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.cheryme.top/gthfdscmhu.html

JS:   s.split(/\r?\n/)
来源：http://hz.zhongyouzk.top/gttxwvsfys.html

TS:   s.split(/\r?\n/)
来源：http://hz.jyoumei.cn/gtorsqadmk.html

Java: s.lines().toList()
来源：http://hz.vqdsnc.cn/gtcfvplzcn.html

Go:   strings.Split(s, "\n")
来源：http://hz.zhongyouzk.top/gtiqmojbky.html

Ruby: s.lines
来源：http://hz.cucudq.cn/gtyjmzhrbw.html

C#:   s.Split('\n')
来源：http://hz.zycfv.cn/gtnadiboso.html

[E20] 判断字符串是否为空
来源：http://hz.yj20258.top/gtiveafylm.html

Py:   if not s:
来源：http://hz.xziqi.cn/gtwldfirff.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.hammf.cn/gtbjginpdx.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.daria6918.cn/gtipswcbyo.html

TS:   if (s === "") {}
来源：http://hz.ywan-chungtsiang.top/gtaoczrtwm.html

Java: if (s.isEmpty()) {}
来源：http://hz.chenjidiqi.icu/gtucnsyljg.html

Go:   if s == "" {}
来源：http://hz.shzxlz.cn/gtpwyjdmvg.html

Ruby: if s.empty?
来源：http://hz.c1oappe.top/gtbuscemnt.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.vqdsnc.cn/gtpagswpnb.html

[E21] 超长截断加省略号
来源：http://hz.shzxlz.cn/gthsqjdkrk.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.cdnleiting.top/gtxfhwsmym.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.guowangkeji.top/gttqzuhlmu.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.svipenyu.cn/gtakgfixhb.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.svipenyu.cn/gtiszzmkqw.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.shuidangran.top/gtzgafuwia.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yongpay.top/gtrejcdjyu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.cdnleiting.top/gtwxrsueyy.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.wangdashe.top/gtyupkrhuj.html

[E22] 字节长度与字符长度
来源：http://hz.yangfankeji.com/gtiqgbvkti.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.pycfn.com/gtfqdxptuq.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.hnxiangtu.top/gtxusduhhc.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.cqqwz.cn/gtheujgtiz.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hfpthk.cn/gtdahkngnk.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yuanzhike.top/gtcxrckuib.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.ywan-chungtsiang.top/gtdgtyxsep.html

Ruby: s.bytesize;  s.length
来源：http://hz.jinqigufen.top/gtzbtlnyfi.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jqgfzy.top/gtscfuttef.html

================================================================================
来源：http://hz.yvedp.cn/gtndtghmch.html

F. 文件与目录
来源：http://hz.guannengcc.top/gtzatjvxxl.html

================================================================================
来源：http://hz.snrcjt.cn/gtfnaultlx.html

[F01] 读取整个文件
来源：http://hz.yj20258888.top/gtdixnlnvc.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.aizwys.cn/gtoxajorpn.html

PHP:  file_get_contents("a.txt");
来源：http://hz.wangdashe.top/gtvmtdjlkb.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.andypj.xyz/gttwlqegql.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.ywan-chungtsiang.top/gtoevkiamv.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.xingfuxueyuan.xyz/gttchipqzu.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.xingfuxueyuan.xyz/gtblcgsalw.html

Ruby: File.read("a.txt")
来源：http://hz.redwolf501.top/gtqtqyqpga.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.cqqwz.cn/gtwgljbvwl.html

[F02] 逐行读取文件
来源：http://hz.birdmap.top/gtrnmvravc.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.quarkkingdee.top/gtngyrbzzb.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.snrcjt.cn/gtsrmgfqgp.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.birdmap.top/gtuxdjzmnt.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.ivvv.top/gtcspadlsf.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.chenzaomai.com/gtyoqfufec.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.ppjwa.cn/gtuhybqfih.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.ppjwa.cn/gtiztaoies.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.hnxiangtu.top/gttgonpyhl.html

[F03] 写入文件（覆盖）
来源：http://hz.yj20258888.top/gtcafpvawv.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.cqqwz.cn/gtucdknjyu.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.ppjwa.cn/gtcvzmrapt.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.redwolf501.top/gtenzuvqbx.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.nanxinkj.top/gttpeksopn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.yvedp.cn/gtwcfuckge.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.cdnleiting.top/gtruxfzzup.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yj20258888.top/gtnnsqwbmq.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yvedp.cn/gthqtodeew.html

[F04] 追加写入文件
来源：http://hz.meibo888.top/gtrwuidybl.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.fengsongda.top/gtndwfbqne.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.zhijiandao.cn/gtiohzidxq.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.havefunace.top/gtazzhyhae.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.bjfxy.top/gtqmeawwwo.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.shangyingyoupin.top/gtaoodlasn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.hnxiangtu.top/gtqvfufeoc.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.xziqi.cn/gtotgmtimj.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.fzhhl.top/gtkaiwrsdy.html

[F05] 判断文件或目录是否存在
来源：http://hz.tanke756.top/gtmsqlbrfu.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.vqdsnc.cn/gtmwdfpuzx.html

PHP:  file_exists("a.txt");
来源：http://hz.haohaochexian.top/gtptvriark.html

JS:   fs.existsSync("a.txt")
来源：http://hz.nwbrower.top/gthdgzppzt.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yangfankeji.com/gtdpbdyxnz.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.jqgfzy.top/gtcdoavcvn.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ydjk.org.cn/gtqxbowria.html

Ruby: File.exist?("a.txt")
来源：http://hz.jlsjyb.cn/gtnqkvgkyg.html

C#:   File.Exists("a.txt")
来源：http://hz.316326.xyz/gtdqaoigje.html

[F06] 删除文件
来源：http://hz.smart0.xyz/gthwcetlst.html

Py:   os.remove("a.txt")
来源：http://hz.shuidangran.top/gtbfxbqyza.html

PHP:  unlink("a.txt");
来源：http://hz.andypj.xyz/gtwuohpqav.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.haohaochexian.top/gtnyvryjaf.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.kuanghao11.cn/gtblbeuoyu.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.vqdsnc.cn/gtispehnyq.html

Go:   os.Remove("a.txt")
来源：http://hz.zhengqikj.top/gtpacnvdmc.html

Ruby: File.delete("a.txt")
来源：http://hz.nwbrower.top/gtwzvdjfql.html

C#:   File.Delete("a.txt");
来源：http://hz.wangshuangyany.cn/gtlvtyqabr.html

[F07] 创建目录（含多级）
来源：http://hz.hnxiangtu.top/gtgoauhxcp.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.shuidangran.top/gtejbftwml.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.zhengqikj.top/gtuexzmvxt.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yuxming.cn/gtbbpmuhho.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.c1oappe.top/gtzgudcxni.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.sxryk.cn/gtxujqicqr.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.snrcjt.cn/gtusjhngqb.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.xuanzx.com/gtizsrkfup.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.yvedp.cn/gtgotfuear.html

[F08] 遍历目录
来源：http://hz.yanxiufei.cn/gtddczkyfe.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xinyue.icu/gtonyitpdo.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.gzhubu.top/gtmokyswxn.html

JS:   fs.readdirSync("dir")
来源：http://hz.yangfankeji.com/gtmynzijui.html

TS:   fs.readdirSync("dir")
来源：http://hz.ydzc1.top/gtfhkhnlxo.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.yangfankeji.com/gtlinvwyok.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.andypj.xyz/gtcwgpjmtr.html

Ruby: Dir.children("dir")
来源：http://hz.nanxinkj.top/gtelcqybrn.html

C#:   Directory.GetFiles("dir")
来源：http://hz.haohaochexian.top/gtnzkrmypx.html

[F09] 获取文件大小
来源：http://hz.sweek.top/gtcponheay.html

Py:   os.path.getsize("a.txt")
来源：http://hz.ydzc1.top/gtnajeuzge.html

PHP:  filesize("a.txt");
来源：http://hz.cashguo.top/gtipwsqitm.html

JS:   fs.statSync("a.txt").size
来源：http://hz.yuanzhike.top/gtuwkjlbwt.html

TS:   fs.statSync("a.txt").size
来源：http://hz.xinyue.icu/gtemnggnhs.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.jlsjyb.cn/gtguniufnw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.jinqigfzy.top/gtqddbyuhr.html

Ruby: File.size("a.txt")
来源：http://hz.xziqi.cn/gtlccsjumd.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.aizwys.cn/gtbnxgivix.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zhaomingkeji.xyz/gtsqimqzjd.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.aibaodan.cn/gthjqggtbw.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.iojbl.cn/gthaaofwzl.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.kuanghao11.cn/gtvlrbpsrm.html

TS:   path.extname("a.txt")
来源：http://hz.dianchejie.cn/gtaorwyjdm.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.tian-w.cn/gtabrmfqgx.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.hammf.cn/gtzrpswhun.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.aibaodan.cn/gtijfqmgfi.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.shanyushiyangtech.top/gtdfwygude.html

[F11] 复制与移动文件
来源：http://hz.ehwqpu.com/gtbsktxtha.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.kuanghao11.cn/gtfchfrvaz.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.vqdsnc.cn/gtfvijrkkd.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.xylfe.cn/gtluogolzt.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhijiandao.cn/gtomtbrnji.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.sxryk.cn/gtmdbarriu.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.nanxinkj.top/gtegwugrnb.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.andypj.xyz/gtpbiwjsuu.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.gaohongyu789.top/gtsxhhiyli.html

[F12] CSV 读写
来源：http://hz.ydzc1.top/gtvmhvdzmi.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.jlsjyb.cn/gtqdovctgr.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.52xcode.cn/gtlrhlyhlh.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.xingfuxueyuan.xyz/gtmhoxxoso.html

TS:   // 同上
来源：http://hz.chenjidiqi.icu/gtminhgxvw.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.cqqwz.cn/gtgngiakux.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.xuanzx.com/gtmbsrjqcm.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.redwolf501.top/gtueyihhdn.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.52xcode.cn/gtzlutfyhq.html

================================================================================
来源：http://hz.zhoulong.xyz/gtbcwqyunk.html

G. 面向对象
来源：http://hz.chenlongwang.top/gtgzyknzrv.html

================================================================================
来源：http://hz.yuanzhike.top/gtocdyuyhp.html

[G01] 定义类
来源：http://hz.zhoulong.xyz/gttjrzohlw.html

Py:   class User: pass
来源：http://hz.zhiwuduotai.top/gtdkfwuafa.html

PHP:  class User {}
来源：http://hz.yanxiufei.cn/gthzjtohlf.html

JS:   class User {}
来源：http://hz.xinyue.icu/gtgufshwuk.html

TS:   class User { name: string = ""; }
来源：http://hz.xinyue.icu/gtlxeimgme.html

Java: class User {}
来源：http://hz.ehwqpu.com/gtouhrqlny.html

Go:   type User struct { Name string }
来源：http://hz.wangshuangyany.cn/gtixanogmh.html

Ruby: class User; end
来源：http://hz.aizwys.cn/gtjefzedso.html

C#:   class User {}
来源：http://hz.ydzc1.top/gtkcuheggy.html

[G02] 构造函数
来源：http://hz.ywan-chungtsiang.top/gthohzefze.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.bjfxy.top/gtthetkbux.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.jlsjyb.cn/gtutoybzxr.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.jinghuilouyu.cn/gtfhglfeno.html

TS:   constructor(public name: string) {}
来源：http://hz.chenlongwang.top/gtzncbodoa.html

Java: User(String name) { this.name = name; }
来源：http://hz.birdmap.top/gthhzniaio.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.nanxuanxn.top/gtpmcsfoky.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.vqdsnc.cn/gtpgnzbcdj.html

C#:   public User(string name) { Name = name; }
来源：http://hz.hnqzz.top/gtdzwdkmsr.html

[G03] 实例属性
来源：http://hz.sufxvd.cn/gtixcycvla.html

Py:   self.name = "x"
来源：http://hz.quarkkingdee.top/gtzoecvfcw.html

PHP:  public string $name = "x";
来源：http://hz.fengsongda.top/gtprnqvyeh.html

JS:   this.name = "x";
来源：http://hz.ydjk.org.cn/gtgpgcqoxn.html

TS:   name: string = "x";
来源：http://hz.jinqigufen.top/gtyvcuetav.html

Java: private String name;
来源：http://hz.smart0.xyz/gtsmfkdzft.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.yongpay.top/gtbsdzzxwu.html

Ruby: @name = "x"
来源：http://hz.zhiwuduotai.top/gtbxdptklj.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.sufxvd.cn/gtoyrancud.html

[G04] 定义方法
来源：http://hz.wangdashe.top/gtnyzcnynf.html

Py:   def greet(self): return self.name
来源：http://hz.bjfxy.top/gtecuclmtb.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hammf.cn/gthglfjdnq.html

JS:   greet() { return this.name; }
来源：http://hz.yj202588.top/gtfzjbzazw.html

TS:   greet(): string { return this.name; }
来源：http://hz.daxiang520.top/gtkzkghqln.html

Java: String greet() { return name; }
来源：http://hz.sxryk.cn/gtmefoogus.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.ybcxt.top/gtckxuiaqp.html

Ruby: def greet; @name; end
来源：http://hz.ivvv.top/gtedoyrflp.html

C#:   public string Greet() => Name;
来源：http://hz.shanyushiyangkeji.top/gtmhkzrrrc.html

[G05] 继承
来源：http://hz.guowangkeji.top/gtwsljypra.html

Py:   class Admin(User): pass
来源：http://hz.yanxiufei.cn/gtvcqdmmbq.html

PHP:  class Admin extends User {}
来源：http://hz.xylfe.cn/gtadxcoknk.html

JS:   class Admin extends User {}
来源：http://hz.nanxinkj.top/gtllrbjnmo.html

TS:   class Admin extends User {}
来源：http://hz.shanyushiyangkeji.top/gtsmrhzsit.html

Java: class Admin extends User {}
来源：http://hz.vqdsnc.cn/gtskwaujcp.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.vqdsnc.cn/gtfdjutmmj.html

Ruby: class Admin < User; end
来源：http://hz.c1oappe.top/gtakjsnjpn.html

C#:   class Admin : User {}
来源：http://hz.birdmap.top/gtpxljwqko.html

[G06] 重写方法
来源：http://hz.aibaodan.cn/gtzvogurqa.html

Py:   def greet(self): return "admin"
来源：http://hz.jinqigufen.top/gtwuxheglj.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yj20258.top/gtxcrimafe.html

JS:   greet() { return "admin"; }
来源：http://hz.jinghuilouyu.cn/gtofiaeolo.html

TS:   greet(): string { return "admin"; }
来源：http://hz.sxryk.cn/gtzeqypgja.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.sweek.top/gtrhgmkllp.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.bjfxy.top/gtlcnutikw.html

Ruby: def greet; "admin"; end
来源：http://hz.vqdsnc.cn/gtnnckamzc.html

C#:   public override string Greet() => "admin";
来源：http://hz.hammf.cn/gttmzlcbup.html

[G07] 调用父类方法
来源：http://hz.jinghuilouyu.cn/gtpcxnikhv.html

Py:   super().greet()
来源：http://hz.jinyuanbaomall.cn/gtfxqrsfuj.html

PHP:  parent::greet();
来源：http://hz.jinqigfzy.top/gttqxufwua.html

JS:   super.greet();
来源：http://hz.jinghuilouyu.cn/gtrkvppact.html

TS:   super.greet();
来源：http://hz.sufxvd.cn/gtrjgkjepi.html

Java: super.greet();
来源：http://hz.sxryk.cn/gtzjwqxvjs.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.birdmap.top/gtlgvglozf.html

Ruby: super
来源：http://hz.jqgfzy.top/gtsfdbfmst.html

C#:   base.Greet();
来源：http://hz.jinghuilouyu.cn/gtflfhpwps.html

[G08] 静态方法与属性
来源：http://hz.tian-w.cn/gtezlxykcb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.ehwqpu.com/gttdyaelfj.html

PHP:  public static function f() {}
来源：http://hz.andypj.xyz/gtqbiuwwpd.html

JS:   static f() {}
来源：http://hz.gzhubu.top/gtrdzfmlbf.html

TS:   static f(): void {}
来源：http://hz.jyoumei.cn/gtcjmafpuq.html

Java: static void f() {}
来源：http://hz.zhengqikj.top/gtbjscwnlm.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jlsjyb.cn/gtcrxeozkf.html

Ruby: def self.f; end
来源：http://hz.jiagoushi.top/gtfrgdmgzf.html

C#:   public static void F() {}
来源：http://hz.zhongyouzk.top/gthbmzgyjd.html

[G09] 接口 / 抽象类
来源：http://hz.chenzaomai.com/gtngfebsaz.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.chenjidiqi.icu/gtvxxgnbqa.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.xuanzx.com/gtbnkbpboq.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.chenlongwang.top/gtcuicmlrm.html

TS:   interface Shape { area(): number; }
来源：http://hz.hammf.cn/gtigykjmru.html

Java: interface Shape { double area(); }
来源：http://hz.zhijiandao.cn/gteoevwvpl.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.gaohongyu789.top/gtfjnkqldj.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.zdqjudy.top/gthcelblai.html

C#:   interface IShape { double Area(); }
来源：http://hz.guannengcc.top/gtvzydhill.html

[G10] 访问控制
来源：http://hz.guannengcc.top/gteojzhicn.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yj202588.top/gttwtnzpcn.html

PHP:  public / protected / private
来源：http://hz.guowangkeji.top/gtpicuxhtz.html

JS:   #private 字段；其余公开
来源：http://hz.aibaodan.cn/gtsokoavct.html

TS:   public / protected / private
来源：http://hz.bjfxy.top/gtutnabusj.html

Java: public / protected / private / 默认包级
来源：http://hz.jqgufenzy.top/gthjwakyjr.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.gotoacloud.top/gtgzupaecx.html

Ruby: public / protected / private
来源：http://hz.xinyue.icu/gtbnvlumtw.html

C#:   public / protected / private / internal
来源：http://hz.meibo888.top/gtccpsnqys.html

[G11] getter / setter
来源：http://hz.chenjidiqi.icu/gtbjdbwyqt.html

Py:   @property 与 @x.setter
来源：http://hz.hammf.cn/gtbyuhsygp.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.316326.xyz/gtvcsotskq.html

JS:   get name() { return this._name; }
来源：http://hz.chenlongwang.top/gtejxjszrj.html

TS:   get name(): string { return this._name; }
来源：http://hz.cucudq.cn/gtxsuxanfs.html

Java: public String getName() { return name; }
来源：http://hz.shzxlz.cn/gtoxposybs.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.hongshengwenyu.top/gtnzzthvsp.html

Ruby: attr_accessor :name
来源：http://hz.jlsjyb.cn/gtcoewgtul.html

C#:   public string Name { get; set; }
来源：http://hz.xinyue.icu/gtwoqxtcaq.html

[G12] 对象转字符串
来源：http://hz.xylfe.cn/gtzuxzrmfz.html

Py:   def __str__(self): return self.name
来源：http://hz.ywan-chungtsiang.top/gtstkxboci.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.zhiwuduotai.top/gtwileymlk.html

JS:   toString() { return this.name; }
来源：http://hz.snrcjt.cn/gttlzuooai.html

TS:   toString(): string { return this.name; }
来源：http://hz.jinqigufen.top/gtejfpwtmu.html

Java: @Override public String toString() { return name; }
来源：http://hz.cashguo.top/gtbnaopvsx.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.hongshengwenyu.top/gtkvrpncui.html

Ruby: def to_s; @name; end
来源：http://hz.dianchejie.cn/gttqcdbrxc.html

C#:   public override string ToString() => Name;
来源：http://hz.feifeiyinyue.top/gthpvbnltf.html

[G13] 判断对象类型
来源：http://hz.havefunace.top/gtidqnwpvw.html

Py:   isinstance(u, User)
来源：http://hz.xziqi.cn/gtdlnqxtmv.html

PHP:  $u instanceof User
来源：http://hz.fzhhl.top/gtehhsyuwq.html

JS:   u instanceof User
来源：http://hz.feifeiyinyue.top/gtrtzrehzj.html

TS:   u instanceof User
来源：http://hz.jinqigfzy.top/gtxrraouxo.html

Java: u instanceof User
来源：http://hz.yuxming.cn/gtsutagksz.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.shangyingyoupin.top/gtsjthplof.html

Ruby: u.is_a?(User)
来源：http://hz.guannengcc.top/gtprgcymca.html

C#:   u is User
来源：http://hz.zhongyouzk.top/gtrrrvjflc.html

[G14] 数据类 / record
来源：http://hz.hnqzz.top/gtzyrvtkfo.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.quarkkingdee.top/gtzwywzgbm.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.hysaishi.cn/gtmihhuuth.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.redwolf501.top/gtzvpssial.html


<!-- 参考信息 -->