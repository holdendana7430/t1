代发 wailian999

JS:   s.split(/\r?\n/)
来源：http://hz.sxryk.cn/gtbbfwnfml.html

TS:   s.split(/\r?\n/)
来源：http://hz.c1oappe.top/gtdklnvnob.html

Java: s.lines().toList()
来源：http://hz.tian-w.cn/gtpyihlgrb.html

Go:   strings.Split(s, "\n")
来源：http://hz.jinqigufen.top/gtipxsqqlz.html

Ruby: s.lines
来源：http://hz.snrcjt.cn/gtsvwoqdcg.html

C#:   s.Split('\n')
来源：http://hz.yanxiufei.cn/gtbiofptdt.html

[E20] 判断字符串是否为空
来源：http://hz.tianlin.xyz/gttwoidwcr.html

Py:   if not s:
来源：http://hz.fzhhl.top/gtpcywhfzc.html

PHP:  if ($s === "") {}      // 注意 empty("0") 也为 true
来源：http://hz.tanke756.top/gttvcobqmy.html

JS:   if (s === "") {} 或 if (!s) {}
来源：http://hz.0kj1m.cn/gtbcafxuln.html

TS:   if (s === "") {}
来源：http://hz.wangdashe.top/gtlqgknjvf.html

Java: if (s.isEmpty()) {}
来源：http://hz.zhaomingkeji.xyz/gtqgscqvom.html

Go:   if s == "" {}
来源：http://hz.xuetiantiany.cn/gtjbrccyuv.html

Ruby: if s.empty?
来源：http://hz.nwbrower.top/gtbyfmhuxb.html

C#:   if (string.IsNullOrEmpty(s)) {}
来源：http://hz.0kj1m.cn/gtbnkfdask.html

[E21] 超长截断加省略号
来源：http://hz.zhoulong.xyz/gtvnshiqng.html

Py:   (s[:20] + "…") if len(s) > 20 else s
来源：http://hz.ehwqpu.com/gtqbdqzlhk.html

PHP:  mb_strimwidth($s, 0, 20, "…", "UTF-8");
来源：http://hz.pengpengdd.cyou/gtwjusniji.html

JS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yueranfly.top/gtlytnombj.html

TS:   s.length > 20 ? s.slice(0, 20) + "…" : s
来源：http://hz.yuanzhike.top/gtygivqjir.html

Java: s.length() > 20 ? s.substring(0, 20) + "…" : s
来源：http://hz.smart0.xyz/gtjrgcckqn.html

Go:   // 按 rune 判断长度后截断
来源：http://hz.nanxuanxn.top/gtnzjynrwp.html

Ruby: s.length > 20 ? s[0, 20] + "…" : s
来源：http://hz.aizwys.cn/gtuzueedui.html

C#:   s.Length > 20 ? s[..20] + "…" : s
来源：http://hz.zhaomingkeji.xyz/gtpwwzzawl.html

[E22] 字节长度与字符长度
来源：http://hz.aibaodan.cn/gtbsujxtbl.html

Py:   len(s.encode("utf-8"));  len(s)
来源：http://hz.pengpengdd.cyou/gteyngicwm.html

PHP:  strlen($s);  mb_strlen($s, "UTF-8");
来源：http://hz.cucudq.cn/gtqapilxvi.html

JS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.hywenlv.cn/gtizjkfzwe.html

TS:   new TextEncoder().encode(s).length;  s.length
来源：http://hz.shuidangran.top/gtpkyicqdw.html

Java: s.getBytes(StandardCharsets.UTF_8).length;  s.length()
来源：http://hz.ehwqpu.com/gtdxqvfuvw.html

Go:   len(s);  utf8.RuneCountInString(s)     # 前者字节数，后者字符数
来源：http://hz.yanxiufei.cn/gthajvueub.html

Ruby: s.bytesize;  s.length
来源：http://hz.shanyushiyangtech.top/gtvaibrmit.html

C#:   Encoding.UTF8.GetByteCount(s);  s.Length
来源：http://hz.zhongyouzk.top/gtqvzayese.html

================================================================================
来源：http://hz.tanke756.top/gtepxtqjnl.html

F. 文件与目录
来源：http://hz.kuanghao11.cn/gtepaxiefh.html

================================================================================
来源：http://hz.9152youxi.cn/gtvlelbrww.html

[F01] 读取整个文件
来源：http://hz.jinyuanbaomall.cn/gttcmsxywp.html

