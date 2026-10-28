代发 wailian999

Ruby: CGI.escapeHTML(s);  CGI.unescapeHTML(s)
来源：http://hz.snrcjt.cn/gtouzhpplb.html

C#:   WebUtility.HtmlEncode(s);  WebUtility.HtmlDecode(s)
来源：http://hz.gotoacloud.top/gtmdgruheq.html

[E16] 数字千分位
来源：http://hz.hnxiangtu.top/gttywgvxqj.html

Py:   f"{1234567:,}"
来源：http://hz.shzxlz.cn/gtramaqyac.html

PHP:  number_format(1234567);
来源：http://hz.cashguo.top/gtkenczcum.html

JS:   (1234567).toLocaleString("en-US")
来源：http://hz.hysaishi.cn/gtkhwwttpc.html

TS:   (1234567).toLocaleString("en-US")
来源：http://hz.ybcxt.top/gtlybfcypu.html

Java: NumberFormat.getNumberInstance(Locale.US).format(1234567)
来源：http://hz.0kj1m.cn/gtqyabzaol.html

Go:   // 用 golang.org/x/text/message 或手写分组
来源：http://hz.jinghuilouyu.cn/gtgxprmcoi.html

Ruby: "1234567".reverse.scan(/\d{1,3}/).join(",").reverse
来源：http://hz.xingfuxueyuan.xyz/gtczriuqhe.html

C#:   1234567.ToString("N0")
来源：http://hz.yj202588.top/gtanzddled.html

[E17] 首字母大写
来源：http://hz.jlsjyb.cn/gthogiunuv.html

Py:   s[0].upper() + s[1:];  s.capitalize();  s.title()
来源：http://hz.nwbrower.top/gtzwrmhtht.html

PHP:  ucfirst($s);  ucwords($s);
来源：http://hz.hammf.cn/gtbuwkpvrx.html

JS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.bjfxy.top/gtodubtibs.html

TS:   s.charAt(0).toUpperCase() + s.slice(1)
来源：http://hz.dianchejie.cn/gtpnqzkudc.html

Java: Character.toUpperCase(s.charAt(0)) + s.substring(1)
来源：http://hz.xuetiantiany.cn/gtajmaskry.html

Go:   strings.ToUpper(s[:1]) + s[1:]
来源：http://hz.jiagoushi.top/gtvcyapjzi.html

Ruby: s.capitalize
来源：http://hz.ywan-chungtsiang.top/gtzvqugcyd.html

C#:   char.ToUpper(s[0]) + s[1..]
来源：http://hz.yueranfly.top/gtemyfnomi.html

[E18] 模板占位符替换
来源：http://hz.ydjk.org.cn/gtfcbnkgty.html

Py:   "Hello, {name}".format(name="A");  tpl.replace("{name}", "A")
来源：http://hz.snrcjt.cn/gtoivitfzm.html

PHP:  str_replace("{name}", "A", $tpl);  sprintf("Hello, %s", $name);
来源：http://hz.mhx1999.top/gtdzujpjdf.html

JS:   tpl.replaceAll("{name}", name)
来源：http://hz.daria6918.cn/gthrmtmmmb.html

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.shzxlz.cn/gtjlpvtzof.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.52xcode.cn/gtscujtfcz.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.yj202588.top/gtrpfoasrw.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.vqdsnc.cn/gthdlhabsy.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.yonumen.top/gtjubftsiw.html

[E19] 多行文本按行拆分
来源：http://hz.yj20258888.top/gtryapevdh.html

Py:   s.splitlines()
来源：http://hz.jqgufenzy.top/gthgoussze.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.aibaodan.cn/gtzpjakuxm.html

JS:   s.split(/\r?\n/)
来源：http://hz.fzhhl.top/gthdxyjdwa.html

TS:   s.split(/\r?\n/)
来源：http://hz.kuanghao11.cn/gthunhkped.html

Java: s.lines().toList()
来源：http://hz.zhijiandao.cn/gtnpffguix.html

Go:   strings.Split(s, "\n")
来源：http://hz.52xcode.cn/gtyrqkcqea.html

Ruby: s.lines
来源：http://hz.xylfe.cn/gtxcqndblv.html

