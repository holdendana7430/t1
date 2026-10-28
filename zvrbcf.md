代发 wailian999

TS:   tpl.replaceAll("{name}", name)
来源：http://hz.havefunace.top/gtidqrmona.html

Java: "Hello, %s".formatted(name);  tpl.replace("{name}", name)
来源：http://hz.mhx1999.top/gtrwxnpcwd.html

Go:   strings.ReplaceAll(tpl, "{name}", name)
来源：http://hz.daria6918.cn/gtjbqyzoek.html

Ruby: tpl.gsub("{name}", name);  "Hello, #{name}"
来源：http://hz.wangdashe.top/gtfdffgpiq.html

C#:   tpl.Replace("{name}", name);  $"Hello, {name}"
来源：http://hz.jqgufenzy.top/gthwsoxkga.html

[E19] 多行文本按行拆分
来源：http://hz.yuxming.cn/gtpuamymli.html

Py:   s.splitlines()
来源：http://hz.quarkkingdee.top/gtayhhidxt.html

PHP:  preg_split('/\r\n|\r|\n/', $s);
来源：http://hz.zhijiandao.cn/gtksehipim.html

JS:   s.split(/\r?\n/)
来源：http://hz.zhengqikj.top/gthkxedzhb.html

TS:   s.split(/\r?\n/)
来源：http://hz.tianlin.xyz/gtybsvrdpn.html

Java: s.lines().toList()
来源：http://hz.gzhubu.top/gtmfrnjwcx.html

Go:   strings.Split(s, "\n")
来源：http://hz.xinyue.icu/gtcbktyrbq.html

Ruby: s.lines
来源：http://hz.dashuyun.cn/gtifshfxmx.html

C#:   s.Split('\n')
来源：http://hz.daxiang520.top/gtwlyjhamr.html

[E20] 判断字符串是否为空
来源：http://hz.guannengcc.top/gtykvaquuq.html

Py:   if not s:
来源：http://hz.gaohongyu789.top/gttivbkttr.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.chenlongwang.top/gtjzcqgmzi.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.haohaochexian.top/gttybsbavg.html

TS:   if (s === "") {}
来源：http://hz.cashguo.top/gtssijodwk.html

Java: if (s.isEmpty()) {}
来源：http://hz.aibaodan.cn/gtdqxjkwwm.html

Go:   if s == "" {}
来源：http://hz.nwbrower.top/gtwklbvvcx.html

Ruby: if s.empty?
来源：http://hz.fzhhl.top/gtycvjzngq.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.hfpthk.cn/gtgioncqnk.html

[E21] 超长截断加省略号
来源：http://hz.sysykeji.top/gtrbkfjdyp.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.shanyushiyangkeji.top/gtislzymvw.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.sysykeji.top/gtetsrvbnq.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.svipenyu.cn/gtilrtrqtf.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yonumen.top/gtkrzhtikn.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.xingfuxueyuan.xyz/gtdlmtkrdl.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.yj202588.top/gtexfdbxnf.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.316326.xyz/gtqxskptjj.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.daria6918.cn/gtlpggpnqo.html

[E22] 字节长度与字符长度
来源：http://hz.hongshengwenyu.top/gtuwfkseng.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.jqgufenzy.top/gtokiazojd.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.zhijiandao.cn/gtqdzrykkj.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.nanxuanxn.top/gtlqrklnfl.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.jianghu66.top/gtafwcivad.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.yueranfly.top/gtapeirbrw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.meibo888.top/gtjglnvdkw.html

Ruby: s.bytesize;  s.length
来源：http://hz.smart0.xyz/gtxsocjaca.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.jiagoushi.top/gttfagmkbx.html

================================================================================
来源：http://hz.cdnleiting.top/gtzkxmcmmn.html

F. 文件与目录
来源：http://hz.tanke756.top/gtyudatdlx.html

================================================================================
来源：http://hz.xylfe.cn/gtysmpgthe.html

[F01] 读取整个文件
来源：http://hz.jiagoushi.top/gtkgersoya.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.yvedp.cn/gtbpaneryg.html