Py:   open("a.txt", encoding="utf-8").read();  Path("a.txt").read_text()
来源：http://hz.redwolf501.top/gtmvpvzoza.html

PHP:  file_get_contents("a.txt");
来源：http://hz.hnxiangtu.top/gtagojxlzk.html

JS:   fs.readFileSync("a.txt", "utf8")          // Node.js
来源：http://hz.ppjwa.cn/gtqoyuiktk.html

TS:   fs.readFileSync("a.txt", "utf8")
来源：http://hz.mhx1999.top/gtyqkwmrzh.html

Java: Files.readString(Path.of("a.txt"))
来源：http://hz.jyoumei.cn/gtcdbfgurn.html

Go:   data, err := os.ReadFile("a.txt")        // []byte，用 string(data) 转文本
来源：http://hz.cashguo.top/gthvqabiyb.html

Ruby: File.read("a.txt")
来源：http://hz.gzhubu.top/gtjoeensgw.html

C#:   File.ReadAllText("a.txt");
来源：http://hz.zhongyouzk.top/gtqextmqeb.html

[F02] 逐行读取文件
来源：http://hz.chenlongwang.top/gtzodlqgzg.html

Py:   for line in open("a.txt", encoding="utf-8"): print(line.rstrip())
来源：http://hz.andypj.xyz/gtlsyhvsvy.html

PHP:  foreach (file("a.txt", FILE_IGNORE_NEW_LINES) as $line) { echo $line; }
来源：http://hz.yueranfly.top/gtunauisxj.html

JS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.yj20258.top/gtodvhyxrs.html

TS:   for (const line of fs.readFileSync("a.txt", "utf8").split("\n")) {}
来源：http://hz.gzhubu.top/gthknqdytb.html

Java: Files.lines(Path.of("a.txt")).forEach(System.out::println)
来源：http://hz.zhaomingkeji.xyz/gtjanlrvbb.html

Go:   scanner := bufio.NewScanner(f); for scanner.Scan() { fmt.Println(scanner.Text()) }
来源：http://hz.ehwqpu.com/gtraeehdck.html

Ruby: File.foreach("a.txt") { |line| puts line }
来源：http://hz.jyoumei.cn/gtpzubuegz.html

C#:   foreach (var line in File.ReadLines("a.txt")) { Console.WriteLine(line); }
来源：http://hz.nanxinkj.top/gtsdnclxof.html

[F03] 写入文件（覆盖）
来源：http://hz.yuanzhike.top/gtgjjojaos.html

Py:   open("a.txt", "w", encoding="utf-8").write("hi")
来源：http://hz.zhixingplan.top/gtlnywbeuo.html

PHP:  file_put_contents("a.txt", "hi");
来源：http://hz.haohaochexian.top/gteyrsbqvl.html

JS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jqgfzy.top/gtgchplewq.html

TS:   fs.writeFileSync("a.txt", "hi", "utf8")
来源：http://hz.jinqigufen.top/gtreuifjue.html

Java: Files.writeString(Path.of("a.txt"), "hi")
来源：http://hz.fzhhl.top/gtzqzhzvnk.html

Go:   os.WriteFile("a.txt", []byte("hi"), 0644)
来源：http://hz.pycfn.com/gtwcnztpvz.html

Ruby: File.write("a.txt", "hi")
来源：http://hz.yanxiufei.cn/gtshljlyqj.html

C#:   File.WriteAllText("a.txt", "hi");
来源：http://hz.cdnleiting.top/gtviatfcsr.html

[F04] 追加写入文件
来源：http://hz.cucudq.cn/gtyahdbxro.html

Py:   open("a.txt", "a", encoding="utf-8").write("more\n")
来源：http://hz.yj20258888.top/gtxtnayxzu.html

PHP:  file_put_contents("a.txt", "more\n", FILE_APPEND);
来源：http://hz.gotoacloud.top/gtlrqvqyeg.html

JS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.chenjidiqi.icu/gtpuibrqdm.html

TS:   fs.appendFileSync("a.txt", "more\n")
来源：http://hz.wangshuangyany.cn/gtfaqvxrux.html

Java: Files.writeString(Path.of("a.txt"), "more\n", StandardOpenOption.APPEND)
来源：http://hz.nanxinkj.top/gtlrnbwvvu.html