C#:   s.Split('\n')
来源：http://hz.ppjwa.cn/gtlsrmvqlo.html

[E20] 判断字符串是否为空
来源：http://hz.gotoacloud.top/gtqahcgdee.html

Py:   if not s:
来源：http://hz.xingfuxueyuan.xyz/gtiirhqqzm.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.shangyingyoupin.top/gtlwmkqxyq.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.wangdashe.top/gtkjxtrcbp.html

TS:   if (s === "") {}
来源：http://hz.ydjk.org.cn/gtgyclccgl.html

Java: if (s.isEmpty()) {}
来源：http://hz.aizwys.cn/gtdmzrmhra.html

Go:   if s == "" {}
来源：http://hz.gzhubu.top/gttnzemnbf.html

Ruby: if s.empty?
来源：http://hz.yj20258888.top/gtihvdzumh.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.cqqwz.cn/gtyzljlbgy.html

[E21] 超长截断加省略号
来源：http://hz.jinyuanbaomall.cn/gtchdgvqrl.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.nwbrower.top/gtfrfyfxkn.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.dashuyun.cn/gtutnhmtsh.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.shanyushiyangtech.top/gtscsqpqgt.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.sweek.top/gtbncxwwje.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.svipenyu.cn/gtsfuajpbe.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.gogol.net.cn/gtutqnthpu.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.yongpay.top/gtnuimaaru.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.ydjk.org.cn/gtlnszsasf.html

[E22] 字节长度与字符长度
来源：http://hz.guowangkeji.top/gtxalthhqr.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.xinyue.icu/gtujpdyxvv.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhongyouzk.top/gtcpgizlvq.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hnqzz.top/gtjgsidnmv.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.dianchejie.cn/gtrzapfbrx.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yueranfly.top/gtsryomxmq.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.sysykeji.top/gtilmeikln.html

Ruby: s.bytesize;  s.length
来源：http://hz.chenjidiqi.icu/gtrzatkfym.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.hammf.cn/gtquazaian.html

================================================================================
来源：http://hz.xziqi.cn/gtmwqtgnue.html

F. 文件与目录
来源：http://hz.hammf.cn/gtnwkxdvgy.html

================================================================================
来源：http://hz.andypj.xyz/gtcrugehml.html

[F01] 读取整个文件
来源：http://hz.vqdsnc.cn/gtjdmowscd.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.guannengcc.top/gtgklwuhwj.html

PHP:  file_get_contents("a.txt");
来源：http://hz.svipenyu.cn/gtprxqbsiy.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.daxiang520.top/gtvufxfvcd.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.quarkkingdee.top/gtmbkhmxbh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jyoumei.cn/gtcwjrbsnb.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.hfpthk.cn/gtkcdurxur.html

Ruby: File.read("a.txt")
来源：http://hz.xziqi.cn/gtsctjoubm.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.aibaodan.cn/gtrfffjbbi.html

[F02] 逐行读取文件
来源：http://hz.zdqjudy.top/gtpemjvisu.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.cdnleiting.top/gtvpzrubgk.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.zhongyouzk.top/gtgeaqewjz.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.haohaochexian.top/gtolxwsrfr.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.tian-w.cn/gtaxatvwap.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.kuanghao11.cn/gticbsopzk.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.svipenyu.cn/gtregkzoxn.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.sufxvd.cn/gtoroxfesa.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.fzhhl.top/gtmpalawgr.html

[F03] 写入文件（覆盖）
来源：http://hz.jinghuilouyu.cn/gtvfrbvina.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.svipenyu.cn/gtpklmxetm.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.cheryme.top/gtabbyqjic.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.zhoulong.xyz/gtzlmceode.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.fzhhl.top/gtmaenmrcn.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.jiagoushi.top/gtjqtaegwz.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.yvedp.cn/gtzdfylkir.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.ydjk.org.cn/gtpccgklmy.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.yvedp.cn/gtlhprqukm.html