PHP:  file_get_contents("a.txt");
来源：http://hz.yj20258.top/gtlezejmuo.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.zycfv.cn/gtkgolrleo.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.feifeiyinyue.top/gthrjcgiji.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.316326.xyz/gtqufebxav.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.gogol.net.cn/gtxdahrjzc.html

Ruby: File.read("a.txt")
来源：http://hz.svipenyu.cn/gtivtgeown.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.hnqzz.top/gtuvaybmym.html

[F02] 逐行读取文件
来源：http://hz.ybcxt.top/gtqgngyhfq.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.hnxiangtu.top/gtupbthhll.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.tianlin.xyz/gtuclmfktn.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yj202588.top/gtftpmkojk.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.9152youxi.cn/gttfpkrrgy.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.cucudq.cn/gtgmqqugiv.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.guannengcc.top/gtngmwvulj.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.iojbl.cn/gtktlzgesd.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.chenzaomai.com/gttrvmlfax.html

[F03] 写入文件（覆盖）
来源：http://hz.cashguo.top/gtgfslqwdi.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.yj20258888.top/gtkndtiexl.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.jinyuanbaomall.cn/gtjdtvtsla.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.sweek.top/gtzhinhhgn.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.feifeiyinyue.top/gtapykvitt.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.ybcxt.top/gtbnsesnzb.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.jinyuanbaomall.cn/gtddedpavo.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.quarkkingdee.top/gtauwjcesk.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.gzhubu.top/gtbwdojzet.html

[F04] 追加写入文件
来源：http://hz.meibo888.top/gtitjnhabk.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.sxryk.cn/gthgpwravb.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.daxiang520.top/gthkrkqlnw.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.chenzaomai.com/gtznsoznie.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.gogol.net.cn/gtbymumuda.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.jinqigufen.top/gtqehxiutn.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.nanxinkj.top/gtfkazyazq.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.wangdashe.top/gtkecxstlc.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.havefunace.top/gtfbintlfy.html

[F05] 判断文件或目录是否存在
来源：http://hz.sysykeji.top/gtidzzlaib.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.jinqigufen.top/gtfuivcdys.html

PHP:  file_exists("a.txt");
来源：http://hz.hywenlv.cn/gtywhwsyel.html

JS:   fs.existsSync("a.txt")
来源：http://hz.sufxvd.cn/gtbsdnmoig.html

TS:   fs.existsSync("a.txt")
来源：http://hz.zdqjudy.top/gtbvmjrssq.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.shanyushiyangtech.top/gtzoxqsiml.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.ydjk.org.cn/gtpszbxclm.html

Ruby: File.exist?("a.txt")
来源：http://hz.wangshuangyany.cn/gteorjgfau.html

C#:   File.Exists("a.txt")
来源：http://hz.dashuyun.cn/gtmztgjmrs.html

[F06] 删除文件
来源：http://hz.sufxvd.cn/gtqzbkyhmr.html

Py:   os.remove("a.txt")
来源：http://hz.xuanzx.com/gtelmbbdxh.html

PHP:  unlink("a.txt");
来源：http://hz.nanxuanxn.top/gtksldupqy.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.gaohongyu789.top/gtrlztgjmp.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.ppjwa.cn/gtlcnlkkme.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.jinghuilouyu.cn/gtngifjikf.html

Go:   os.Remove("a.txt")
来源：http://hz.hammf.cn/gtaedrfjgc.html

Ruby: File.delete("a.txt")
来源：http://hz.nwbrower.top/gtuonepvoj.html

C#:   File.Delete("a.txt");
来源：http://hz.zhixingplan.top/gteshjjdlt.html

[F07] 创建目录（含多级）
来源：http://hz.52xcode.cn/gtpwlzcjgr.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.ywan-chungtsiang.top/gtugrlwwtv.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.nwbrower.top/gtmtpdfosn.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.quarkkingdee.top/gtiydjewxp.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.yj202588.top/gtnwmdpmcr.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.ydjk.org.cn/gtdtxykwql.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.yj202588.top/gtafotffet.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.sysykeji.top/gtxapnhxfn.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.pycfn.com/gtkxrjiqdl.html