Go:   f, _ := os.OpenFile("a.txt", os.O_APPEND|os.O_WRONLY, 0644); f.WriteString("more\n")
来源：http://hz.gzhubu.top/gtdkumvrfn.html

Ruby: File.open("a.txt", "a") { |f| f.puts "more" }
来源：http://hz.ybcxt.top/gtrxrgrdln.html

C#:   File.AppendAllText("a.txt", "more\n");
来源：http://hz.gaohongyu789.top/gtsifgdydb.html

[F05] 判断文件或目录是否存在
来源：http://hz.yj20258.top/gtwcjswoof.html

Py:   os.path.exists("a.txt");  Path("a.txt").exists()
来源：http://hz.shanyushiyangtech.top/gtolhrvsxc.html

PHP:  file_exists("a.txt");
来源：http://hz.jqgufenzy.top/gtotafgdta.html

JS:   fs.existsSync("a.txt")
来源：http://hz.tianlin.xyz/gtrjgdhvkr.html

TS:   fs.existsSync("a.txt")
来源：http://hz.yuxming.cn/gtcpsajsao.html

Java: Files.exists(Path.of("a.txt"))
来源：http://hz.birdmap.top/gtfxzrcmhw.html

Go:   if _, err := os.Stat("a.txt"); err == nil { /* 存在 */ }
来源：http://hz.dianchejie.cn/gtrwuuwhzj.html

Ruby: File.exist?("a.txt")
来源：http://hz.iojbl.cn/gtudzpbjpl.html

C#:   File.Exists("a.txt")
来源：http://hz.jianghu66.top/gtljmmwwab.html

[F06] 删除文件
来源：http://hz.zhiwuduotai.top/gtlhylqqgo.html

Py:   os.remove("a.txt")
来源：http://hz.sysykeji.top/gtwcaeynhv.html

PHP:  unlink("a.txt");
来源：http://hz.cashguo.top/gtjvjcluys.html

JS:   fs.unlinkSync("a.txt")
来源：http://hz.hysaishi.cn/gtydnqdjbe.html

TS:   fs.unlinkSync("a.txt")
来源：http://hz.hfpthk.cn/gtexbhrhrq.html

Java: Files.deleteIfExists(Path.of("a.txt"))
来源：http://hz.pycfn.com/gtsaaxsbpv.html

Go:   os.Remove("a.txt")
来源：http://hz.hysaishi.cn/gtemnhlqar.html

Ruby: File.delete("a.txt")
来源：http://hz.kuanghao11.cn/gtklewpwia.html

C#:   File.Delete("a.txt");
来源：http://hz.chenjidiqi.icu/gtrqnfgvou.html

[F07] 创建目录（含多级）
来源：http://hz.fengsongda.top/gtevaqjnce.html

Py:   os.makedirs("dir/sub", exist_ok=True)
来源：http://hz.shangyingyoupin.top/gtnoxgsllk.html

PHP:  mkdir("dir/sub", 0777, true);
来源：http://hz.snrcjt.cn/gtmdaovdxw.html

JS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.zhaomingkeji.xyz/gtdrytnlfr.html

TS:   fs.mkdirSync("dir/sub", { recursive: true })
来源：http://hz.52xcode.cn/gtntcqvnob.html

Java: Files.createDirectories(Path.of("dir/sub"))
来源：http://hz.yuanzhike.top/gttaqchfeo.html

Go:   os.MkdirAll("dir/sub", 0755)
来源：http://hz.guannengcc.top/gtbkxvjxnt.html

Ruby: FileUtils.mkdir_p("dir/sub")
来源：http://hz.hongshengwenyu.top/gtvjyjsair.html

C#:   Directory.CreateDirectory("dir/sub");
来源：http://hz.zhiwuduotai.top/gtobrxakep.html

[F08] 遍历目录
来源：http://hz.gotoacloud.top/gtyakjywtn.html

Py:   for name in os.listdir("dir"): print(name)
来源：http://hz.kuanghao11.cn/gtsnelkxlh.html

PHP:  foreach (scandir("dir") as $f) { echo $f; }
来源：http://hz.jqgfzy.top/gtkghapzmg.html

JS:   fs.readdirSync("dir")
来源：http://hz.xingfuxueyuan.xyz/gthqjlnutc.html

TS:   fs.readdirSync("dir")
来源：http://hz.cqqwz.cn/gtaommihqr.html

Java: Files.list(Path.of("dir")).forEach(System.out::println)
来源：http://hz.zhaomingkeji.xyz/gtxbattzkg.html