[F04] 追加写入文件
来源：http://hz.feifeiyinyue.top/gtjesxnxhj.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.wangshuangyany.cn/gtlybdhxpi.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.hnqzz.top/gtpnrsmube.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.c1oappe.top/gtimdjyuro.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.cdnleiting.top/gtsoxaxzyx.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.birdmap.top/gtaqctiyxv.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.tanke756.top/gtdyfdqsbk.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.jinghuilouyu.cn/gtrfasrkba.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.yongpay.top/gtyidspdsk.html

[F05] 判断文件或目录是否存在
来源：http://hz.ydjk.org.cn/gtyxaixyyb.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.yj20258888.top/gtazznjolg.html

PHP:  file_exists("a.txt");
来源：http://hz.jiagoushi.top/gtssmqhyii.html

JS:   fs.existsSync("a.txt")
来源：http://hz.daria6918.cn/gtjxpmeczs.html

TS:   fs.existsSync("a.txt")
来源：http://hz.jinqigfzy.top/gtvwehvzhb.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.gaohongyu789.top/gtuiqngsmt.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.jqgufenzy.top/gtxoteiddu.html

Ruby: File.exist?("a.txt")
来源：http://hz.shanyushiyangtech.top/gtwkrjnbem.html

C#:   File.Exists("a.txt")
来源：http://hz.shuidangran.top/gtxmuxzzsd.html

[F06] 删除文件
来源：http://hz.sweek.top/gtcejrmale.html

Py:   os.remove("a.txt")
来源：http://hz.chenlongwang.top/gtlpbjvkwi.html

PHP:  unlink("a.txt");
来源：http://hz.zhijiandao.cn/gteqsfopjy.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.cdnleiting.top/gtqyibssju.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.jinghuilouyu.cn/gtyneaxnbz.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.sweek.top/gtqypoplao.html

Go:   os.Remove("a.txt")
来源：http://hz.yvedp.cn/gtdylchitg.html

Ruby: File.delete("a.txt")
来源：http://hz.feifeiyinyue.top/gtfzdrulvr.html

C#:   File.Delete("a.txt");
来源：http://hz.zhiwuduotai.top/gtijjyldjw.html

[F07] 创建目录（含多级）
来源：http://hz.hnxiangtu.top/gtwumipeub.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.ybcxt.top/gtyucpdgak.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.kuanghao11.cn/gtngzlnjdn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhengqikj.top/gtbydintjl.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.quarkkingdee.top/gttycvbpvz.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.ydjk.org.cn/gtikmnrqlj.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.dashuyun.cn/gtdaofyvek.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.sufxvd.cn/gtrtuprydm.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zhengqikj.top/gtmluhpjrm.html

[F08] 遍历目录
来源：http://hz.jqgufenzy.top/gtsxrdbufi.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.jlsjyb.cn/gtnlgcsimh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.daria6918.cn/gtlvxuqrls.html

JS:   fs.readdirSync("dir")
来源：http://hz.shangyingyoupin.top/gtokioabzi.html

TS:   fs.readdirSync("dir")
来源：http://hz.cashguo.top/gtxwwwpyua.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zdqjudy.top/gtkflleieo.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.cdnleiting.top/gtejvgzarg.html

Ruby: Dir.children("dir")
来源：http://hz.shanyushiyangtech.top/gtyaugflvz.html

C#:   Directory.GetFiles("dir")
来源：http://hz.chenzaomai.com/gthahywxpv.html

[F09] 获取文件大小
来源：http://hz.ybcxt.top/gtqsibisie.html

Py:   os.path.getsize("a.txt")
来源：http://hz.nanxinkj.top/gtxtmaxhas.html

PHP:  filesize("a.txt");
来源：http://hz.cheryme.top/gtceamqpjz.html

JS:   fs.statSync("a.txt").size
来源：http://hz.316326.xyz/gtoyapkyus.html

TS:   fs.statSync("a.txt").size
来源：http://hz.pycfn.com/gtvtyuesaz.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.cucudq.cn/gtozwqdcyw.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.havefunace.top/gtntjvidwk.html

Ruby: File.size("a.txt")
来源：http://hz.jqgfzy.top/gtgmhdmjvx.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.feifeiyinyue.top/gtdffuscxz.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.zhixingplan.top/gtoeoedqzl.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jqgufenzy.top/gtzhmxivor.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.aizwys.cn/gtqcqhskzi.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.jqgfzy.top/gtymmkpiqn.html