[F08] 遍历目录
来源：http://hz.yvedp.cn/gtwxkonzzo.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.xuanzx.com/gtdyznzeas.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.redwolf501.top/gtsgkxwkob.html

JS:   fs.readdirSync("dir")
来源：http://hz.0kj1m.cn/gtvclpsrae.html

TS:   fs.readdirSync("dir")
来源：http://hz.gogol.net.cn/gtoukphxbc.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.havefunace.top/gtklrjhbbm.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.chenlongwang.top/gtloxdkdaz.html

Ruby: Dir.children("dir")
来源：http://hz.chenzaomai.com/gtiiiyeion.html

C#:   Directory.GetFiles("dir")
来源：http://hz.gogol.net.cn/gtbjdotuor.html

[F09] 获取文件大小
来源：http://hz.yuxming.cn/gtcfopjhhf.html

Py:   os.path.getsize("a.txt")
来源：http://hz.cdnleiting.top/gtnadlukiu.html

PHP:  filesize("a.txt");
来源：http://hz.svipenyu.cn/gtaauxaivd.html

JS:   fs.statSync("a.txt").size
来源：http://hz.aizwys.cn/gtbmjswaux.html

TS:   fs.statSync("a.txt").size
来源：http://hz.hnqzz.top/gtlwzxtnuh.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.xziqi.cn/gtzxodiqhu.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.bjfxy.top/gtmclremmr.html

Ruby: File.size("a.txt")
来源：http://hz.shanyushiyangtech.top/gthlpjyfsn.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.guowangkeji.top/gtyblbrvez.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.52xcode.cn/gturfeugqz.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.sweek.top/gteggbojkk.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.svipenyu.cn/gtlfwehxqy.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.hammf.cn/gtufzhcoxi.html

TS:   path.extname("a.txt")
来源：http://hz.nanxuanxn.top/gtpbfxxxjy.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.daria6918.cn/gtrsxwbtta.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.yangfankeji.com/gtdrpngysr.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.hysaishi.cn/gtjqztpjvh.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.316326.xyz/gtpxvsuejr.html

[F11] 复制与移动文件
来源：http://hz.sweek.top/gttktwnatq.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.jyoumei.cn/gtpihapcqg.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.316326.xyz/gtdqwzmqoj.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.guowangkeji.top/gtfievaadc.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.jqgufenzy.top/gtdohvxlbi.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.jinyuanbaomall.cn/gtfjkpdakf.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.ybcxt.top/gtnqreszrf.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.havefunace.top/gtfcfgnmnn.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.ybcxt.top/gtysvsohvv.html

[F12] CSV 读写
来源：http://hz.sufxvd.cn/gthsambgul.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.haohaochexian.top/gtsajtchls.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.haohaochexian.top/gtntovjddl.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.havefunace.top/gtyopbxnwc.html

TS:   // 同上
来源：http://hz.hywenlv.cn/gtnfsqohwv.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.hfpthk.cn/gtrnjjknan.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.jlsjyb.cn/gtbxxfutgz.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.aizwys.cn/gttclallde.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.tanke756.top/gttnwlfwhn.html

================================================================================
来源：http://hz.pengpengdd.cyou/gtiaihuwre.html

G. 面向对象
来源：http://hz.nwbrower.top/gtlbtpwsyw.html

================================================================================
来源：http://hz.feifeiyinyue.top/gtmfhtzdtk.html

[G01] 定义类
来源：http://hz.sxryk.cn/gttqbpcmuv.html

Py:   class User: pass
来源：http://hz.ivvv.top/gtlfmebpjr.html

PHP:  class User {}
来源：http://hz.hnxiangtu.top/gtgiorrdmk.html

JS:   class User {}
来源：http://hz.cheryme.top/gtbtpmrseh.html

TS:   class User { name: string = ""; }
来源：http://hz.fzhhl.top/gtbmlmhalt.html

Java: class User {}
来源：http://hz.cheryme.top/gtqlgbkepd.html

Go:   type User struct { Name string }
来源：http://hz.gogol.net.cn/gtnagenpaq.html