Go:   entries, _ := os.ReadDir("dir")
来源：http://hz.redwolf501.top/gtwybvbsxd.html

Ruby: Dir.children("dir")
来源：http://hz.tanke756.top/gtvvcknmuz.html

C#:   Directory.GetFiles("dir")
来源：http://hz.hfpthk.cn/gtmgyacwzf.html

[F09] 获取文件大小
来源：http://hz.shanyushiyangkeji.top/gtkxhmktku.html

Py:   os.path.getsize("a.txt")
来源：http://hz.gzhubu.top/gtltficyzl.html

PHP:  filesize("a.txt");
来源：http://hz.zhiwuduotai.top/gtugkclqop.html

JS:   fs.statSync("a.txt").size
来源：http://hz.jqgfzy.top/gtwcjvrdcm.html

TS:   fs.statSync("a.txt").size
来源：http://hz.sysykeji.top/gtzkkcnjte.html

Java: Files.size(Path.of("a.txt"))
来源：http://hz.tanke756.top/gtpwofjenk.html

Go:   info, _ := os.Stat("a.txt"); info.Size()
来源：http://hz.xinyue.icu/gtavpgzbza.html

Ruby: File.size("a.txt")
来源：http://hz.xylfe.cn/gtgrfyppdv.html

C#:   new FileInfo("a.txt").Length
来源：http://hz.shanyushiyangtech.top/gtzgxtlxix.html

[F10] 取文件扩展名 / 文件名
来源：http://hz.c1oappe.top/gtncxxmvow.html

Py:   os.path.splitext("a.txt");  os.path.basename("/x/a.txt")
来源：http://hz.jyoumei.cn/gtiycpmyfh.html

PHP:  pathinfo("a.txt", PATHINFO_EXTENSION);  basename("/x/a.txt");
来源：http://hz.cqqwz.cn/gttrxpbkey.html

JS:   path.extname("a.txt");  path.basename("/x/a.txt")
来源：http://hz.shanyushiyangtech.top/gtugipnvrl.html

TS:   path.extname("a.txt")
来源：http://hz.bjfxy.top/gtsbkcaoku.html

Java: // 手动 substring(lastIndexOf('.'))
来源：http://hz.0kj1m.cn/gtmlomqaie.html

Go:   filepath.Ext("a.txt");  filepath.Base("/x/a.txt")
来源：http://hz.cucudq.cn/gtbzxaslyk.html

Ruby: File.extname("a.txt");  File.basename("/x/a.txt")
来源：http://hz.dashuyun.cn/gtatbozhry.html

C#:   Path.GetExtension("a.txt");  Path.GetFileName("/x/a.txt")
来源：http://hz.cheryme.top/gtxvlaqklm.html

[F11] 复制与移动文件
来源：http://hz.guannengcc.top/gtlgobgqsw.html

Py:   shutil.copy("a.txt", "b.txt");  shutil.move("a.txt", "b.txt")
来源：http://hz.hysaishi.cn/gtdgtqdzow.html

PHP:  copy("a.txt", "b.txt");  rename("a.txt", "b.txt");
来源：http://hz.gaohongyu789.top/gthxsunmln.html

JS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.guannengcc.top/gtbvbavujr.html

TS:   fs.copyFileSync("a.txt", "b.txt");  fs.renameSync("a.txt", "b.txt")
来源：http://hz.hnxiangtu.top/gtwzcgjziz.html

Java: Files.copy(Path.of("a"), Path.of("b"));  Files.move(a, b)
来源：http://hz.zhiwuduotai.top/gteloeextj.html

Go:   data, _ := os.ReadFile("a.txt"); os.WriteFile("b.txt", data, 0644)   // 移动用 os.Rename
来源：http://hz.aibaodan.cn/gtwfhqpbae.html

Ruby: FileUtils.cp("a.txt", "b.txt");  FileUtils.mv("a.txt", "b.txt")
来源：http://hz.jlsjyb.cn/gtsulraipj.html

C#:   File.Copy("a", "b", true);  File.Move("a", "b", true);
来源：http://hz.birdmap.top/gtbbjcryrh.html

[F12] CSV 读写
来源：http://hz.zhiwuduotai.top/gtrzwbkmpx.html

Py:   csv.reader(open("a.csv"));  csv.writer(f).writerow(row)
来源：http://hz.sxryk.cn/gtaulydaux.html