TS:   path.extname("a.txt")
来源：http://hz.meibo888.top/gtlqrzhpmn.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.jiagoushi.top/gtyodtjsfw.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.wangdashe.top/gtxnxqjtzo.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.jiagoushi.top/gtbzfgfvos.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.xylfe.cn/gtqlfxfrqk.html

[F11] 复制与移动文件
来源：http://hz.zhongyouzk.top/gthdimhebr.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.zhengqikj.top/gtixxngjsj.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.yj20258888.top/gtyzljudzs.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jinghuilouyu.cn/gtvavnuwfh.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.zhaomingkeji.xyz/gtotanjotb.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.guowangkeji.top/gthjspriel.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.gzhubu.top/gthrewiigf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.havefunace.top/gtiearbhgl.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.xuanzx.com/gtoxnvkqwl.html

[F12] CSV 读写
来源：http://hz.yuanzhike.top/gtvrdgmujl.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.zhijiandao.cn/gtsuxabljm.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.xuanzx.com/gtrnujwymc.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.hywenlv.cn/gtyhoerqal.html

TS:   // 同上
来源：http://hz.hfpthk.cn/gtxacewzvi.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.yongpay.top/gtgzrxcnde.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.hysaishi.cn/gtmawmvuza.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.xziqi.cn/gtudvtxgel.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.guowangkeji.top/gtkemnelmm.html

================================================================================
来源：http://hz.xuanzx.com/gtofqmmumj.html

G. 面向对象
来源：http://hz.shanyushiyangtech.top/gtjpcttigo.html

================================================================================
来源：http://hz.ivvv.top/gtclduzxyc.html

[G01] 定义类
来源：http://hz.ybcxt.top/gtatkriwxk.html

Py:   class User: pass
来源：http://hz.yuanzhike.top/gttvflltkw.html

PHP:  class User {}
来源：http://hz.chenlongwang.top/gtfivorkry.html

JS:   class User {}
来源：http://hz.daria6918.cn/gtbenhpbjr.html

TS:   class User { name: string = ""; }
来源：http://hz.jinqigfzy.top/gtobunjkkg.html

Java: class User {}
来源：http://hz.jqgfzy.top/gtgidqpdkh.html

Go:   type User struct { Name string }
来源：http://hz.yongpay.top/gtoffzijmn.html

Ruby: class User; end
来源：http://hz.mhx1999.top/gtsvypfyiq.html

C#:   class User {}
来源：http://hz.yuxming.cn/gtpxrxabfo.html

[G02] 构造函数
来源：http://hz.nwbrower.top/gtqxrdsnle.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.gogol.net.cn/gtrsyvpgow.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.zhengqikj.top/gtxokqlufp.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.sysykeji.top/gtiurhvplf.html

TS:   constructor(public name: string) {}
来源：http://hz.cheryme.top/gtigjjmihz.html

Java: User(String name) { this.name = name; }
来源：http://hz.chenzaomai.com/gtitdbuvpc.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.aizwys.cn/gtuutblogs.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.dashuyun.cn/gtmglcezmf.html

C#:   public User(string name) { Name = name; }
来源：http://hz.wangshuangyany.cn/gtxalnvblk.html

[G03] 实例属性
来源：http://hz.daxiang520.top/gtzraaqmzv.html

Py:   self.name = "x"
来源：http://hz.shuidangran.top/gtmzxavbru.html

PHP:  public string $name = "x";
来源：http://hz.yj202588.top/gtzxzweeck.html

JS:   this.name = "x";
来源：http://hz.cucudq.cn/gtudfzavll.html

TS:   name: string = "x";
来源：http://hz.ehwqpu.com/gthctgzlpw.html

Java: private String name;
来源：http://hz.smart0.xyz/gtxnrifanu.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.316326.xyz/gttjmoviws.html

Ruby: @name = "x"
来源：http://hz.ivvv.top/gtsyozxapk.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.ybcxt.top/gtrqnyxgoj.html

[G04] 定义方法
来源：http://hz.ehwqpu.com/gtmkuajbgm.html

Py:   def greet(self): return self.name
来源：http://hz.pengpengdd.cyou/gtndgcnuqp.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.ydzc1.top/gtigbblipx.html