Ruby: class User; end
来源：http://hz.redwolf501.top/gtxzdggfex.html

C#:   class User {}
来源：http://hz.jlsjyb.cn/gtkigzfscn.html

[G02] 构造函数
来源：http://hz.jianghu66.top/gtnjdwilzg.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.wangdashe.top/gtyapalfms.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.shangyingyoupin.top/gtypsgzeup.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.shanyushiyangtech.top/gtoulljglo.html

TS:   constructor(public name: string) {}
来源：http://hz.smart0.xyz/gtecysruwh.html

Java: User(String name) { this.name = name; }
来源：http://hz.jianghu66.top/gtesdvrubf.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.shuidangran.top/gterexhugw.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.aizwys.cn/gtsyfwcydz.html

C#:   public User(string name) { Name = name; }
来源：http://hz.daxiang520.top/gtgaxxpbrb.html

[G03] 实例属性
来源：http://hz.jlsjyb.cn/gtibapjeyj.html

Py:   self.name = "x"
来源：http://hz.tianlin.xyz/gtvwvnioua.html

PHP:  public string $name = "x";
来源：http://hz.feifeiyinyue.top/gtgfxodnnw.html

JS:   this.name = "x";
来源：http://hz.kuanghao11.cn/gtnomqdffw.html

TS:   name: string = "x";
来源：http://hz.jlsjyb.cn/gtttrybbwp.html

Java: private String name;
来源：http://hz.snrcjt.cn/gtlxzeniqk.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.shzxlz.cn/gtubirnnji.html

Ruby: @name = "x"
来源：http://hz.sxryk.cn/gthtrlbosq.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.dianchejie.cn/gtcwziqmxw.html

[G04] 定义方法
来源：http://hz.vqdsnc.cn/gtzvxbneaj.html

Py:   def greet(self): return self.name
来源：http://hz.hnxiangtu.top/gtyjdnpmbw.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.xuetiantiany.cn/gtizarlfxo.html

JS:   greet() { return this.name; }
来源：http://hz.cashguo.top/gtctkvfjqh.html

TS:   greet(): string { return this.name; }
来源：http://hz.fzhhl.top/gtzrelnsri.html

Java: String greet() { return name; }
来源：http://hz.hnqzz.top/gtvmqbdiju.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.guannengcc.top/gtiavkibiw.html

Ruby: def greet; @name; end
来源：http://hz.sufxvd.cn/gtfhwqkmiv.html

C#:   public string Greet() => Name;
来源：http://hz.yj20258.top/gtqhxfwrgi.html

[G05] 继承
来源：http://hz.jinghuilouyu.cn/gtjhusblqx.html

Py:   class Admin(User): pass
来源：http://hz.wangshuangyany.cn/gtwjhfcnyk.html

PHP:  class Admin extends User {}
来源：http://hz.hnqzz.top/gtqxgxltva.html

JS:   class Admin extends User {}
来源：http://hz.xylfe.cn/gthmofmuru.html

TS:   class Admin extends User {}
来源：http://hz.jianghu66.top/gtzntcptrm.html

Java: class Admin extends User {}
来源：http://hz.shanyushiyangtech.top/gttxvtmtet.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.daxiang520.top/gtlscubiwc.html

Ruby: class Admin < User; end
来源：http://hz.ydzc1.top/gtwcpraglh.html

C#:   class Admin : User {}
来源：http://hz.9152youxi.cn/gtiocbcgjw.html

[G06] 重写方法
来源：http://hz.gzhubu.top/gtuscbupbc.html

Py:   def greet(self): return "admin"
来源：http://hz.yuxming.cn/gtzsxyrqke.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.pengpengdd.cyou/gtdbpxfhqi.html

JS:   greet() { return "admin"; }
来源：http://hz.xuetiantiany.cn/gtlciqmkdd.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yuanzhike.top/gtputntnjx.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.daria6918.cn/gtqmfrdrfg.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.tanke756.top/gtlgbdcuqm.html

Ruby: def greet; "admin"; end
来源：http://hz.shzxlz.cn/gtzbqpezhz.html