PHP:  $rows = array_map("str_getcsv", file("a.csv"));
来源：http://hz.andypj.xyz/gtsxdsymwm.html

JS:   // 无内置：按行 split(",")，复杂场景用 csv-parse 库
来源：http://hz.xziqi.cn/gtibjgfwxl.html

TS:   // 同上
来源：http://hz.xylfe.cn/gttziktxhd.html

Java: // 无内置：用 OpenCSV / Apache Commons CSV
来源：http://hz.jqgfzy.top/gtiltpwipn.html

Go:   csv.NewReader(f).ReadAll()        // encoding/csv
来源：http://hz.guowangkeji.top/gtmumjcazi.html

Ruby: CSV.read("a.csv")                 // require "csv"
来源：http://hz.svipenyu.cn/gtdfinykiw.html

C#:   // 无内置：用 CsvHelper 库
来源：http://hz.hammf.cn/gtzyysyqec.html

================================================================================
来源：http://hz.wangdashe.top/gtaqydkuvy.html

G. 面向对象
来源：http://hz.yonumen.top/gtexxnnqaj.html

================================================================================
来源：http://hz.xylfe.cn/gtxvjibiyg.html

[G01] 定义类
来源：http://hz.snrcjt.cn/gttyohhipm.html

Py:   class User: pass
来源：http://hz.hongshengwenyu.top/gtpftkaszf.html

PHP:  class User {}
来源：http://hz.sysykeji.top/gtrjszmhvi.html

JS:   class User {}
来源：http://hz.dashuyun.cn/gtoomaxquy.html

TS:   class User { name: string = ""; }
来源：http://hz.316326.xyz/gtrhytdvjd.html

Java: class User {}
来源：http://hz.9152youxi.cn/gtdbrwunhh.html

Go:   type User struct { Name string }
来源：http://hz.jinghuilouyu.cn/gtlqyzkooc.html

Ruby: class User; end
来源：http://hz.chenjidiqi.icu/gteckwqdmc.html

C#:   class User {}
来源：http://hz.ivvv.top/gtwynzabfg.html

[G02] 构造函数
来源：http://hz.daxiang520.top/gteiuysmfx.html

Py:   def __init__(self, name): self.name = name
来源：http://hz.svipenyu.cn/gtwqzexick.html

PHP:  public function __construct(public string $name) {}
来源：http://hz.xinyue.icu/gtjpkfgxff.html

JS:   constructor(name) { this.name = name; }
来源：http://hz.xuetiantiany.cn/gtvkdnqyau.html

TS:   constructor(public name: string) {}
来源：http://hz.havefunace.top/gttdtlozte.html

Java: User(String name) { this.name = name; }
来源：http://hz.redwolf501.top/gtwiwjsqrp.html

Go:   func NewUser(name string) *User { return &User{Name: name} }
来源：http://hz.hysaishi.cn/gtlvfxqtgt.html

Ruby: def initialize(name); @name = name; end
来源：http://hz.guowangkeji.top/gtxzkshhjh.html

C#:   public User(string name) { Name = name; }
来源：http://hz.zhoulong.xyz/gtxmuhiyul.html

[G03] 实例属性
来源：http://hz.snrcjt.cn/gtfkbmczfs.html

Py:   self.name = "x"
来源：http://hz.havefunace.top/gtdoicfyqs.html

PHP:  public string $name = "x";
来源：http://hz.vqdsnc.cn/gtvzkxifvr.html

JS:   this.name = "x";
来源：http://hz.zhengqikj.top/gtdhyztcqo.html

TS:   name: string = "x";
来源：http://hz.jinqigfzy.top/gtoxlsolkm.html

Java: private String name;
来源：http://hz.zhongyouzk.top/gtittomkcg.html

Go:   u := User{Name: "x"}         // 结构体字段
来源：http://hz.xingfuxueyuan.xyz/gtyfnbnbfk.html

Ruby: @name = "x"
来源：http://hz.jqgfzy.top/gtqfqguopw.html

C#:   public string Name { get; set; } = "x";
来源：http://hz.aizwys.cn/gtnrrozvre.html

[G04] 定义方法
来源：http://hz.tian-w.cn/gtbvmxrkay.html

Py:   def greet(self): return self.name
来源：http://hz.hnxiangtu.top/gtplzqbpja.html

PHP:  public function greet(): string { return $this->name; }
来源：http://hz.hywenlv.cn/gtzrpgqomo.html