JS:   greet() { return this.name; }
来源：http://hz.daxiang520.top/gtqravglyf.html

TS:   greet(): string { return this.name; }
来源：http://hz.fengsongda.top/gtfykfotmx.html

Java: String greet() { return name; }
来源：http://hz.sufxvd.cn/gtqrbmlwpq.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.316326.xyz/gtwlmmasrt.html

Ruby: def greet; @name; end
来源：http://hz.sweek.top/gtzmbitpbk.html

C#:   public string Greet() => Name;
来源：http://hz.cdnleiting.top/gtzbpmretp.html

[G05] 继承
来源：http://hz.meibo888.top/gtfjoyvmch.html

Py:   class Admin(User): pass
来源：http://hz.meibo888.top/gtqbjcspqs.html

PHP:  class Admin extends User {}
来源：http://hz.zhaomingkeji.xyz/gtrgcdzdrp.html

JS:   class Admin extends User {}
来源：http://hz.jinqigufen.top/gteowojfax.html

TS:   class Admin extends User {}
来源：http://hz.andypj.xyz/gtmxhyngtl.html

Java: class Admin extends User {}
来源：http://hz.pycfn.com/gtrvgrlzir.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.cucudq.cn/gtfylufxyf.html

Ruby: class Admin < User; end
来源：http://hz.yangfankeji.com/gtyvngbypd.html

C#:   class Admin : User {}
来源：http://hz.0kj1m.cn/gtqnafrixp.html

[G06] 重写方法
来源：http://hz.daxiang520.top/gtkirqxnwc.html

Py:   def greet(self): return "admin"
来源：http://hz.nanxuanxn.top/gtwqsgjcjo.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.yvedp.cn/gtvzdkmhie.html

JS:   greet() { return "admin"; }
来源：http://hz.daria6918.cn/gtdximhjas.html

TS:   greet(): string { return "admin"; }
来源：http://hz.xziqi.cn/gtsveployu.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.yvedp.cn/gtmepeemff.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.aibaodan.cn/gtblnjpghb.html

Ruby: def greet; "admin"; end
来源：http://hz.316326.xyz/gtnrmpnqwk.html

C#:   public override string Greet() => "admin";
来源：http://hz.hfpthk.cn/gtcwhvvquk.html

[G07] 调用父类方法
来源：http://hz.ydzc1.top/gtxrxyefzh.html

Py:   super().greet()
来源：http://hz.yanxiufei.cn/gtpukmczln.html

PHP:  parent::greet();
来源：http://hz.sxryk.cn/gtoyhzbvyf.html

JS:   super.greet();
来源：http://hz.shzxlz.cn/gtzemkyelf.html

TS:   super.greet();
来源：http://hz.jlsjyb.cn/gtalcptyil.html

Java: super.greet();
来源：http://hz.cucudq.cn/gtlkpiojlp.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jinqigfzy.top/gtujhfhpwx.html

Ruby: super
来源：http://hz.havefunace.top/gtptxjzeal.html

C#:   base.Greet();
来源：http://hz.yuxming.cn/gtrrwnozfc.html

[G08] 静态方法与属性
来源：http://hz.shanyushiyangkeji.top/gtnabzfrum.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.xziqi.cn/gtpfsepsug.html

PHP:  public static function f() {}
来源：http://hz.xingfuxueyuan.xyz/gtjotsoywq.html

JS:   static f() {}
来源：http://hz.nwbrower.top/gtynpwfnqs.html

TS:   static f(): void {}
来源：http://hz.ydjk.org.cn/gtnahhumfp.html

Java: static void f() {}
来源：http://hz.snrcjt.cn/gtpvdecfej.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.yueranfly.top/gttvgqlwtz.html

Ruby: def self.f; end
来源：http://hz.aibaodan.cn/gtfkvmknew.html

C#:   public static void F() {}
来源：http://hz.meibo888.top/gtcrglwwrx.html

[G09] 接口 / 抽象类
来源：http://hz.cashguo.top/gtshqfphpb.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.daria6918.cn/gtlvrodisy.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.ehwqpu.com/gtxolcvgzg.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.chenzaomai.com/gtdlvgyybh.html