C#:   public override string Greet() => "admin";
来源：http://hz.xylfe.cn/gtjhisigyc.html

[G07] 调用父类方法
来源：http://hz.sufxvd.cn/gtyvyewkab.html

Py:   super().greet()
来源：http://hz.gogol.net.cn/gtrhsvhzpw.html

PHP:  parent::greet();
来源：http://hz.jqgufenzy.top/gtwgzybqpo.html

JS:   super.greet();
来源：http://hz.shangyingyoupin.top/gtvcjsmvhb.html

TS:   super.greet();
来源：http://hz.xuetiantiany.cn/gtgnsqxawx.html

Java: super.greet();
来源：http://hz.sweek.top/gtdrcnwpvn.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.jinqigfzy.top/gtcvbsmdmq.html

Ruby: super
来源：http://hz.xuetiantiany.cn/gtwlmfjfdr.html

C#:   base.Greet();
来源：http://hz.jinghuilouyu.cn/gtzldhrokz.html

[G08] 静态方法与属性
来源：http://hz.kuanghao11.cn/gtehqytnpb.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.aizwys.cn/gtwgpgbldt.html

PHP:  public static function f() {}
来源：http://hz.cdnleiting.top/gtcozagnqw.html

JS:   static f() {}
来源：http://hz.pycfn.com/gtbgrrprsj.html

TS:   static f(): void {}
来源：http://hz.shangyingyoupin.top/gtnpdeadaz.html

Java: static void f() {}
来源：http://hz.ehwqpu.com/gtpijjkvrx.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.ehwqpu.com/gtdfegitze.html

Ruby: def self.f; end
来源：http://hz.zhaomingkeji.xyz/gtmwrtehzq.html

C#:   public static void F() {}
来源：http://hz.hammf.cn/gtsyimeoop.html

[G09] 接口 / 抽象类
来源：http://hz.sufxvd.cn/gtkfzkqvtt.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.andypj.xyz/gturculjej.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.shanyushiyangtech.top/gtqqifzayo.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.0kj1m.cn/gtjiebkfkc.html

TS:   interface Shape { area(): number; }
来源：http://hz.wangshuangyany.cn/gtctuhpahw.html

Java: interface Shape { double area(); }
来源：http://hz.chenjidiqi.icu/gtizmvsbrr.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.sysykeji.top/gtlladgudo.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.daria6918.cn/gtoeertfim.html

C#:   interface IShape { double Area(); }
来源：http://hz.0kj1m.cn/gtqqihbbji.html

[G10] 访问控制
来源：http://hz.shangyingyoupin.top/gtmjyekpwj.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.jinqigfzy.top/gtzvpimttp.html

PHP:  public / protected / private
来源：http://hz.xylfe.cn/gtxsxyitge.html

JS:   #private 字段；其余公开
来源：http://hz.andypj.xyz/gtdnwjhbfy.html

TS:   public / protected / private
来源：http://hz.jinyuanbaomall.cn/gtaxkpqcfw.html

Java: public / protected / private / 默认包级
来源：http://hz.kuanghao11.cn/gtbmhrjbhj.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.gogol.net.cn/gttdnquxla.html

Ruby: public / protected / private
来源：http://hz.sysykeji.top/gtnhorgtge.html

C#:   public / protected / private / internal
来源：http://hz.dashuyun.cn/gtmswmoexz.html

[G11] getter / setter
来源：http://hz.xuetiantiany.cn/gtmrotmhvo.html

Py:   @property 与 @x.setter
来源：http://hz.tanke756.top/gtazmoewuf.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.aibaodan.cn/gtgejeyvjz.html

JS:   get name() { return this._name; }
来源：http://hz.jlsjyb.cn/gtmwmbbngz.html

TS:   get name(): string { return this._name; }
来源：http://hz.yj20258.top/gtpnkfvbzg.html

Java: public String getName() { return name; }
来源：http://hz.yangfankeji.com/gtpbspihjd.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.yangfankeji.com/gtjjeuilkn.html

Ruby: attr_accessor :name
来源：http://hz.xuanzx.com/gtqlcufzoh.html