JS:   greet() { return this.name; }
来源：http://hz.xziqi.cn/gtevuvyyan.html

TS:   greet(): string { return this.name; }
来源：http://hz.nwbrower.top/gtfmbarbdn.html

Java: String greet() { return name; }
来源：http://hz.hnqzz.top/gtrhwkfegy.html

Go:   func (u User) Greet() string { return u.Name }
来源：http://hz.kuanghao11.cn/gtwxjboufi.html

Ruby: def greet; @name; end
来源：http://hz.sysykeji.top/gtfjgioexi.html

C#:   public string Greet() => Name;
来源：http://hz.nwbrower.top/gtxkwnlzmv.html

[G05] 继承
来源：http://hz.vqdsnc.cn/gtycdcnhfy.html

Py:   class Admin(User): pass
来源：http://hz.zhoulong.xyz/gtopdtckqt.html

PHP:  class Admin extends User {}
来源：http://hz.yuanzhike.top/gtiignsnlo.html

JS:   class Admin extends User {}
来源：http://hz.snrcjt.cn/gtcadwwaif.html

TS:   class Admin extends User {}
来源：http://hz.xingfuxueyuan.xyz/gtryyshthg.html

Java: class Admin extends User {}
来源：http://hz.shanyushiyangkeji.top/gtbtngmtcf.html

Go:   type Admin struct { User }     // 用嵌入代替继承
来源：http://hz.sweek.top/gtncrpqqte.html

Ruby: class Admin < User; end
来源：http://hz.iojbl.cn/gtjyowbhhw.html

C#:   class Admin : User {}
来源：http://hz.zdqjudy.top/gtlgzrawfb.html

[G06] 重写方法
来源：http://hz.tian-w.cn/gtxxefqakx.html

Py:   def greet(self): return "admin"
来源：http://hz.yanxiufei.cn/gtfokrduye.html

PHP:  public function greet(): string { return "admin"; }
来源：http://hz.smart0.xyz/gthsfjfctr.html

JS:   greet() { return "admin"; }
来源：http://hz.chenzaomai.com/gtgfudagxh.html

TS:   greet(): string { return "admin"; }
来源：http://hz.yangfankeji.com/gtjdrzpwfb.html

Java: @Override String greet() { return "admin"; }
来源：http://hz.gogol.net.cn/gtdyeraozj.html

Go:   // 嵌入类型定义同名方法即覆盖
来源：http://hz.aibaodan.cn/gtmvyzdzfs.html

Ruby: def greet; "admin"; end
来源：http://hz.xinyue.icu/gtwhgkzcoi.html

C#:   public override string Greet() => "admin";
来源：http://hz.nwbrower.top/gthvackrht.html

[G07] 调用父类方法
来源：http://hz.jiagoushi.top/gturwnmtrw.html

Py:   super().greet()
来源：http://hz.fzhhl.top/gtndyvoeid.html

PHP:  parent::greet();
来源：http://hz.hnxiangtu.top/gtcekmiosx.html

JS:   super.greet();
来源：http://hz.xingfuxueyuan.xyz/gtwwinxusz.html

TS:   super.greet();
来源：http://hz.gaohongyu789.top/gtqvcihlbw.html

Java: super.greet();
来源：http://hz.ydjk.org.cn/gtwqaavmbx.html

Go:   u.User.Greet()               // 显式调用嵌入字段的方法
来源：http://hz.xuanzx.com/gtlbsxsqwu.html

Ruby: super
来源：http://hz.cashguo.top/gtuwfjnifv.html

C#:   base.Greet();
来源：http://hz.dianchejie.cn/gtgcpnxbha.html

[G08] 静态方法与属性
来源：http://hz.xinyue.icu/gtjmhfgrqd.html

Py:   @staticmethod⏎def f(): ...      # 类方法用 @classmethod，首个参数为 cls
来源：http://hz.hnqzz.top/gtxsxdbcvr.html

PHP:  public static function f() {}
来源：http://hz.pycfn.com/gtbxnazfzm.html

JS:   static f() {}
来源：http://hz.dianchejie.cn/gtrkgcofue.html

TS:   static f(): void {}
来源：http://hz.fzhhl.top/gtyndtuosq.html

Java: static void f() {}
来源：http://hz.yuanzhike.top/gtjmeniywq.html

Go:   // 无 static：用包级函数，按包名调用
来源：http://hz.jinyuanbaomall.cn/gtnjpzuchm.html