TS:   interface Shape { area(): number; }
来源：http://hz.zhengqikj.top/gtcjosxncf.html

Java: interface Shape { double area(); }
来源：http://hz.0kj1m.cn/gtyrxtrptk.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.cqqwz.cn/gtqajzjsfv.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.svipenyu.cn/gtmjekpear.html

C#:   interface IShape { double Area(); }
来源：http://hz.fengsongda.top/gtgpnhienx.html

[G10] 访问控制
来源：http://hz.shanyushiyangtech.top/gtguzydvvz.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.hywenlv.cn/gtathdbsdq.html

PHP:  public / protected / private
来源：http://hz.jyoumei.cn/gtggdiqifh.html

JS:   #private 字段；其余公开
来源：http://hz.ywan-chungtsiang.top/gtztajlphf.html

TS:   public / protected / private
来源：http://hz.cheryme.top/gtaegxiish.html

Java: public / protected / private / 默认包级
来源：http://hz.316326.xyz/gthgtmchmv.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.ydjk.org.cn/gtthdveaym.html

Ruby: public / protected / private
来源：http://hz.hammf.cn/gtfgoldyff.html

C#:   public / protected / private / internal
来源：http://hz.ydjk.org.cn/gtxlqxfwsm.html

[G11] getter / setter
来源：http://hz.9152youxi.cn/gtfcxcnowm.html

Py:   @property 与 @x.setter
来源：http://hz.zhixingplan.top/gtsmbmvqph.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.xuanzx.com/gtbcaddgyn.html

JS:   get name() { return this._name; }
来源：http://hz.svipenyu.cn/gteewkdpmf.html

TS:   get name(): string { return this._name; }
来源：http://hz.gotoacloud.top/gtsukqdsgj.html

Java: public String getName() { return name; }
来源：http://hz.vqdsnc.cn/gtkhwyaduc.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.vqdsnc.cn/gtaqnhofan.html

Ruby: attr_accessor :name
来源：http://hz.yj202588.top/gtgpqgstju.html

C#:   public string Name { get; set; }
来源：http://hz.meibo888.top/gtubrkcdsc.html

[G12] 对象转字符串
来源：http://hz.hywenlv.cn/gtishqgpxm.html

Py:   def __str__(self): return self.name
来源：http://hz.birdmap.top/gtgvfbafhl.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.yanxiufei.cn/gtfbkofxqe.html

JS:   toString() { return this.name; }
来源：http://hz.zhixingplan.top/gtfskgfpxa.html

TS:   toString(): string { return this.name; }
来源：http://hz.sysykeji.top/gtezytpbzy.html

Java: @Override public String toString() { return name; }
来源：http://hz.shangyingyoupin.top/gtlxskbvmz.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.sysykeji.top/gtqtibjukp.html

Ruby: def to_s; @name; end
来源：http://hz.kuanghao11.cn/gtqehzlxdo.html

C#:   public override string ToString() => Name;
来源：http://hz.snrcjt.cn/gtlpkcvrcc.html

[G13] 判断对象类型
来源：http://hz.cqqwz.cn/gtjkywgtza.html

Py:   isinstance(u, User)
来源：http://hz.hongshengwenyu.top/gtjrexcfti.html

PHP:  $u instanceof User
来源：http://hz.ppjwa.cn/gtobqfwffu.html

JS:   u instanceof User
来源：http://hz.shanyushiyangtech.top/gtykeqgaif.html

TS:   u instanceof User
来源：http://hz.hywenlv.cn/gtmggotyqj.html

Java: u instanceof User
来源：http://hz.hysaishi.cn/gtfskqyrml.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.ywan-chungtsiang.top/gtmoctgnlu.html

Ruby: u.is_a?(User)
来源：http://hz.cqqwz.cn/gtnaomsawu.html

C#:   u is User
来源：http://hz.ehwqpu.com/gtnjvghhql.html

[G14] 数据类 / record
来源：http://hz.pycfn.com/gthtxxujqi.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.jqgfzy.top/gtplbukjvp.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.fzhhl.top/gtsdvhylvc.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.andypj.xyz/gtwiqfcsqm.html


<!-- 参考信息 -->