C#:   public string Name { get; set; }
来源：http://hz.zhoulong.xyz/gtjuibeazt.html

[G12] 对象转字符串
来源：http://hz.aibaodan.cn/gttrvxeojn.html

Py:   def __str__(self): return self.name
来源：http://hz.ybcxt.top/gtfiiivgbn.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.haohaochexian.top/gtqosklvtz.html

JS:   toString() { return this.name; }
来源：http://hz.yonumen.top/gtcjiwfszr.html

TS:   toString(): string { return this.name; }
来源：http://hz.fzhhl.top/gtusceiqen.html

Java: @Override public String toString() { return name; }
来源：http://hz.52xcode.cn/gtotjpbveg.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.dashuyun.cn/gtljsdkely.html

Ruby: def to_s; @name; end
来源：http://hz.guannengcc.top/gthjnrgkqr.html

C#:   public override string ToString() => Name;
来源：http://hz.gaohongyu789.top/gthgxjgnzb.html

[G13] 判断对象类型
来源：http://hz.wangshuangyany.cn/gtdlopuzoo.html

Py:   isinstance(u, User)
来源：http://hz.guannengcc.top/gthupgajgd.html

PHP:  $u instanceof User
来源：http://hz.sufxvd.cn/gtjfpkudkg.html

JS:   u instanceof User
来源：http://hz.sysykeji.top/gtsqvxrfta.html

TS:   u instanceof User
来源：http://hz.daxiang520.top/gtantnnmdm.html

Java: u instanceof User
来源：http://hz.ehwqpu.com/gtfvwowobt.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.cashguo.top/gtzzmumyrz.html

Ruby: u.is_a?(User)
来源：http://hz.zhiwuduotai.top/gtrlcppnfu.html

C#:   u is User
来源：http://hz.9152youxi.cn/gtaqlaafkg.html

[G14] 数据类 / record
来源：http://hz.jiagoushi.top/gtayzsenko.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.iojbl.cn/gtzfmxgjjj.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.sxryk.cn/gtiaewkegi.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.cqqwz.cn/gtxflmervw.html

TS:   type User = { name: string; age: number };
来源：http://hz.xziqi.cn/gtoarzlyrb.html

Java: record User(String name, int age) {}
来源：http://hz.cucudq.cn/gtibwzcyab.html

Go:   type User struct { Name string; Age int }
来源：http://hz.tanke756.top/gttpxntfdi.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.52xcode.cn/gtvznampuu.html

C#:   record User(string Name, int Age);
来源：http://hz.quarkkingdee.top/gtimecsbiq.html

[G15] 枚举
来源：http://hz.kuanghao11.cn/gteawhalec.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.ppjwa.cn/gtefuvlbma.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.pengpengdd.cyou/gtokayqobj.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.fzhhl.top/gtgfxqrkch.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.zhoulong.xyz/gtebhyvhyu.html

Java: enum Color { RED, GREEN }
来源：http://hz.jinghuilouyu.cn/gtqxfafatf.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.yueranfly.top/gtsetqiled.html

Ruby: Color = %i[red green].freeze
来源：http://hz.yueranfly.top/gtxoyippqc.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.kuanghao11.cn/gtrwebigno.html

[G16] 对象转数组 / 字典
来源：http://hz.jinyuanbaomall.cn/gtmnumpdkm.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.jinghuilouyu.cn/gtgnwmrhop.html

PHP:  get_object_vars($obj);
来源：http://hz.quarkkingdee.top/gtgpyesmnm.html

JS:   Object.entries(obj)
来源：http://hz.zhiwuduotai.top/gturxvvfxn.html

TS:   Object.entries(obj)
来源：http://hz.jyoumei.cn/gtnrtbngij.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.dianchejie.cn/gteogtzval.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.wangshuangyany.cn/gtdoptqror.html

Ruby: obj.instance_variables
来源：http://hz.daria6918.cn/gtwfcksbyp.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.ehwqpu.com/gtwnsvujlz.html

================================================================================
来源：http://hz.sweek.top/gtnspkhowo.html


<!-- 参考信息 -->