Ruby: def self.f; end
来源：http://hz.yuanzhike.top/gtfblkbwjt.html

C#:   public static void F() {}
来源：http://hz.zhijiandao.cn/gtosxwosxl.html

[G09] 接口 / 抽象类
来源：http://hz.0kj1m.cn/gtwbddeags.html

Py:   from abc import ABC, abstractmethod
来源：http://hz.meibo888.top/gtxnrayron.html

PHP:  interface Shape { public function area(): float; }
来源：http://hz.hfpthk.cn/gtgtecatlm.html

JS:   // 无接口：靠约定或 JSDoc
来源：http://hz.zhiwuduotai.top/gtgcgriuma.html

TS:   interface Shape { area(): number; }
来源：http://hz.gzhubu.top/gtvzjiwxht.html

Java: interface Shape { double area(); }
来源：http://hz.shanyushiyangtech.top/gtvlizdfnw.html

Go:   type Shape interface { Area() float64 }
来源：http://hz.hysaishi.cn/gtjnvwqldt.html

Ruby: # 无接口：用 module 混入或鸭子类型
来源：http://hz.quarkkingdee.top/gtehzmflvm.html

C#:   interface IShape { double Area(); }
来源：http://hz.yongpay.top/gtpywpoflk.html

[G10] 访问控制
来源：http://hz.guannengcc.top/gtbwuttozm.html

Py:   约定 _protected / __private（不强制）
来源：http://hz.yueranfly.top/gtdecsqoti.html

PHP:  public / protected / private
来源：http://hz.fengsongda.top/gtzuxisknc.html

JS:   #private 字段；其余公开
来源：http://hz.hongshengwenyu.top/gtrilfnwnu.html

TS:   public / protected / private
来源：http://hz.yuanzhike.top/gtzazxwyko.html

Java: public / protected / private / 默认包级
来源：http://hz.zhengqikj.top/gtsxianfus.html

Go:   首字母大写可导出，小写仅包内可见
来源：http://hz.andypj.xyz/gtugztfecm.html

Ruby: public / protected / private
来源：http://hz.shanyushiyangtech.top/gtlrvokvri.html

C#:   public / protected / private / internal
来源：http://hz.chenzaomai.com/gtlknwyjyt.html

[G11] getter / setter
来源：http://hz.hfpthk.cn/gtdpnvkonz.html

Py:   @property 与 @x.setter
来源：http://hz.jiagoushi.top/gtltvomyde.html

PHP:  public function getName(): string { return $this->name; }
来源：http://hz.kuanghao11.cn/gtafohltih.html

JS:   get name() { return this._name; }
来源：http://hz.shanyushiyangtech.top/gtxijjfujz.html

TS:   get name(): string { return this._name; }
来源：http://hz.aibaodan.cn/gtosxacayb.html

Java: public String getName() { return name; }
来源：http://hz.52xcode.cn/gtfbcfkpuk.html

Go:   func (u User) GetName() string { return u.Name }
来源：http://hz.jqgfzy.top/gtjohkommc.html

Ruby: attr_accessor :name
来源：http://hz.yuanzhike.top/gtxvwvqvyh.html

C#:   public string Name { get; set; }
来源：http://hz.cqqwz.cn/gtbzygsvto.html

[G12] 对象转字符串
来源：http://hz.gotoacloud.top/gttzwrkzic.html

Py:   def __str__(self): return self.name
来源：http://hz.feifeiyinyue.top/gtclhselsj.html

PHP:  public function __toString(): string { return $this->name; }
来源：http://hz.snrcjt.cn/gtaqsdejwg.html

JS:   toString() { return this.name; }
来源：http://hz.hammf.cn/gtakndaopt.html

TS:   toString(): string { return this.name; }
来源：http://hz.jinqigufen.top/gtkvlputie.html

Java: @Override public String toString() { return name; }
来源：http://hz.hysaishi.cn/gtvhqglhhu.html

Go:   func (u User) String() string { return u.Name }
来源：http://hz.yj20258.top/gttkogyazc.html

Ruby: def to_s; @name; end
来源：http://hz.hysaishi.cn/gtgziadrmo.html

C#:   public override string ToString() => Name;
来源：http://hz.tian-w.cn/gtvyvhdvjk.html

[G13] 判断对象类型
来源：http://hz.ydzc1.top/gtppubynxp.html

Py:   isinstance(u, User)
来源：http://hz.xuetiantiany.cn/gttanqielq.html

PHP:  $u instanceof User
来源：http://hz.yj20258888.top/gthuowkdhb.html

JS:   u instanceof User
来源：http://hz.sxryk.cn/gttmfpydcf.html

TS:   u instanceof User
来源：http://hz.yangfankeji.com/gtyuiwzefi.html

Java: u instanceof User
来源：http://hz.9152youxi.cn/gtdstjxseo.html

Go:   u, ok := v.(User)            // 类型断言
来源：http://hz.snrcjt.cn/gthgtanuiw.html

Ruby: u.is_a?(User)
来源：http://hz.yueranfly.top/gtcpadolxs.html

C#:   u is User
来源：http://hz.xuetiantiany.cn/gtztbqyyxg.html

[G14] 数据类 / record
来源：http://hz.yonumen.top/gtgllieysa.html

Py:   @dataclass⏎class User: name: str; age: int
来源：http://hz.zhiwuduotai.top/gtgcftwrcn.html

PHP:  // 用 readonly 属性模拟
来源：http://hz.iojbl.cn/gtununigah.html

JS:   // 无内置：普通类或对象字面量
来源：http://hz.xziqi.cn/gtisirlxtj.html

TS:   type User = { name: string; age: number };
来源：http://hz.tianlin.xyz/gtsdgbdsdd.html

Java: record User(String name, int age) {}
来源：http://hz.aizwys.cn/gtgvanxllp.html

Go:   type User struct { Name string; Age int }
来源：http://hz.wangdashe.top/gtongropuy.html

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://hz.xinyue.icu/gtrekpjjcu.html

C#:   record User(string Name, int Age);
来源：http://hz.zhaomingkeji.xyz/gttilfqcix.html

[G15] 枚举
来源：http://hz.wangshuangyany.cn/gtxexewmfk.html

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hz.aizwys.cn/gtdxrzeqiw.html

PHP:  enum Color: string { case Red = "red"; }
来源：http://hz.cucudq.cn/gtxruptrfn.html

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://hz.zycfv.cn/gtbqhqvbbh.html

TS:   enum Color { Red = 1, Green = 2 }
来源：http://hz.gzhubu.top/gtvwqesveh.html

Java: enum Color { RED, GREEN }
来源：http://hz.hfpthk.cn/gtoejdtiwv.html

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://hz.9152youxi.cn/gtquqzmpkp.html

Ruby: Color = %i[red green].freeze
来源：http://hz.mhx1999.top/gtwrroyvox.html

C#:   enum Color { Red = 1, Green = 2 }
来源：http://hz.c1oappe.top/gtyxhbugkj.html

[G16] 对象转数组 / 字典
来源：http://hz.shzxlz.cn/gtjhrmsfct.html

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://hz.hongshengwenyu.top/gtgvvwdzhf.html

PHP:  get_object_vars($obj);
来源：http://hz.zhiwuduotai.top/gtjxmjjvii.html

JS:   Object.entries(obj)
来源：http://hz.aizwys.cn/gtbfoavwmt.html

TS:   Object.entries(obj)
来源：http://hz.quarkkingdee.top/gtilfzebsj.html

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://hz.jinqigufen.top/gtwpnfvnbr.html

Go:   // 手写转换，或用 mapstructure 库
来源：http://hz.guannengcc.top/gtciwrmulm.html

Ruby: obj.instance_variables
来源：http://hz.zhaomingkeji.xyz/gtqgniskyt.html

C#:   // 用反射或 System.Text.Json
来源：http://hz.cucudq.cn/gtvtvnywvv.html

================================================================================
来源：http://hz.nwbrower.top/gthetjyaom.html

H. 异常与错误处理
来源：http://hz.nwbrower.top/gttpsewati.html

================================================================================
来源：http://hz.wangshuangyany.cn/gtuloarukl.html

[H01] try / catch 基础
来源：http://hz.yanxiufei.cn/gtcthfgfyy.html

Py:   try: f()⏎except Exception as e: print(e)
来源：http://hz.fzhhl.top/gtdefztblu.html

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://hz.bjfxy.top/gtlchplmoz.html

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://hz.shangyingyoupin.top/gtinswtvnx.html

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://hz.hysaishi.cn/gteghiaxkk.html

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://hz.hammf.cn/gtxknmwbde.html


<!-- 参考信息 -->